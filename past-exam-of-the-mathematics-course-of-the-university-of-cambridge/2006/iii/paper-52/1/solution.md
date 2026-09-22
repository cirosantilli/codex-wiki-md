<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use natural units and the [Minkowski metric](../../../../../minkowski-metric.md) $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$. A massive spin-one particle has three physical [particle polarizations](../../../../../particle-polarization.md), whereas a massless [gauge boson](../../../../../gauge-boson.md) has two. Giving a vector a mass must account for this extra longitudinal state while preserving a positive physical state space, controlled high-energy scattering and, if a fundamental perturbative theory is sought, [renormalizability](../../../../../renormalizable-quantum-field-theory.md).

At the free-field level there is no inconsistency. The [Proca action](../../../../../proca-action.md)

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}+\frac12m^2A_\mu A^\mu,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu
$$

gives the [Proca equation](../../../../../proca-equation.md) $\partial_\nu F^{\nu\mu}+m^2A^\mu=0$. Taking its divergence gives $m^2\partial_\mu A^\mu=0$, and then $(\Box+m^2)A^\mu=0$. For $m>0$ the divergence constraint removes one of the four components, leaving three positive-norm physical modes. The time component is constrained, rather than an independent negative-norm propagating oscillator. The mass term does, however, change under $A_\mu\mapsto A_\mu+\partial_\mu\omega$, so the ordinary massless [gauge invariance](../../../../../gauge-invariance.md) is no longer manifest.

The difficulty becomes acute for generic interactions. Inverting the quadratic operator gives the [Proca propagator](../../../../../proca-propagator.md)

$$
D_{\mu\nu}(k)=\frac{-i}{k^2-m^2+i0}\left(g_{\mu\nu}-\frac{k_\mu k_\nu}{m^2}\right).
$$

The longitudinal part approaches order $1/m^2$ at large momentum, rather than falling as $1/k^2$. Thus the usual ultraviolet [power counting](../../../../../power-counting-in-quantum-field-theory.md) deteriorates. There is a parallel external-state problem: for $p^\mu=(E,\mathbf p)$,

$$
\varepsilon_L^\mu(p)=\frac1m(|\mathbf p|,E\widehat{\mathbf p})=\frac{p^\mu}{m}+O(m/E).
$$

Longitudinal external legs can generate powers of $E/m$ in a [scattering amplitude](../../../../../scattering-amplitude.md). These are the [high-energy obstruction for a hard vector mass](../../../../../high-energy-obstruction-for-a-hard-vector-mass.md). Conserved Abelian currents can remove dangerous contractions, so one should not conclude that every massive-vector interaction is impossible.

For a massive non-Abelian vector with gauge-like cubic and quartic couplings, cancellations among diagrams remove the largest powers, but without a suitable additional sector longitudinal scattering still grows like $s/v^2$, where $v$ is the symmetry-breaking scale. A partial-wave coefficient is then of order $s/(16\pi v^2)$. [Partial-wave unitarity](../../../../../partial-wave-unitarity.md) requires its real part to remain bounded, so perturbation theory fails at energies of order the electroweak scale times a modest loop factor, around the TeV scale for electroweak vectors. This is a limit on the perturbative description, not a proof that a low-energy massive-vector [effective field theory](../../../../../effective-field-theory.md) is inconsistent.

The [Higgs mechanism](../../../../../higgs-mechanism.md) supplies a weakly coupled completion. For an Abelian example, take a [complex scalar field](../../../../../complex-scalar-field.md) with

$$
\mathcal L=-\frac14F^2+|D_\mu\phi|^2-\lambda(|\phi|^2-v^2/2)^2,\qquad D_\mu=\partial_\mu-igA_\mu.
$$

Locally write $\phi=(v+h)e^{i\chi/v}/\sqrt2$. Its [gauge-covariant kinetic term](../../../../../gauge-covariant-kinetic-term.md) becomes

$$
|D_\mu\phi|^2=\frac12(\partial_\mu h)^2+\frac12(v+h)^2(\partial_\mu\chi/v-gA_\mu)^2.
$$

The combination is invariant under $A_\mu\mapsto A_\mu+\partial_\mu\omega$, $\chi\mapsto\chi+gv\omega$. In [unitary gauge](../../../../../unitary-gauge.md) $\chi=0$, it contains $m^2A_\mu A^\mu/2$ with $m=gv$, as well as the correlated $hAA$ and $hhAA$ interactions. The two original gauge polarizations and two real scalar components become three massive-vector polarizations and one radial [Higgs boson](../../../../../higgs-boson.md). The would-be [Goldstone boson](../../../../../goldstone-boson.md) supplies the longitudinal state. This counting explains why the [Goldstone theorem](../../../../../goldstone-theorem.md) for spontaneously broken global symmetries does not imply an extra physical massless particle here. Local [gauge symmetry](../../../../../gauge-invariance.md) is a redundancy; choosing a Higgs background after [gauge fixing](../../../../../gauge-fixing.md) does not explicitly break the gauge invariance of the action.

The extra scalar interactions also repair high-energy scattering. By the [Goldstone-boson equivalence theorem](../../../../../goldstone-boson-equivalence-theorem.md), the leading longitudinal-vector amplitude can be computed using the would-be [Goldstone bosons](../../../../../goldstone-boson.md). For a charged-to-neutral channel in the linear scalar model, the scalar contact and radial-exchange terms give

$$
\mathcal M=-\frac{m_H^2}{v^2}-\frac{m_H^4}{v^2(s-m_H^2)}
=\frac{s}{v^2}-\frac{s^2}{v^2(s-m_H^2)}\longrightarrow-\frac{m_H^2}{v^2}.
$$

This [Higgs cancellation in longitudinal vector scattering](../../../../../higgs-cancellation-in-longitudinal-vector-scattering.md) removes the uncontrolled $s/v^2$ growth. It also shows why a very large scalar self-coupling would itself make perturbation theory unreliable; introducing a scalar is not a license to ignore [partial-wave unitarity](../../../../../partial-wave-unitarity.md).

Although the [unitary gauge](../../../../../unitary-gauge.md) propagator looks like the badly behaved [Proca propagator](../../../../../proca-propagator.md), renormalizability is conveniently established in an [R-xi gauge](../../../../../r-xi-gauge.md). Using Cartesian scalar fluctuations, the quadratic mixing is $-mA_\mu\partial^\mu\chi$. The gauge-fixing term $-(\partial\cdot A+\xi m\chi)^2/(2\xi)$ cancels it and gives

$$
D_{\mu\nu}^{(\xi)}(k)=\frac{-i}{k^2-m^2+i0}\left[g_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2-\xi m^2+i0}\right].
$$

At fixed finite $\xi$ this falls as $1/k^2$. The would-be scalar modes and [Faddeev-Popov ghosts](../../../../../faddeev-popov-ghost.md) remain in intermediate calculations. Gauge identities, organized through [BRST symmetry](../../../../../brst-symmetry.md), make unphysical states cancel from physical amplitudes and constrain counterterms to the gauge-invariant renormalizable form. With a renormalizable scalar sector and cancellation of [gauge anomalies](../../../../../gauge-anomaly.md), spontaneously broken gauge theory is renormalizable and unitary on its physical states; the bosonic construction is demonstrated in the [original massive Yang-Mills renormalizability proof](https://www.staff.science.uu.nl/~hooft101/gthpub/massive.pdf). The ultraviolet limit and $\xi\to\infty$ limit do not commute, so the unitary-gauge numerator alone is not a valid disproof of this result.

In the [Standard Model](../../../../../standard-model-split.md), a [Higgs doublet](../../../../../higgs-field.md) breaks the manifest electroweak group from $SU(2)_L\times U(1)_Y$ to $U(1)_{\rm em}$. The scalar kinetic term yields

$$
\boxed{M_W=gv/2,\qquad M_Z=\frac v2\sqrt{g^2+g'^2},\qquad M_\gamma=0.}
$$

Three scalar directions supply the longitudinal polarizations of $W^\pm$ and $Z$, while the unbroken electromagnetic generator leaves the [photon](../../../../../photon.md) massless. The radial [Higgs boson](../../../../../higgs-boson.md) remains physical.

There is an important Abelian alternative. The [Stueckelberg mechanism](../../../../../stueckelberg-mechanism.md) introduces a scalar with $\mathcal L_{\rm mass}=(mA_\mu-\partial_\mu\chi)^2/2$, invariant under $A\mapsto A+\partial\omega$, $\chi\mapsto\chi+m\omega$. With suitable conserved-current couplings this can describe a renormalizable massive Abelian gauge theory without a radial Higgs particle. A naive non-Abelian analogue involves a nonlinear group-valued scalar and derivative interactions suppressed by inverse powers of the symmetry-breaking scale; it is generally an [effective field theory](../../../../../effective-field-theory.md), not a power-counting-renormalizable substitute. Strongly coupled or composite sectors can provide other completions. **A free vector mass is consistent; the central problem is obtaining the longitudinal state and its interactions in a theory with controlled ultraviolet behavior and physical unitarity.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
