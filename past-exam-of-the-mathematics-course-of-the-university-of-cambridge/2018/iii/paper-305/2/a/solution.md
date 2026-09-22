<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [scalar potential](../../../../../../scalar-potential.md) can be written as

$$
V=\frac{\lambda}{4}(\phi_a\phi_a-v^2)^2-\frac{\lambda v^4}{4},\qquad v^2=-\frac{m^2}{\lambda}.
$$

Its [vacuum manifold](../../../../../../vacuum-manifold.md) is the sphere $\phi_a\phi_a=v^2$. The [Adjoint double cover from SU(2) to SO(3)](../../../../../../adjoint-double-cover-from-su-2-to-so-3.md) rotates any nonzero [vacuum expectation value](../../../../../../vacuum-expectation-value.md) to $(0,0,v)$, with $v>0$. A local [unitary gauge](../../../../../../unitary-gauge.md) removes the two angular fluctuations, leaving $\phi=(0,0,v+\eta)$. This choice holds in a neighbourhood of the nonzero vacuum; a single global rotation cannot align arbitrary position-dependent fields, and topologically nontrivial configurations can obstruct a global [unitary gauge](../../../../../../unitary-gauge.md).

The generator $t^3$ fixes the [vacuum expectation value](../../../../../../vacuum-expectation-value.md), while $t^1,t^2$ do not. Thus the [Higgs mechanism](../../../../../../higgs-mechanism.md) in this [SU(2) gauge theory with an adjoint Higgs field](../../../../../../su-2-gauge-theory-with-an-adjoint-higgs-field.md) gives

$$
\boxed{SU(2)\longrightarrow U(1).}
$$

The two angular [Goldstone bosons](../../../../../../goldstone-boson.md) become the longitudinal polarizations of two massive [gauge bosons](../../../../../../gauge-boson.md). Define physical fields

$$
A_\mu=B^3_\mu,\qquad W_\mu^\pm=\frac{B_\mu^1\mp iB_\mu^2}{\sqrt2}.
$$

These labels describe the fields of this model; they do not identify it with the [Standard Model](../../../../../../standard-model-split.md). With the stated [adjoint covariant derivative](../../../../../../adjoint-covariant-derivative.md),

$$
(D_\mu\phi)_1=-g(v+\eta)B_\mu^2,\quad (D_\mu\phi)_2=g(v+\eta)B_\mu^1,\quad (D_\mu\phi)_3=\partial_\mu\eta.
$$

To express all [Yang-Mills theory](../../../../../../yang-mills-theory.md) terms in physical fields, introduce the [gauge field strengths](../../../../../../gauge-field-strength.md)

$$
f_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu,\quad
Q_{\mu\nu}=W_\mu^+W_\nu^--W_\nu^+W_\mu^-,\quad
\mathcal W^\pm_{\mu\nu}=(\partial_\mu\pm igA_\mu)W_\nu^\pm-(\partial_\nu\pm igA_\nu)W_\mu^\pm.
$$

Then $F^3_{\mu\nu}=f_{\mu\nu}+igQ_{\mu\nu}$ and $(F^1_{\mu\nu}\mp iF^2_{\mu\nu})/\sqrt2=\mathcal W^\pm_{\mu\nu}$. Dropping the constant vacuum energy, the [Lagrangian density](../../../../../../lagrangian-density.md) is

$$
\begin{aligned}
\mathcal L={}&-\frac14(f_{\mu\nu}+igQ_{\mu\nu})(f^{\mu\nu}+igQ^{\mu\nu})-\frac12\mathcal W^+_{\mu\nu}\mathcal W^{-\mu\nu}
+\frac12\partial_\mu\eta\partial^\mu\eta\\
&-\lambda v^2\eta^2-\lambda v\eta^3-\frac\lambda4\eta^4+g^2(v+\eta)^2W_\mu^+W^{-\mu}.
\end{aligned}
$$

Taking the positive [gauge coupling](../../../../../../gauge-coupling.md) convention $g>0$, the canonically normalized [mass terms](../../../../../../mass-term.md) give

$$
\boxed{m_A=0,\qquad m_{W^+}=m_{W^-}=gv,\qquad m_\eta^2=2\lambda v^2=-2m^2.}
$$

The residual [U(1) gauge symmetry](../../../../../../u-1-gauge-symmetry.md) makes $W^\pm$ oppositely charged. The [Yang-Mills theory](../../../../../../yang-mills-theory.md) terms supply interactions of $A$ with $W^\pm$ and four-vector interactions. The [Higgs mode](../../../../../../higgs-mode.md) has cubic and quartic self-interactions, together with $2g^2v\eta W^+\cdot W^-$ and $g^2\eta^2W^+\cdot W^-$ couplings; it is neutral under the surviving [U(1) gauge symmetry](../../../../../../u-1-gauge-symmetry.md).

Coupling [fermions](../../../../../../fermion.md) permits a massless electromagnetic [gauge boson](../../../../../../gauge-boson.md) and massive charged mediators of the [weak interaction](../../../../../../weak-interaction.md); [fermion](../../../../../../fermion.md) couplings with [chirality](../../../../../../chirality-physics.md) can produce parity-violating [weak charged currents](../../../../../../charged-current.md). However, this model has **no massive neutral [Z boson](../../../../../../z-boson.md)**, and its only charge generator is $t^3$. A fundamental doublet has opposite charges, so it cannot reproduce the observed doublet charge assignments through an independent [hypercharge](../../../../../../hypercharge.md). The [Standard Model](../../../../../../standard-model-split.md) instead has $SU(2)_L\times U(1)_Y\to U(1)_Q$, a complex [Higgs doublet](../../../../../../higgs-field.md), three absorbed [Goldstone bosons](../../../../../../goldstone-boson.md), a massive [Z boson](../../../../../../z-boson.md) and a [weak mixing angle](../../../../../../weinberg-angle.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
