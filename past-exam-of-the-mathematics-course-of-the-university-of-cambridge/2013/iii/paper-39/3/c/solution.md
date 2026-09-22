<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each terminal event $A$, [market completeness](../../../../../../complete-market.md) supplies a portfolio $H_A$ replicating its [indicator function](../../../../../../indicator-function.md). The two pricing identities give

$$
\mathbb E[X\mathbf1_A]=H_A^T\mathbb E[XP_1]=H_A^TP_0
=H_A^T\mathbb E[YP_1]=\mathbb E[Y\mathbf1_A].
$$

The constant payoff is also replicable, so these positive pricing variables are integrable under the stated finite pricing expectations. Equivalently, the preceding finite-atom result makes them finite-valued modulo null sets. Taking $A=\{X>Y\}$, the equality says that the nonnegative variable $(X-Y)\mathbf1_A$ has expectation zero; thus $X\le Y$ almost surely. Reversing the roles gives

$$
\boxed{X=Y\quad\text{almost surely}.}
$$

This is [uniqueness of a one-period pricing density](../../../../../../uniqueness-of-a-one-period-pricing-density.md) in a [complete market](../../../../../../complete-market.md). It uses replication of every event, not only matching a few marginal asset expectations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
