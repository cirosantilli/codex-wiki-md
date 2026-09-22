<h1 id="10h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $v=(v_1,\ldots,v_r)^t$ belongs to the [kernel](../../../../../../kernel-of-a-linear-map.md) of the displayed [matrix](../../../../../../matrix.md) $\Lambda$. Define the [polynomial](../../../../../../polynomial-split.md) $q(z)=\sum_{k=1}^r v_kz^k$. Then $q(\lambda_j)=0$ for all $j$, and $q(0)=0$. These are $r+1$ distinct roots of a [polynomial](../../../../../../polynomial-split.md) of degree at most $r$. Repeated application of the [factor theorem](../../../../../../factor-theorem.md) therefore makes $q$ identically zero, so every $v_k=0$. Hence $\Lambda$ is injective and, by finite-dimensional [rank-nullity theorem](../../../../../../rank-nullity-theorem.md), invertible. Its transpose is invertible with inverse $(\Lambda^{-1})^t$, proving **both kernels are trivial**.

For the second [matrix](../../../../../../matrix.md), membership of the all-ones vector in the [kernel](../../../../../../kernel-of-a-linear-map.md) means

$$
\sum_{j=1}^n\lambda_j^k=0\qquad(1\le k\le n).
$$

Group the distinct nonzero values as $\mu_1,\ldots,\mu_r$, with multiplicities $m_1,\ldots,m_r>0$. Zero values contribute nothing to these positive powers. The first $r$ equations are

$$
\sum_{j=1}^r m_j\mu_j^k=0\qquad(1\le k\le r),
$$

or $\Lambda(\mu)^t m=0$. The proved transpose-kernel statement implies $m=0$, contradicting its positive entries if $r>0$. Therefore $r=0$ and

$$
\boxed{\lambda_1=\cdots=\lambda_n=0.}
$$

Conversely, all zero values plainly give a zero [matrix](../../../../../../matrix.md). This proves the [zero power sums force a finite complex multiset to vanish](../../../../../../zero-power-sums-force-a-finite-complex-multiset-to-vanish.md) criterion, including repetitions and zero values rather than assuming all [eigenvalues](../../../../../../eigenvalue.md) distinct.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10H](../../10h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
