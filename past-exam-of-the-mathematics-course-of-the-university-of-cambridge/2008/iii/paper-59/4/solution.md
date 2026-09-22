<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Poisson manifold](../../../../../poisson-manifold.md) is a smooth manifold $M$ with a bilinear bracket on smooth functions that is antisymmetric, obeys the Leibniz rule and satisfies the [Jacobi identity](../../../../../jacobi-identity.md). Equivalently, a [Poisson tensor](../../../../../poisson-tensor.md) $\pi$ gives $\{f,g\}=\pi(df,dg)$. Its rank need not be constant or maximal. Here define Hamiltonian evolution by $X_Hf=\{f,H\}$, agreeing with the canonical bracket $\{q^i,p_j\}=\delta^i_j$.

A smooth [Lie group action](../../../../../lie-group-action.md) sends each $x$ along its orbit $Gx$, with [stabilizer](../../../../../stabilizer-subgroup.md) $G_x$. If the action is free and proper, the orbit space is a smooth quotient manifold and the projection is a submersion. Without these hypotheses the quotient can have singular orbit-type strata, or even fail to be Hausdorff. For an action preserving the [Poisson bracket](../../../../../poisson-bracket.md), invariant functions form a Poisson subalgebra. On a smooth quotient $M/G$, their identification with smooth quotient functions defines

$$
\{\bar f,\bar g\}_{M/G}\circ r=\{\bar f\circ r,\bar g\circ r\}_M.
$$

Thus $r$ is a [Poisson map](../../../../../poisson-map.md). The quotient is generally Poisson, not necessarily symplectic: different reduced [momentum](../../../../../momentum.md) sectors can be different leaves. An arbitrary smooth [group action](../../../../../group-action.md) alone does not guarantee this bracket descent.

For a [Lie group](../../../../../lie-group.md) $G$, conjugation $h\mapsto ghg^{-1}$ differentiates at the identity to the [Adjoint representation of a Lie group](../../../../../adjoint-representation-of-a-lie-group.md), $\operatorname{Ad}_g:\mathfrak g\to\mathfrak g$. Its infinitesimal version is $\operatorname{ad}_\xi\eta=[\xi,\eta]$. The [coadjoint representation](../../../../../coadjoint-representation.md) on the dual space is defined by

$$
\langle\operatorname{Ad}^*_g\ell,\xi\rangle=\langle\ell,\operatorname{Ad}_{g^{-1}}\xi\rangle,\qquad\langle\operatorname{ad}^*_\xi\ell,\eta\rangle=-\langle\ell,[\xi,\eta]\rangle.
$$

The inverse in the first formula makes this a left action. These definitions distinguish the representation on infinitesimal generators from its dual action on momenta.

There is a natural positive [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) on $\mathfrak g^*$:

$$
\boxed{\{F,G\}_+(\ell)=\langle\ell,[dF_\ell,dG_\ell]\rangle.}
$$

The differentials lie in $(\mathfrak g^*)^*\simeq\mathfrak g$. In a basis with $[e_a,e_b]=c_{ab}{}^ce_c$, linear coordinates satisfy $\{\ell_a,\ell_b\}_+=c_{ab}{}^c\ell_c$. The bracket extends by the chain rule and Leibniz rule to smooth functions. Its coordinate Jacobi condition reduces precisely to the [Jacobi identity](../../../../../jacobi-identity.md) for $c_{ab}{}^c$, proving that it is Poisson. Reversing its overall sign also gives a [Poisson bracket](../../../../../poisson-bracket.md) and is useful for body-frame conventions below.

On a general [Poisson manifold](../../../../../poisson-manifold.md), the vectors $X_f$ span a distribution. The [Jacobi identity](../../../../../jacobi-identity.md) closes this family under commutators, and its orbits under Hamiltonian flows form the [symplectic foliation](../../../../../symplectic-foliation.md). On each leaf the induced two-form satisfies

$$
\omega(X_f,X_g)=\{f,g\}.
$$

It is well-defined after quotienting out differential covectors giving zero [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md), is nondegenerate on the leaf, and is closed by the [Jacobi identity](../../../../../jacobi-identity.md). Leaf dimensions can vary, so ordinary constant-rank foliation terminology must be qualified. A Hamiltonian trajectory remains in one leaf; a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md) is constant along all such trajectories, but its level set can contain more than one leaf.

For $\mathfrak g^*$, $X_F(\ell)=\operatorname{ad}^*_{dF_\ell}\ell$ under the convention above. Hence the connected [coadjoint orbits](../../../../../coadjoint-orbit.md) are exactly its [symplectic leaves](../../../../../symplectic-leaf.md) for connected $G$; for disconnected $G$, take connected orbit components. The orbit two-form is the [Kirillov–Kostant–Souriau symplectic form](../../../../../kirillov-kostant-souriau-symplectic-form.md):

$$
\boxed{\omega_\ell(\operatorname{ad}^*_\xi\ell,\operatorname{ad}^*_\eta\ell)=\langle\ell,[\xi,\eta]\rangle.}
$$

If a generator is in the [stabilizer](../../../../../stabilizer-subgroup.md), its pairing with every bracket vanishes, proving independence of the choice of tangent generator. Conversely, vanishing pairing with all tangent generators puts it in that [stabilizer](../../../../../stabilizer-subgroup.md), proving nondegeneracy. The cyclic derivative relation giving $d\omega=0$ is the [Lie algebra](../../../../../lie-algebra-split.md) [Jacobi identity](../../../../../jacobi-identity.md). This explains the symplectic structure of the orbit rather than just naming it.

Identify the [SO(3) Lie algebra](../../../../../so-3-lie-algebra.md) with $\mathbb R^3$ by the hat map $\widehat{\boldsymbol\xi}\mathbf v=\boldsymbol\xi\times\mathbf v$. Its Lie bracket becomes the vector cross product, and the invariant Euclidean pairing identifies the dual with angular-momentum vectors $\mathbf M$. The [coadjoint action](../../../../../coadjoint-representation.md) is ordinary rotation, with infinitesimal action $\boldsymbol\xi\times\mathbf M$. Therefore its nonzero orbits are spheres $|\mathbf M|=r$; the origin is a zero-dimensional leaf. In these coordinates,

$$
\{F,G\}_+=\mathbf M\cdot(\nabla F\times\nabla G),\qquad C(\mathbf M)=|\mathbf M|^2
$$

is a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md), since its gradient is parallel to $\mathbf M$. For tangent vectors $\mathbf v,\mathbf w$ to a nonzero sphere, the positive orbit form is

$$
\omega_{\mathbf M}(\mathbf v,\mathbf w)=\frac{\mathbf M\cdot(\mathbf v\times\mathbf w)}{r^2}.
$$

Its area integral with the corresponding orientation is $4\pi r$, and it reverses sign with the negative bracket.

For a torque-free [rigid body](../../../../../rigid-body-dynamics.md), choose body [angular momentum](../../../../../angular-momentum.md) $\mathbf M$ and principal moments $I_1,I_2,I_3>0$. Reduction of $T^*SO(3)$ by spatial rotations gives the body-frame negative [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) and Hamiltonian

$$
\{F,G\}_{\mathrm{body}}=-\mathbf M\cdot(\nabla F\times\nabla G),\qquad H=\frac12\sum_{i=1}^3\frac{M_i^2}{I_i}.
$$

Keeping the sign convention explicit is essential: using the positive bracket with the same body identification would reverse the Euler evolution. The negative bracket gives

$$
\boxed{\dot{\mathbf M}=\mathbf M\times\boldsymbol\Omega,\qquad\Omega_i=M_i/I_i,\qquad\dot M_1=(I_3^{-1}-I_2^{-1})M_2M_3,}
$$

with cyclic expressions for the other two components. These are the [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md). The Hamiltonian and $C$ are conserved because $\boldsymbol\Omega\cdot(\mathbf M\times\boldsymbol\Omega)=0$ and $\mathbf M\cdot(\mathbf M\times\boldsymbol\Omega)=0$. Trajectories therefore lie on intersections of energy ellipsoids with [momentum](../../../../../momentum.md) spheres, the latter being the [symplectic leaves](../../../../../symplectic-leaf.md).

The body's orientation is reconstructed from $\dot R=R\widehat{\boldsymbol\Omega}$. Its spatial [momentum](../../../../../momentum.md) $\mathbf J=R\mathbf M$ is constant, since $\dot{\mathbf J}=R(\boldsymbol\Omega\times\mathbf M+\mathbf M\times\boldsymbol\Omega)=0$. Thus the body [momentum](../../../../../momentum.md) need not be constant even though the spatial conserved [momentum](../../../../../momentum.md) is. **Poisson reduction retains the dynamics and its [momentum](../../../../../momentum.md) leaves while eliminating orientation variables; the unreduced motion is recovered by reconstruction.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
