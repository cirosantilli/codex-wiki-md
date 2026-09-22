<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [hierarchy problem](../../../../../hierarchy-problem.md) concerns the enormous separation between the [electroweak scale](../../../../../electroweak-scale.md) and a possible fundamental ultraviolet scale such as the [reduced Planck mass](../../../../../reduced-planck-mass.md): $v\simeq246\,\mathrm{GeV}$ whereas $M_{\mathrm{Pl}}\simeq2.4\times10^{18}\,\mathrm{GeV}$. For an elementary [Higgs field](../../../../../higgs-field.md), heavy states or a physical high-energy [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) generically generate

$$
\delta m_H^2\sim\frac{\kappa}{16\pi^2}\Lambda_{\mathrm{UV}}^2.
$$

Here $\kappa$ represents the appropriate dimensionless couplings. Maintaining a small physical Higgs mass then requires a very accurate cancellation against its bare mass parameter. The problem is sensitivity to actual high-energy physics, rather than merely the presence of a quadratic divergence in one choice of regulator.

The [cosmological constant problem](../../../../../cosmological-constant-problem.md) concerns the much smaller gravitationally observable [vacuum energy](../../../../../vacuum-energy.md). In the [Einstein equation](../../../../../einstein-field-equations.md), a constant term in the [effective action](../../../../../effective-action.md) contributes to the [cosmological constant](../../../../../cosmological-constant.md), with $\Lambda_{\mathrm{eff}}=\Lambda_{\mathrm{bare}}+\rho_{\mathrm{vac}}/M_{\mathrm{Pl}}^2$ in the usual normalization. Generic zero-point contributions scale as $\Lambda_{\mathrm{UV}}^4$, and vacuum transitions also change $\rho_{\mathrm{vac}}$. The dark-energy density is only of order $10^{-47}\,\mathrm{GeV}^4\sim(\text{a few meV})^4$. The puzzle is why the total remains so small despite much larger individual contributions. A constant shift of the nongravitational [Hamiltonian](../../../../../hamiltonian.md) cannot remove its gravitational effect.

[Supersymmetry](../../../../../supersymmetry-split.md) relates [bosonic](../../../../../boson.md) and [fermionic](../../../../../fermion.md) [degrees of freedom](../../../../../degree-of-freedom.md), including their interactions. Their opposite loop signs cancel the quadratic contributions to a [scalar field](../../../../../scalar-field.md) mass in the unbroken theory. With [soft supersymmetry breaking](../../../../../soft-supersymmetry-breaking.md), the surviving correction is controlled by the mass splitting, schematically

$$
\delta m_H^2\sim\frac{g^2}{16\pi^2}m_{\mathrm{soft}}^2\log\frac{\Lambda_{\mathrm{UV}}}{m_{\mathrm{soft}}}.
$$

Thus a sufficiently low soft-breaking scale protects a small [electroweak scale](../../../../../electroweak-scale.md) against a much higher ultraviolet scale. This is the useful supersymmetric response to the [hierarchy problem](../../../../../hierarchy-problem.md).

Exact global [supersymmetry](../../../../../supersymmetry-split.md) also cancels [vacuum energy](../../../../../vacuum-energy.md): the [supersymmetry algebra](../../../../../super-poincare-algebra.md) expresses the [Hamiltonian](../../../../../hamiltonian.md) as a positive sum of anticommutators, so a vacuum annihilated by every [supercharge](../../../../../supersymmetry-generator.md) has zero energy. Equivalently, with canonical [kinetic terms](../../../../../kinetic-term.md),

$$
V=\sum_i|F_i|^2+\frac12\sum_a(D^a)^2
$$

vanishes in a [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md). However, ordinary particles and their [superpartners](../../../../../sparticle.md) cannot have the identical mass spectrum of unbroken [supersymmetry](../../../../../supersymmetry-split.md), so a useful phenomenological theory needs [supersymmetry breaking](../../../../../supersymmetry-breaking.md). Its [vacuum energy](../../../../../vacuum-energy.md) is generically of order the fourth power of the breaking scale; even a scale of order $10^2\,\mathrm{GeV}$ gives about $10^8\,\mathrm{GeV}^4$, enormously above the required value. In [supergravity](../../../../../supergravity.md), a negative term can cancel positive breaking contributions:

$$
V_F=e^{K/M_{\mathrm{Pl}}^2}\left(K^{i\bar j}D_iW\,D_{\bar j}\overline W-\frac{3|W|^2}{M_{\mathrm{Pl}}^2}\right),\qquad D_iW=W_i+\frac{K_iW}{M_{\mathrm{Pl}}^2},
$$

but arranging a tiny residual is a new tuning. Consequently **[supersymmetry](../../../../../supersymmetry-split.md) can protect the hierarchy after soft breaking, while its exact vacuum-energy cancellation does not by itself survive realistic breaking.**

One higher-dimensional proposal uses [large extra dimensions](../../../../../large-extra-dimensions.md). Take $n$ flat compact dimensions of common radius $R$, with gravity propagating in the bulk and [Standard Model](../../../../../standard-model-split.md) fields confined to a four-dimensional [brane](../../../../../brane.md). Reducing the gravitational [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) gives

$$
\frac{M_*^{n+2}}2\int d^4x\,d^ny\sqrt{-G}\,\mathcal R_{4+n}\ \longrightarrow\ \frac{M_*^{n+2}(2\pi R)^n}{2}\int d^4x\sqrt{-g}\,\mathcal R_4,
$$

so

$$
\boxed{M_{\mathrm{Pl}}^2=M_*^{n+2}(2\pi R)^n.}
$$

A fundamental gravitational scale $M_*$ near a TeV then produces apparently weak four-dimensional gravity through dilution into the large compact volume. For $n=2$ and $M_*=1\,\mathrm{TeV}$, $R=M_{\mathrm{Pl}}/(2\pi M_*^2)$ is about $0.075\,\mathrm{mm}$, using $1\,\mathrm{GeV}^{-1}\simeq1.97\times10^{-16}\,\mathrm m$. At distances much smaller than $R$, the gravitational potential scales as $r^{-(n+1)}$; at distances much larger than $R$ it scales as $r^{-1}$. Confining charged [Standard Model](../../../../../standard-model-split.md) fields to the [brane](../../../../../brane.md) avoids a light tower of charged [Kaluza-Klein modes](../../../../../kaluza-klein-mode.md) associated with the large radius. The primary explanatory challenge is [radius stabilization](../../../../../radius-stabilization.md): one must generate and stabilize $RM_*\gg1$, rather than simply postulate a huge volume and transfer the original hierarchy into a modulus.

A second proposal is the [Randall–Sundrum model](../../../../../randall-sundrum-model.md). Compactify on an interval, equivalently an orbifold with [branes](../../../../../brane.md) at $y=0$ and $y=L$, and use the warped metric

$$
ds^2=e^{-2k|y|}\eta_{\mu\nu}dx^\mu dx^\nu+dy^2.
$$

A negative bulk [cosmological constant](../../../../../cosmological-constant.md) and suitably related [brane tensions](../../../../../brane-tension.md) support this geometry. Integrating over the full orbifold interval $[-L,L]$ gives

$$
M_{\mathrm{Pl}}^2=M_5^3\int_{-L}^Le^{-2k|y|}\,dy=\frac{M_5^3}{k}(1-e^{-2kL}).
$$

For a [scalar field](../../../../../scalar-field.md) $h$ on the [brane](../../../../../brane.md) at $L$, its induced metric gives the kinetic coefficient $e^{-2kL}$ and mass coefficient $e^{-4kL}m_0^2$. The canonical field is $h_c=e^{-kL}h$, hence

$$
\boxed{m_{\mathrm{phys}}=e^{-kL}m_0.}
$$

With $k$ and $M_5$ of the same fundamental order, an exponent $kL\simeq35$--$37$ converts a fundamental mass into a weak-scale mass, without requiring a large proper [compactification](../../../../../compactification-physics.md) volume.

Again the separation must be selected dynamically. The original warped solution leaves a massless [radion](../../../../../radion.md), so merely choosing $L$ does not complete the explanation. For example, the [Goldberger–Wise stabilization mechanism](../../../../../goldberger-wise-stabilization-mechanism.md) introduces a bulk [scalar field](../../../../../scalar-field.md) with boundary values $v_0,v_L$ and a small mass $m_\chi$. Its static equation and solution are

$$
\chi''-4k\chi'-m_\chi^2\chi=0,\qquad \chi=Ae^{(4+\epsilon)ky}+Be^{-\epsilon ky},\qquad\epsilon=\sqrt{4+m_\chi^2/k^2}-2\simeq\frac{m_\chi^2}{4k^2}.
$$

For small backreaction and large $kL$, the leading radius-dependent potential is proportional to $e^{-4kL}(v_L-v_0e^{-\epsilon kL})^2$. Its leading minimum obeys $kL\simeq\epsilon^{-1}\log(v_0/v_L)$, so a modest boundary-value ratio and a small $\epsilon$ can give the required exponent. Corrections and the residual four-dimensional [cosmological constant](../../../../../cosmological-constant.md) must still be controlled. **Both proposals need a stable dynamical origin for the [compactification](../../../../../compactification-physics.md) geometry; their volume or warp relations alone do not supply it.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
