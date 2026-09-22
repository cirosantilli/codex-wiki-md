# Paper 305

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_305.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_305.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
    - [v](#3/a/v)
      - [Solution](#3/a/v/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In the [mode expansion of a Dirac field](../../../relativistic-quantum-field.md#mode-expansion-of-a-dirac-field), $b^s(p)$ is the [fermionic annihilation operator](../../../relativistic-quantum-field.md#fermionic-annihilation-operator) for a particle of [four-momentum](../../../special-relativity.md#four-momentum) $p$ and [spin angular momentum](../../../quantum-mechanics.md#spin) label $s$, while $d^{s\dagger}(p)$ is the [fermionic creation operator](../../../relativistic-quantum-field.md#fermionic-creation-operator) for the corresponding [antiparticle](../../../relativistic-quantum-field.md#antiparticle). The [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) $u^s(p)$ is the positive-frequency particle wavefunction and $v^s(p)$ is the negative-frequency antiparticle wavefunction; they solve $(\not p-m)u^s=0$ and $(\not p+m)v^s=0$, respectively.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Apply the [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) to the given [mode expansion of a Dirac field](../../../relativistic-quantum-field.md#mode-expansion-of-a-dirac-field):

$$
\widehat P\psi(x)\widehat P^{-1}
=\sum_{p,s}\left[\eta_Pb^s(p_P)u^s(p)e^{-ip\cdot x}
-\eta_Pd^{s\dagger}(p_P)v^s(p)e^{ip\cdot x}\right].
$$

The stated [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor) identities are equivalently $u^s(p)=\gamma^0u^s(p_P)$ and $v^s(p)=-\gamma^0v^s(p_P)$. Relabel the momentum sum by $p\mapsto p_P$ and use $p_P\cdot x=p\cdot x_P$ to obtain

$$
\widehat P\psi(x)\widehat P^{-1}
=\eta_P\gamma^0\sum_{p,s}\left[b^s(p)u^s(p)e^{-ip\cdot x_P}+d^{s\dagger}(p)v^s(p)e^{ip\cdot x_P}\right]
=\boxed{\eta_P\gamma^0\psi(x_P)}.
$$

The phase $|\eta_P|=1$ is the intrinsic parity convention.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $\psi^P(x)=\eta_P\gamma^0\psi(x_P)$. The [chain rule](../../../calculus.md#chain-rule) gives $\partial_0\psi(x_P)=(\partial_0\psi)(x_P)$ and $\partial_i\psi(x_P)=-(\partial_i\psi)(x_P)$. Using the [gamma matrix](../../../algebra.md#gamma-matrices) relations $(\gamma^0)^2=1$ and $\gamma^i\gamma^0=-\gamma^0\gamma^i$,

$$
\begin{aligned}
(i\gamma^\mu\partial_\mu-m)\psi^P(x)
&=\eta_P\left(i\gamma^0\gamma^0\partial_0-i\gamma^i\gamma^0\partial_i-m\gamma^0\right)\psi(x_P)\\
&=\eta_P\gamma^0(i\gamma^\mu\partial_\mu-m)\psi(x_P)=0.
\end{aligned}
$$

Thus the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) is invariant under [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) interaction is $\mathcal L_{\rm int}=-e j^\mu A_\mu$, where the [Dirac electromagnetic current](../../../quantum-field-theory.md#dirac-electromagnetic-current) is $j^\mu=\bar\psi\gamma^\mu\psi$. Under [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory),

$$
j^\mu(x)\mapsto {\Lambda_P^\mu}_\nu j^\nu(x_P),
\qquad \Lambda_P=\operatorname{diag}(1,-1,-1,-1).
$$

Invariance of the interaction therefore requires the [electromagnetic four-potential](../../../electromagnetism.md#electromagnetic-four-potential) to transform as the same [Lorentz four-vector](../../../special-relativity.md#four-vector):

$$
\boxed{\widehat P A^\mu(x)\widehat P^{-1}={\Lambda_P^\mu}_\nu A^\nu(x_P)},
$$

so $A^0$ is parity even and $\mathbf A$ is parity odd. Under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), the current is odd, $j^\mu\mapsto-j^\mu$, so invariance requires

$$
\boxed{\widehat C A^\mu(x)\widehat C^{-1}=-A^\mu(x)}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The operator $ia\bar\psi\sigma^{\mu\nu}\gamma^5\psi F_{\mu\nu}$ is the relativistic [fermion electric dipole moment operator](../../../quantum-field-theory.md#fermion-electric-dipole-moment-operator). Its nonrelativistic limit contains $\mathbf S\cdot\mathbf E$: [spin angular momentum](../../../quantum-mechanics.md#spin) is an [axial vector](../../../vector-space.md#pseudovector), whereas the [electric field](../../../electromagnetism.md#electric-field) is a polar vector. It is consequently odd under [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory). Both the pseudotensor fermion bilinear and the [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor) are odd under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), so their product is even. Therefore

$$
\boxed{P:-1,\qquad C:+1,\qquad CP:-1.}
$$

The [CPT theorem](../../../quantum-field-theory.md#cpt-theorem) then makes it odd under [time-reversal symmetry](../../../quantum-field-theory.md#t-symmetry). Such an interaction can arise only from [CP violation](../../../quantum-field-theory.md#cp-violation). The [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) therefore induces a nonzero Standard Model electric dipole moment at sufficiently high loop order, but its flavor structure and loop suppressions make the result extraordinarily small.

## 2

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $V_i=\partial V/\partial\phi_i$ and $M^2_{ij}=\partial_i\partial_jV|_{\phi_0}$ be the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix), which is the [Hessian matrix](../../../calculus.md#hessian-matrix) of the [scalar potential](../../../quantum-field-theory.md#scalar-potential) at the vacuum. Invariance under the infinitesimal [Lie group action](../../../lie-theory.md#lie-group-action) gives

$$
V_i(\phi)(it^a\phi)_i=0.
$$

Differentiate with respect to $\phi_j$ and evaluate at the [vacuum expectation value](../../../quantum-field-theory.md#vacuum-expectation-value) $\phi_0$. Since $V_i(\phi_0)=0$ at a minimum,

$$
M^2_{ji}(it^a\phi_0)_i=0.
$$

Thus every tangent vector $it^a\phi_0$ generated by a broken [Lie algebra generator](../../../lie-algebra.md#lie-algebra-generator) is a [zero eigenvalue](../../../linear-operator-theory.md#zero-eigenvalue) eigenvector of the [scalar mass matrix](../../../quantum-field-theory.md#scalar-mass-matrix). The unbroken generators are precisely those in the stabilizer Lie algebra $\mathfrak h$ and give the zero tangent vector; independent broken directions span $\mathfrak g/\mathfrak h$. Hence [Goldstone theorem](../../../quantum-field-theory.md#goldstone-theorem) gives

$$
\boxed{\dim G-\dim H}
$$

massless scalar modes at the classical level.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The minima of the [scalar potential](../../../quantum-field-theory.md#scalar-potential)

$$
V(\phi)=m^2\phi^\dagger\phi+\frac\lambda2(\phi^\dagger\phi)^2
$$

satisfy

$$
\phi^\dagger\phi=-\frac{m^2}{\lambda}=\frac{v^2}{2},
\qquad
v^2=-\frac{2m^2}{\lambda}.
$$

The [SU(2) group](../../../topological-group.md#su-2-group) acts transitively on this three-sphere of vacua, and the stabilizer of a nonzero fundamental doublet is trivial. A global transformation may therefore choose $\phi_0=(0,v)^T/\sqrt2$. Because the symmetry is gauged, [unitary gauge](../../../standard-model.md#unitary-gauge) removes all three angular [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson), leaving only the real radial [Higgs mode](../../../quantum-field-theory.md#higgs-mode) $h$:

$$
\phi(x)=\frac1{\sqrt2}\binom0{v+h(x)}.
$$

Substitution into the [gauge-covariant kinetic term](../../../quantum-field-theory.md#gauge-covariant-kinetic-term) gives

$$
\boxed{
\mathcal L=-\frac14F^a_{\mu\nu}F^{a\mu\nu}
+\frac12(\partial h)^2+\frac{g^2}{8}(v+h)^2B^a_\mu B^{a\mu}
-\frac12m_h^2h^2-\frac{\lambda v}{2}h^3-\frac\lambda8h^4+\text{constant}
}
$$

with

$$
\boxed{m_h^2=\lambda v^2=-2m^2,\qquad m_B^2=\frac{g^2v^2}{4}.}
$$

The interaction terms produce $h^3$, $h^4$, $hBB$, $hhBB$, and the cubic and quartic non-Abelian gauge-boson vertices shown below.

<a id="2/b/image-interaction-vertices-after-complete-su-2-symmetry-breaking"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-305-higgs-interactions.png)

**[Figure 1](#2/b/image-interaction-vertices-after-complete-su-2-symmetry-breaking). Interaction vertices after complete SU(2) symmetry breaking**.

The three broken generators supply the three longitudinal polarizations of the equally massive gauge bosons. No physical massless [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson) remains, and because the unbroken subgroup is trivial there is no massless [gauge boson](../../../relativistic-quantum-field.md#gauge-boson) either. The remaining physical spectrum has $3\times3+1=10$ degrees of freedom, equal to the original $3\times2+4=10$.

## 3

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

**Forbidden at tree level.** A photon, gluon, $Z$ boson, or neutral Higgs interaction is flavor diagonal in the quark mass basis, while a $W$ boson connects an up-type quark to a down-type quark. The process $u\bar c\to c\bar u$ would therefore require a [flavor-changing neutral current](../../../standard-model.md#flavor-changing-neutral-current), which first appears through loops in the [Standard Model](../../../standard-model.md).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

**Allowed.** A single $t$-channel [W boson](../../../standard-model.md#w-boson) mediates the [weak charged current](../../../standard-model.md#charged-current) transitions $u\to d$ and $\bar c\to\bar s$. The amplitude is proportional to the [Cabibbo-Kobayashi-Maskawa matrix](../../../standard-model.md#cabibbo-kobayashi-maskawa-matrix) product $V_{ud}V_{cs}^*$.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

**Forbidden.** The initial state has total [lepton number](../../../standard-model.md#lepton-number) two and the final state has total lepton number minus two. No renormalizable Standard Model vertex changes total lepton number by four.

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/a/iv)

**Allowed.** There are two [tree-level Feynman diagrams](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram): $t$-channel [Z boson](../../../standard-model.md#z-boson) exchange through the [weak neutral current](../../../standard-model.md#neutral-current), and $s$-channel $W^+$ formation through the [weak charged current](../../../standard-model.md#charged-current).

<h4 id="3/a/v">v</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/v/solution">Solution</h5>

↑ **Parent:** [V](#3/a/v)

**Allowed.** There are again two [tree-level Feynman diagrams](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram): $t$-channel [Z boson](../../../standard-model.md#z-boson) exchange and the crossed charged-current diagram with a [W boson](../../../standard-model.md#w-boson) exchanged between the neutrino and electron lines.

The complete tree-level list for (ii), (iv), and (v) is:

<a id="3/a/v/image-tree-level-processes-in-the-standard-model"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-305-standard-model-processes.png)

**[Figure 2](#3/a/v/image-tree-level-processes-in-the-standard-model). Tree-level processes in the Standard Model**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The first four-fermion operator is the low-energy [Fermi interaction](../../../quantum-field-theory.md#fermi-interaction) obtained by replacing the crossed $W$ propagator in the charged-current diagram by $-g_{\mu\nu}/M_W^2$. The second operator is obtained analogously from the $Z$-exchange [weak neutral current](../../../standard-model.md#neutral-current); $c_V$ and $c_A$ are its electron vector and axial-vector couplings. Thus the two terms represent respectively the charged-current and neutral-current diagrams in part (v), with their interference retained when the amplitude is squared.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A [Fierz rearrangement](../../../quantum-field-theory.md#fierz-identity) puts the charged-current operator in the same current ordering as the neutral-current operator. Accounting for the interchange of fermionic fields, the combined amplitude is

$$
\mathcal M=\frac{G_F}{\sqrt2}
[\bar u(k')\gamma^\alpha(1-\gamma^5)u(k)]
[\bar u(p')\gamma_\alpha(C_V-C_A\gamma^5)u(p)],
\qquad C_V=c_V+1,\quad C_A=c_A+1.
$$

Sum over final spins and average over the initial electron spin. The [fermion spin sum](../../../relativistic-quantum-field.md#fermion-spin-sum) and [gamma-matrix trace](../../../relativistic-quantum-field.md#gamma-matrix-trace) identities give

$$
\overline{|\mathcal M|^2}
=4G_F^2\left[(C_V+C_A)^2s^2+(C_V-C_A)^2u^2\right].
$$

For massless two-body scattering in the [centre-of-momentum frame](../../../special-relativity.md#center-of-momentum-frame), $d\sigma/dt=\overline{|\mathcal M|^2}/(16\pi s^2)$ and $u=-s-t$. Integrating $-s\leq t\leq0$ therefore yields

$$
\begin{aligned}
\sigma
&=\frac{G_F^2s}{4\pi}\left[(c_V+c_A+2)^2+\frac13(c_V-c_A)^2\right]\\
&=\boxed{\frac{G_F^2s}{3\pi}\left(c_V^2+c_A^2+c_Vc_A+3c_V+3c_A+3\right)}.
\end{aligned}
$$

Consequently

$$
\boxed{H(s)=\frac{s}{3\pi},\qquad B=1,\quad C=1,\quad D=3,\quad E=3,\quad F=3.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The result grows linearly with the squared [centre-of-momentum energy](../../../special-relativity.md#centre-of-momentum-energy), $\sigma\propto G_F^2s$. This growth eventually violates [partial-wave unitarity](../../../quantum-mechanics.md#partial-wave-unitarity) and signals the breakdown of the pointlike [Fermi interaction](../../../quantum-field-theory.md#fermi-interaction). At energies comparable to $M_W$ or $M_Z$, the full gauge-boson propagators must replace the contact interaction; the renormalizable electroweak theory then softens the high-energy behavior.

## 4

↑ **Parent:** [Paper 305](paper-305.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Since $\alpha_i=g_i^2/(4\pi)$, the stated [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) implies

$$
\frac{d\alpha_i}{d\log\mu}=-\frac{\beta_i}{2\pi}\alpha_i^2,
\qquad
\frac{d\alpha_i^{-1}}{d\log\mu}=\frac{\beta_i}{2\pi}.
$$

For $\beta_i>0$, the [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) decreases at high energy: the theory is [asymptotically free](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) and becomes strong in the infrared, as in [Quantum chromodynamics](../../../standard-model.md#quantum-chromodynamics). For $\beta_i<0$, it is infrared free but grows toward an ultraviolet [Landau pole](../../../perturbative-quantum-field-theory.md#landau-pole).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Integrating the [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) and defining $\Lambda$ by $\alpha_3^{-1}(\Lambda)=0$ gives

$$
\alpha_3^{-1}(\mu)=\frac{\beta_3}{2\pi}\log\frac\mu\Lambda,
$$

so

$$
\boxed{\alpha_3(\mu)=\frac{2\pi}{\beta_3\log(\mu/\Lambda)}}.
$$

The scale $\Lambda$ is the [QCD scale](../../../standard-model.md#qcd-scale) in this one-loop approximation.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Direct integration between the two [renormalization scales](../../../perturbative-quantum-field-theory.md#renormalization-scale) gives

$$
\boxed{\alpha_i^{-1}(\mu)=\alpha_i^{-1}(m_Z)+\frac{\beta_i}{2\pi}\log\frac{\mu}{m_Z}}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Put $L=(2\pi)^{-1}\log(M_{\rm GUT}/m_Z)$. At the [gauge coupling unification](../../../perturbative-quantum-field-theory.md#gauge-coupling-unification) scale, write the common normalized coupling as $\alpha_U=\alpha_2(M_{\rm GUT})=\alpha_3(M_{\rm GUT})=(5/3)\alpha_1(M_{\rm GUT})$. Running downward gives

$$
\alpha_3^{-1}(m_Z)=\alpha_U^{-1}-\beta_3L,
\quad
\alpha_2^{-1}(m_Z)=\alpha_U^{-1}-\beta_2L,
\quad
\frac35\alpha_1^{-1}(m_Z)=\alpha_U^{-1}-\frac35\beta_1L.
$$

Subtracting the second equation from the third determines

$$
L=\frac{\frac35\alpha_1^{-1}(m_Z)-\alpha_2^{-1}(m_Z)}{\beta_2-\frac35\beta_1}.
$$

Eliminating $L$ from the first two equations yields

$$
\boxed{
\alpha_3^{-1}(m_Z)=\alpha_2^{-1}(m_Z)
+\frac{\beta_3-\beta_2}{\frac35\beta_1-\beta_2}
\left[\frac35\alpha_1^{-1}(m_Z)-\alpha_2^{-1}(m_Z)\right].
}
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For one generation, the [Standard Model representation](../../../standard-model.md#standard-model-representation) content under $SU(2)_L\times SU(3)_C$ is

$$
Q_L=(u_L,d_L):(\mathbf2,\mathbf3),\quad
u_R:(\mathbf1,\mathbf3),\quad d_R:(\mathbf1,\mathbf3),
$$



$$
L_L=(\nu_{eL},e_L):(\mathbf2,\mathbf1),\quad
e_R:(\mathbf1,\mathbf1),\quad
H:(\mathbf2,\mathbf1),
$$

with no [right-handed neutrino](../../../standard-model.md#right-handed-neutrino). For $SU(3)_C$, three generations give $n_L=6$ from the two left-handed quark flavors and $n_R=6$ from the two right-handed quark flavors, while $n_s=0$. Therefore

$$
\boxed{\beta_3=\frac{11}{3}(3)-\frac13(6+6)=7.}
$$

For $SU(2)_L$, each generation supplies three colored quark doublets and one lepton doublet, so $n_L=12$, $n_R=0$, and the single complex [Higgs doublet](../../../standard-model.md#higgs-field) gives $n_s=1$. Hence

$$
\boxed{\beta_2=\frac{11}{3}(2)-\frac13(12)-\frac16=\frac{19}{6}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
