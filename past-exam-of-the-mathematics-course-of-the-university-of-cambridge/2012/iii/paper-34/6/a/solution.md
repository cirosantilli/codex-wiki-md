<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the diffusion operator

$$
Lf=\tfrac12\sum_{i,j}a_{ij}\partial_{ij}f+\sum_i b_i\partial_i f,
$$

a continuous adapted process solves the [diffusion martingale problem](../../../../../../diffusion-martingale-problem.md) when, for every $f\in C_b^2(\mathbb R^d)$,

$$
\boxed{f(X_t)-f(X_0)-\int_0^tLf(X_s)\,ds\text{ is a true martingale}.}
$$

Here $C_b^2$ means that the function and its derivatives through order two are bounded and continuous. An equivalent compact-support/local convention is often used for the general [martingale problem](../../../../../../martingale-problem.md); the bounded-coefficient setting lets us use the true-martingale convention explicitly. The matrix $a$ is interpreted as a covariance matrix in the diffusion formulation, hence is symmetric nonnegative; the displayed operator in any case uses only its symmetric part.

A [well-posed martingale problem](../../../../../../well-posed-martingale-problem.md) has existence and uniqueness in law on continuous path space for each specified starting point, or for each initial law in the initial-law formulation. This is uniqueness of the process law, not an assertion of pathwise uniqueness on a prescribed Brownian probability space.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
