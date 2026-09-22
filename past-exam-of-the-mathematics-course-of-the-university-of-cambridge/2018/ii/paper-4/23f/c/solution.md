<h1 id="23f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
\overline h_R=\frac{\int_{-R}^Rh(y)e^{-\Phi(y)}\,dy}{\int_{-R}^Re^{-\Phi(y)}\,dy},
\qquad
q=h-\overline h_R.
$$

Then $q'=h'$ and $q$ has zero weighted mean. Part (b) gives

$$
\|q\|_\infty^2\leq C_R^2\int_{-R}^R|h'|^2e^{-\Phi}.
$$

Therefore, with $Z_R=\int_{-R}^Re^{-\Phi}$,

$$
\int_{-R}^R|h-\overline h_R|^2e^{-\Phi}
\leq Z_RC_R^2\int_{-R}^R|h'|^2e^{-\Phi}.
$$

Thus the compact-interval [Weighted Poincare inequality](../../../../../../weighted-poincare-inequality.md) holds with

$$
\boxed{\lambda_R=(Z_RC_R^2)^{-1}>0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
