<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [exterior algebra](../../../../../exterior-algebra.md) of a vector space $V$ is $\Lambda^*V^*=\bigoplus_{r=0}^{\dim V}\Lambda^rV^*$, whose degree-$r$ elements are alternating $r$-linear forms. Its [exterior product](../../../../../exterior-product.md) satisfies $\alpha\wedge\beta=(-1)^{rs}\beta\wedge\alpha$ for degrees $r,s$. For example, one-forms anticommute, so $dx^i\wedge dx^i=0$. A [differential form](../../../../../differential-form-split.md) of degree $r$ on a [smooth manifold](../../../../../smooth-manifold.md) is a smooth section of $\Lambda^rT^*M$; in coordinates it is an alternating sum of products of $r$ coordinate one-forms. Its [exterior derivative](../../../../../exterior-derivative.md) increases degree by one, satisfies $d^2=0$, and obeys

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta.
$$

The coordinate definition and [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) are compatible, making differential forms suitable for coordinate-independent integration.

An orientation and a nondegenerate [metric tensor](../../../../../metric-tensor.md) define the [Hodge star operator](../../../../../hodge-star-operator.md) by $\alpha\wedge*\beta=\langle\alpha,\beta\rangle\,\mathrm{vol}_g$ for equal-degree forms. It maps degree $r$ to degree $d-r$. If the metric has $s$ negative directions, its square is $*^2=(-1)^{r(d-r)+s}$. Thus Hodge duality turns antisymmetric tensors into complementary-degree tensors, using the metric and orientation rather than merely the underlying vector space. The [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) says $\int_Md\eta=\int_{\partial M}\eta$, with the induced boundary orientation, for appropriate smooth forms and compactness or support assumptions. It generalizes the fundamental theorem of calculus, circulation version of [Stokes theorem](../../../../../stokes-theorem.md), and divergence theorem.

For the field calculation, choose signature $(-,+,+)$ and a fixed orientation on [Minkowski spacetime](../../../../../minkowski-spacetime.md). Write $a=\delta A$, so $\delta F=da$. Symmetry of the metric pairing and the [Hodge star operator](../../../../../hodge-star-operator.md) gives $\delta(F\wedge*F)=2da\wedge*F$. Applying the [exterior derivative](../../../../../exterior-derivative.md) product rule,

$$
da\wedge*F=d(a\wedge*F)+a\wedge d*F,\qquad
A\wedge da=F\wedge a-d(A\wedge a).
$$

Since $F\wedge a=a\wedge F$, variation of the action is

$$
\delta S=\int_M a\wedge(d*F+kF)
+\int_{\partial M}\left(a\wedge*F-\frac k2A\wedge a\right).
$$

Fix the boundary data or use compactly supported variations. Arbitrary interior one-forms $a$ then imply **the bulk field equation**

$$
\boxed{d*F+kF=0.}
$$

With $B=*F$, the Lorentzian [Hodge star operator](../../../../../hodge-star-operator.md) squares to $-1$ on both one- and two-forms, hence $F=-*B$. Thus the [Maxwell–Chern–Simons one-form equation](../../../../../maxwell-chern-simons-one-form-equation.md) becomes

$$
\boxed{dB-k*B=0,\qquad *dB+kB=0.}
$$

These two displayed equations are equivalent. Also $dF=0$ gives $d*B=0$. For $k\ne0$ the latter follows from applying $d$ to the field equation; for $k=0$ it must be retained as the identity inherited from $F=dA$. Using the opposite metric-sign convention changes the corresponding $*^2$ sign; the signature-independent equation is $d*F+kF=0$.

Under the Abelian [gauge transformation](../../../../../gauge-transformation.md) $A\mapsto A+d\Lambda$, the curvature $F=dA$ and the one-form $B$ are unchanged because $d^2\Lambda=0$. The field equation is therefore exactly [gauge-invariant](../../../../../gauge-invariance.md). The kinetic term is unchanged, while the other term changes by

$$
\boxed{\Delta S=\frac k2\int_Md\Lambda\wedge F
=\frac k2\int_Md(\Lambda F)
=\frac k2\int_{\partial M}\Lambda F.}
$$

The last equality uses $dF=0$ and the [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md). Thus the action density changes by a total derivative and the integrated action can change on a boundary. The source's statement that the action is not invariant needs this qualification: **on a boundaryless spacetime, or when the boundary integral vanishes, the integrated action is invariant too**. No such boundary restriction is needed for invariance of the bulk field equation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
