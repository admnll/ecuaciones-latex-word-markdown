# Como crear texto con ecuaciones en Markdown

## Antes que nada, hay que instalar la extensión de [Mathjax](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima/related) para Chrome.

En caso de que no puedan instalar la extensión y les aparezca algo como esto:
**'Could not load extension icon 'icon16.png'.'**

Sigan las instrucciones de [aquí](https://github.com/orsharir/github-mathjax/issues/24#issuecomment-462956434)

También hay una extensión para firefox, pero está desactualizada y no funciona. 

>Primeramente vamos a realizar una suma:

$$a+b=c$$

>Luego una división:

$$a/b=c$$

Si queremos una ecuación en línea con variables en línea  $a \ne 0$, entonces tenemos algo como esto $a + b = c$.

El ejemplo de la página de Mathjax es este:

When $a \ne 0$, there are two solutions to \(ax^2 + bx + c = 0\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

No funciona adecuadamente usando \(...\) pero si funciona usando el símbolo '$'

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

>Una ecuación más complicada es la siguiente:

\begin{equation}
\frac{x^2}{x^2 + y^2} = \frac15 + \frac1{x}
\end{equation}

>Para una ecuación con referencia, por ejemplo, la ecuación (\ref{eq:ej}):

\begin{equation}\label{eq:ej}
y(x_{i}) = 4 + x_{i}^{2}
\end{equation}

>También se pueden definir límites

\begin{equation}
\lim_{x \to \infty} \frac{\sin(x)}{x} = 0
\end{equation}

>O sumatorias

$$J_\alpha(x) = \sum_{m=0}^\infty \frac{(-1)^m}{m! \, \Gamma(m + \alpha + 1)}{\left({\frac{x}{2}}\right)}^{2 m + \alpha}$$

>Un sistema de ecuaciones

\begin{equation}
f(n) =
  \begin{cases}
    n/2       & \quad \text{if } n \text{ is even} \newline
    -(n+1)/2  & \quad \text{if } n \text{ is odd}
  \end{cases}
\end{equation}

> Otra forma de definir ecuaciones es esta:

\begin{equation*}
\begin{cases}
  a &= b + c \newline
  d &= e + f + g \newline
  h &= i + j + k + l
\end{cases}
\text{ three equations}
\end{equation*}

> Se puede poner una llave a la izquierda

\begin{equation}
f(x) = \left\lbrace
\begin{array}{lr}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}

> Y alinear cada columna a la derecha:

\begin{equation}
f(x) = \left\lbrace
\begin{array}{rr}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}


> O a la izquierda:

\begin{equation}
f(x) = \left\lbrace
\begin{array}{ll}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}

> O si quieremos la llave en la derecha

\begin{equation}
f(x) = \left.
\begin{array}{ll}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right\rbrace 
\end{equation}


> Ahora escribimos un arreglo de ecuaciones sin llaves

\begin{equation}
\begin{array}{l}{C_1} = {C_2} = \frac{{{V_o}D}}{{\Delta {V_{C1}}R{f_s} \left({1 - D} \right)}} \newline {C_3} = \frac{{{V_o}D}}{{\Delta {V_{C3}}R{f_s}}} \newline {C_r} = \frac{{{D^2}}}{{{\pi ^2}{f_s}}} \left( {\frac{{1 - D}}{{{f_s}{L_r}}} + \frac{{{\Delta_{Lr}}}}{E}} \right) \end{array}
\end{equation}


> Otro ejemplo más, pero alineando la primera columna a la izquierda, la columna del igual al centro y la otra a la derecha.

\begin{array}{lcr} z & = & a \newline f(x,y,z) & = & x + y + z \end{array}


> También se pueden agregar letras griegas

$\min _\Theta \sum {r\left(s, o\right)\in \Omega } \log(1+exp(-Y{rso}\phi (s,r, o; \Theta)) + \lambda\left | \Theta \right |_2^2 $


>Aquí les dejo otros ejemplos:

\begin{equation}
\begin{array}{ccc}
  a = 0  \newline 
  a + b \newline 
  a + b + c_p
\end{array}
\end{equation}


Este último también usa '$$'

$$
\phi_r=\left\lbrace
\begin{array}{ll}
1 & \textrm{if x = 'water'  
and y = 'chocolate'}  \newline
0 & \textrm{otherwise}
\end{array}
\right.
$$
