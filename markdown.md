# Como crear texto con ecuaciones en Markdown

## Antes que nada, hay que instalar la extensión de [Mathjax](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima/related) para  Chrome.

>Primeramente vamos a realizar una suma:

$$a+b=c$$

\[a+b=c\]

Si queremos una ecuación en línea con variables en línea  $a \ne 0$, entonces tenemos algo como esto $a + b = c$.

El ejemplo de la página de MAthjax es este:

When $a \ne 0$, there are two solutions to \(ax^2 + bx + c = 0\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

No funciona adecuadamente usando \(...\) pero si funciona usando el símbolo '$'

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

>Ahora una división

\begin{equation}
\frac{x^2}{x^2 + y^2} + \frac15 + \frac1{x}
\end{equation}

>Para una ecuación con referencia, por ejemplo, la ecuación (\ref{eq:ej}):

\begin{equation}\label{eq:ej}
y(x_{i}) = 4 + x_{i}^{2}
\end{equation}

>Agregando un límite

\begin{equation}
\lim_{x \to \infty} \frac{\sin(x)}{x} = 0
\end{equation}


>Una sumatoria

$$J_\alpha(x) = \sum_{m=0}^\infty \frac{(-1)^m}{m! \, \Gamma(m + \alpha + 1)}{\left({\frac{x}{2}}\right)}^{2 m + \alpha}$$

>Un sistema de ecuaciones

¿Qué esta mal?

\begin{equation}
f(n) =
  \begin{cases}
    n/2       & \quad \text{if } n \text{ is even} \newline
    -(n+1)/2  & \quad \text{if } n \text{ is odd}
  \end{cases}
\end{equation}

>También se pueden definir ecuaciones por intervalos


\begin{equation*}
\begin{cases}
  a &= b + c \newline
  d &= e + f + g \newline
  h &= i + j + k + l
\end{cases}
\text{ three equations}
\end{equation*}

Brazo a la izquierda

\begin{equation}
f(x) = \left\lbrace
\begin{array}{lr}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}

Si no funciona esto:

\begin{equation}
f(x) = \left\lbrace
\begin{array}{rr}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}


Poner esto:

\begin{equation}
f(x) = \left\lbrace
\begin{array}{ll}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}

Si quieremos la llave en la derecha
\begin{equation}
f(x) = \left
\begin{array}{ll}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right \rbrace 
\end{equation}


>Ahora escribimos un arreglo de ecuaciones

\begin{equation}
\begin{array}{l}{C_1} = {C_2} = \frac{{{V_o}D}}{{\Delta {V_{C1}}R{f_s} \left({1 - D} \right)}} \newline {C_3} = \frac{{{V_o}D}}{{\Delta {V_{C3}}R{f_s}}} \newline {C_r} = \frac{{{D^2}}}{{{\pi ^2}{f_s}}} \left( {\frac{{1 - D}}{{{f_s}{L_r}}} + \frac{{{\Delta_{Lr}}}}{E}} \right) \end{array}
\end{equation}


Probando

\begin{array}{lcl} z & = & a \newline f(x,y,z) & = & x + y + z \end{array}

Finalmente

$\min _\Theta \sum {r\left(s, o\right)\in \Omega } \log(1+exp(-Y{rso}\phi (s,r, o; \Theta)) + \lambda\left | \Theta \right |_2^2 $
