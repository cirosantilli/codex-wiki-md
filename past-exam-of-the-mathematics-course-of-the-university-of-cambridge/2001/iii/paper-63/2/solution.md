<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the current convention in the question, whose vertex prefactor is $g/(2\cos\theta_W)$. The [neutral-current vector and axial couplings](../../../../../neutral-current-vector-and-axial-couplings.md) are then

$$
c_V=T_3-2Q\sin^2\theta_W,\qquad c_A=T_3.
$$

For a charged [lepton](../../../../../lepton.md), $T_3=-1/2$, $Q=-1$, giving

$$
\boxed{c_V=2\sin^2\theta_W-\tfrac12,\qquad c_A=-\tfrac12.}
$$

For an active [neutrino](../../../../../neutrino.md), $T_3=1/2$, $Q=0$, so $c_V=c_A=1/2$. The right-handed weak singlet contribution is purely vectorlike in the charge term; combining it with the left-handed contribution gives precisely this Dirac-current form. These coefficients would be halved if the vertex prefactor were $g/\cos\theta_W$ instead.

Let $p=k+k'$ be the [Z boson](../../../../../z-boson.md) momentum and $k,k'$ the outgoing massless [lepton](../../../../../lepton.md) momenta. The [decay amplitude](../../../../../decay-amplitude.md) is

$$
\mathcal M=\frac{g}{2\cos\theta_W}\epsilon_\mu(p)\bar u(k)\gamma^\mu(c_V-c_A\gamma_5)v(k').
$$

Use the [fermion spin sums](../../../../../fermion-spin-sum.md) $\sum u\bar u=\not k$ and $\sum v\bar v=\not k'$. Anticommutation of $\gamma_5$ with the [Dirac gamma matrices](../../../../../gamma-matrices.md) gives the symmetric part of the trace,

$$
L_{\rm sym}^{\mu\nu}=4(c_V^2+c_A^2)[k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'].
$$

The vector-axial cross term is antisymmetric in $\mu,\nu$, and hence drops out of the [massive vector polarization sum](../../../../../polarization-sum-for-a-massive-vector-boson.md). The massless equations also give $p_\mu L^{\mu\nu}=0$: in the symmetric part, the first two contractions sum to $p^\nu k\cdot k'$, canceling the last; the antisymmetric term vanishes because $p=k+k'$. The longitudinal $p_\mu p_\nu/m_Z^2$ term therefore makes no contribution.

Since $2k\cdot k'=m_Z^2$, contraction with $-g_{\mu\nu}$ gives $4(c_V^2+c_A^2)m_Z^2$. Thus the [massless fermion Z decay spin sum](../../../../../massless-fermion-z-decay-spin-sum.md), including all three initial polarizations, is

$$
\boxed{\sum_{Z,\ell,\bar\ell\ {
m spins}}|\mathcal M|^2=\frac{g^2m_Z^2}{\cos^2\theta_W}(c_V^2+c_A^2).}
$$

To use this fully summed expression for the decay width of one unpolarized [Z boson](../../../../../z-boson.md), apply the [massive-vector spin average](../../../../../massive-vector-spin-average.md), dividing by three. The width of each fixed polarization is the same after integration over all directions, so that procedure also gives the physical single-particle width. Omitting the division would sum the widths of three initial states.

For two massless distinguishable final particles, the [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) is

$$
d\Phi_2=\frac{d\Omega}{32\pi^2},\qquad \int d\Phi_2=\frac1{8\pi}.
$$

Consequently

$$
\Gamma=\frac1{2m_Z}\frac13\sum|\mathcal M|^2\frac1{8\pi}=\frac{g^2m_Z}{48\pi\cos^2\theta_W}(c_V^2+c_A^2).
$$

The tree-level [electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md) relation is $m_W=m_Z\cos\theta_W$. Combining it with the [Fermi constant](../../../../../fermi-constant.md) normalization gives

$$
\boxed{\Gamma_{Z\to\ell\bar\ell}=\frac{G_Fm_Z^3}{6\sqrt2\pi}(c_V^2+c_A^2).}
$$

For an active [neutrino](../../../../../neutrino.md), the vertex itself projects out inactive chiralities, so no additional helicity factor is needed. This is the tree-level [massless leptonic Z decay width](../../../../../massless-leptonic-z-decay-width.md); lepton masses and radiative corrections have been excluded.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
