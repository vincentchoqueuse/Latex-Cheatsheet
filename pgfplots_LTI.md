# Pgfplot command for LTI system Analysis

## Block Diagram

```
\begin{tikzpicture}
	\sbEntree{E}
	\sbBloc[3]{H}{SLIT}{E}
	\sbSortie[3]{S}{H}
	\sbRelier[{$e[n]$}]{E}{H}
	\sbRelier[{$s[n]$}]{H}{S}
\end{tikzpicture}
```

## Poles / Zeros Diagram

```
\begin{tikzpicture}
	\begin{axis}[xlabel near ticks,ylabel near ticks, xmin=-2, xmax=2, ymin=-2,ymax=2, axis equal, axis x line=center, axis y line=center,xlabel=$\Re e(p)$,ylabel=$\Im m (p)$]
		  \draw[pattern=north west lines] (axis cs: 0,-2) rectangle (axis cs: 2, 2);
	\end{axis}
\end{tikzpicture}
