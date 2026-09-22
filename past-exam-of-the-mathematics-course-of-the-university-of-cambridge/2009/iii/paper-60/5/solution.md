<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Take a complete smooth asymptotically flat spacelike initial-data hypersurface $\Sigma$, carrying a [spin structure](../../../../../spin-structure.md), without inner boundary. Let $n$ be its future unit normal, $h$ its induced metric, and use the [extrinsic curvature](../../../../../extrinsic-curvature.md) convention $k_{ij}=-g(\nabla_i n,e_j)$. Assume the Einstein constraints, the [dominant energy condition](../../../../../dominant-energy-condition.md), and the standard decay sufficient for finite ADM charges. In one asymptotically Cartesian end it is enough here to work with $h_{ij}=\delta_{ij}+q_{ij}$, $q=O(r^{-1})$, $\partial q=O(r^{-2})$, $k=O(r^{-2})$, and the corresponding differentiated decay and integrability assumptions. The desired conclusion is positivity of the whole ADM four-momentum, not merely of the energy in one selected frame.

Introduce a commuting auxiliary spinor $\epsilon$; this is not an anticommuting gravitino field. With $\bar\epsilon=-\epsilon^\dagger\gamma^{\hat0}$ its [causal Dirac spinor current](../../../../../causal-dirac-spinor-current.md) is $K^\mu=\bar\epsilon\gamma^\mu\epsilon$, future causal. The [Nester two-form](../../../../../nester-two-form.md) is

$$
B^{\mu\nu}=\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\rho\epsilon
-\overline{\nabla_\rho\epsilon}\gamma^{\mu\nu\rho}\epsilon.
$$

It is real in these conventions and antisymmetric in $\mu,\nu$. Differentiating, the two terms quadratic in first derivatives become equal after exchanging $\nu,\rho$. The remaining terms are curvature commutators. The [Einstein tensor contraction of spin curvature](../../../../../einstein-tensor-contraction-of-spin-curvature.md) gives $\gamma^{\mu\nu\rho}\nabla_\nu\nabla_\rho=G^\mu{}_\lambda\gamma^\lambda/2$; the adjoint term supplies the other half. Thus

$$
\nabla_\nu B^{\mu\nu}
=2\overline{\nabla_\nu\epsilon}\gamma^{\mu\nu\rho}\nabla_\rho\epsilon
+G^\mu{}_\lambda K^\lambda.
$$

This is the central spinor-curvature identity, derived by differentiation rather than posited as a positivity formula.

Project onto $\Sigma$ and put $b^i=n_\mu B^{\mu i}$. In an adapted orthonormal frame $n_\mu=(-1,0,0,0)$, Clifford algebra gives

$$
b^i=-2\operatorname{Re}(\epsilon^\dagger\gamma^{ij}\nabla_j\epsilon),\qquad
n_\mu\,2\overline{\nabla_\nu\epsilon}\gamma^{\mu\nu\rho}\nabla_\rho\epsilon
=2\left(\sum_i|\nabla_i\epsilon|^2-|\gamma^i\nabla_i\epsilon|^2\right).
$$

Indeed the expansion of $|\gamma^i\nabla_i\epsilon|^2$ is $\sum_i|\nabla_i\epsilon|^2+(\nabla_i\epsilon)^\dagger\gamma^{ij}\nabla_j\epsilon$. With a Gaussian normal extension of the slice, the symmetric second fundamental form has zero contraction with the antisymmetric $B$, so the projected divergence is the intrinsic spatial divergence. This proves the [Witten-Nester identity](../../../../../witten-nester-identity.md)

$$
\boxed{D_ib^i=2\left(\sum_i|\nabla_i\epsilon|^2-|\mathcal D\epsilon|^2\right)
+G_{\mu\nu}n^\mu K^\nu,\qquad\mathcal D=\gamma^i\nabla_i.}
$$

Here $D_i$ on $b$ denotes the spatial metric derivative. On spinors, $\nabla_i$ is the [Sen spinor connection](../../../../../sen-spinor-connection.md), the restriction of the spacetime connection, not just the intrinsic three-dimensional one:

$$
\nabla_i\epsilon=D_i^{(3)}\epsilon-\frac12k_{ij}\gamma^j\gamma^{\hat0}\epsilon.
$$

The extrinsic-curvature term is essential when the data have momentum.

Choose $\epsilon$ to solve the [Witten spinor equation](../../../../../witten-spinor-equation.md), $\mathcal D\epsilon=0$, approaching a prescribed constant $\epsilon_\infty$ in the chosen end and zero constants in any other ends. The Einstein constraints identify $G_{\mu\nu}n^\mu K^\nu=8\pi G\,T_{\mu\nu}n^\mu K^\nu$. The [dominant energy condition](../../../../../dominant-energy-condition.md) makes this nonnegative because both $n$ and $K$ are future causal. Consequently the right-hand side of the identity becomes a sum of nonnegative terms.

Existence of that spinor is an analytic part of the proof, not something established by the positivity identity alone. Extend $\epsilon_\infty$ smoothly using a cutoff and solve $\mathcal D u=-\mathcal D\epsilon_0$ for a decaying correction. The spatial principal symbol $\gamma^i\xi_i$ squares to $|\xi|_h^2$, so the equation is elliptic. For a compactly supported spinor, the integrated identity gives

$$
\|\mathcal D\epsilon\|_{L^2}^2
=\|\nabla\epsilon\|_{L^2}^2+4\pi G\int_\Sigma T(n,K)\,dV\geq\|\nabla\epsilon\|_{L^2}^2.
$$

Together with the weighted asymptotic estimates this gives the coercivity needed for [elliptic existence of a Witten spinor](../../../../../elliptic-existence-of-a-witten-spinor.md). A decaying homogeneous solution would be parallel by the same identity and hence zero, excluding the kernel; the appropriate weighted elliptic solvability gives the correction. Under the stated smooth decay assumptions it has $\epsilon-\epsilon_\infty=O(r^{-1})$ and first derivative $O(r^{-2})$. The rigorous analytic step is supplied by [the spinor existence proof](https://users.math.msu.edu/users/parker/witten.pdf). This also explains why completeness, asymptotic data and the absence of uncontrolled inner boundary terms are hypotheses of the argument.

It remains to identify the boundary integral with the physical ADM charge. In the asymptotic symmetric coframe $e_i{}^a=\delta_i{}^a+q_{ia}/2+O(r^{-2})$, the leading spatial [spin connection](../../../../../spin-connection.md) is

$$
\omega_{jkl}^{(3)}=\frac12(\partial_lq_{jk}-\partial_kq_{jl})+O(r^{-3}).
$$

Insert this and the Sen correction into $b^i$. The real scalar part of $\gamma^{ij}\gamma^{kl}$ is $\delta^{il}\delta^{jk}-\delta^{ik}\delta^{jl}$; its two-gamma part has imaginary expectation and drops out. It follows that the intrinsic connection contributes $\frac12(\partial_jq_{ij}-\partial_iq_{jj})K_\infty^{\hat0}$. For the other term, symmetry of $k$ removes the three-spatial-gamma product, leaving $-(k_{ij}-kh_{ij})K_\infty^{\hat j}$. Thus the [ADM boundary term of the Nester two-form](../../../../../adm-boundary-term-of-the-nester-two-form.md) has the expansion

$$
b^i=\frac12(\partial_jq_{ij}-\partial_iq_{jj})K_\infty^{\hat0}
-(k_{ij}-kh_{ij})K_\infty^{\hat j}
-2\operatorname{Re}\bigl(\epsilon_\infty^\dagger\gamma^{ij}\partial_j(\epsilon-\epsilon_\infty)\bigr)+O(r^{-3}).
$$

The constant-spinor derivative contribution integrates to zero on a large coordinate sphere. Its coefficient is antisymmetric in $i,j$; the corresponding tangential vector on the sphere is divergence free, so integration by parts removes it. Equivalently, the flux of $\gamma^{ij}\partial_j u$ has identically zero divergence, with its asymptotic leading term having zero flux. The quadratic correction terms are $O(r^{-3})$ and their surface integrals vanish in the limit.

Define the [ADM energy](../../../../../arnowitt-deser-misner-energy.md) and [ADM momentum](../../../../../adm-momentum.md) with the same conventions:

$$
E=\frac1{16\pi G}\lim\int_{S_r}(\partial_jq_{ij}-\partial_iq_{jj})s^i\,dS,\qquad
P_i=\frac1{8\pi G}\lim\int_{S_r}(k_{ij}-kh_{ij})s^j\,dS.
$$

The boundary calculation then gives, including every normalization factor,

$$
\boxed{\frac1{8\pi G}\lim\int_{S_r}b^is_i\,dS
=EK_\infty^{\hat0}-\mathbf P\cdot\mathbf K_\infty.}
$$

This is the energy associated with the asymptotic spinor's causal translation. In the zero-momentum rest frame it is the ADM mass times $K_\infty^{\hat0}$; more generally it proves the full energy-momentum bound.

Finally apply the divergence theorem to the Witten identity. There is no inner boundary, and the spinors assigned zero at other ends give no charge there. Therefore

$$
\boxed{EK_\infty^{\hat0}-\mathbf P\cdot\mathbf K_\infty
=\frac1{4\pi G}\int_\Sigma\sum_i|\nabla_i\epsilon|^2dV
+\int_\Sigma T(n,K)\,dV\geq0.}
$$

Asymptotic constant spinors can produce every future null direction. Normalize $K_\infty^{\hat0}=1$ and choose its spatial direction along $\mathbf P$; the inequality gives

$$
\boxed{E\geq|\mathbf P|\geq0.}
$$

This establishes the [positive energy theorem](../../../../../positive-energy-theorem.md) and nonnegativity of the invariant mass when it is defined. For zero ADM energy, repeat the identity for a basis of asymptotic spinors: all become parallel and all matter contractions vanish. Their curvature integrability forces the spacetime curvature to vanish on the initial surface; the standard rigidity conclusion is that the data embed in Minkowski spacetime. Merely having a parallel null spinor in a local wave geometry would not by itself prove this global rigidity: completeness and asymptotic flatness remain essential.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
