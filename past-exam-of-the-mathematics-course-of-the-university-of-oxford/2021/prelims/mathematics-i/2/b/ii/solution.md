<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Suppose, for a contradiction, that $p$ and $q$ have no common [root of a polynomial](../../../../../../../root-of-a-polynomial.md). Since the [polynomial ring](../../../../../../../polynomial-ring.md) $\mathbb C[x]$ has no [zero divisors](../../../../../../../zero-divisor.md) and $p,q\ne0$, the relation $ap+bq=0$ with $a,b$ not both zero forces both $a$ and $b$ to be nonzero.

By the [fundamental theorem of algebra](../../../../../../../fundamental-theorem-of-algebra.md), write

$$
p(x)=c\prod_{j=1}^r(x-\alpha_j)^{m_j},\qquad c\ne0,\quad \sum_{j=1}^r m_j=n,
$$

where the $\alpha_j$ are distinct. For each $j$, $q(\alpha_j)\ne0$. The equality $bq=-ap$ implies that $(x-\alpha_j)^{m_j}$ divides $bq$. The [multiplicity of a root](../../../../../../../multiplicity-of-a-root.md) in [polynomial multiplication](../../../../../../../polynomial-multiplication.md) is the sum of its multiplicities in the factors: factor out the largest powers of $x-\alpha_j$ and note that the two remaining factors have nonzero values at $\alpha_j$. Since $q(\alpha_j)\ne0$, $b$ must contain $(x-\alpha_j)^{m_j}$.

Thus $b$ has at least $\sum_jm_j=n$ [roots of a polynomial](../../../../../../../root-of-a-polynomial.md) counted with [multiplicity of a root](../../../../../../../multiplicity-of-a-root.md), so $\deg b\geq n$. This contradicts $b\in V_{n-1}$. Consequently

$$
\boxed{\text{there is }\alpha\in\mathbb C\text{ with }p(\alpha)=q(\alpha)=0.}
$$

Counting [multiplicity of a root](../../../../../../../multiplicity-of-a-root.md) is necessary: counting only distinct [roots of a polynomial](../../../../../../../root-of-a-polynomial.md) would miss repeated factors.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [2](../../../2.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
