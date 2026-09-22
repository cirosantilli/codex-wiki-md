<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $G(z)=\sum_{n\ge0}p_nz^n$ be the [probability generating function](../../../../../../probability-generating-function.md). For $|z|<1$ the series can be differentiated term by term: $\sum n p_n|z|^{n-1}$ is finite, even without a finite claim-count [expected value](../../../../../../expected-value.md). Multiply the [Panjer claim-count class](../../../../../../panjer-claim-count-class.md) recurrence by $n$ and put $m=n-1$. Then

$$
G'(z)=\sum_{n\ge1}np_nz^{n-1}=\sum_{m\ge0}\{a(m+1)+b\}p_mz^m=azG'(z)+(a+b)G(z).
$$

Hence

$$
\boxed{(1-az)G'(z)=(a+b)G(z).}
$$

This argument is valid throughout the open unit disk. Values at boundary points may be obtained by a limit when the required derivatives exist; one need not assume $\mathbb EN<\infty$ to establish the identity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
