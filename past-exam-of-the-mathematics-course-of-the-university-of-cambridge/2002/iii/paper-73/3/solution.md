<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use signature $(-,+,+,+)$ and $c=1$. The mass here is the asymptotic rest-frame [Arnowitt-Deser-Misner energy](../../../../../arnowitt-deser-misner-energy.md); it is useful to prove the stronger energy-momentum inequality. Interpret [asymptotic flatness](../../../../../asymptotically-flat-spacetime.md) with its usual differentiable falloff, for example $h_{ij}=\delta_{ij}+O(r^{-1})$, $\partial_kh_{ij}=O(r^{-2})$, and [extrinsic curvature](../../../../../extrinsic-curvature.md) $k_{ij}=O(r^{-2})$, with the additional decay/integrability needed for the charges and integrations below. The complete nonsingular slice has no inner boundary. An oriented three-dimensional slice admits a [spin structure](../../../../../spin-structure.md). If there are several asymptotically flat ends, prescribe a constant [spinor](../../../../../spinor.md) at the end whose mass is being measured and zero constants at the other ends.

Let $n$ be the future unit normal and write $\mathcal D_i=h_i{}^\mu\nabla_\mu$ for the restricted spacetime [spin connection](../../../../../spin-connection.md). This is the [Sen spinor connection](../../../../../sen-spinor-connection.md), not merely the intrinsic connection $D_i^{(3)}$:

$$
\mathcal D_i\epsilon=D_i^{(3)}\epsilon-\frac12k_{ij}\gamma^j\gamma^{\hat0}\epsilon,
\qquad k_{ij}=-g(\nabla_i n,e_j).
$$

Omitting this term on a general slice would omit the ADM momentum. Choose $\gamma^{\hat0}$ anti-Hermitian, the spatial [gamma matrices](../../../../../gamma-matrices.md) Hermitian, and $\bar\epsilon=-\epsilon^\dagger\gamma^{\hat0}$. The commuting-[spinor](../../../../../spinor.md) [Dirac current](../../../../../dirac-current.md) $V^\mu=\bar\epsilon\gamma^\mu\epsilon$ is future causal and $V^{\hat0}=|\epsilon|^2$.

The [Nester two-form](../../../../../nester-two-form.md) supplies the needed integration identity. Define

$$
B^{\mu\nu}=\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\rho\epsilon-\overline{\nabla_\rho\epsilon}\gamma^{\mu\nu\rho}\epsilon,
\qquad b^i=n_\mu B^{\mu i},
\qquad \mathscr D\epsilon=\gamma^i\mathcal D_i\epsilon.
$$

Here multiple gamma indices denote antisymmetrized products. To derive the identity, differentiate $B$, use $\nabla\gamma=0$, and antisymmetrize the two derivatives in the terms containing $\nabla\nabla\epsilon$. Their commutator is the [spinor curvature identity](../../../../../spinor-curvature-identity.md)

$$
[\nabla_\mu,\nabla_\nu]\epsilon=\frac14R_{\mu\nu ab}\gamma^{ab}\epsilon.
$$

Expansion of the gamma products and the [first Bianchi identity](../../../../../first-bianchi-identity.md) reduce this curvature contribution to an [Einstein tensor](../../../../../einstein-tensor.md) contraction. It vanishes for the [Vacuum Einstein equations](../../../../../vacuum-einstein-equations.md). At a point in a normal-adapted orthonormal frame the remaining contraction is

$$
-2(\mathcal D_i\epsilon)^\dagger\gamma^{ij}\mathcal D_j\epsilon
=2\bigl(|\mathcal D\epsilon|^2-|\gamma^i\mathcal D_i\epsilon|^2\bigr),
$$

because $\gamma^i\gamma^j=\delta^{ij}+\gamma^{ij}$. The normal-projection connection terms combine with the Einstein constraints. Thus, in vacuum, the [Witten-Nester identity](../../../../../witten-nester-identity.md) is

$$
D_i b^i=2\bigl(|\mathcal D\epsilon|^2-|\mathscr D\epsilon|^2\bigr).
$$

All norms here use the positive [spinor](../../../../../spinor.md) norm on the spacelike slice. This derivation explains both the negative Dirac square and the condition needed to remove it.

Solve the [Witten spinor equation](../../../../../witten-spinor-equation.md) $\mathscr D\epsilon=0$ with $\epsilon\to\epsilon_\infty$. The existence step is part of the argument. Extend the desired constant smoothly from infinity to a [spinor](../../../../../spinor.md) $\epsilon_0$ and seek a decaying correction $\chi$ satisfying $\mathscr D\chi=-\mathscr D\epsilon_0$. The principal symbol $\gamma^i\xi_i$ squares to $|\xi|^2I$, so this is an [elliptic differential operator](../../../../../elliptic-differential-operator.md). On the asymptotically flat ends, the Euclidean Dirac estimate and the weighted estimate from [Hardy's inequality](../../../../../hardy-s-inequality.md) control the decaying correction; on a compact interior the usual elliptic estimate applies. Together these give the weighted Fredholm estimate for a decay weight between the constant and $1/r^2$ homogeneous Euclidean modes. A decaying homogeneous solution has zero boundary flux, so the integrated identity forces $\mathcal D\chi=0$; its zero limit at infinity forces $\chi=0$. The [formal adjoint](../../../../../formal-adjoint.md) has the same obstruction: with the conventions above $\mathscr D=\gamma^iD_i^{(3)}-k\gamma^{\hat0}/2$ is formally skew-adjoint. Consequently the decaying kernel and cokernel vanish, and the [Fredholm alternative](../../../../../fredholm-alternative.md) gives the required correction. Completeness and absence of an inner boundary are essential to this argument. This is the [elliptic existence of a Witten spinor](../../../../../elliptic-existence-of-a-witten-spinor.md), rather than an assumption that an arbitrary prescribed [spinor](../../../../../spinor.md) solves the equation.

For completeness, identify the asymptotic flux. Expanding the intrinsic [spin connection](../../../../../spin-connection.md) in an asymptotically Cartesian orthonormal frame gives

$$
b^i=\frac12(\partial_jh_{ij}-\partial_i h_{jj})V_\infty^0-(k_{ij}-kh_{ij})V_\infty^j+\text{terms with zero limiting flux}.
$$

The derivative of the decaying [spinor](../../../../../spinor.md) correction has zero linear flux by antisymmetry of its gamma-matrix coefficient; quadratic correction terms decay away. Since the ADM energy and momentum have the respective $1/(16\pi G)$ and $1/(8\pi G)$ surface normalizations, the [ADM boundary term of the Nester two-form](../../../../../adm-boundary-term-of-the-nester-two-form.md) is

$$
\lim_{r\to\infty}\int_{S_r}b^i s_i\,dS
=8\pi G\bigl(EV_\infty^0-P_iV_\infty^i\bigr).
$$

Apply the [divergence theorem](../../../../../divergence-theorem.md) to the complete slice and use $\mathscr D\epsilon=0$. There is no inner flux to discard:

$$
8\pi G\bigl(EV_\infty^0-P_iV_\infty^i\bigr)=2\int_\Sigma|\mathcal D\epsilon|^2\,d\Sigma\ge0.
$$

Asymptotic constant [spinors](../../../../../spinor.md) can be chosen with a future null current in any specified spatial direction. Choosing the direction of $\mathbf P$ yields

$$
\boxed{E\ge|\mathbf P|\ge0.}
$$

In particular, the rest-frame mass is nonnegative. This proves the [positive energy theorem](../../../../../positive-energy-theorem.md) in the vacuum setting rather than applying it as an unexplained bound.

If this mass is zero, then $E=0$ in the asymptotic rest frame and the inequality gives $\mathbf P=0$. The same identity with any nonzero $\epsilon_\infty$ has zero right-hand side. Smoothness then makes its integrand vanish pointwise:

$$
\boxed{\mathcal D_i\epsilon=h_i{}^j\nabla_j\epsilon=0.}
$$

The [spinor](../../../../../spinor.md) is nonzero, since it has nonzero asymptotic value. This is a [spinor](../../../../../spinor.md) parallel along $\Sigma$; no time-parallel condition has yet been inferred merely from the integral.

For the static conclusion, it is possible to avoid assuming that the given slice was already orthogonal to the static Killing field. Because $E=\mathbf P=0$, repeat the zero-energy construction for four linearly independent asymptotic Dirac spinors. Parallel transport by the [Sen spinor connection](../../../../../sen-spinor-connection.md) is invertible, so the resulting spinors form a basis everywhere on $\Sigma$. Tangential curvature annihilates each of them:

$$
[\mathcal D_i,\mathcal D_j]\epsilon_A
=\frac14R_{ijab}\gamma^{ab}\epsilon_A=0,\qquad A=1,\ldots,4.
$$

Thus $R_{ijab}\gamma^{ab}=0$ as an operator. The six antisymmetric gamma products give a faithful [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md), so $R_{ijab}=0$ for tangential $i,j$. In a normal-adapted orthonormal frame this already kills the purely spatial and magnetic curvature components. The remaining components vanish by the [Vacuum Einstein equations](../../../../../vacuum-einstein-equations.md):

$$
0=R_{ij}=-R_{\hat0 i\hat0 j}+\sum_kR_{kikj}
\quad\Longrightarrow\quad R_{\hat0 i\hat0 j}=0.
$$

Consequently the full spacetime [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) vanishes on $\Sigma$.

A static [Killing vector field](../../../../../killing-vector-field.md) generates isometries and preserves this curvature. Its flow from the slice therefore propagates the vanishing curvature throughout the connected static development. Extend one of the spinors by spacetime parallel transport along these time orbits, so that $\nabla_t\epsilon=0$. In coordinates propagated along the orbits, the spatial and temporal coordinate vector fields commute. Zero spin curvature then gives

$$
\nabla_t(\nabla_i\epsilon)=\nabla_i(\nabla_t\epsilon)=0.
$$

The initial tangential derivative is zero, so it stays zero. This constructs the required nonzero spacetime [parallel spinor](../../../../../parallel-spinor.md); the initial parallel frame also removes any spin-holonomy ambiguity inherited from loops in $\Sigma$. The [static zero-energy parallel-spinor rigidity](../../../../../static-zero-energy-parallel-spinor-rigidity.md) conclusion is

$$
\boxed{\nabla_\mu\epsilon=0.}
$$

An equivalent check in a regular orthogonal static slicing is to write $ds^2=-N^2dt^2+h_{ij}dx^i dx^j$. The slice has zero [extrinsic curvature](../../../../../extrinsic-curvature.md). An intrinsic parallel spinor forces the spatial [Ricci tensor](../../../../../ricci-tensor.md) to vanish by contracting its spin-curvature identity and using the invertibility of [Clifford multiplication](../../../../../clifford-multiplication.md) by a nonzero real vector. By [three-dimensional curvature from the Ricci tensor](../../../../../three-dimensional-curvature-from-the-ricci-tensor.md), $h$ is flat. The static vacuum equation $D_iD_jN=N R_{ij}(h)$ then makes the lapse gradient parallel, and asymptotic normalization forces $N=1$. The temporal spin connection vanishes as well.

An explicit example is [Minkowski spacetime](../../../../../minkowski-spacetime.md), $ds^2=-dt^2+dx^2+dy^2+dz^2$, where every constant spinor in a Cartesian tetrad is a spacetime [parallel spinor](../../../../../parallel-spinor.md) and the ADM mass is zero. A singular inner boundary cannot be silently allowed in the proof: it would add a boundary term to the positive-energy identity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
