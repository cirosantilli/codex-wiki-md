<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

**Geometric quantization.** A classical [symplectic manifold](../../../../../symplectic-manifold.md) supplies observables as real functions, their [Poisson bracket](../../../../../poisson-bracket.md), and [Hamiltonian flows](../../../../../hamiltonian-flow.md). [Geometric quantization](../../../../../geometric-quantization.md) seeks a [Hilbert space](../../../../../hilbert-space-split.md) of quantum states and operators that encode this structure, including $\widehat1=I$ and a commutator corresponding to the [Poisson bracket](../../../../../poisson-bracket.md). A direct prescription cannot make every classical product become an operator product without qualification; operator ordering and the choice of physically admissible observables matter. The aim is to build the state space and operators from the geometry rather than from a preferred coordinate chart.

For [prequantization](../../../../../prequantization.md), with $\iota_{X_f}\omega=df$, choose a Hermitian [line bundle](../../../../../line-bundle.md) $L\to P$ with a unitary [connection on a vector bundle](../../../../../connection-vector-bundle.md) of curvature

$$
F_\nabla=\frac{i}{\hbar}\omega.
$$

Its first [Chern class](../../../../../chern-class.md) requires the integrality condition

$$
\boxed{[\omega/(2\pi\hbar)]\text{ lies in the image of }H^2(P;\mathbb Z)\to H^2_{\rm dR}(P).}
$$

Equivalently the symplectic period on every closed integral two-cycle is a multiple of $2\pi\hbar$. Conversely an integral class supplies a [line bundle](../../../../../line-bundle.md), and a unitary connection can be adjusted by a one-form to have the required curvature. Locally choose $\theta$ with $\omega=-d\theta$; then $\nabla=d-i\theta/\hbar$. Potentials differing by an exact one-form change the local phase of the section. Integrality is precisely what makes these local descriptions glue consistently.

On sections the [Kostant-Souriau prequantum operator](../../../../../kostant-souriau-prequantum-operator.md) is

$$
\widehat f=-i\hbar\nabla_{X_f}+f.
$$

The curvature identity $[\nabla_X,\nabla_Y]=\nabla_{[X,Y]}+F_\nabla(X,Y)$, together with $[X_f,X_g]=-X_{\{f,g\}}$, gives

$$
[\widehat f,\widehat g]=i\hbar\widehat{\{f,g\}}.
$$

Indeed the derivative part of the commutator is $\hbar^2\nabla_{X_{\{f,g\}}}$, the curvature part is $-i\hbar\{f,g\}$, and the two multiplication/derivative cross terms total $2i\hbar\{f,g\}$. These combine to the displayed operator identity. The prequantum inner product uses the Hermitian fiber metric and the [symplectic volume form](../../../../../symplectic-volume-form.md) $\omega^n/n!$, with appropriate square-integrability and operator-domain conditions.

This is not yet the desired quantum state space: a prequantum section depends on all $2n$ phase-space variables, whereas a wavefunction normally depends on only $n$ configuration variables. A [polarization in geometric quantization](../../../../../polarization-in-geometric-quantization.md) is an involutive Lagrangian rank-$n$ subbundle of $T_{\mathbb C}P$. Polarized sections obey $\nabla_Xs=0$ along that distribution. The [symplectic form](../../../../../symplectic-form.md) vanishes on it, so its restricted curvature vanishes and these differential conditions are locally compatible.

For $T^*Q$, the vertical polarization is spanned locally by $\partial_{p_i}$. With $\theta=p_i dq^i$, polarized sections depend only on $q$, and the basic [prequantum operators](../../../../../kostant-souriau-prequantum-operator.md) become

$$
\boxed{\widehat q^i=q^i,\qquad\widehat p_i=-i\hbar\partial_{q^i}.}
$$

Only observables whose [Hamiltonian flows](../../../../../hamiltonian-flow.md) preserve the polarization act directly on this polarized space. A generic quadratic kinetic energy does not preserve the vertical polarization, so obtaining its quantum operator needs an additional construction rather than simply restricting every prequantum operator. A compatible complex structure can instead provide a Kähler polarization, yielding holomorphic-type states, as for oscillator variables. The [Blattner-Kostant-Sternberg pairing](../../../../../blattner-kostant-sternberg-pairing.md) compares suitable state spaces of different polarizations and can implement some transported observables.

Finding a useful global polarization is a genuine problem: it may not exist as a nonsingular real foliation; leaf holonomy can obstruct globally nonzero flat sections; singular leaves and compact leaves impose further conditions. A [metaplectic correction](../../../../../metaplectic-correction.md) uses half-forms to improve the inner product and coordinate transformation law and account for familiar zero-point shifts, when its additional square-root data exist. Thus prequantum integrality, polarization, Hilbert-space completion and observable domains are separate steps, each with geometric constraints.

**Applications of Stokes's theorem.** For an oriented manifold $W$ with boundary and a differential form $\alpha$ of degree $\dim W-1$,

$$
\int_W d\alpha=\int_{\partial W}\alpha
$$

with the outward-normal-first boundary orientation. Locally the identity is integration by parts in a half-space; a partition of unity reduces the general manifold to that local calculation, and contributions along internal patch boundaries cancel. The [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) unifies the fundamental theorem of calculus, circulation/flux formulas and the relation between local conservation laws and conserved integrated charges.

For a charged [brane](../../../../../brane.md) with worldvolume $W$ of dimension $p+1$, let $X:W\to M$ be its embedding, $\gamma=X^*g$ its [induced worldvolume metric](../../../../../induced-worldvolume-metric.md), and $A$ a $(p+1)$-form [gauge potential](../../../../../gauge-field.md) with $F=dA$. Take

$$
S[X]=-T_p\int_W\sqrt{-\gamma}\,d^{p+1}\sigma+q\int_W X^*A.
$$

Under $A\mapsto A+d\Lambda$, the [Wess-Zumino brane coupling](../../../../../wess-zumino-brane-coupling.md) changes by $q\int_{\partial W}X^*\Lambda$. It is invariant for a closed worldvolume, or for suitable boundary conditions; open branes can require compensating boundary terms.

For an embedding variation $V=\delta X$, differentiation of the pullback and [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) give

$$
\delta\int_W X^*A=\int_W X^*(\mathcal L_VA)=\int_W X^*(\iota_VF)+\int_{\partial W}X^*(\iota_VA).
$$

Thus the interior force depends only on the [gauge field strength](../../../../../gauge-field-strength.md). In components, define the worldvolume wave-map/mean-curvature vector by

$$
K^\mu=\frac1{\sqrt{-\gamma}}\partial_a(\sqrt{-\gamma}\gamma^{ab}\partial_bX^\mu)+\Gamma^\mu_{\rho\sigma}\gamma^{ab}\partial_aX^\rho\partial_bX^\sigma.
$$

Varying the area term and integrating by parts gives $\delta S_{\rm area}=T_p\int_W\sqrt{-\gamma}K_\mu V^\mu$. Combining the two variations yields the [field-strength force on a charged brane](../../../../../field-strength-force-on-a-charged-brane.md) equation

$$
\boxed{T_pK_\mu+\frac q{(p+1)!\sqrt{-\gamma}}\epsilon^{a_0\cdots a_p}F_{\mu\nu_0\cdots\nu_p}\partial_{a_0}X^{\nu_0}\cdots\partial_{a_p}X^{\nu_p}=0.}
$$

It is gauge invariant because $A$ no longer occurs. Its tangential projection vanishes identically by antisymmetry, consistently with worldvolume reparametrization invariance. At $p=0$, the chosen Lorentzian worldline convention has $K=-\ddot X$ in proper time and recovers the usual Lorentz-force sign.

For topological conservation, let the spatial manifold compactify to a closed oriented $n$-manifold $\Sigma$, and let a field $U:\Sigma\to N$ take values in a closed oriented $n$-dimensional target with normalized volume form $\Omega$, $\int_N\Omega=1$. Then

$$
Q=\int_\Sigma U^*\Omega=\deg U\in\mathbb Z.
$$

This is the [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md): for a regular value it is the signed sum of inverse images. To relate the integral to that count, use a normalized target form supported near a regular value and change variables on its inverse-image neighborhoods. Any two normalized top forms on a connected closed oriented target differ by an exact form, whose pulled-back integral vanishes by the [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md). Hence the value is independent of this localization and equals the integer signed count.

If $U$ varies smoothly in time, its spacetime pullback $j=U^*\Omega$ satisfies $dj=U^*(d\Omega)=0$. Apply [Stokes theorem](../../../../../stokes-theorem.md) to the spacetime slab between two slices: the difference of their charges is minus the flux through the spatial boundary. With no flux at infinity, **$Q$ is conserved independently of the field equations**. Equivalently a smooth homotopy cannot change the degree. Singularities, altered boundary conditions or nonzero boundary flux are the ways the argument can fail.

For the [Skyrme model](../../../../../skyrme-model.md), finite-energy fields approach $U=I$ at spatial infinity, so $\mathbb R^3$ compactifies to $S^3$ and $U:S^3\to SU(2)\cong S^3$. With the conventional target orientation choose

$$
\Omega=-\frac1{24\pi^2}\operatorname{tr}(U^{-1}dU)^{\wedge3}.
$$

This is a normalized closed target [volume form](../../../../../volume-form.md). The resulting [topological baryon number in the Skyrme model](../../../../../topological-baryon-number-in-the-skyrme-model.md) is

$$
\boxed{B=-\frac1{24\pi^2}\int_{\mathbb R^3}\epsilon^{ijk}\operatorname{tr}(L_iL_jL_k)\,d^3x\in\mathbb Z,\qquad L_i=U^{-1}\partial_iU.}
$$

The corresponding identically conserved spacetime current is $j^\mu=-(24\pi^2)^{-1}\epsilon^{\mu\nu\rho\sigma}\operatorname{tr}(L_\nu L_\rho L_\sigma)$ in oriented flat coordinates. For the hedgehog $U=\cos f(r)I+i\widehat x\cdot\boldsymbol\sigma\sin f(r)$ with $f(0)=\pi$ and $f(\infty)=0$, substitution gives

$$
B=-\frac2\pi\int_0^\infty f'(r)\sin^2f(r)\,dr=-\frac1\pi\left[f-\frac12\sin2f\right]_0^\infty=1.
$$

The [Skyrmion](../../../../../skyrmion.md) therefore supplies a concrete topologically conserved unit charge. Topological conservation alone does not guarantee a stable finite-size static solution: the positive [Skyrme term](../../../../../skyrme-term.md), with four derivatives, opposes collapse of the two-derivative energy. Under size rescaling, these contributions behave as $E_2\propto\lambda$ and $E_4\propto\lambda^{-1}$, allowing a nonzero equilibrium size while preserving the degree.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
