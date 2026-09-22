<h1 id="13e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $m_\alpha(x)$ be the monic [minimal polynomial](../../../../../../minimal-polynomial.md). The [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) says $\chi_\alpha(\alpha)=0$. Divide $\chi_\alpha$ by $m_\alpha$; its remainder also annihilates $\alpha$, and a nonzero remainder of smaller degree would contradict minimality. Thus $m_\alpha$ divides $\chi_\alpha$.

Every characteristic root $\lambda_i$ is an [eigenvalue](../../../../../../eigenvalue.md), with a nonzero [eigenvector](../../../../../../eigenvector.md) $v_i$. Since $m_\alpha(\alpha)v_i=m_\alpha(\lambda_i)v_i=0$, it must be a root of the [minimal polynomial](../../../../../../minimal-polynomial.md) as well. This proves there are no possibilities beyond

$$
\boxed{m_\alpha(x)=\prod_i(x-\lambda_i)^{r_i},\qquad 1\le r_i\le n_i.}
$$

Every such choice really occurs. For each $i$, take one [Jordan block](../../../../../../jordan-block.md) of size $r_i$ at $\lambda_i$, together with $n_i-r_i$ scalar blocks at that [eigenvalue](../../../../../../eigenvalue.md), and form their direct sum. The [characteristic polynomial](../../../../../../characteristic-polynomial.md) has the prescribed multiplicities. The nilpotent part of a block of size $r_i$ has its $r_i$th power zero and its $(r_i-1)$st power nonzero, so this component's minimal exponent is exactly $r_i$. A polynomial annihilates the direct sum precisely when it annihilates every component, establishing the displayed [minimal polynomial](../../../../../../minimal-polynomial.md) without any extra restrictions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [13E](../../13e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
