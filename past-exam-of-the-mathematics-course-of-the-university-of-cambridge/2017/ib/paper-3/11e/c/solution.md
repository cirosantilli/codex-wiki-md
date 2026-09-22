<h1 id="11e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the [Gaussian integer](../../../../../../gaussian-integer.md) $\alpha=a+bi$, with $a,b\in\mathbb Z$, and set $R=\mathbb Z[\alpha]$. Complex conjugation preserves $R$, because $\bar\alpha=2a-\alpha$. Choose a nonzero $\beta\in P$. Then $N=\beta\bar\beta$ is a positive integer in $P$. It cannot be one because $P$ is a proper [prime ideal](../../../../../../prime-ideal.md). Factoring $N$ into rational primes and applying primality repeatedly gives a prime $p\in P$.

The element $\alpha$ satisfies the monic [polynomial](../../../../../../polynomial-split.md) $F(t)=t^2-2at+a^2+b^2$. Evaluation induces a [ring homomorphism](../../../../../../ring-homomorphism.md) that is a [surjection](../../../../../../surjective-function.md)

$$
\mathbb Z[t]/(p,F)\longrightarrow R/P.
$$

The source has $p^2$ elements by part (b), so

$$
\boxed{|\mathbb Z[\alpha]/P|\le p^2<\infty.}
$$

If $b=0$, use $F(t)=t-a$ instead and get at most $p$ elements. Moreover $R/P$ is an [integral domain](../../../../../../integral-domain.md), so its finiteness makes it a field. This proves the [finite residue-field theorem for Gaussian integer orders](../../../../../../finite-residue-field-theorem-for-gaussian-integer-orders.md) without incorrectly assuming that every Gaussian integer order is a [principal ideal domain](../../../../../../principal-ideal-domain.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11E](../../11e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
