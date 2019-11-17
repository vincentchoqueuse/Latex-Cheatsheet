# PGFPLOT

## General Commands

### General plot

```
\usepackage{pgfplots}

...

\begin{tikzpicture}
    \begin{axis}[xlabel near ticks,ylabel near ticks,grid=both]
    \addplot+[thick] table[mark=none,x index=0, y index=1, col sep=comma] {./csv/3tfclb_2_RI.csv}; 
    \end{axis}
\end{tikzpicture}
```

### Draw sine wave

```
 \addplot+[no marks, samples=100,,domain=0:1] {sin(deg(x))};
```

### Import csv file

```
\addplot table[mark=none,x index=0,y index!1, col sep=comma]{file.csv};
```

### Particular xaxis point

```
\begin{axis}[...,xtick={3},yticklabels={label}...]
...
\end{axis}
```

## Specific Command

### Define Cycle List

```
\pgfplotscreateplotcyclelist{mycolorlist}{
        {thick,red,mark=o,dashed,mark options=solid},
        {thick,black,mark=none},
        {thick,blue,mark=+,brown},
        {thick,black,mark=none,dashed},
        {thick,blue,mark=star},
      }
      
\begin{tikzpicture}
     \begin{axis}[cycle list name=mycolorlist]
     
     \end{axis}
\end{tikzpicture}
```
