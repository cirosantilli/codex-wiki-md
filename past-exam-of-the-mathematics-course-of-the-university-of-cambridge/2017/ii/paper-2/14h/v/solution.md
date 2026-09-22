<h1 id="14h/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

**True.** A useful fact is that squaring is strictly increasing on [ordinals](../../../../../../ordinal.md). If $A<B$, monotonicity in both arguments gives $A^2\leq BA$, and strict increase in the right argument for the positive left factor $B$ gives $BA<B^2$. Hence $A^2<B^2$.

Suppose, for a contradiction, that $\alpha\beta<\beta\alpha$. Again using monotonicity and [associativity](../../../../../../associative-property.md) of [ordinal multiplication](../../../../../../ordinal-multiplication.md),

$$
\alpha^2\beta^2=\alpha(\alpha\beta)\beta
\leq\alpha(\beta\alpha)\beta=(\alpha\beta)^2
<(\beta\alpha)^2=\beta(\alpha\beta)\alpha
\leq\beta(\beta\alpha)\alpha=\beta^2\alpha^2.
$$

This contradicts the hypothesized equality of the outer terms. Reversing the roles excludes $\beta\alpha<\alpha\beta$. If either factor is zero, they already commute. Therefore the [commuting squares of ordinals](../../../../../../commuting-squares-of-ordinals.md) property is

$$
\boxed{\alpha^2\beta^2=\beta^2\alpha^2\ \Longrightarrow\ \alpha\beta=\beta\alpha.}
$$

The proof uses monotonicity, which follows directly from the ordered-copy definition; it does not assume a cancellation law for [ordinals](../../../../../../ordinal.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [14H](../../14h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
