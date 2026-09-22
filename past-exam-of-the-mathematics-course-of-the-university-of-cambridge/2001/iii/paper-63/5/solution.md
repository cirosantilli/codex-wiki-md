<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For massless up and down [quarks](../../../../../quark.md), the [Quantum chromodynamics](../../../../../quantum-chromodynamics.md) kinetic term splits into two independent chirality sectors,

$$
\mathcal L_q=i\bar q_L\gamma^\mu D_\mu q_L+i\bar q_R\gamma^\mu D_\mu q_R.
$$

The colour [covariant derivative](../../../../../covariant-derivative.md) acts identically on both flavours and commutes with constant flavour matrices. Independent transformations $q_R\mapsto Aq_R$, $q_L\mapsto Bq_L$, with $A,B\in SU(2)$, therefore leave the action invariant. This is [chiral symmetry](../../../../../chiral-symmetry.md). The non-singlet axial transformations have traceless flavour generators, so they are not broken by the colour axial anomaly; the anomalous axial $U(1)$ is not being included in this symmetry.

For $V_{ij}=\bar q_{Lj}q_{Ri}$, transforming each index gives

$$
\boxed{V\mapsto AVB^\dagger=AVB^{-1}.}
$$

The nonzero condensate $\langle V\rangle=-vI$ is unchanged precisely when $A=B$. Thus [chiral symmetry breaking](../../../../../chiral-symmetry-breaking.md) leaves the diagonal vector subgroup $SU(2)_V$. Three of the six generators are broken, producing three massless [Goldstone bosons](../../../../../goldstone-boson.md) in the exact massless limit. They are the [pions](../../../../../pion.md), represented at low energy by the coset coordinate $U\in SU(2)$.

The [uniqueness of the two-derivative two-flavour chiral action](../../../../../uniqueness-of-the-two-derivative-two-flavour-chiral-action.md) follows from the symmetry, rather than merely from guessing an invariant. The chiral group acts transitively on $U$, so every derivative-free invariant is constant. At $U=I$, the stabilizer acts on the three tangent directions by conjugation, the irreducible rotation representation. Its invariant symmetric quadratic form is a single multiple of $\delta_{ab}$. Transporting that form around the group gives a unique invariant two-derivative metric. Equivalently, the [Maurer-Cartan form](../../../../../maurer-cartan-form.md) $U^\dagger\partial_\mu U$ is traceless, so an independent double-trace term vanishes; the remaining contracted single trace is the same metric. Lorentz invariance supplies the spacetime contraction. Up to total derivatives, a constant term and its overall coefficient, the massless action is therefore

$$
\boxed{\mathcal L_{\pi}=\frac{F^2}{4}\operatorname{tr}(\partial^\mu U^\dagger\partial_\mu U).}
$$

The positive coefficient is conveniently expressed through the [pion decay constant](../../../../../pion-decay-constant.md) $F$.

Use the [Pauli matrices](../../../../../pauli-matrices.md) with $\operatorname{tr}(\tau_a\tau_b)=2\delta_{ab}$. Expanding the [matrix exponential](../../../../../matrix-exponential.md) gives $\partial_\mu U=i\tau_a\partial_\mu\pi_a/F+\cdots$. Hence

$$
\mathcal L_{\pi}=\frac12\partial^\mu\boldsymbol\pi\cdot\partial_\mu\boldsymbol\pi+\cdots,
$$

so the three fields have canonical [kinetic terms](../../../../../kinetic-term.md). There is no nonconstant invariant potential in the exact chiral theory, consistent with their masslessness.

For real diagonal $M$, the two terms in the mass trace are

$$
\operatorname{tr}(MV)=m_u\bar u_Lu_R+m_d\bar d_Ld_R,\qquad \operatorname{tr}(MV^\dagger)=m_u\bar u_Ru_L+m_d\bar d_Rd_L.
$$

Their sum therefore gives the usual [Dirac mass](../../../../../dirac-mass-term.md) term,

$$
\mathcal L_m=-m_u\bar uu-m_d\bar dd.
$$

These terms explicitly break [chiral symmetry](../../../../../chiral-symmetry.md). In the low-energy [chiral perturbation theory](../../../../../chiral-perturbation-theory.md) prescription, $V\mapsto-vU$ yields

$$
\mathcal L_{\pi,m}=v\operatorname{tr}[M(U+U^\dagger)].
$$

The [Pauli matrix](../../../../../pauli-matrices.md) algebra implies $(\boldsymbol\pi\cdot\boldsymbol\tau)^2=|\boldsymbol\pi|^2I$. Thus

$$
U+U^\dagger=2I-\frac{|\boldsymbol\pi|^2}{F^2}I+O(\pi^4),
$$

and

$$
\mathcal L_{\pi,m}=2v(m_u+m_d)-\frac{v(m_u+m_d)}{F^2}|\boldsymbol\pi|^2+O(\pi^4).
$$

Comparing with the canonically normalized scalar mass term gives the [leading pion mass from a two-flavour condensate](../../../../../leading-pion-mass-from-a-two-flavour-condensate.md):

$$
\boxed{m_{\pi_1}^2=m_{\pi_2}^2=m_{\pi_3}^2=\frac{2v(m_u+m_d)}{F^2}.}
$$

Positive quark masses therefore give positive pion squared masses. Even if $m_u\ne m_d$, this leading action depends only on their sum and gives equal masses for all three [pions](../../../../../pion.md). Strong isospin-breaking effects beyond this order and electromagnetic effects can split them. In the condensate convention used here, $\langle\bar uu\rangle=\langle\bar dd\rangle=-2v$, which also explains the factor of two in the mass relation. The massive pions are [pseudo-Goldstone bosons](../../../../../pseudo-goldstone-boson.md), becoming massless as both quark masses tend to zero.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
