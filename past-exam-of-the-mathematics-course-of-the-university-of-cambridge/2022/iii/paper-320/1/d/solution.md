<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an intrinsic [probability density function](../../../../../../probability-density-function.md) $\mathcal P(q)$, the [law of total probability](../../../../../../law-of-total-probability.md) averages the conditional density from part c. An object observed with ratio $Q$ can only have $q\leq Q$, so

$$
\boxed{
\mathcal P(Q)
=Q\int_0^Q
\frac{\mathcal P(q)}{\sqrt{1-q^2}\sqrt{Q^2-q^2}}\,dq,
\qquad 0<Q<1}.
$$

This is an [Abel transform](../../../../../../abel-transform.md) of $\mathcal P(q)/\sqrt{1-q^2}$. Its normalization follows by reversing the order of integration and using $\int_q^1\mathcal P(Q\mid q)dQ=1$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
