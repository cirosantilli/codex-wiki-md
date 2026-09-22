<h1 id="27j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The queue length is an [M/M/1 queue](../../../../../../m-m-1-queue.md) and hence a [birth-death process](../../../../../../birth-death-process.md) with birth rate $\lambda$ and death rate $\mu$ away from zero. The [detailed-balance](../../../../../../detailed-balance-for-a-birth-death-process.md) equations are

$$
\pi_n\lambda=\pi_{n+1}\mu,
\qquad n\geq0.
$$

Writing $\rho=\lambda/\mu$, they give $\pi_n=\pi_0\rho^n$. Since $\rho<1$, this measure is summable and normalization yields

$$
\boxed{\pi_n=(1-\rho)\rho^n,\qquad n\geq0}.
$$

The existence of this invariant probability distribution for the irreducible nonexplosive chain proves [positive recurrence](../../../../../../positive-recurrence-of-an-m-m-1-queue.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27J](../../27j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
