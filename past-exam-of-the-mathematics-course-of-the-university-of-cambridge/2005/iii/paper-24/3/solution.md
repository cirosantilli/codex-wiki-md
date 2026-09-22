<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use shifted degrees

$$
L_Y=\bigoplus_{j\ge1}\pi_{j+1}(Y)\otimes\mathbb Q
=\pi_*(\Omega Y)\otimes\mathbb Q.
$$

Its [graded Lie bracket](../../../../../graded-lie-bracket.md) is the sign-adjusted [Whitehead bracket](../../../../../whitehead-product.md) from Question 2, equivalently the [Samelson product](../../../../../samelson-product.md) on loops. This regrading is essential: the geometric bracket has degree minus one in the unshifted sphere grading. A [free graded Lie algebra](../../../../../free-graded-lie-algebra.md) on a graded [vector space](../../../../../vector-space-split.md) $V$ means $\mathbb L(V)$ with the universal extension property for linear maps from $V$ to any [graded Lie algebra](../../../../../graded-lie-algebra.md).

Here are the general results used. The [Bott–Samelson theorem](../../../../../bott-samelson-theorem.md) says that, for a connected based [CW complex](../../../../../cw-complex.md) $X$, the inclusion $X\to\Omega\Sigma X$ induces an isomorphism of graded algebras

$$
T(\widetilde H_*(X;\mathbb Q))\xrightarrow{\sim}
H_*(\Omega\Sigma X;\mathbb Q)
$$

with the [Pontryagin product](../../../../../pontryagin-product-on-loop-space-homology.md). The [Milnor–Moore theorem](../../../../../milnor-moore-theorem.md) says that for [simply connected](../../../../../simply-connected-space.md) $Y$, rational loop [Hurewicz homomorphism](../../../../../hurewicz-homomorphism.md) identifies $L_Y$ with the primitives of that loop-homology [Hopf algebra](../../../../../hopf-algebra.md) and induces $U(L_Y)\cong H_*(\Omega Y;\mathbb Q)$. The graded [Poincaré-Birkhoff-Witt theorem](../../../../../poincare-birkhoff-witt-theorem.md) identifies the associated graded algebra of $U(L)$, for its word-length filtration, with the [graded symmetric algebra](../../../../../graded-symmetric-algebra.md) on $L$; hence its [primitive elements of a Hopf algebra](../../../../../primitive-element-of-a-hopf-algebra.md) are exactly $L$ over $\mathbb Q$. Finally the [rational Whitehead theorem](../../../../../rational-whitehead-theorem.md) identifies [rational homology](../../../../../rational-homology.md) equivalences of [simply connected](../../../../../simply-connected-space.md) [CW complexes](../../../../../cw-complex.md) with [rational homotopy equivalences](../../../../../rational-homotopy-equivalence.md). [Rationalization of a topological space](../../../../../rationalization-of-a-topological-space.md) induces the corresponding isomorphisms of loop-space [homotopy](../../../../../homotopy.md) and [rational homology](../../../../../rational-homology.md).

Suppose first $Y$ has the [rational homotopy type](../../../../../rational-homotopy-type.md) of $\Sigma X$. A [reduced suspension](../../../../../reduced-suspension.md) is [simply connected](../../../../../simply-connected-space.md) when $X$ is connected; a disconnected $X$ has $H_1(\Sigma X;\mathbb Q)=\widetilde H_0(X;\mathbb Q)\ne0$, so it cannot have the rational homology of the simply connected $Y$. Put $V=\widetilde H_*(X;\mathbb Q)$, in strictly positive degrees. [Bott–Samelson theorem](../../../../../bott-samelson-theorem.md) gives $H_*(\Omega Y;\mathbb Q)\cong T(V)$ as an algebra. To deduce freeness of the primitive [Lie algebra](../../../../../lie-algebra-split.md), its coproduct must also be considered: the initial [Bott–Samelson theorem](../../../../../bott-samelson-theorem.md) generators can have reduced-diagonal terms when $X$ has nontrivial [cup products](../../../../../cup-product.md).

By [Milnor–Moore theorem](../../../../../milnor-moore-theorem.md) write this [Hopf algebra](../../../../../hopf-algebra.md) as $U(L_Y)$. Its algebra indecomposables satisfy

$$
Q(U(L_Y))\cong L_Y/[L_Y,L_Y],\qquad Q(T(V))\cong V.
$$

The first identity follows from the enveloping relation: after all positive products are killed, every bracket is killed and no additional linear relation is introduced. Hence each homogeneous [basis](../../../../../basis.md) vector of $V$ has a primitive representative in $H_*(\Omega Y;\mathbb Q)$. Choose such representatives $p_v$. Sending $v$ to $p_v$ defines an algebra map from $T(V)$ to itself whose effect on indecomposables is the identity. It is an isomorphism: $p_v=v+$ decomposable terms, and every factor in those terms has smaller positive degree than $v$. Degree induction solves recursively for each original generator and constructs the inverse. This works even with arbitrarily many generators in a degree.

Equip the source [tensor algebra](../../../../../tensor-algebra.md) with primitive generators. The map is now a Hopf-algebra isomorphism, because the chosen images are primitive. The primitives in this tensor [Hopf algebra](../../../../../hopf-algebra.md) are exactly $\mathbb L(V)$: $U(\mathbb L(V))=T(V)$ by the two universal properties, and the graded [Graded Poincaré–Birkhoff–Witt theorem](../../../../../graded-poincare-birkhoff-witt-theorem.md) gives its primitive subspace. Consequently $L_Y\cong\mathbb L(V)$, proving the forward direction without assuming a primitive coproduct for the original generators.

Conversely suppose $L_Y\cong\mathbb L(W)$ for a positively graded $W$. Choose a homogeneous [basis](../../../../../basis.md) $w_\lambda$ of $W$. Represent its corresponding [homotopy class](../../../../../homotopy-class.md) by a based sphere map $S^{|w_\lambda|+1}\to Y_{\mathbb Q}$, and combine these maps into

$$
F:Z=\bigvee_\lambda S^{|w_\lambda|+1}\longrightarrow Y_{\mathbb Q}.
$$

The [wedge sum](../../../../../wedge-sum.md) is a [reduced suspension](../../../../../reduced-suspension.md), namely $Z=\Sigma(\bigvee_\lambda S^{|w_\lambda|})$. The preceding direction, applied to this [wedge sum](../../../../../wedge-sum.md), gives its free rational [homotopy](../../../../../homotopy.md) [Lie algebra](../../../../../lie-algebra-split.md) on the sphere inclusions. Indeed these particular tensor generators are primitive because the reduced diagonal of each sphere is zero, and loop [Hurewicz homomorphism](../../../../../hurewicz-homomorphism.md) sends the adjoint sphere inclusion to that generator. Naturality of the bracket shows that $F_*$ sends the free generating [basis](../../../../../basis.md) to the prescribed free generating [basis](../../../../../basis.md) of $L_Y$. It is therefore an isomorphism of [free graded Lie algebras](../../../../../free-graded-lie-algebra.md), hence an isomorphism in every rational [homotopy](../../../../../homotopy.md) degree. The [rational Whitehead theorem](../../../../../rational-whitehead-theorem.md) makes $F$ a [rational homotopy equivalence](../../../../../rational-homotopy-equivalence.md). This proves the reverse implication and also shows that a [wedge sum](../../../../../wedge-sum.md) of spheres can be chosen as the [reduced suspension](../../../../../reduced-suspension.md).

For every chosen connected $X$ with $Y\simeq_{\mathbb Q}\Sigma X$, the required algebra statement is precisely the [Bott–Samelson theorem](../../../../../bott-samelson-theorem.md) isomorphism, transported along [rational homotopy equivalence](../../../../../rational-homotopy-equivalence.md):

$$
\boxed{H_*(\Omega Y;\mathbb Q)\cong
T(\widetilde H_*(X;\mathbb Q))
=\bigoplus_{r\ge0}\widetilde H_*(X;\mathbb Q)^{\otimes r}.}
$$

Multiplication is concatenation of tensors and the degree-zero tensor is the unit. All freeness assertions here are graded, with the Koszul signs described above.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
