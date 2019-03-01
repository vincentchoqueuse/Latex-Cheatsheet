# Pgfplot command for LTI system Analysis

## Block Diagram


```
\usepackage{schemabloc}
\begin{tikzpicture}
	\sbEntree{E}
	\sbBloc[3]{H}{SLIT}{E}
	\sbSortie[3]{S}{H}
	\sbRelier[{$e[n]$}]{E}{H}
	\sbRelier[{$s[n]$}]{H}{S}
\end{tikzpicture}
```

## Closed Loop Block Diagram

```
\begin{tikzpicture}
\sbEntree{E}   
\sbComp{comp}{E}   
\sbRelier[$E(p)$]{E}{comp}
\sbBloc{sys}{$F(p)$}{comp}
\sbRelier{comp}{sys}
\sbSortie[4]{S}{sys}   
\sbRelier[$S(p)$]{sys}{S}
\sbDecaleNoeudy[4]{sys}{U}
\sbBlocr[-1.5]{cap}{$\beta$}{U}      
\sbRelieryx{sys-S}{cap}
\sbRelierxy{cap}{comp}
\end{tikzpicture}
```

## Poles / Zeros Diagram

```
\begin{tikzpicture}
	\begin{axis}[xlabel near ticks,ylabel near ticks, xmin=-2, xmax=2, ymin=-2,ymax=2, axis equal, axis x line=center, axis y line=center,xlabel=$\Re e(p)$,ylabel=$\Im m (p)$]
		  \draw[pattern=north west lines] (axis cs: 0,-2) rectangle (axis cs: 2, 2);
	\end{axis}
\end{tikzpicture}
