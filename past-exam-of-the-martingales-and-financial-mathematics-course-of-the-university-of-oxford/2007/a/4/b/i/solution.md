<h1 id="a/4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [tail sigma-algebra](../../../../../../tail-sigma-algebra.md) is

$$
\boxed{\mathcal T=\bigcap_{m\geq1}
\sigma(X_m,X_{m+1},\ldots).}
$$

Fix $S\in\mathcal T$. [independence](../../../../../../independent-random-variables.md) of the variables and the [pi-systems](../../../../../../pi-system.md) criterion imply [independence](../../../../../../independent-random-variables.md) of $\sigma(X_1,\ldots,X_n)$ from $\sigma(X_{n+1},X_{n+2},\ldots)$. Hence $S$ is independent of every finite-head [sigma-algebra](../../../../../../sigma-algebra.md) $\mathcal H_n=\sigma(X_1,\ldots,X_n)$.

The increasing union $\bigcup_n\mathcal H_n$ is an algebra, hence a [pi-system](../../../../../../pi-system.md), and generates $\mathcal H_\infty=\sigma(X_1,X_2,\ldots)$. Another pi-lambda argument extends the equality $\mathbb P(S\cap A)=\mathbb P(S)\mathbb P(A)$ from that union to all of $\mathcal H_\infty$. Since $S$ itself belongs to $\mathcal H_\infty$, take $A=S$:

$$
\mathbb P(S)=\mathbb P(S)^2.
$$

Therefore

$$
\boxed{\mathbb P(S)\in\{0,1\}.}
$$

This is [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md); no moment assumptions on the variables are needed.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
