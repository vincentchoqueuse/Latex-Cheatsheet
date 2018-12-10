# PGFPLOT

## General plot

```
\begin{tikzpicture}
    \begin{axis}[xlabel near ticks,ylabel near ticks,grid=both]
    \addplot+[thick] table[mark=none,x index=0, y index=1, col sep=comma] {./csv/3tfclb_2_RI.csv}; 
    \end{axis}
\end{tikzpicture}
```

## Import csv file

```
\addplot table[mark=none,x index=0,y index!1, col sep=comma]{file.csv};
```

## Particular xaxis point

```
\begin{axis}[...,xtick={3},yticklabels={label}...]
...
\end{axis}
```

## Draw sine wave

```
 \addplot+[no marks, samples=100,,domain=0:1] {sin(deg(x))};
```
