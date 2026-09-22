<h1 id="13/solution">Solution</h1>

↑ **Parent:** [13](../13.md)

Put $\mu=\operatorname{cf}(\lambda)$ and choose an increasing cofinal sequence of infinite [cardinals](../../../../../cardinal-number.md) $\langle\lambda_i:i<\mu\rangle$ below $\lambda$. Since $\lambda$ is a [strong limit cardinal](../../../../../strong-limit-cardinal.md), $2^{\lambda_i}<\lambda$ for every $i$. Encode a subset $A\subseteq\lambda$ by its restrictions $\langle A\cap\lambda_i:i<\mu\rangle$. Cofinality makes this encoding [injective](../../../../../injective-function.md), giving

$$
2^\lambda\le\prod_{i<\mu}2^{\lambda_i}\le\lambda^\mu.
$$

The second inequality chooses an injection of each restriction set into $\lambda$. Conversely,

$$
\lambda^\mu\le(2^\lambda)^\mu=2^{\lambda\cdot\mu}=2^\lambda,
$$

since $\mu\le\lambda$ and an infinite cardinal satisfies $\lambda\cdot\mu=\lambda$. The two inequalities prove the [singular strong limit power-set identity](../../../../../singular-strong-limit-power-set-identity.md)

$$
\boxed{2^\lambda=\lambda^{\operatorname{cf}(\lambda)}}.
$$

This does not assume the [singular cardinals hypothesis](../../../../../singular-cardinals-hypothesis.md) or determine either side as $\lambda^+$. The strong-limit assumption is what bounds each restricted power set.

## ↑ Ancestors (10)

1. [13](../13.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
