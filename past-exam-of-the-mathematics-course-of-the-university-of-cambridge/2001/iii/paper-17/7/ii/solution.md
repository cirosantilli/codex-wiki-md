<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $U(C)\cong\mathcal C(R,C)$ naturally and $\mathcal C$ has small [coproducts in a category](../../../../../../coproduct.md). Define

$$
F(X)=\coprod_{x\in X}R.
$$

For a function $v:X\to Y$, define $F(v)$ by sending the $x$-summand by the identity of $R$ to the $v(x)$-summand. The [coproduct](../../../../../../coproduct.md) property gives the identity and composition laws, so $F$ is a [functor](../../../../../../functor.md). There are natural [bijections](../../../../../../bijection.md)

$$
\mathcal C(F(X),C)\cong\prod_{x\in X}\mathcal C(R,C)
\cong\mathbf{Set}(X,U(C)).
$$

The first chooses a [morphism](../../../../../../morphism.md) on every summand; the second views that family as a function. Hence this is the [left adjoint to a covariant representable functor](../../../../../../left-adjoint-to-a-covariant-representable-functor.md):

$$
\boxed{F\dashv U,\qquad F(X)=\coprod_{x\in X}R.}
$$

For empty $X$, the formula uses the empty [coproduct](../../../../../../coproduct.md), an [initial object](../../../../../../initial-object.md), and the same bijection remains valid.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
