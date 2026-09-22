<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

The first and third equations form a constant-coefficient [linear system of differential equations](../../../../../linear-system-of-differential-equations.md)

$$
\frac d{dt}\binom{x}{z}
=\begin{pmatrix}-1&3\\3&-1\end{pmatrix}\binom{x}{z}.
$$

The [eigenvectors](../../../../../eigenvector.md) $(1,1)$ and $(1,-1)$ have [eigenvalues](../../../../../eigenvalue.md) $2$ and $-4$. Applying the initial data gives

$$
x(t)=\frac{e^{2t}-e^{-4t}}2,
\qquad
z(t)=\frac{e^{2t}+e^{-4t}}2.
$$

The remaining equation becomes

$$
y'-2y=-3e^{-4t}+\cos t-2\sin t.
$$

An [integrating factor](../../../../../integrating-factor.md), or the usual exponential and trigonometric particular solutions, gives

$$
\boxed{x(t)=\frac{e^{2t}-e^{-4t}}2,
\quad y(t)=\sin t+\frac{e^{-4t}-e^{2t}}2,
\quad z(t)=\frac{e^{2t}+e^{-4t}}2}.
$$

These values satisfy all three initial conditions.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
