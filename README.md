# Latex-Cheatsheet


## Figures

### Side by Side figures

```
\usepackage{caption}
\usepackage{subcaption}

...
\begin{figure}
\centering
\begin{subfigure}{.5\textwidth}
\centering
...
\caption{XXX}
\end{subfigure}
\begin{subfigure}{.5\textwidth}
\centering
...
\caption{XXX}
\end{subfigure}
\end{figure}
```

## Code

```
\usepackage{listings}
...
\begin{lstlisting}[language=Python]
...
\end{lstlisting}
```

### Only one part of a source file

```
\lstinputlisting[firstline=300,lastline=500]{file.c}
```
