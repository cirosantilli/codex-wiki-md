<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Itô formula](../../../../../../ito-s-lemma.md) separately to cosine and sine, using $[B]_t=t$:

$$
\boxed{dX_t=-Y_t\,dB_t-\tfrac12X_t\,dt,\qquad dY_t=X_t\,dB_t-\tfrac12Y_t\,dt.}
$$

In vector standard form $dZ_t=\sigma(Z_t)\,dB_t+b(Z_t)\,dt$, with one-dimensional driving noise and two-dimensional state, the coefficient functions are

$$
\boxed{\sigma(x,y)=\begin{pmatrix}-y\\x\end{pmatrix},\qquad b(x,y)=-\tfrac12\begin{pmatrix}x\\y\end{pmatrix}.}
$$

The original trigonometric process starts at $(1,0)$, but these coefficient functions define a [stochastic differential equation](../../../../../../stochastic-differential-equation.md) on all of $\mathbb R^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
