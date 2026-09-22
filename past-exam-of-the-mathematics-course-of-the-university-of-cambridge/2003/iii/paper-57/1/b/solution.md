<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep the metric and hence the [Hodge star](../../../../../../hodge-star-operator.md) fixed. Write $\alpha=\delta A$, so $\delta F=d\alpha$, and use the [Bianchi identity for an Abelian p-form](../../../../../../bianchi-identity-for-an-abelian-p-form.md) $dF=d^2A=0$. The bilinear pairing $U\wedge\star V$ on real four-forms is symmetric even for a fixed indefinite metric. Consequently the variation of the kinetic term is $d\alpha\wedge\star F$.

The two differentiated four-form factors in the cubic term have the same sign, since moving a four-form through another four-form or through a three-form contributes an even exponent. Thus

$$
\delta(F\wedge F\wedge A)=2d\alpha\wedge F\wedge A+\alpha\wedge F\wedge F.
$$

The [graded Leibniz rule](../../../../../../graded-leibniz-rule.md) gives

$$
d(\alpha\wedge\star F)=d\alpha\wedge\star F-\alpha\wedge d\star F,
\qquad
d(\alpha\wedge F\wedge A)=d\alpha\wedge F\wedge A-\alpha\wedge F\wedge F.
$$

Using the [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md), the complete [first variation](../../../../../../first-variation.md) is therefore

$$
\delta S=\int_M\alpha\wedge(d\star F+3F\wedge F)
+\int_{\partial M}(\alpha\wedge\star F+2\alpha\wedge F\wedge A).
$$

For compactly supported variations, a closed $M$, or boundary conditions removing this last term, the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) and the [Bianchi identity for an Abelian p-form](../../../../../../bianchi-identity-for-an-abelian-p-form.md) are

$$
\boxed{d\star F+3F\wedge F=0,\qquad dF=0.}
$$

The coefficient three follows from the normalization actually present in the action; inserting a differently normalized supergravity coupling would change it. This is the [eleven-dimensional three-form action variation](../../../../../../eleven-dimensional-three-form-action-variation.md).

Under the [gauge transformation](../../../../../../gauge-transformation.md) $A\mapsto A+d\Lambda$, the four-form $F$ is unchanged because $d^2\Lambda=0$. The kinetic density is unchanged, and the cubic density changes by

$$
F\wedge F\wedge d\Lambda=d(F\wedge F\wedge\Lambda).
$$

It is an exact eleven-form, so the action changes only by a boundary integral. The [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) depend only on $F$ and are invariant even when this boundary integral is nonzero. Invariance of the action itself additionally requires suitable boundary or support conditions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
