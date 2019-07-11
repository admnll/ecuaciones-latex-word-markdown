# Como crear texto con ecuaciones en Markdown

## Antes que nada, hay que instalar la extensión de [Mathjax](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima/related) para Chrome.

En caso de que no puedan instalar la extensión y les aparezca algo como esto:
**'Could not load extension icon 'icon16.png'.'**, sigan las instrucciones de [aquí](https://github.com/orsharir/github-mathjax/issues/24#issuecomment-462956434).

También hay una extensión para firefox, pero está desactualizada y no funciona, por lo que no se recomienda descargarla. 

### Nota
**Los siguientes ejemplos tienen por objeto evidenciar diferentes formas en que se muestran las ecuaciones. Seleccione el ejemplo más adecuado a sus necesidades.** 


### Estos son los ejemplos

>Primeramente vamos a realizar una suma,

$$a+b=c$$


>luego una división:

$$a/b=c$$


Además se pueden escribir variables en línea como $v_z$, o  $a \ne 0$, o una ecuación en línea como $a + b = c$.

El ejemplo de la página de Mathjax es este:

When $a \ne 0$, there are two solutions to \(ax^2 + bx + c = 0\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$


No funciona adecuadamente usando `\(...\)`, pero sí funciona usando el símbolo `$`, tal como se muestra enseguida:

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$


>Una ecuación con fracciones se puede representar como aquí(\ref{etiqueta:uno}):

\begin{equation}\label{etiqueta:uno}
\frac{x^2}{x^2 + y^2} = \frac15 + \frac1{x}
\end{equation}


>Para una ecuación con referencia, por ejemplo, la ecuación (\ref{eq:ej}), se utiliza el código `(\ref{eq:ej})`.

\begin{equation}\label{eq:ej}
y(x_{i}) = 4 + x_{i}^{2}
\end{equation}


>También se pueden definir límites como en (\ref{eq:dos}),

\begin{equation}\label{eq:dos}
\lim_{x \to \infty} \frac{\sin(x)}{x} = 0
\end{equation}


> sumatorias,

$$J_\alpha(x) = \sum_{m=0}^\infty \frac{(-1)^m}{m! \, \Gamma(m + \alpha + 1)}{\left({\frac{x}{2}}\right)}^{2 m + \alpha}$$


>y sistemas de ecuaciones

\begin{equation}
f(n) =
  \begin{cases}
    n/2       & \quad \text{if } n \text{ is even} \newline
    -(n+1)/2  & \quad \text{if } n \text{ is odd}
  \end{cases}
\end{equation}.


> Otra forma de definir ecuaciones es esta:

\begin{equation*}
\begin{cases}
  a &= b + c \newline
  d &= e + f + g \newline
  h &= i + j + k + l
\end{cases}
\text{ three equations}
\end{equation*}


> Se puede poner una llave a la izquierda,

\begin{equation}
f(x) = \left\lbrace
\begin{array}{lr}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}


> y alinear cada columna a la derecha,

\begin{equation}
f(x) = \left\lbrace
\begin{array}{rr}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}


> a la izquierda:

\begin{equation}
f(x) = \left\lbrace
\begin{array}{ll}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right.
\end{equation}


> o mover la llave en la derecha.

\begin{equation}
f(x) = \left.
\begin{array}{ll}
\text{si } x>5000 & 10000 \newline
\text{si } x\leq 5 & 0
\end{array}
\right\rbrace 
\end{equation}


> Ahora escribimos un arreglo de ecuaciones sin llaves.

\begin{equation}
\begin{array}{l}{C_1} = \frac{{{V_o}x}}{{\Delta {VC_{1}}R{f_s} \left({x} \right)}} \newline {C_3} = \frac{{{V_o}x ^2}}{{\Delta {VC_{3}}R{f_s}}} \newline {C_p} = \frac{{{D/2}}}{{{\pi ^4}{f_s}}} \left( {\frac{{x}}{{{f_s}{L_r}}} + \frac{{{\Delta_{Lr}}}}{E}} \right) \end{array}
\end{equation}


> Otro ejemplo más, pero alineando la primera columna a la izquierda, la columna del igual al centro y la otra a la derecha.

\begin{array}{lcr} z & = & a \newline f(x,y,z) & = & x + y + z \end{array}


> También se pueden agregar letras griegas.

$\min _\Theta \sum {r\left(s, o\right)\in \Omega } \log(1+exp(-Y{rso}\phi (s,r, o; \Theta)) + \lambda\left | \Theta \right |_2^2 $


Si no tiene el `\begin{equation} y \end{equation}` entonces no se enumeran las ecuaciones.


>Aquí les dejo otros ejemplos:

\begin{equation}
\begin{array}{ccc}
  a = 0  \newline 
  a + b \newline 
  a + b + c_p
\end{array}
\end{equation}


Este último también usa `$$` y no se enumera.

$$
\phi_r=\left\lbrace
\begin{array}{ll}
1 & \textrm{if x = 'water'  
and y = 'chocolate'}  \newline
0 & \textrm{otherwise}
\end{array}
\right.
$$
