<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The cases $n=0$ and $n=d$ can indeed be finite: a [Noetherian ring](../../../../../../noetherian-ring.md) has finitely many minimal primes, and a semilocal ring may have finitely many maximal ideals. We prove that every intermediate height occurs infinitely often.

Because $d$ is a finite integer equal to the supremum of prime-chain lengths, there is a chain

$$
\mathfrak p_0\subsetneq\mathfrak p_1\subsetneq\cdots
\subsetneq\mathfrak p_d.
$$

Each $\mathfrak p_i$ has height exactly $i$: its displayed lower chain gives height at least $i$, while any longer lower chain could be extended by the remaining displayed primes and would contradict $\operatorname{ht}\mathfrak p_d=d$.

Suppose $0<n<d$. The three primes

$$
\mathfrak p_{n-1}\subsetneq\mathfrak p_n
\subsetneq\mathfrak p_{n+1}
$$

fall under [prime ideals between a three-prime chain](../../../../../../prime-ideals-between-a-three-prime-chain.md), so infinitely many primes $\mathfrak q$ satisfy

$$
\mathfrak p_{n-1}\subsetneq\mathfrak q
\subsetneq\mathfrak p_{n+1}.
$$

Every such $\mathfrak q$ has height exactly $n$: the lower inclusion gives height at least $n$, and height at least $n+1$ would, after appending $\mathfrak p_{n+1}$, contradict its height $n+1$. Therefore there are infinitely many height-$n$ primes. The assumed finiteness forces

$$
\boxed{n\in\{0,d\}}.
$$

This is [infinitude of intermediate-height prime ideals](../../../../../../infinitude-of-intermediate-height-prime-ideals.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
