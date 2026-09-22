<h1 id="28l/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an initial value $X_0$. One sweep of the [Gibbs sampler](../../../../../../gibbs-sampler.md) consists of

$$
Y_m\sim f_{Y\mid X}(\,\cdot\mid X_{m-1}),
\qquad
X_m\sim f_{X\mid Y}(\,\cdot\mid Y_m).
$$

After a burn-in period, the pairs $(Y_m,X_m)$ are retained as approximate samples. Standard irreducibility and recurrence conditions are needed for convergence from the chosen starting point.

The transition density from $(y,x)$ to $(y',x')$ is

$$
k((y,x),(y',x'))
=f_{Y\mid X}(y'\mid x)f_{X\mid Y}(x'\mid y').
$$

Suppose $(Y,X)$ currently has density $f_{XY}$. The density after one sweep is

$$
\begin{aligned}
&\int_{\mathbb R^2}
f_{XY}(y,x)
f_{Y\mid X}(y'\mid x)
f_{X\mid Y}(x'\mid y')\,dy\,dx\\
&\quad=f_{X\mid Y}(x'\mid y')
\int_{\mathbb R}f_X(x)f_{Y\mid X}(y'\mid x)\,dx\\
&\quad=f_{X\mid Y}(x'\mid y')f_Y(y')
=f_{XY}(x',y').
\end{aligned}
$$

This proves the [stationarity of the two-coordinate Gibbs sampler](../../../../../../stationarity-of-the-two-coordinate-gibbs-sampler.md):

$$
\boxed{f_{XY}\text{ is stationary for the Gibbs transition kernel}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28L](../../28l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
