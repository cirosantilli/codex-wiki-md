<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $z_u,z_d$ be the state-price-density values at the higher and lower risky payoff. Pricing the two assets gives

$$
\tfrac12\,6(z_u+z_d)=5,\qquad\tfrac12(7z_u+4z_d)=5.
$$

Solving yields

$$
\boxed{Z=\begin{cases}10/9&S_1=7,\\5/9&S_1=4.\end{cases}}
$$

Both values are positive, and the two independent equations make the solution unique. The payoff matrix has nonzero determinant, so this is a [complete two-state market](../../../../../../complete-two-state-market.md). The actual [Arrow state prices](../../../../../../arrow-debreu-state-price.md), including physical probabilities, are $q_u=5/9$ and $q_d=5/18$. Their sum is $5/6$, the [discount factor](../../../../../../discount-factor.md). Normalizing gives [risk-neutral probabilities](../../../../../../risk-neutral-probability.md) $2/3,1/3$. Thus $Z$ itself is not a probability density of mean one: its mean is $5/6$ because the riskless asset earns interest.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
