<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [moment-generating function](../../../../../../moment-generating-function.md) satisfies $0<\phi(\lambda)<\infty$. The proposed process is nonnegative and adapted to the [natural filtration](../../../../../../natural-filtration.md) of the [random walk](../../../../../../random-walk.md), and [independence](../../../../../../independent-random-variables.md) of the increments gives

$$
\mathbb EM_n^\lambda=\frac{\prod_{j=1}^n\mathbb Ee^{\lambda X_j}}{\phi(\lambda)^n}=1.
$$

Moreover $X_{n+1}$ is independent of $\mathcal F_n$, so

$$
\mathbb E[M_{n+1}^\lambda\mid\mathcal F_n]
=\frac{e^{\lambda S_n}}{\phi(\lambda)^{n+1}}\mathbb Ee^{\lambda X_{n+1}}
=M_n^\lambda.
$$

Therefore **$M^\lambda$ is a mean-one nonnegative martingale**, the [exponential martingale of a random walk](../../../../../../exponential-martingale-of-a-random-walk.md). For $\lambda=0$ it is the constant process one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
