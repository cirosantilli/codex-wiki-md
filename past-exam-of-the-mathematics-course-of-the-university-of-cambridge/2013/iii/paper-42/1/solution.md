<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [SU(2) group](../../../../../su-2-group.md) consists of complex $2\times2$ matrices $U$ with $U^\dagger U=I$ and $\det U=1$. The [SO(3) group](../../../../../so-3-group.md) consists of real $3\times3$ matrices $R$ with $R^TR=I$ and $\det R=1$. Differentiate these equations along a path through the identity. This gives

$$
\mathfrak{su}(2)=\{X:X^\dagger=-X,\ \operatorname{tr}X=0\},\qquad
\mathfrak{so}(3)=\{L:L^T=-L\}.
$$

Conversely the [matrix exponential](../../../../../matrix-exponential.md) of each displayed infinitesimal matrix satisfies the corresponding group equations, so these are exactly the [Lie algebras](../../../../../lie-algebra-split.md), with bracket the matrix [commutator](../../../../../commutator.md).

Using the [Pauli matrices](../../../../../pauli-matrices.md), put $t_a=-i\sigma_a/2$. They form a real basis of the [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md). The [Pauli matrix commutator identity](../../../../../pauli-matrix-commutator-identity.md) gives $[t_a,t_b]=\epsilon_{abc}t_c$. Define $J_a$ on $\mathbb R^3$ by $J_av=e_a\times v$. These are a basis of the [SO(3) Lie algebra](../../../../../so-3-lie-algebra.md); the vector triple-product identity gives $[J_a,J_b]=\epsilon_{abc}J_c$. Thus

$$
\boxed{\sum_a u_at_a\longmapsto\sum_a u_aJ_a}
$$

is a real linear bijection preserving the bracket. This is the [SU(2)-SO(3) Lie algebra isomorphism](../../../../../cross-product-model-of-su-2.md). It is a Lie-algebra isomorphism, not a group isomorphism: the [Adjoint double cover from SU(2) to SO(3)](../../../../../adjoint-double-cover-from-su-2-to-so-3.md) has kernel $\{I,-I\}$.

The [SU(3) group](../../../../../su-3-group.md) is defined similarly by $U^\dagger U=I$ and $\det U=1$ on complex $3\times3$ matrices. One [SU(2)](../../../../../su-2-group.md) subgroup is $\{\operatorname{diag}(V,1):V\in SU(2)\}$. The real orthogonal matrices with determinant one form an [SO(3) group](../../../../../so-3-group.md) subgroup, since real orthogonality is also complex unitarity.

Under the defining [group action](../../../../../group-action.md), the [group orbit](../../../../../orbit-of-a-group-action.md) of $e_1$ is exactly the unit sphere in $\mathbb C^3$:

$$
\boxed{SU(3)e_1=\{z:z^\dagger z=1\}=S^5.}
$$

Unitarity proves containment. Conversely, extend a unit vector $z$ to an orthonormal basis and use it as the first column of a unitary matrix. Multiplying the last column by the inverse of its determinant makes that determinant one without changing the first column. The [isotropy group](../../../../../stabilizer-subgroup.md) of $e_1$ must also preserve its orthogonal complement, and therefore is

$$
\boxed{\{\operatorname{diag}(1,V):V\in SU(2)\}\cong SU(2).}
$$

This proves the [unit sphere orbit of the defining special unitary action](../../../../../unit-sphere-orbit-of-the-defining-special-unitary-action.md), including $S^5\cong SU(3)/SU(2)$.

For the complex quadric, write $z=x+iy$. Its defining relation separates into

$$
|x|^2-|y|^2=1,\qquad x\cdot y=0.
$$

The Hermitian norm is then $z^\dagger z=1+2|y|^2$, which is not constant on this set. For example, $e_1$ and $\sqrt2e_1+ie_2$ both satisfy the complex bilinear relation but have Hermitian norms one and three. Since the [SU(3) group](../../../../../su-3-group.md) preserves that norm, **the quadric cannot be a single SU(3) [group orbit](../../../../../orbit-of-a-group-action.md)**. In fact it is not even invariant under the whole group: $\operatorname{diag}(e^{it},e^{-it},1)e_1$ fails the bilinear relation when $e^{2it}\ne1$.

The real [SO(3) group](../../../../../so-3-group.md) does preserve the quadric, acting simultaneously on $x$ and $y$. Its [group orbits](../../../../../orbit-of-a-group-action.md) are classified completely by $r=|y|\geq0$. For $r=0$, $y=0$ and $x$ is a real unit vector, giving the [group orbit](../../../../../orbit-of-a-group-action.md) $S^2$ and [stabilizer subgroup](../../../../../stabilizer-subgroup.md) $SO(2)$. For $r>0$, the vectors $x/\sqrt{1+r^2}$ and $y/r$ are orthonormal. Adjoining their cross product gives an oriented orthonormal frame. There is a unique rotation taking the standard frame to this one; hence the action is transitive at fixed $r$ and the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is trivial. Thus the [real rotation orbits on a complex unit quadric](../../../../../real-rotation-orbits-on-a-complex-unit-quadric.md) are

$$
\boxed{M_0\cong S^2,\qquad M_r\cong SO(3)\ (r>0),\qquad M/SO(3)\cong[0,\infty).}
$$

In particular the real subgroup does not act transitively on the whole quadric. The parametrization $x=\sqrt{1+|y|^2}\,n$ with $n\in S^2$ and $y\perp n$ also identifies the quadric, as a real manifold, with the [tangent bundle](../../../../../tangent-bundle.md) of $S^2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
