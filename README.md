# Latex-Cheatsheet


## Figures

### Side by Side figures

```
\uespackage{caption}
\usepackage{subcaption}

...
\begin{figure}
\centering
\begin{subfigure}{.5\linewidth}
\centering
...
\caption{XXX}
\end{subfigure}
\begin{subfigure}{.5\linewidth}
\centering
...
\caption{XXX}
\end{subfigure}
\end{figure}
```
