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
$$
\left. 2x + y  = 1 \atop x + y = 4 \right}
$$

Entonces

$$\begin{equation}
    o=g(h)=\left\{\begin{array}{rcl}
                     1 & if & h <   0 \\
                     0 & if & h \le 0
\end{array}\right.
\end{equation}$$

>También se pueden definir ecuaciones por intervalos

\begin{equation}
f(n) = \left \{\begin{matrix} n/2 & \mbox{si }n \mbox{ es par} \\ 3n + 1 & \mbox{si }n \mbox{ es impar} \end{matrix} \right. \end{equation}




>Ahora escribimos un arreglo de ecuaciones

\begin{array}{l}{C_1} = {C_2} = \frac{{{V_o}D}}{{\Delta {V_{C1}}R{f_s} \left({1 - D} \right)}} \\ {C_3} = \frac{{{V_o}D}}{{\Delta {V_{C3}}R{f_s}}} \\ {C_r} = \frac{{{D^2}}}{{{\pi ^2}{f_s}}} \left( {\frac{{1 - D}}{{{f_s}{L_r}}} + \frac{{{\Delta_{Lr}}}}{E}} \right) \end{array}

\begin{array}{lcl} z & = & a \\ f(x,y,z) & = & x + y + z \end{array}

$$\begin{equation}
\begin{array}{lrcl}
\textbf{Conservation of energy}     & E_{kin}               &=& E'_{kin}                \\
                & m_1 v_1^2 + m_2 v_2^2         &=& m_1 {v'}_{1}^{2} + m_2 {v'}_{2}^{2} \\
                & m_1 (v_1^2 - {v'}_1^2)        &=& m_2 ({v'}_2^2 - v_2^2)      \\
                & m_1 (v_1 + {v'}_1) (v_1 - {v'}_1)     &=& m_2 ({v'}_2 + v_2) ({v'}_2 - v_2)   \\
\\

\textbf{Conservation of momentum}   & p                 &=& p' \\
                & m_1 v_1 + m_2 v_2             &=& m_1 {v'}_1 + m_2 {v'}_2 \\
                & m_1 (v_1 - {v'}_1)            &=& m_2 ({v'}_2 - v_2) \\
\end{array}
\end{equation}$$


