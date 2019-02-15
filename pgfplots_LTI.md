# Pgfplot command for LTI system Analysis

## Poles / Zeros Diagram

```
\begin{tikzpicture}
    \begin{axis}[xlabel near ticks,ylabel near ticks, xmin=-2, xmax=2, ymin=-2,ymax=2, axis equal, axis x line=center, axis y line=center,xlabel=$\Re e(p)$,ylabel=$\Im m (p)$]
		  \draw[pattern=north west lines] (axis cs: 0,-2) rectangle (axis cs: 2, 2);
    \end{axis}
\end{tikzpicture}
