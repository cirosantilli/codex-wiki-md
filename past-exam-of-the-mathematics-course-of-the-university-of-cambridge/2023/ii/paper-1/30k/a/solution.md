<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $y_1\leq y_2$, then the [utility function](../../../../../../utility-function-split.md) is increasing, so for every $X\in\mathcal X$,

$$
\mathbb E[U(X+y_1)]\leq\mathbb E[U(X+y_2)].
$$

Taking [suprema](../../../../../../supremum.md) gives $F(y_1)\leq F(y_2)$.

For $0\leq t\leq1$, let $X_1$ and $X_2$ attain the suprema at $y_1$ and $y_2$. Because $\mathcal X$ is a [vector space](../../../../../../vector-space-split.md),

$$
X_t=tX_1+(1-t)X_2\in\mathcal X.
$$

The [concavity](../../../../../../concave-function.md) of $U$ now gives

$$
\begin{aligned}
F(ty_1+(1-t)y_2)
&\geq\mathbb E\left[U\left(X_t+ty_1+(1-t)y_2\right)\right]\\
&\geq t\mathbb E[U(X_1+y_1)]
 +(1-t)\mathbb E[U(X_2+y_2)]\\
&=tF(y_1)+(1-t)F(y_2).
\end{aligned}
$$

**Thus $F$ is increasing and concave, as stated by [optimized affine shift of concave utility](../../../../../../optimized-affine-shift-of-concave-utility.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
