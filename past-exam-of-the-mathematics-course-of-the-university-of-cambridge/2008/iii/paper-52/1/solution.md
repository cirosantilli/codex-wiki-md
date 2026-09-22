<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The local gauge symmetries of the [Polyakov action](../../../../../polyakov-action.md) are [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md). Under a reparametrization $\sigma^\alpha\mapsto\sigma'^\alpha$, the embedding coordinates $X^\mu$ transform as scalars and the [worldsheet metric](../../../../../worldsheet-metric.md) as a covariant tensor; the contracted integrand is a scalar density. Infinitesimally, with the active convention, $\delta X=-\xi^\alpha\partial_\alpha X$ and $\delta\gamma=-\mathcal L_\xi\gamma$. A [Weyl transformation](../../../../../weyl-transformation.md) sends $\gamma_{\alpha\beta}\mapsto e^{2\omega}\gamma_{\alpha\beta}$ and leaves $X$ fixed. In two dimensions the factors from $\sqrt{-\gamma}$ and $\gamma^{\alpha\beta}$ cancel. Target-space Poincaré transformations are additional global symmetries, rather than [worldsheet](../../../../../worldsheet.md) gauge symmetries.

These gauge freedoms put the metric locally in [conformal gauge](../../../../../conformal-gauge.md), $\gamma_{\alpha\beta}=\eta_{\alpha\beta}$. Its variation must still be imposed: it gives the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) constraints $T_{++}=T_{--}=0$. The field equation is the [wave equation](../../../../../wave-equation-split.md), and periodicity of a [closed string](../../../../../closed-string.md) gives independent left- and right-moving oscillator sets. In a normalization with $\alpha_0^\mu=\widetilde\alpha_0^\mu=\sqrt{\alpha'/2}\,k^\mu$, their commutators and normal-ordered generators are

$$
[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0},\qquad
L_n=\frac12\sum_{r\in\mathbb Z}:\alpha_{n-r}\cdot\alpha_r:,
\qquad L_0=\frac{\alpha'k^2}{4}+N,
$$

with the same formulas for the tilded sector and zero mixed commutators.

The [closed-string physical-state Virasoro conditions](../../../../../closed-string-physical-state-virasoro-conditions.md) in the critical flat-space theory are

$$
\boxed{L_{n>0}|\Phi\rangle=\widetilde L_{n>0}|\Phi\rangle=0,
\quad(L_0-1)|\Phi\rangle=(\widetilde L_0-1)|\Phi\rangle=0.}
$$

They act on the oscillator [Fock space](../../../../../fock-space.md), and physical spurious (null) states are quotiented out. Equivalently physical states are the suitable [BRST cohomology](../../../../../brst-cohomology.md) classes. Positive modes constrain kets; their adjoints constrain bras, so one does not impose every positive and negative matter mode on the same ket. Subtracting the two zero-mode equations gives [closed-string level matching](../../../../../closed-string-level-matching.md), $N=\widetilde N$, and adding their mass-shell content gives $M^2=4(N-1)/\alpha'$. Quantum consistency fixes the intercept to one and, for just these flat coordinate fields, $d=26$: the matter [central charge](../../../../../central-charge.md) $d$ cancels the reparametrization ghost [central charge](../../../../../central-charge.md) $-26$. Other dimensions require additional [worldsheet](../../../../../worldsheet.md) degrees of freedom or a noncritical completion.

For the residual symmetry, take $\sigma^\pm=\tau\pm\sigma$. The conformal Killing equations leave independent transformations $\sigma^+\mapsto f(\sigma^+)$ and $\sigma^-\mapsto\widetilde f(\sigma^-)$, with a compensating Weyl rescaling restoring the flat metric. On the Euclidean plane the corresponding holomorphic vector fields are $\ell_n=-z^{n+1}\partial_z$ and their antiholomorphic partners. They satisfy the [Witt algebra](../../../../../witt-algebra.md) $[\ell_m,\ell_n]=(m-n)\ell_{m+n}$. The conserved contour generators are the Virasoro modes $L_n=(2\pi i)^{-1}\oint z^{n+1}T(z)\,dz$. Their quantum [Virasoro algebra](../../../../../virasoro-algebra.md) is

$$
[L_m,L_n]=(m-n)L_{m+n}+\frac d{12}(m^3-m)\delta_{m+n,0},
\qquad[L_m,\widetilde L_n]=0,
$$

with a second independent copy for the right movers. These are the generators of the residual conformal transformations, including their quantum central extension.

The [two-dimensional quantum-gravity interpretation of strings](../../../../../two-dimensional-quantum-gravity-interpretation-of-strings.md) follows from what is integrated, not from an analogy: at genus $h$, the Polyakov path integral integrates over both $X$ and the metric, divided by diffeomorphism and Weyl gauge volume. [String perturbation theory](../../../../../string-perturbation-theory.md) sums these surface topologies, weighted by $g_s^{2h-2}$ before external-state coupling factors. Gauge fixing leaves [worldsheet](../../../../../worldsheet.md) ghost determinants and integrals over [worldsheet moduli](../../../../../worldsheet-moduli.md). Thus it is [two-dimensional quantum gravity](../../../../../two-dimensional-quantum-gravity.md) coupled to the $d$ coordinate matter fields. A flat gauge is local; general higher-genus surfaces retain conformal-structure moduli and need not admit a globally flat representative.

Target-space gravity is a different conclusion. At $N=\widetilde N=1$, the state $\epsilon_{\mu\nu}\alpha_{-1}^\mu\widetilde\alpha_{-1}^\nu|k\rangle$ is massless, transverse in both indices, and has longitudinal gauge identifications. Its symmetric traceless transverse polarization is a [graviton](../../../../../graviton.md); the antisymmetric and scalar polarizations give the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and [dilaton](../../../../../dilaton.md). The [graviton](../../../../../graviton.md) gauge identification is precisely the linearized metric diffeomorphism. Moreover the leading [string-frame massless effective action](../../../../../string-frame-massless-effective-action.md) contains $\int\sqrt{-G}e^{-2\Phi}R$, and [worldsheet](../../../../../worldsheet.md) Weyl invariance with constant [dilaton](../../../../../dilaton.md) and zero two-form requires $R_{\mu\nu}=0$ at leading order in $\alpha'$. Thus both the propagating massless spin-two state and its low-energy interactions reproduce gravity. **[Closed strings](../../../../../closed-string.md) contain the [graviton](../../../../../graviton.md) and yield Einstein gravity in their low-energy massless sector**, together with other fields and higher-derivative corrections; the bosonic [tachyon](../../../../../tachyon.md) instability remains.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
