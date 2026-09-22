<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Harris lemma](../../../../../../harris-inequality.md) says that, in any finite product of independent Bernoulli coordinates, two [increasing events](../../../../../../increasing-event.md) satisfy

$$
\mathbb P(A\cap B)\geq\mathbb P(A)\mathbb P(B).
$$

The coordinates need not have the same parameter. For completeness, the same statement for increasing functions follows by induction on the number of coordinates. Conditional on the last bit, induction makes the conditional covariance nonnegative; the covariance of the two conditional means is $p(1-p)(a_1-a_0)(b_1-b_0)\geq0$. The covariance decomposition proves the induction step. Complementing both events gives the inequality for [decreasing events](../../../../../../decreasing-event.md) too. Finite-cylinder approximation extends it to the countable product setting when needed.

For increasing events $A_1,\ldots,A_r$ of a common [probability](../../../../../../probability.md) $a$, their decreasing complements give

$$
\mathbb P\Bigl(\bigcap_{j=1}^rA_j^c\Bigr)\geq\prod_{j=1}^r\mathbb P(A_j^c)=(1-a)^r.
$$

Therefore the [nth root trick](../../../../../../square-root-trick-for-positively-associated-events.md) is

$$
\boxed{a\geq1-\left(1-\mathbb P\Bigl(\bigcup_{j=1}^rA_j\Bigr)\right)^{1/r}.}
$$

This is a lower bound for an individual success probability when a symmetric union is very likely. Without equality of the individual probabilities, the conclusion applies to their maximum. Independence among the $A_j$ is not required.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
