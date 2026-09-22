<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

Substitution of

$$
w(z)=\int_\gamma e^{zt}f(t)\,dt
$$

and integration by parts give

$$
w'''-zw
=\int_\gamma e^{zt}(t^3f+f')\,dt
-\left[e^{zt}f(t)\right]_{\partial\gamma}.
$$

Thus take

$$
\boxed{f(t)=e^{-t^4/4}},
$$

and require the endpoint term to vanish. Infinite contour ends must lie in sectors where $\operatorname{Re}(t^4)>0$, namely sectors centred on the positive and negative real and imaginary axes, each of angular width $\pi/4$.

Let the common final segment be the positive real ray from $0$ to $+\infty$, and choose the initial rays from $-\infty$, $+i\infty$, and $-i\infty$ to $0$. Call the resulting contours $\gamma_1,\gamma_2,\gamma_3$. Put

$$
A_r=\int_0^\infty t^re^{-t^4/4}\,dt
=4^{(r-3)/4}\Gamma\!\left(\frac{r+1}{4}\right).
$$

Since $w_i^{(r)}(0)=\int_{\gamma_i}t^re^{-t^4/4}\,dt$, for $r=0,1,2$ the three rows are

$$
\begin{pmatrix}
2A_0&0&2A_2\\
(1-i)A_0&2A_1&(1+i)A_2\\
(1+i)A_0&2A_1&(1-i)A_2
\end{pmatrix}.
$$

Consequently

$$
\det\begin{pmatrix}
w_1(0)&w_1'(0)&w_1''(0)\\
w_2(0)&w_2'(0)&w_2''(0)\\
w_3(0)&w_3'(0)&w_3''(0)
\end{pmatrix}
=-16iA_0A_1A_2.
$$

Using the [Gamma function](../../../../../gamma-function.md) reflection identity,

$$
\boxed{\det=-2\sqrt2\,i\,\pi^{3/2}\ne0}.
$$

The initial-data vectors are therefore [linearly independent](../../../../../linear-independence.md), so the three contour integrals are linearly independent solutions.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
