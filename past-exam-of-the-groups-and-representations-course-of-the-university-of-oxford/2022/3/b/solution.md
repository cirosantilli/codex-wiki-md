<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $X=\begin{pmatrix}A&B\\C&D\end{pmatrix}$. Commuting with all $\operatorname{diag}(U_1,U_2)$ requires

$$
AU_1=U_1A,\quad DU_2=U_2D,\quad BU_2=U_1B,\quad CU_1=U_2C.
$$

For $n_1,n_2\geq2$, the defining [complex representations](../../../../complex-representation.md) of each factor are [irreducible](../../../../irreducible-representation.md). [Schur lemma](../../../../schur-s-lemma.md) gives $A=zI_{n_1}$ and $D=wI_{n_2}$. The two block [vector spaces](../../../../vector-space-split.md) are inequivalent [representations](../../../../group-representation.md) of the product [group](../../../../group-split.md), even when $n_1=n_2$: the first factor acts nontrivially on just the first block. Thus their off-diagonal [intertwiners](../../../../intertwiner.md) vanish, $B=C=0$. [Unitarity](../../../../unitary-operator.md) and the unit [determinant](../../../../determinant.md) give

$$
\boxed{C_G(H)=\{\operatorname{diag}(zI_{n_1},wI_{n_2}):|z|=|w|=1,\ z^{n_1}w^{n_2}=1\}.}
$$

**The assertion that this full group is always a circle needs correction.** Put $d=\gcd(n_1,n_2)$, $a=n_1/d$, $b=n_2/d$. The continuous [group homomorphism](../../../../group-homomorphism.md)

$$
(z,w)\longmapsto z^aw^b
$$

maps this [centralizer](../../../../centralizer.md) onto the $d$th [roots of unity](../../../../root-of-unity.md). Its [kernel](../../../../kernel-of-a-linear-map-split.md) is the [identity component of a Lie group](../../../../identity-component-of-a-lie-group.md), parametrized injectively by $e^{i\theta}\mapsto(e^{ib\theta},e^{-ia\theta})$. Coprimality of $a,b$ proves injectivity; a [Bezout identity](../../../../bezout-s-identity.md) proves that this parametrization exhausts the [kernel](../../../../kernel-of-a-linear-map-split.md). Extending the primitive integer row $(a,b)$ to a determinant-one integer matrix gives coordinates in which the constraint is simply $t^d=1$. Consequently

$$
\boxed{C_G(H)\cong U(1)\times\mathbb Z_d,\qquad C_G(H)^0\cong U(1).}
$$

For a concrete counterexample, take $n_1=n_2=2$. The constraint is $(zw)^2=1$, giving two separate circles $zw=1$ and $zw=-1$. The element $\operatorname{diag}(I_2,-I_2)$ lies in the second component, so this [centralizer](../../../../centralizer.md) cannot be isomorphic as a [Lie group](../../../../lie-group.md) to the connected [circle group](../../../../circle-group.md).

For the intended specialization of this [centralizer of two special unitary blocks](../../../../centralizer-of-two-special-unitary-blocks.md), $d=\gcd(2,3)=1$ and therefore the full [centralizer](../../../../centralizer.md) really is a [circle group](../../../../circle-group.md):

$$
\boxed{U_c(1)=\{e^{i\theta X_c}:\theta\in\mathbb R/2\pi\mathbb Z\},\qquad
X_c=\operatorname{diag}(3,3,-2,-2,-2).}
$$

We use this primitive integer [U(1) charge](../../../../u-1-charge.md) normalization below. If exactly one $n_i$ equals $1$ and the other is at least $2$, the same block-scalar formula still holds. If $n_1=n_2=1$, both factors are trivial and the [centralizer](../../../../centralizer.md) is all of [SU(2)](../../../../su-2-group.md), another exception to the printed claim.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
