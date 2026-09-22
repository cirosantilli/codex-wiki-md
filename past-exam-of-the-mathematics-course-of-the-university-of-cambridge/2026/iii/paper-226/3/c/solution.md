<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [one-arm event](../../../../../../one-arm-event.md) $A_R(a)$ depends on the field values in the finite ball $B_R$. Replace $V_x$ by $U_x+a$ for $x\in B_R$. In the new variables the event has threshold zero, while the product [normal distribution](../../../../../../normal-distribution.md) density is $\prod_{x\in B_R}\varphi(U_x+a)$. Differentiating this finite-dimensional integral under the integral sign gives the Gaussian shift identity

$$
-\frac d{da}\theta_R(a)
=\sum_{x\in B_R}\mathbb E[V_x\mathbf1_{A_R(a)}].
$$

This is also an instance of [Gaussian integration by parts](../../../../../../stein-s-lemma-probability.md). In particular, the asserted inequality holds, in fact with equality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
