<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Condition on the number $M$ of stars. The [independence](../../../../../../independent-random-variables.md) assumptions give $\mathbb E[e^{itF_n}\mid M]=q_n(t)^M$, with the inverse-square one-star [characteristic function](../../../../../../characteristic-function.md) $q_n$ from part (a). Averaging over the [Poisson distribution](../../../../../../poisson-distribution.md) therefore gives the [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) formula directly:

$$
\mathbb Ee^{itF_n}
=\sum_{k=0}^\infty e^{-n}\frac{n^k}{k!}q_n(t)^k
=\exp\{n(q_n(t)-1)\}
=\exp\{-I_n(t)\}.
$$

Since $I_n(t)\to\sqrt{\pi m/2}\,|t|^{1/2}$, the [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) gives exactly the same [weak convergence of random variables](../../../../../../convergence-in-distribution.md) as in part (a):

$$
\boxed{\phi(t)=\exp\!\left(-\sqrt{\frac{\pi m}{2}}\,|t|^{1/2}\right).}
$$

The random number of stars introduces no additional limiting term: its effect is already contained in the exact exponential formula. This is the [symmetric inverse-power Poisson field on a line](../../../../../../symmetric-inverse-power-poisson-field-on-a-line.md) at spatial intensity $1/2$ and exponent $p=2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
