<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $t^A$ be [Hermitian](../../../../../hermitian-operator.md) color generators with $\operatorname{Tr}(t^At^B)=\delta^{AB}/2$, and take $D_\mu=\partial_\mu-ig_sG_\mu^At^A$. In explicit [spinor](../../../../../spinor.md), color and flavor indices the massless [kinetic term](../../../../../kinetic-term.md) is

$$
\mathcal L_q=i\sum_{\alpha,\beta,i,j,f}\bar q_{\alpha if}(\gamma^\mu)_{\alpha\beta}\bigl[\delta_{ij}\partial_\mu-ig_sG_\mu^A(t^A)_{ij}\bigr]q_{\beta jf}.
$$

The full [Quantum chromodynamics](../../../../../quantum-chromodynamics.md) [Lagrangian](../../../../../lagrangian.md) also has $-G_{\mu\nu}^AG^{A\mu\nu}/4$. A local color [gauge transformation](../../../../../gauge-transformation.md) acts as

$$
q_{\alpha if}(x)\mapsto V_{ij}(x)q_{\alpha jf}(x),\qquad \bar q_{\alpha if}\mapsto\bar q_{\alpha jf}(V^\dagger)_{ji},\qquad G_\mu\mapsto VG_\mu V^\dagger-\frac{i}{g_s}(\partial_\mu V)V^\dagger.
$$

Thus $D_\mu q\mapsto VD_\mu q$ and the [kinetic term](../../../../../kinetic-term.md) is [gauge-invariant](../../../../../gauge-invariance.md).

Since the [gauge coupling](../../../../../gauge-coupling.md) is independent of flavor and [chirality](../../../../../chirality-physics.md), the classical internal global transformations are $q_L\mapsto U_Lq_L$, $q_R\mapsto U_Rq_R$, with constant flavor matrices $U_L,U_R\in U(2)$. Equivalently these consist of $SU(2)_L\times SU(2)_R$, a common vector phase, and a singlet axial phase $q\mapsto e^{i\eta\gamma_5}q$, modulo shared discrete factors. The vector phase measures [quark](../../../../../quark.md) number, or [baryon number](../../../../../baryon-number.md) after dividing its generator by three. The nonsinglet axial rotations may be written $q\mapsto e^{-i\theta_a\gamma_5\tau_a/2}q$. At the quantum level the singlet axial phase is anomalous; the exact continuous internal [symmetry](../../../../../symmetry-physics.md) is $SU(2)_L\times SU(2)_R\times U(1)_V$ up to those discrete identifications. The usual spacetime Poincaré transformations also leave the theory invariant; the massless classical theory has [dilation](../../../../../uniform-dilation.md) [symmetry](../../../../../symmetry-physics.md), which is broken by quantum running. These distinctions are [massless two-flavor QCD symmetries](../../../../../massless-two-flavor-qcd-symmetries.md).

At equal time the canonical relations, including all indices, are

$$
\boxed{\{q_{\alpha if}(t,\mathbf x),q_{\beta jg}^\dagger(t,\mathbf y)\}=\delta_{\alpha\beta}\delta_{ij}\delta_{fg}\delta^{(3)}(\mathbf x-\mathbf y),\qquad\{q,q\}=\{q^\dagger,q^\dagger\}=0.}
$$

No constraint removes any of the four [spinor](../../../../../spinor.md) components of the [Dirac field](../../../../../dirac-field.md) in these equal-time relations.

To evaluate the [axial charges](../../../../../axial-charge.md), first prove the elementary [bilinear](../../../../../bilinear-map.md) identity. For any constant [matrix](../../../../../matrix.md) $K$ on the [spinor](../../../../../spinor.md)/flavor space,

$$
[\int q_I^\dagger K_{IJ}q_J\,d^3y,q_K(x)]=-K_{KJ}q_J(x),\qquad [\int q^\dagger Kq\,d^3y,q_K^\dagger(x)]=q_I^\dagger(x)K_{IK}.
$$

For example $[q_I^\dagger q_J,q_K]=q_I^\dagger\{q_J,q_K\}-\{q_I^\dagger,q_K\}q_J$; the spatial delta function collapses the [integral](../../../../../integral.md). This proves the charge action directly from the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md).

For $K_a=\gamma_5\tau_a/2$, anticommutation of $\gamma^0$ and $\gamma_5$ then gives

$$
[Q_{5,a},q]=-K_aq,\qquad[Q_{5,a},\bar q]=q^\dagger K_a\gamma^0=-\bar qK_a.
$$

The charge is an even operator, so its [commutator](../../../../../commutator.md) obeys the ordinary product rule. Consequently

$$
[Q_{5,a},S]=-\bar q(K_a+K_a)q=-\bar q\gamma_5\tau_aq=\boxed{iP_a}.
$$

Similarly, using $\gamma_5^2=1$ and the [Pauli matrices](../../../../../pauli-matrices.md) identity $\{\tau_a,\tau_b\}=2\delta_{ab}I$,

$$
[Q_{5,a},P_b]=-\frac i2\bar q\bigl(\tau_a\tau_b+\tau_b\tau_a\bigr)q=\boxed{-i\delta_{ab}S}.
$$

Composite fields can be defined with a common symmetry-preserving regulator; these nonsinglet identities have no color axial anomaly. This is the [nonsinglet axial charge algebra of quark densities](../../../../../nonsinglet-axial-charge-algebra-of-quark-densities.md).

If every conserved [axial charge](../../../../../axial-charge.md) left the vacuum invariant, the vacuum expectation of each such [commutator](../../../../../commutator.md) would vanish. A nonzero [quark chiral condensate](../../../../../quark-chiral-condensate.md) instead makes $\langle[Q_{5,a},P_b]\rangle=-i\delta_{ab}\langle S\rangle\ne0$ for $a=b$. It therefore diagnoses spontaneous breaking of the nonsinglet [chiral symmetry](../../../../../chiral-symmetry.md). In the massless two-flavor limit, the observed hadronic pattern is described by $SU(2)_L\times SU(2)_R\to SU(2)_V$, with three [Goldstone boson](../../../../../goldstone-boson.md) modes identified with the [pions](../../../../../pion.md). The vacuum condensate is a dynamical property of QCD, not something derivable from the canonical algebra alone. The light [pion](../../../../../pion.md) multiplet and absence of parity-degenerate light hadrons support this pattern; the singlet axial anomaly prevents interpreting an additional singlet mode as a fourth [Goldstone boson](../../../../../goldstone-boson.md).

For equal nonzero masses, add $\mathcal L_m=-m\bar qq$. It is invariant under local color [gauge transformation](../../../../../gauge-transformation.md)s and common vector flavor rotations, but not under independent left/right rotations. The exact continuous [flavor symmetry](../../../../../flavor-symmetry.md) becomes $SU(2)_V\times U(1)_V$. The [kinetic term](../../../../../kinetic-term.md) and canonical [anticommutators](../../../../../anticommutator.md) are unchanged, and the two proved equal-time [commutators](../../../../../commutator.md) still hold. The charges, however, are no longer conserved:

$$
\boxed{\partial_\mu A_a^\mu=mP_a,\qquad A_a^\mu=\tfrac12\bar q\gamma^\mu\gamma_5\tau_aq,\qquad\dot Q_{5,a}=m\int P_a\,d^3x.}
$$

The first equation follows from the massive [Dirac equations](../../../../../dirac-equation.md), or the last from $H_m=m\int S$ and $\dot Q=i[H,Q]$. This is the [flavor-nonsinglet axial Ward identity with equal quark masses](../../../../../flavor-nonsinglet-axial-ward-identity-with-equal-quark-masses.md). The [pions](../../../../../pion.md) become [pseudo-Goldstone bosons](../../../../../pseudo-goldstone-boson.md) with $m_\pi^2=O(m)$, rather than exact massless modes. To leading order, in the convention $S=\bar uu+\bar dd$, $f_\pi^2m_\pi^2=-m\langle S\rangle+O(m^2)$. The condensate persists for small masses, but the [symmetry](../../../../../symmetry-physics.md) is now explicitly broken, so the exact-symmetry Goldstone argument is replaced by an approximate one. The singlet anomaly and [gauge symmetry](../../../../../gauge-invariance.md) are unaffected.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
