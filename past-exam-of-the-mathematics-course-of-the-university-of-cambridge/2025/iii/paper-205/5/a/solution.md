<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [ridge regression](../../../../../../ridge-regression.md) estimator minimizes

$$
\lVert Y-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_2^2.
$$

Its gradient vanishes exactly when $(X^TX+\lambda I)\beta=X^TY$. Since $\lambda>0$ makes this matrix positive definite,

$$
\boxed{\widehat\beta_\lambda=(X^TX+\lambda I)^{-1}X^TY.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
