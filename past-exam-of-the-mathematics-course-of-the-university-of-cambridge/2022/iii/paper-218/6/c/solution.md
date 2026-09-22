<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a Laplace prior $\phi(u)\propto e^{-\lambda|u|}$, maximizing the posterior is equivalent to minimizing

$$
\frac12\|Y-X\beta\|_2^2+\lambda\|\beta\|_1,
$$

so the posterior mode is the [Lasso](../../../../../../lasso.md). For a Gaussian prior $\phi(u)\propto e^{-\lambda u^2/2}$, the mode minimizes

$$
\frac12\|Y-X\beta\|_2^2+\frac\lambda2\|\beta\|_2^2
$$

and is the [ridge regression](../../../../../../ridge-regression.md) estimator $(X^TX+\lambda I)^{-1}X^TY$. Gaussian conjugacy makes the posterior normal, so its mode and [posterior mean](../../../../../../posterior-mean.md) coincide at this ridge estimate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
