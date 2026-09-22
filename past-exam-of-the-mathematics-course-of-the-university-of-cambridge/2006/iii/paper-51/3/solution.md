<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [partition function](../../../../../canonical-partition-function.md) sums the [Boltzmann weights](../../../../../boltzmann-factor.md) of all states: $Z=\sum_s e^{-\beta_TH(s)}$ for discrete states, or the corresponding integral for continuous fields. It normalizes equilibrium probabilities. Its physical [Helmholtz free energy](../../../../../helmholtz-free-energy.md) is $\mathscr F=-k_BT\log Z$, and its [free-energy density](../../../../../free-energy-density.md) is $\mathscr F/V$. With a momentum [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) $\Lambda_0$, a scalar-field example is

$$
Z_{\Lambda_0}=\int_{|q|<\Lambda_0}\mathcal D\phi\,e^{-\beta_TH_{\Lambda_0}[\phi]}.
$$

The normalization of the [functional measure](../../../../../functional-measure.md) and field-independent energy terms must be tracked when discussing absolute [free energy](../../../../../thermodynamic-free-energy.md).

Choose a smaller cutoff $\Lambda$ and split the field into retained modes $\phi_<$ with $|q|<\Lambda$ and eliminated modes $\phi_>$ with $\Lambda<|q|<\Lambda_0$. Define the [Wilsonian coarse-grained statistical Hamiltonian](../../../../../wilsonian-coarse-grained-statistical-hamiltonian.md) by

$$
e^{-\beta_TH_\Lambda[\phi_<]}=\int\mathcal D\phi_>\,e^{-\beta_TH_{\Lambda_0}[\phi_<+\phi_>]}.
$$

Substitution into the [partition function](../../../../../canonical-partition-function.md) proves $Z=\int\mathcal D\phi_<e^{-\beta_TH_\Lambda[\phi_<]}$ for every intermediate cutoff. A source retained in this definition similarly preserves long-wavelength [connected correlation functions](../../../../../connected-correlation-function.md) and response. Thus the coefficients in a [Hamiltonian density](../../../../../hamiltonian-density.md) must run with $\Lambda$: the dependence induced by eliminated modes compensates the dependence of the remaining field integral. Holding the original bare coefficients fixed while changing the cutoff would generally change the system. Exact integration generates all interactions allowed by [symmetry](../../../../../symmetry-physics.md), including higher powers, [derivative](../../../../../derivative.md) terms and an [additive constant](../../../../../additive-constant.md); a [local derivative expansion](../../../../../local-derivative-expansion.md) or a truncation to a few couplings is an extra approximation.

Cutoff independence makes arbitrary intermediate coarse-graining scales unphysical. It allows calculations at the scale of the observable, avoids repeatedly resolving irrelevant short-distance details and exposes the [renormalization-group fixed points](../../../../../renormalization-group-fixed-point.md) responsible for [universality](../../../../../universality-of-critical-phenomena.md). A microscopic cutoff, such as a [Bravais lattice](../../../../../bravais-lattice.md) spacing, can still label a physical microscopic model; taking it to infinity as a [continuum limit](../../../../../continuum-limit.md) requires tuning appropriate bare couplings. This is distinct from lowering an intermediate Wilsonian cutoff in a fixed model.

To interpret the zero-cutoff limit, define $M=V^{-1}\int\phi(x)\,d^Dx$, the spatially uniform mode of the [order parameter](../../../../../order-parameter.md). Keep this mode fixed and integrate the others, rather than integrating over $M$ too. Write $\phi=M+\eta$, with $\int\eta=0$, and define the [constrained order-parameter free energy](../../../../../constrained-order-parameter-free-energy.md) by

$$
e^{-\beta_TVF_c(M)}=Z_M=\int_{\int\eta=0}\mathcal D\eta\,e^{-\beta_TH_{\Lambda_0}[M+\eta]}.
$$

In a finite periodic box, once $\Lambda$ is below the smallest nonzero momentum, all nonconstant modes have been eliminated. The remaining effective energy is $H_\Lambda[M]=VU_\Lambda(M)$, so its defining integral is exactly $Z_M$. Therefore, with consistent normalization,

$$
\boxed{F_c(M)=\lim_{\Lambda\to0}U_\Lambda(M).}
$$

When $\mathcal H(\Lambda,M)$ denotes this uniform effective [Hamiltonian density](../../../../../hamiltonian-density.md), this is the stated identification of $F(M)$ with its zero-cutoff limit. It requires a [free-energy density](../../../../../free-energy-density.md) constrained at fixed $M$, not the unconstrained extensive [free energy](../../../../../thermodynamic-free-energy.md); all integrated fluctuations and [additive constants](../../../../../additive-constant.md) are included, the [zero mode in field theory](../../../../../zero-mode-in-field-theory.md) is retained, and a density for the uniform configuration is well defined. The finite-volume argument avoids an interchange of the thermodynamic and cutoff limits without justification. On a homogeneous pure-phase branch one may use a local potential description, while a [thermodynamic limit](../../../../../thermodynamic-limit.md) allowing [phase separation](../../../../../phase-separation.md) can convexify the constrained potential. A bare nonconvex Landau polynomial is accordingly a homogeneous-branch approximation, not a claim that the exact equilibrium Legendre potential stays nonconvex.

In a field $h$, the remaining integral is $Z(h)=\int dM\,e^{-\beta_TV[F_c(M)-hM]}$, up to the consistently chosen zero-mode measure. The thermodynamic saddle then gives $f(h)=\inf_M\{F_c(M)-hM\}$ and selects the [equilibrium magnetization](../../../../../equilibrium-magnetization.md). [Landau theory](../../../../../landau-theory.md) assumes that the relevant uniform potential can be approximated by a regular analytic expansion in $M$, with symmetry-constrained coefficients, and minimizes it. At tree level the integrated fluctuations are neglected, recovering the familiar bare polynomial. With fluctuations retained, the coefficients run and can become singular near criticality; the [zero-cutoff identification of constrained free energy](../../../../../zero-cutoff-identification-of-constrained-free-energy.md) alone does not justify [mean-field critical exponents](../../../../../mean-field-critical-exponent.md).

For an ordinary short-range scalar [thermodynamic critical point](../../../../../thermodynamic-critical-point.md), the leading interaction is quartic. Absorb [inverse temperature](../../../../../inverse-temperature.md) and the [gradient](../../../../../gradient.md) coefficient into field normalization and write

$$
\beta_TH=\int d^Dx\left\{\frac12(\nabla\phi)^2+\frac r2\phi^2+\frac g{4!}\phi^4+\cdots\right\}.
$$

Scale $x=bx'$ and $\phi(x)=b^{-(D-2)/2}\phi'(x')$ to leave the [gradient](../../../../../gradient.md) term invariant. The quartic term changes to $gb^{4-D}\int\phi'^4/4!$, so its engineering scaling exponent is $4-D$. It is irrelevant at the [Gaussian fixed point](../../../../../gaussian-fixed-point.md) for $D>4$, relevant for $D<4$, and marginal for $D=4$. Hence

$$
\boxed{D_c=4.}
$$

The loop expansion makes the breakdown concrete. A quartic-vertex correction is proportional to $g^2I_2(r)$, where

$$
I_2(r)=\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac1{(q^2+r)^2}.
$$

For $0<D<4$, rescaling $q=\sqrt r\,k$ gives $I_2(r)\sim C_Dr^{(D-4)/2}$, diverging as $r\to0$. At $D=4$, radial integration gives

$$
I_2(r)=\frac1{16\pi^2}\left\{\log\frac{\Lambda^2+r}{r}+\frac r{\Lambda^2+r}-1\right\},
$$

which is logarithmically divergent. Above four dimensions its infrared limit is finite; the leading cutoff-dependent constant can be absorbed into a coupling renormalization. The effective expansion parameter is thus of order $g\xi^{4-D}$ below four, or $g\log(\Lambda\xi)$ at four, since $\xi\sim r^{-1/2}$. It eventually becomes large for any fixed bare interaction in the lower-dimensional critical limit, defeating the uncorrected mean-field expansion. The [Ginzburg criterion](../../../../../ginzburg-criterion.md) gives the same threshold by comparing correlation-volume fluctuations with the squared mean [order parameter](../../../../../order-parameter.md).

Below four dimensions an interacting [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md) can replace the [Gaussian fixed point](../../../../../gaussian-fixed-point.md) and change [critical exponents](../../../../../critical-exponent.md), provided a continuous transition exists. At four dimensions the interaction is marginal and produces logarithmic corrections: the leading power exponents can remain their mean-field values, so “breakdown” there means that pure mean-field [power laws](../../../../../power-law.md) omit those corrections, rather than necessarily that every power exponent changes. Above four the stabilizing quartic interaction is dangerously irrelevant for the ordered phase, explaining why mean-field thermodynamic exponents need not obey naive hyperscaling with the spatial dimension.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
