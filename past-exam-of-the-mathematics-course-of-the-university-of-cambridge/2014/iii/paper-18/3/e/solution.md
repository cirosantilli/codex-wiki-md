<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose a representing object $R$ and a [natural isomorphism](../../../../../../natural-isomorphism.md) $\theta_X:\mathcal C(R,X)\cong U X$. Using the assumed small [coproducts in a category](../../../../../../coproduct.md), define

$$
\boxed{F(S)=\coprod_{s\in S}R.}
$$

For a function $v:S\to S'$, define $F(v)$ by $F(v)\iota_s=\iota_{v(s)}$. The [coproduct in a category](../../../../../../coproduct.md) uniqueness clause proves preservation of identities and composition, so this is a [functor](../../../../../../functor.md).

Restriction to the coproduct summands, followed by $\theta$, gives

$$
\mathcal C(F(S),X)\cong\prod_{s\in S}\mathcal C(R,X)\cong\mathbf{Set}(S,U X).
$$

These [bijections](../../../../../../bijection.md) are natural in $S$ by the definition of $F(v)$, and natural in $X$ by naturality of $\theta$. They establish **$F\dashv U$**, the [left adjoint to a covariant representable functor](../../../../../../left-adjoint-to-a-covariant-representable-functor.md). The empty set is sent to the empty coproduct.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
