<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed $\lambda_2$, letting $\lambda_1\downarrow0$ gives [ridge regression](../../../../../../ridge-regression.md), including ordinary least squares when $\lambda_2=0$; letting $\lambda_1\to\infty$ forces every coefficient to zero. For fixed $\lambda_1$, letting $\lambda_2\downarrow0$ gives the [Lasso](../../../../../../lasso.md). Letting both penalties vanish gives an [ordinary least squares](../../../../../../ordinary-least-squares.md) solution, unique when $X$ has full column rank and otherwise potentially nonunique or path-dependent.

When $\lambda_2>0$, the term $\lambda_2\lVert\beta\rVert_2^2$ is strictly convex. Its sum with the convex squared loss and $\ell^1$ penalty is strictly convex and coercive, so the [elastic net](../../../../../../elastic-net-regularization.md) solution exists and is unique.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
