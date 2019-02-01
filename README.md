# Latex-Cheatsheet

## Bootstrap document

```
\documentclass{article}
\usepackage{amsmath,amssymb}
\usepackage[french]{babel}
\usepackage[utf8]{inputenc}
\usepackage{subcaption}
\usepackage{fullpage}
\usepackage{graphicx}

\title{Entrainement d'un Moteur à Courant Continu}
\author{Vincent Choqueuse}
\date{}

\begin{document}
\maketitle


\end{document}
```


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

## Columns

```
\begin{columns}
\begin{column}{0.5\textwidth}
   ...
\end{column}
\begin{column}{0.5\textwidth} 
   ...
\end{column}
\end{columns}
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
