<h1 id="31e/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $x\ne\pm1$, eliminating time gives the [separable differential equation](../../../../../../separable-differential-equation.md)

$$
\frac{dy}{dx}=\frac{kxy}{x^2-1},
$$

and hence

$$
y=C|x^2-1|^{k/2}.
$$

Define the possible limit at $x=s\in\{-1,1\}$ for a trajectory starting off the boundary lines by

$$
L_s=
\begin{cases}
\{(s,0)\},&k>0\text{ or }y_0=0,\\
\{(s,y_0)\},&k=0,\\
\varnothing,&k<0\text{ and }y_0\ne0.
\end{cases}
$$

The $k<0$ set is empty because $|y|\to\infty$, so there is no finite accumulation point. Since $\dot x<0$ on $(-1,1)$ and $\dot x>0$ outside $[-1,1]$, the complete classification off the boundary lines is

$$
\begin{array}{c|c|c}
\text{initial }x_0&\alpha(x_0,y_0)&\omega(x_0,y_0)\\ \hline
x_0<-1&\varnothing&L_{-1}\\
-1<x_0<1&L_1&L_{-1}\\
x_0>1&L_1&\varnothing.
\end{array}
$$

For $x_0>1$ the solution has forward [finite-time blow-up](../../../../../../finite-time-blow-up-of-an-ordinary-differential-equation.md), and for $x_0<-1$ it has backward finite-time blow-up, explaining the other empty entries under the usual infinite-time definitions.

It remains to treat $x_0=s=\pm1$. Here $x(t)=s$ and $y(t)=y_0e^{kst}$. If $y_0=0$, both limit sets equal $\{(s,0)\}$. If $y_0\ne0$, then

$$
\begin{array}{c|c|c}
ks&\alpha(s,y_0)&\omega(s,y_0)\\ \hline
ks>0&\{(s,0)\}&\varnothing\\
ks=0&\{(s,y_0)\}&\{(s,y_0)\}\\
ks<0&\varnothing&\{(s,0)\}.
\end{array}
$$

This includes all boundary cases in both $k$ and the initial point.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
