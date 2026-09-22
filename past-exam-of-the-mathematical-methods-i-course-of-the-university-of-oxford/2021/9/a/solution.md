<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [matrix exponential](../../../../matrix-exponential.md) power series is absolutely convergent for a finite matrix, so taking the [conjugate transpose](../../../../conjugate-transpose.md) term by term is valid. Since $M^\dagger=M$,

$$
U^\dagger=\left(\sum_{n=0}^\infty\frac{i^nM^n}{n!}\right)^\dagger
=\sum_{n=0}^\infty\frac{(-i)^nM^n}{n!}=e^{-iM}.
$$

The absolute convergence also justifies the [Cauchy product](../../../../cauchy-product.md). In $e^{-iM}e^{iM}$, the coefficient of $M^n$ is proportional to $\sum_{k=0}^n(-1)^k\binom nk$, which is zero for $n>0$ and one for $n=0$, by the [binomial theorem](../../../../binomial-theorem.md). Consequently $U^\dagger U=I$; the reversed product is also $I$. This proves that the exponential is [unitary](../../../../unitary-connection.md) directly from the power series, without invoking diagonalization.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
