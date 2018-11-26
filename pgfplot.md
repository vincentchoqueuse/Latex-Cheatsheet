# PGFPLOT

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
