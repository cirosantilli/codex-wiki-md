<h1 id="24j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Uniform integrability](../../../../../../uniform-integrability.md) means $\sup_n\mathbb E[|X_n|\mathbf1_{\{|X_n|>K\}}]\to0$ as $K\to\infty$. In particular the first absolute moments are uniformly bounded. By the [Portmanteau theorem](../../../../../../portmanteau-theorem.md), $\mathbb E|X|\leq\liminf_n\mathbb E|X_n|<\infty$. Let $T_K(x)=\max(-K,\min(x,K))$, a bounded continuous truncation. [Convergence in distribution](../../../../../../convergence-in-distribution.md) gives $\mathbb E T_K(X_n)\to\mathbb E T_K(X)$. Therefore

$$
\limsup_n|\mathbb EX_n-\mathbb EX|\leq\sup_n\mathbb E\bigl[|X_n|\mathbf1_{\{|X_n|>K\}}\bigr]+\mathbb E\bigl[|X|\mathbf1_{\{|X|>K\}}\bigr].
$$

The first term tends to zero by [uniform integrability](../../../../../../uniform-integrability.md), the second by [integrability](../../../../../../integrability.md) of $X$. Hence $\boxed{\mathbb EX_n\to\mathbb EX}$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [24J](../../24j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
