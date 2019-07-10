# Como crear texto con ecuaciones en Markdown

## Antes que nada, hay que instalar la extensión de [Mathjax](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima/related) para  Chrome.

>Primeramente vamos a realizar una suma:

$$a+b=c$$

>Ahora una ecuación, por ejemplo, la ecuación (\ref{eq:ej}):

\begin{equation}\label{eq:ej}
y(x_{i}) = 4 + x_{i}^{2}
\end{equation}

>Ahora escribimos un arreglo de ecuaciones

$$\begin{array}{l}{C_1}={C_2}=\frac{{{V_o}D}}{{\Delta{V_{C1}}R{f_s}\left({1-D}\right)}}\\{C_3}=\frac{{{V_o}D}}{{\Delta{V_{C3}}R{f_s}}}\\{C_r}=\frac{{{D^2}}}{{{\pi^2}{f_s}}}\left({\frac{{1-D}}{{{f_s}{L_r}}}+\frac{{{\Delta_{Lr}}}}{E}}\right)\end{array}$$
