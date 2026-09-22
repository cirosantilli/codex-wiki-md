<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $p$ is real on the [unit circle](../../../../../../../complex-unit-circle.md),

$$
\sum_{k=-d}^dp_kz^k
=\overline{p(z)}
=\sum_{k=-d}^d\overline{p_k}z^{-k}
=\sum_{k=-d}^d\overline{p_{-k}}z^k.
$$

Multiply the difference by $z^d$. It is an ordinary [polynomial](../../../../../../../polynomial-split.md) of [polynomial degree](../../../../../../../degree-of-a-polynomial.md) at most $2d$ vanishing at every point of the [unit circle](../../../../../../../complex-unit-circle.md). A nonzero [polynomial](../../../../../../../polynomial-split.md) has only finitely many [roots of a polynomial](../../../../../../../root-of-a-polynomial.md), so all its [coefficients](../../../../../../../coefficient.md) vanish. This proves the [conjugate symmetry of trigonometric polynomial coefficients](../../../../../../../conjugate-symmetry-of-trigonometric-polynomial-coefficients.md):

$$
\boxed{p_{-k}=\overline{p_k}\quad(0\leq k\leq d)}.
$$

For arbitrary nonzero complex $z$, [coefficient](../../../../../../../coefficient.md) substitution now gives precisely

$$
\boxed{p(z^{-1})=\overline{p(\overline z)}}.
$$

Equivalently $p(1/\overline z)=\overline{p(z)}$. The [complex conjugation](../../../../../../../complex-conjugation.md) on the right applies to the whole value, including the [coefficients](../../../../../../../coefficient.md); it cannot simply be discarded away from the circle.

The PDF additionally assumes $p_d\ne0$. Then $p_{-d}=\overline{p_d}\ne0$, so the ensuing [polynomial](../../../../../../../polynomial-split.md) $P=z^dp$ has [polynomial degree](../../../../../../../degree-of-a-polynomial.md) exactly $2d$ and nonzero constant term. These clauses and this subpart are absent from the damaged TeX, but present in the PDF.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
