<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $X$ has [full column rank](../../../../../../full-column-rank.md), $X^TX$ is invertible. The [ordinary least squares](../../../../../../ordinary-least-squares.md) estimator is

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY}.
$$

It satisfies the [normal equations](../../../../../../normal-equation.md)

$$
X^T(Y-X\widehat\beta)=0,
$$

so the residual is orthogonal to the [column space](../../../../../../column-space.md) of $X$. For any $\beta$,

$$
Y-X\beta
=(Y-X\widehat\beta)+X(\widehat\beta-\beta).
$$

The two terms are orthogonal, and the [Pythagorean theorem in an inner-product space](../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
S(\beta)
=S(\widehat\beta)
+(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta)
\ge S(\widehat\beta).
$$

**Thus $\widehat\beta$ minimizes the least-squares objective.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
