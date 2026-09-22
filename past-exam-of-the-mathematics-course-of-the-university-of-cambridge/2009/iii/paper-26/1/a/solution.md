<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), with origin $O$ at infinity. For $P,Q$, draw their chord, or the tangent if they coincide, and call its third intersection $R$, counted with [intersection multiplicity](../../../../../../intersection-multiplicity.md). The line through $R$ and $O$ gives a third point $S$; define $P+Q=S$. This is the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md). The inverse of an affine point on $y^2+a_1xy+a_3y=x^3+a_2x^2+a_4x+a_6$ is $(x,-y-a_1x-a_3)$, obtained from its vertical line through $O$. These conventions give identity $O$, and cover tangent and flex cases by multiplicity.

Here is a proof of associativity, without assuming that the geometric construction already defines a group. Work first over an [algebraic closure](../../../../../../algebraic-closure.md) and use [divisors on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md). The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) says $\ell(D)-\ell(K_E-D)=\deg D+1-g$. For a smooth genus-one curve the [canonical divisor](../../../../../../canonical-divisor.md) has degree zero, so every degree-one divisor has $\ell(D)=1$. Thus every [divisor class](../../../../../../divisor-class.md) of degree one has a unique effective representative, necessarily a single point. Existence follows from a nonzero section; uniqueness follows because two distinct effective representatives would give linearly independent sections in the same one-dimensional space. Consequently

$$
E\longrightarrow\operatorname{Pic}^0(E),\qquad P\longmapsto[(P)-(O)]
$$

is a bijection: add $(O)$ to any degree-zero [divisor class](../../../../../../divisor-class.md), and use its unique degree-one representative.

A line through $P,Q,R$ cuts out a divisor linearly equivalent to $3(O)$, since the line at infinity has triple intersection at the Weierstrass flex $O$. Equivalently, the ratio of the line equation to that of the line at infinity has [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) $(P)+(Q)+(R)-3(O)$. Thus the three corresponding degree-zero classes sum to zero. Applying the same fact to $O,R,S$ shows that the point produced by the chord-and-tangent process satisfies

$$
[(P+Q)-(O)]=[(P)-(O)]+[(Q)-(O)].
$$

Addition of divisors modulo [principal divisors](../../../../../../principal-divisor-on-an-algebraic-curve.md) is associative. The two parenthesizations of $P+Q+T$ therefore have identical classes; injectivity of the displayed bijection makes them the same point. Hence **the chord-and-tangent law is associative**. This is [associativity of the chord-and-tangent law via divisor classes](../../../../../../associativity-of-the-chord-and-tangent-law-via-divisor-classes.md). Its construction is defined over the original field, so the same conclusion holds for its [rational points](../../../../../../rational-point.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
