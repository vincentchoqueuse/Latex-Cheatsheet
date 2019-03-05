# TIKZ Cheatsheed

## OFDM Communication chain

```
\begin{tikzpicture}[node distance=8em]
  \node[block](n1){Symbols};
  \node[block,right of=n1] (n2) {OFDM Modulation};
  \node[block,right of=n2](n3){CP Insertion};
  \node[block,right of=n3,yshift=-6em](n4){Channel};
  \node[block,left of=n4,yshift=-6em](n5){CP Deletion};
  \node[block,left of=n5](n6){OFDM Demodulation};
  \node[block,left of=n6](n7){Symbols};
  \draw[->,>=latex](n1)--(n2);
  \draw[->,>=latex](n2)--(n3);
  \draw[->,>=latex](n3)-|(n4);
  \draw[->,>=latex](n4)|-(n5);
  \draw[->,>=latex](n5)--(n6);
  \draw[->,>=latex](n6)--(n7);
\end{tikzpicture}
```
