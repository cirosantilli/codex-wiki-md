<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the following [Jacobson radical](../../../../../../jacobson-radical.md) facts for a unital algebra: a [nilpotent ideal](../../../../../../nilpotent-ideal.md) is contained in the [Jacobson radical](../../../../../../jacobson-radical.md); under a surjective algebra homomorphism the image of the [Jacobson radical](../../../../../../jacobson-radical.md) is contained in the radical of the quotient; and a finite product of fields has zero [Jacobson radical](../../../../../../jacobson-radical.md). For completeness, if $I^N=0$ and $x\in I$, then $ax\in I$ for every $a\in A$, and $1-ax$ is invertible with inverse $\sum_{j=0}^{N-1}(ax)^j$. The usual unit criterion for the [Jacobson radical](../../../../../../jacobson-radical.md) therefore gives $I\subseteq J(A)$. The quotient assumption gives $J(A)\subseteq I$. Hence

$$
\boxed{I=J(A).}
$$

This is the [nilpotent ideal with semisimple quotient radical criterion](../../../../../../nilpotent-ideal-with-semisimple-quotient-radical-criterion.md).

For the finite [quiver](../../../../../../quiver.md) under consideration, let $R$ be the [arrow ideal of a path algebra](../../../../../../arrow-ideal-of-a-path-algebra.md), spanned by paths of positive length. If $Q$ has $r$ vertices and no oriented cycle, a path cannot repeat a vertex, so $R^r=0$. Meanwhile $kQ/R\cong\prod_{i\in Q_0}k$, with the constant paths giving the coordinate idempotents. The criterion just proved yields **$J(kQ)=R$**.

The condition on cycles is necessary. A [quiver with one loop](../../../../../../quiver-with-one-loop.md) has [path algebra](../../../../../../path-algebra.md) $k[t]$, whose arrow ideal is $(t)$. But **$J(k[t])=0\ne(t)$**: the maximal ideals $(t-a)$, $a\in k$, have intersection zero, since the algebraically closed field $k$ is infinite and a nonzero polynomial has only finitely many roots. Thus the arrow ideal need not be the [Jacobson radical](../../../../../../jacobson-radical.md) when oriented cycles are present.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
