# Paper 73

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper73.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper73.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

In a globally static region, choose the time coordinate along the future timelike [Killing vector field](../../../general-relativity.md#killing-vector-field) $K=\partial_t$. A [positive-frequency solution](../../../quantum-field-theory.md#positive-frequency-solution) of the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) has $i\mathcal L_Kp_i=\omega_i p_i$, with $\omega_i>0$. Assume appropriate boundary conditions and a [Cauchy surface](../../../general-relativity.md#cauchy-surface) so that the conserved [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) is

$$
(f,g)=i\int_\Sigma d\Sigma^a\bigl(f^*\nabla_ag-g\nabla_af^*\bigr).
$$

For a real scalar, take the negative-frequency modes to be $n_i=p_i^*$. Choose a complete normalized basis with

$$
(p_i,p_j)=\delta_{ij},\qquad(n_i,n_j)=-\delta_{ij},\qquad(p_i,n_j)=0.
$$

The negative norm of the conjugate modes is crucial; this is not a positive-definite inner product on all classical solutions.

Promote the real [Klein-Gordon field](../../../quantum-field-theory.md#klein-gordon-field) to the operator

$$
\widehat\phi=\sum_i(p_i a_i+n_i a_i^\dagger),\qquad
[a_i,a_j^\dagger]=\delta_{ij},\quad[a_i,a_j]=0.
$$

These [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) implement the canonical field and conjugate-momentum commutator. The static [vacuum state in a stationary spacetime](../../../quantum-field-theory.md#vacuum-state-in-a-stationary-spacetime) satisfies $a_i|0\rangle=0$, and the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is a sum of oscillators, $\sum_i\omega_i(a_i^\dagger a_i+1/2)$ before zero-point regularization. Continuous labels replace sums by correctly normalized integrals. For a complex charged scalar there are separate particle and antiparticle oscillators, with the same mode-mixing argument in each sector.

Choose independently normalized past and future bases, and use the matrix indices of the question. Complex conjugation of the future positive-frequency expansion immediately gives

$$
\boxed{n_i^+=\sum_j\bigl(n_j^- A_{ji}^*+p_j^- B_{ji}^*\bigr).}
$$

Conservation of the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) gives $A^\dagger A-B^\dagger B=I$ and $A^\dagger B^*-B^\dagger A^*=0$ in this column-index convention. These ensure preservation of the [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation).

Let $a_j$ annihilate past modes and $b_i$ annihilate future modes. Extracting the future coefficient from the field gives the [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation)

$$
b_i=(p_i^+,\widehat\phi)=\sum_j\bigl(A_{ji}^*a_j-B_{ji}^*a_j^\dagger\bigr).
$$

The minus sign follows from $(n_j^-,n_k^-)=-\delta_{jk}$. In the [in-vacuum](../../../quantum-field-theory.md#in-vacuum), only $\langle0_{\rm in}|a_j a_k^\dagger|0_{\rm in}\rangle=\delta_{jk}$ contributes to the expectation of the future [number operator](../../../quantum-mechanics.md#number-operator). Therefore

$$
\boxed{\langle0_{\rm in}|b_i^\dagger b_i|0_{\rm in}\rangle=\sum_j|B_{ji}|^2=(B^\dagger B)_{ii}.}
$$

This is [particle number from Bogoliubov coefficients](../../../quantum-field-theory.md#particle-number-from-bogoliubov-coefficients): the intervening time-dependent geometry makes a past positive-frequency mode contain a future negative-frequency component. In infinite volume, localized [wave packets](../../../wave-equation.md#wave-packet) avoid delta-function normalization artifacts; a common Fock-space implementation needs the usual square-summability condition on the creation-mixing coefficients.

For gravitational collapse, the initial vacuum can be defined before the hole forms, while late outgoing modes are defined using the asymptotic stationary time at [future null infinity](../../../general-relativity.md#future-null-infinity). The complete future basis also includes modes falling through the [event horizon](../../../general-relativity.md#event-horizon); exterior outgoing modes alone are not a complete basis of all propagated data. Tracing an outgoing mode backwards near a nonextremal horizon gives the exponential ray relation $v=v_H-Ce^{-\kappa u}$, where $u$ is late retarded time and $\kappa$ is the [surface gravity](../../../general-relativity.md#surface-gravity). An outgoing factor $e^{-i\omega u}$ becomes proportional to $(v_H-v)^{i\omega/\kappa}$ in the early advanced coordinate, and contains both frequency signs when Fourier decomposed there. Their squared Bogoliubov-coefficient ratio is $e^{-2\pi\omega/\kappa}$; the canonical normalization then gives a Bose factor $(e^{2\pi\omega/\kappa}-1)^{-1}$, multiplied by the [greybody factor](../../../general-relativity.md#greybody-factor), the transmission probability through the exterior potential. Thus [Hawking radiation](../../../general-relativity.md#hawking-radiation) has temperature $T_H=\kappa/(2\pi)$ in units $\hbar=k_B=c=1$, with [greybody factor](../../../general-relativity.md#greybody-factor) modifications to the spectrum. This is a free-field calculation on a fixed or slowly evolving background; eventual backreaction is an additional problem, and the nonextremal exponential map must not be blindly used when $\kappa=0$.

## 2

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

[Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem) states that the area of later cross-sections of a classical future [event horizon](../../../general-relativity.md#event-horizon) cannot be smaller than that of earlier cross-sections, including the sum over initially disconnected components. Its hypotheses include the [null energy condition](../../../general-relativity.md#null-energy-condition), the Einstein equations, and the global regularity/predictability conditions that exclude future naked pathologies of the horizon generators. A convenient sufficient version assumes those generators are future complete. Without the energy and global hypotheses the assertion is not unconditional.

Let $k^a$ be an affinely parametrized null generator, with expansion $\theta$. Because the horizon is a [null hypersurface](../../../general-relativity.md#null-hypersurface), the generator congruence has zero [null twist](../../../geodesic-congruence.md#null-twist). The [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) in four dimensions gives

$$
\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}-R_{ab}k^ak^b
\le-\frac12\theta^2.
$$

The [null shear](../../../geodesic-congruence.md#null-shear) square is nonnegative and the [null energy condition](../../../general-relativity.md#null-energy-condition) makes $R_{ab}k^ak^b=8\pi G T_{ab}k^ak^b\ge0$; a cosmological term has zero null contraction. Suppose $\theta(\lambda_0)<0$. Integration of this inequality forces $\theta\to-\infty$ within affine distance at most $2/|\theta(\lambda_0)|$. This produces a focal point to the initial horizon cross-section. Beyond it the [null geodesic](../../../special-relativity.md#null-geodesic) cannot remain on an [achronal boundary](../../../general-relativity.md#achronal-boundary), whereas an [event horizon](../../../general-relativity.md#event-horizon) is precisely such a boundary. Future completeness, or the corresponding standard predictability condition ensuring continuation over this interval, gives the contradiction. Hence

$$
\theta\ge0,\qquad \frac{d(dA)}{d\lambda}=\theta\,dA\ge0.
$$

This proves the local area increase along every smooth generator bundle. Generators can enter the horizon at past crease points, but cannot leave through future endpoints on a regular horizon under these hypotheses. New generators add area, rather than subtracting it, so the result extends across the nonsmooth merger set and to whole horizon cross-sections. This is the [future-complete horizon focusing proof of the area theorem](../../../general-relativity.md#future-complete-horizon-focusing-proof-of-the-area-theorem).

Choose an early cross-section with the two separate components of areas $A_1,A_2$, and a later cross-section of the settled merged hole. Following the old generators forward maps their area elements injectively into the later horizon; a future crossing/focal point would violate the same achronality argument. Each element has nondecreased area. Any additional generators contribute nonnegative area, giving

$$
\boxed{A_3\ge A_1+A_2.}
$$

This is a comparison of event-horizon cross-sections, not an assertion that set containment alone bounds the areas of arbitrary apparent horizons.

For a [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime), $r_h=2Gm/c^2$ and $A=4\pi r_h^2=16\pi G^2m^2/c^4$. Applying the merger inequality to the two equal initial masses and the final Schwarzschild mass gives

$$
\frac{16\pi G^2M^2}{c^4}\ge\frac{32\pi G^2m^2}{c^4},\qquad
\boxed{M\ge\sqrt2\,m.}
$$

For initially well-separated holes at rest, with no extra incoming energy or external work, energy conservation gives $E_{\rm rad}=(2m-M)c^2$. The [area bound on equal-mass Schwarzschild merger radiation](../../../general-relativity.md#area-bound-on-equal-mass-schwarzschild-merger-radiation) is consequently

$$
\boxed{E_{\rm rad}\le(2-\sqrt2)mc^2,\qquad
\frac{E_{\rm rad}}{2mc^2}\le1-\frac1{\sqrt2}\simeq29.3\%.}
$$

This is the maximum permitted by the area/energy inequalities, not a demonstration that a dynamical merger attains it. A reversible limiting area change would be needed to saturate the bound. If initial separation, binding energy or external agents change the initial total energy, replace $2mc^2$ by that energy when computing escaped radiation. Quantum evaporation does not contradict the theorem: the classical energy-condition hypotheses are not retained unchanged in that setting.

## 3

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use signature $(-,+,+,+)$ and $c=1$. The mass here is the asymptotic rest-frame [Arnowitt-Deser-Misner energy](../../../general-relativity.md#arnowitt-deser-misner-energy); it is useful to prove the stronger energy-momentum inequality. Interpret [asymptotic flatness](../../../general-relativity.md#asymptotically-flat-spacetime) with its usual differentiable falloff, for example $h_{ij}=\delta_{ij}+O(r^{-1})$, $\partial_kh_{ij}=O(r^{-2})$, and [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature) $k_{ij}=O(r^{-2})$, with the additional decay/integrability needed for the charges and integrations below. The complete nonsingular slice has no inner boundary. An oriented three-dimensional slice admits a [spin structure](../../../riemannian-geometry.md#spin-structure). If there are several asymptotically flat ends, prescribe a constant [spinor](../../../algebra.md#spinor) at the end whose mass is being measured and zero constants at the other ends.

Let $n$ be the future unit normal and write $\mathcal D_i=h_i{}^\mu\nabla_\mu$ for the restricted spacetime [spin connection](../../../connection-1-form.md#spin-connection). This is the [Sen spinor connection](../../../general-relativity.md#sen-spinor-connection), not merely the intrinsic connection $D_i^{(3)}$:

$$
\mathcal D_i\epsilon=D_i^{(3)}\epsilon-\frac12k_{ij}\gamma^j\gamma^{\hat0}\epsilon,
\qquad k_{ij}=-g(\nabla_i n,e_j).
$$

Omitting this term on a general slice would omit the ADM momentum. Choose $\gamma^{\hat0}$ anti-Hermitian, the spatial [gamma matrices](../../../algebra.md#gamma-matrices) Hermitian, and $\bar\epsilon=-\epsilon^\dagger\gamma^{\hat0}$. The commuting-[spinor](../../../algebra.md#spinor) [Dirac current](../../../quantum-field-theory.md#dirac-current) $V^\mu=\bar\epsilon\gamma^\mu\epsilon$ is future causal and $V^{\hat0}=|\epsilon|^2$.

The [Nester two-form](../../../general-relativity.md#nester-two-form) supplies the needed integration identity. Define

$$
B^{\mu\nu}=\bar\epsilon\gamma^{\mu\nu\rho}\nabla_\rho\epsilon-\overline{\nabla_\rho\epsilon}\gamma^{\mu\nu\rho}\epsilon,
\qquad b^i=n_\mu B^{\mu i},
\qquad \mathscr D\epsilon=\gamma^i\mathcal D_i\epsilon.
$$

Here multiple gamma indices denote antisymmetrized products. To derive the identity, differentiate $B$, use $\nabla\gamma=0$, and antisymmetrize the two derivatives in the terms containing $\nabla\nabla\epsilon$. Their commutator is the [spinor curvature identity](../../../connection-1-form.md#spinor-curvature-identity)

$$
[\nabla_\mu,\nabla_\nu]\epsilon=\frac14R_{\mu\nu ab}\gamma^{ab}\epsilon.
$$

Expansion of the gamma products and the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity) reduce this curvature contribution to an [Einstein tensor](../../../general-relativity.md#einstein-tensor) contraction. It vanishes for the [Vacuum Einstein equations](../../../general-relativity.md#vacuum-einstein-equations). At a point in a normal-adapted orthonormal frame the remaining contraction is

$$
-2(\mathcal D_i\epsilon)^\dagger\gamma^{ij}\mathcal D_j\epsilon
=2\bigl(|\mathcal D\epsilon|^2-|\gamma^i\mathcal D_i\epsilon|^2\bigr),
$$

because $\gamma^i\gamma^j=\delta^{ij}+\gamma^{ij}$. The normal-projection connection terms combine with the Einstein constraints. Thus, in vacuum, the [Witten-Nester identity](../../../general-relativity.md#witten-nester-identity) is

$$
D_i b^i=2\bigl(|\mathcal D\epsilon|^2-|\mathscr D\epsilon|^2\bigr).
$$

All norms here use the positive [spinor](../../../algebra.md#spinor) norm on the spacelike slice. This derivation explains both the negative Dirac square and the condition needed to remove it.

Solve the [Witten spinor equation](../../../general-relativity.md#witten-spinor-equation) $\mathscr D\epsilon=0$ with $\epsilon\to\epsilon_\infty$. The existence step is part of the argument. Extend the desired constant smoothly from infinity to a [spinor](../../../algebra.md#spinor) $\epsilon_0$ and seek a decaying correction $\chi$ satisfying $\mathscr D\chi=-\mathscr D\epsilon_0$. The principal symbol $\gamma^i\xi_i$ squares to $|\xi|^2I$, so this is an [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator). On the asymptotically flat ends, the Euclidean Dirac estimate and the weighted estimate from [Hardy's inequality](../../../real-analysis.md#hardy-s-inequality) control the decaying correction; on a compact interior the usual elliptic estimate applies. Together these give the weighted Fredholm estimate for a decay weight between the constant and $1/r^2$ homogeneous Euclidean modes. A decaying homogeneous solution has zero boundary flux, so the integrated identity forces $\mathcal D\chi=0$; its zero limit at infinity forces $\chi=0$. The [formal adjoint](../../../hilbert-space.md#formal-adjoint) has the same obstruction: with the conventions above $\mathscr D=\gamma^iD_i^{(3)}-k\gamma^{\hat0}/2$ is formally skew-adjoint. Consequently the decaying kernel and cokernel vanish, and the [Fredholm alternative](../../../compact-operator.md#fredholm-alternative) gives the required correction. Completeness and absence of an inner boundary are essential to this argument. This is the [elliptic existence of a Witten spinor](../../../general-relativity.md#elliptic-existence-of-a-witten-spinor), rather than an assumption that an arbitrary prescribed [spinor](../../../algebra.md#spinor) solves the equation.

For completeness, identify the asymptotic flux. Expanding the intrinsic [spin connection](../../../connection-1-form.md#spin-connection) in an asymptotically Cartesian orthonormal frame gives

$$
b^i=\frac12(\partial_jh_{ij}-\partial_i h_{jj})V_\infty^0-(k_{ij}-kh_{ij})V_\infty^j+\text{terms with zero limiting flux}.
$$

The derivative of the decaying [spinor](../../../algebra.md#spinor) correction has zero linear flux by antisymmetry of its gamma-matrix coefficient; quadratic correction terms decay away. Since the ADM energy and momentum have the respective $1/(16\pi G)$ and $1/(8\pi G)$ surface normalizations, the [ADM boundary term of the Nester two-form](../../../general-relativity.md#adm-boundary-term-of-the-nester-two-form) is

$$
\lim_{r\to\infty}\int_{S_r}b^i s_i\,dS
=8\pi G\bigl(EV_\infty^0-P_iV_\infty^i\bigr).
$$

Apply the [divergence theorem](../../../calculus.md#divergence-theorem) to the complete slice and use $\mathscr D\epsilon=0$. There is no inner flux to discard:

$$
8\pi G\bigl(EV_\infty^0-P_iV_\infty^i\bigr)=2\int_\Sigma|\mathcal D\epsilon|^2\,d\Sigma\ge0.
$$

Asymptotic constant [spinors](../../../algebra.md#spinor) can be chosen with a future null current in any specified spatial direction. Choosing the direction of $\mathbf P$ yields

$$
\boxed{E\ge|\mathbf P|\ge0.}
$$

In particular, the rest-frame mass is nonnegative. This proves the [positive energy theorem](../../../general-relativity.md#positive-energy-theorem) in the vacuum setting rather than applying it as an unexplained bound.

If this mass is zero, then $E=0$ in the asymptotic rest frame and the inequality gives $\mathbf P=0$. The same identity with any nonzero $\epsilon_\infty$ has zero right-hand side. Smoothness then makes its integrand vanish pointwise:

$$
\boxed{\mathcal D_i\epsilon=h_i{}^j\nabla_j\epsilon=0.}
$$

The [spinor](../../../algebra.md#spinor) is nonzero, since it has nonzero asymptotic value. This is a [spinor](../../../algebra.md#spinor) parallel along $\Sigma$; no time-parallel condition has yet been inferred merely from the integral.

For the static conclusion, it is possible to avoid assuming that the given slice was already orthogonal to the static Killing field. Because $E=\mathbf P=0$, repeat the zero-energy construction for four linearly independent asymptotic Dirac spinors. Parallel transport by the [Sen spinor connection](../../../general-relativity.md#sen-spinor-connection) is invertible, so the resulting spinors form a basis everywhere on $\Sigma$. Tangential curvature annihilates each of them:

$$
[\mathcal D_i,\mathcal D_j]\epsilon_A
=\frac14R_{ijab}\gamma^{ab}\epsilon_A=0,\qquad A=1,\ldots,4.
$$

Thus $R_{ijab}\gamma^{ab}=0$ as an operator. The six antisymmetric gamma products give a faithful [Spinor representation of the Lorentz group](../../../relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group), so $R_{ijab}=0$ for tangential $i,j$. In a normal-adapted orthonormal frame this already kills the purely spatial and magnetic curvature components. The remaining components vanish by the [Vacuum Einstein equations](../../../general-relativity.md#vacuum-einstein-equations):

$$
0=R_{ij}=-R_{\hat0 i\hat0 j}+\sum_kR_{kikj}
\quad\Longrightarrow\quad R_{\hat0 i\hat0 j}=0.
$$

Consequently the full spacetime [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) vanishes on $\Sigma$.

A static [Killing vector field](../../../general-relativity.md#killing-vector-field) generates isometries and preserves this curvature. Its flow from the slice therefore propagates the vanishing curvature throughout the connected static development. Extend one of the spinors by spacetime parallel transport along these time orbits, so that $\nabla_t\epsilon=0$. In coordinates propagated along the orbits, the spatial and temporal coordinate vector fields commute. Zero spin curvature then gives

$$
\nabla_t(\nabla_i\epsilon)=\nabla_i(\nabla_t\epsilon)=0.
$$

The initial tangential derivative is zero, so it stays zero. This constructs the required nonzero spacetime [parallel spinor](../../../connection-1-form.md#parallel-spinor); the initial parallel frame also removes any spin-holonomy ambiguity inherited from loops in $\Sigma$. The [static zero-energy parallel-spinor rigidity](../../../general-relativity.md#static-zero-energy-parallel-spinor-rigidity) conclusion is

$$
\boxed{\nabla_\mu\epsilon=0.}
$$

An equivalent check in a regular orthogonal static slicing is to write $ds^2=-N^2dt^2+h_{ij}dx^i dx^j$. The slice has zero [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature). An intrinsic parallel spinor forces the spatial [Ricci tensor](../../../general-relativity.md#ricci-tensor) to vanish by contracting its spin-curvature identity and using the invertibility of [Clifford multiplication](../../../algebra.md#clifford-multiplication) by a nonzero real vector. By [three-dimensional curvature from the Ricci tensor](../../../general-relativity.md#three-dimensional-curvature-from-the-ricci-tensor), $h$ is flat. The static vacuum equation $D_iD_jN=N R_{ij}(h)$ then makes the lapse gradient parallel, and asymptotic normalization forces $N=1$. The temporal spin connection vanishes as well.

An explicit example is [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), $ds^2=-dt^2+dx^2+dy^2+dz^2$, where every constant spinor in a Cartesian tetrad is a spacetime [parallel spinor](../../../connection-1-form.md#parallel-spinor) and the ADM mass is zero. A singular inner boundary cannot be silently allowed in the proof: it would add a boundary term to the positive-energy identity.

## 4

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Take $M=|Q|>0$ and use $G=c=1$. The case $M=Q=0$ is flat spacetime and is not a black hole. In the nontrivial extremal [Reissner-Nordstrom metric](../../../general-relativity.md#reissner-nordstrom-spacetime),

$$
ds^2=-f(r)dt^2+f(r)^{-1}dr^2+r^2d\Omega^2,\qquad
f(r)=\left(1-\frac Mr\right)^2.
$$

The horizon is a double zero at $r=M$, with [surface gravity](../../../general-relativity.md#surface-gravity) $\kappa=f'(M)/2=0$. The function $f$ is positive on both sides of the horizon. Thus the intermediate nonstatic region of a nonextremal charged hole disappears; one must not draw that region as a strip of nonzero width in the extremal [Penrose diagram](../../../general-relativity.md#penrose-diagram).

To construct the [Penrose diagram](../../../general-relativity.md#penrose-diagram), first integrate the radial [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate):

$$
\frac{dr_*}{dr}=\frac1f,\qquad
r_*=r-M+2M\log\left|\frac rM-1\right|-\frac{M^2}{r-M}.
$$

The additive constant has been chosen so that $r_*(0)=0$ in the inner block. In the exterior, $r_*\to-\infty$ at $M^+$ and $r_*\to+\infty$ at infinity. In the inner static region $0<r<M$, it increases from $0$ to $+\infty$. Set $u=t-r_*$ and $v=t+r_*$. The radial metric is $-f\,du\,dv$, so its radial null directions are $u=\mathrm{constant}$ and $v=\mathrm{constant}$.

Compactify each static block using

$$
U=\arctan(u/M),\qquad V=\arctan(v/M),\qquad
T=\frac{V+U}{2},\quad X=\frac{V-U}{2}.
$$

This [conformal compactification](../../../geometry-and-topology.md#conformal-compactification) puts radial [null geodesics](../../../special-relativity.md#null-geodesic) at $45$ degrees. The exterior is a diamond: its right-hand edges are past and [future null infinity](../../../general-relativity.md#future-null-infinity), while its left-hand edges are the past and future degenerate horizons. At the left vertex, finite static $t$ and $r\to M^+$ give $u\to+\infty$, $v\to-\infty$. This is an end of the infinite spatial throat, not a regular [bifurcation surface](../../../general-relativity.md#bifurcation-surface) where the two horizon branches meet. A [degenerate Killing horizon](../../../general-relativity.md#degenerate-killing-horizon) has no such bifurcation sphere. The inner block occupies the half-diamond $X>0$, because $r_*>0$ there. Its vertical edge $X=0$ is the timelike [curvature singularity](../../../general-relativity.md#curvature-singularity) $r=0$; its two diagonal edges are the two horizon branches at $r=M$. Its outer vertex likewise represents an excluded infinite-throat end.

The static-coordinate compactification identifies the blocks but does not by itself establish the smooth horizon extension. For that, use [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates) on the future horizon:

$$
v=t+r_*,\qquad ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega^2.
$$

Its radial determinant is $-1$, so it is nonsingular at $r=M$. Glue the exterior future edge, $u\to+\infty$ with $v$ finite, to the inner past edge, $u\to-\infty$ with the same finite $v$. The outgoing coordinate $u$ similarly gives $ds^2=-f\,du^2-2\,du\,dr+r^2d\Omega^2$ and extends the other horizon branch. Continue adjoining these regular blocks across every extendible null edge. The construction repeats indefinitely to the future and past, producing the maximal analytic diagram with infinitely many asymptotic exterior regions and inner static regions bounded by timelike singularities. Horizons are null edges, never the excluded throat vertices. Identical edges in different copies must be glued with their time orientations preserved; they are not all the same exterior infinity.

<a id="4/image-exterior-and-inner-penrose-building-blocks-of-an-extremal-charged-black-hole-the-marked-edges-glue-in-ingoing-coordinates-and-open-circles-are-excluded-throat-ends"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-73-extremal-blocks.png)

**[Figure 1](#4/image-exterior-and-inner-penrose-building-blocks-of-an-extremal-charged-black-hole-the-marked-edges-glue-in-ingoing-coordinates-and-open-circles-are-excluded-throat-ends). Exterior and inner Penrose building blocks of an extremal charged black hole; the marked edges glue in ingoing coordinates and open circles are excluded throat ends**.

The figure shows the two building blocks, rather than compressing the whole infinite extension into a misleading finite diagram. The red edges glue across a future horizon at finite advanced time. Outgoing coordinates extend the next edge to another exterior copy. The thin diagonal lines illustrate the radial light-cone directions.

For spatially conformally flat coordinates, compare the radial and angular parts of $f^{-1}dr^2+r^2d\Omega^2$ with $V(\rho)^2(d\rho^2+\rho^2d\Omega^2)$. The angular coefficient requires $V\rho=r$, and the radial coefficient then gives, in the exterior,

$$
\frac{d\rho}{\rho}=\frac{dr}{r\sqrt f}=\frac{dr}{r-M}.
$$

Choose the integration constant to make $\rho=r-M$ and $V\to1$ at infinity. In Cartesian coordinates $x=\rho\sin\theta\cos\varphi$, $y=\rho\sin\theta\sin\varphi$, $z=\rho\cos\theta$, put $\rho=\sqrt{x^2+y^2+z^2}$. The [Extremal Reissner-Nordstrom isotropic coordinates](../../../general-relativity.md#extremal-reissner-nordstrom-isotropic-coordinates) give

$$
\boxed{V=1+\frac M\rho,\qquad W=\left(1+\frac M\rho\right)^{-1},\qquad
 ds^2=-H^{-2}dt^2+H^2(dx^2+dy^2+dz^2),\quad H=1+M/\rho.}
$$

These coordinates have $\rho>0$ and describe the exterior only. The locus $\rho=0$ is the limit $r=M$, not an ordinary point included in this chart. An independent inner chart is obtained with $\rho=M-r$, $0<\rho<M$, giving $V=M/\rho-1$ and $W=(M/\rho-1)^{-1}$; it must be attached using the regular null coordinates, not by continuing the exterior radial coordinate through a Cartesian origin.

The infinite proper distance is real. Along a constant-$t$ exterior radius,

$$
L(\varepsilon,\rho_0)=\int_\varepsilon^{\rho_0}\left(1+\frac M\rho\right)d\rho
=\rho_0-\varepsilon+M\log(\rho_0/\varepsilon)\longrightarrow\infty.
$$

It is a property of a static spacelike slice. It does not bound the [proper time](../../../special-relativity.md#proper-time) of a freely falling observer. Indeed, a neutral radial timelike [geodesic](../../../riemannian-geometry.md#geodesic) has conserved energy per unit rest mass $E=f\dot t>0$ and normalization $-f\dot t^2+f^{-1}\dot r^2=-1$, giving

$$
\dot r^2=E^2-f,\qquad \dot r=-\sqrt{E^2-f}.
$$

At the horizon $\dot r\to-E$, so the remaining [proper time](../../../special-relativity.md#proper-time) is finite. Moreover,

$$
\dot v=\frac{E+\dot r}{f}=\frac1{E+\sqrt{E^2-f}}\longrightarrow\frac1{2E}.
$$

The observer crosses the regular future horizon with finite $v$ and finite proper time. This is the [Extremal Reissner-Nordstrom causal crossing](../../../general-relativity.md#extremal-reissner-nordstrom-causal-crossing), which the singular static time coordinate conceals.

There is also a direct causal test for the [event horizon](../../../general-relativity.md#event-horizon). Inside the future horizon, outgoing radial null curves in the ingoing chart satisfy $dr/dv=f/2$. To reach $r=M$ from below they would require

$$
v-v_0=2\int_{r_0}^{r}\frac{ds}{f(s)}\longrightarrow+\infty\quad\text{as }r\to M^-.
$$

Near the horizon, $M-r\sim2M^2/v$. A future timelike or nonradial null curve cannot increase $r$ faster than the outgoing radial null curve, since $ds^2\le0$ and $\dot v>0$ imply $dr/dv\le f/2$ after dropping the nonnegative angular term. Hence a signal that crossed inward cannot return to the original exterior's [future null infinity](../../../general-relativity.md#future-null-infinity). Curves can encounter other blocks in the maximal analytic extension, but their infinities are not the original observer's infinity. Relative to that asymptotic end, $r=M$ is the boundary of the causal past of future null infinity: it is an [event horizon](../../../general-relativity.md#event-horizon).

Finally, the [Reissner-Nordstrom trapped spheres](../../../general-relativity.md#reissner-nordstrom-trapped-spheres) test explains why the proposed observation is unsurprising. Normalize future radial null normals by $\ell=\partial_v+(f/2)\partial_r$, $n=-\partial_r$, with $g(\ell,n)=-1$. The round-sphere [null expansions](../../../geodesic-congruence.md#null-expansion) are

$$
\theta_\ell=\frac{f}{r}\ge0,\qquad \theta_n=-\frac2r<0.
$$

There is no region of strictly future-trapped round spheres, while the horizon spheres are marginal with $\theta_\ell=0$. Absence of those particular [trapped surfaces](../../../general-relativity.md#trapped-surface) does not imply absence of an [event horizon](../../../general-relativity.md#event-horizon). The geometry has a nonzero horizon area $4\pi M^2$ and a genuine timelike singularity at $r=0$ in its extension. **The infinite static throat does not remove the black hole: infall crosses its horizon in finite proper time, and no signal returns to the same exterior infinity.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
