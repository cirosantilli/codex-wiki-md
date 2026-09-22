<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The strong-interaction matrix element between two spin-zero [pseudoscalar mesons](../../../../../pseudoscalar-meson.md) has only $p^\mu$ and $k^\mu$ available. The product of the two intrinsic [parities](../../../../../parity.md) is positive. An [axial current](../../../../../axial-current.md) would require a [pseudovector](../../../../../pseudovector.md) constructed from these momenta, but an expression involving the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) needs three independent four-vectors and therefore vanishes. This is a consequence of [parity conservation](../../../../../parity-conservation.md) in the hadronic matrix element, not of parity conservation in the weak interaction. The [vector current](../../../../../vector-current.md) can have the two independent structures $p+k$ and $p-k$. Its coefficients are [Lorentz scalars](../../../../../lorentz-scalar.md); with $p^2=m_K^2$ and $k^2=m_\pi^2$ fixed, their only varying invariant is $s=q^2$. Hence

$$
H^\mu=\langle\pi^+(k)|\bar u\gamma^\mu s|\bar K^0(p)\rangle
=(p+k)^\mu f_+(s)+q^\mu f_-(s).
$$

These are the [pseudoscalar-to-pseudoscalar form factors](../../../../../pseudoscalar-to-pseudoscalar-form-factor.md). With relativistically normalized states they are dimensionless. The vanishing axial matrix element and this decomposition explain the two equalities separately.

Write $q_1$ and $q_2$ for the outgoing electron and antineutrino momenta. From the [Fermi interaction](../../../../../fermi-interaction.md), an invariant [scattering amplitude](../../../../../scattering-amplitude.md), up to an irrelevant overall sign or phase, is

$$
\mathcal M=\frac{G_FV_{us}}{\sqrt2}\,
\bar u(q_1)\gamma_\mu(1-\gamma^5)v(q_2)
\left[(p+k)^\mu f_+(s)+q^\mu f_-(s)\right].
$$

The [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) element $V_{us}$ multiplies the quark current in the convention of this interaction. Let $\ell_\mu=\bar u(q_1)\gamma_\mu(1-\gamma^5)v(q_2)$. For massless leptons, the [massless Dirac equation](../../../../../massless-dirac-equation.md) and [chirality matrix](../../../../../chirality-matrix.md) anticommutation give

$$
q^\mu\ell_\mu=\bar u(q_1)(\not q_1+\not q_2)(1-\gamma^5)v(q_2)=0.
$$

In the second term move $\not q_2$ through the [chiral projector](../../../../../chiral-projector.md) before applying $\not q_2v=0$. Since $p+k=2p-q$, this [transverse massless leptonic current](../../../../../transverse-massless-leptonic-current.md) gives

$$
\boxed{\mathcal M=\sqrt2\,G_FV_{us}f_+(s)\,p^\mu\ell_\mu.}
$$

The disappearance of $f_-$ uses the massless approximation; for a massive charged lepton its contraction is proportional to the lepton mass.

Use the [fermion spin sum](../../../../../fermion-spin-sum.md) and the supplied [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md). The symmetric part of the [leptonic tensor](../../../../../leptonic-tensor.md) is

$$
L_{\mu\nu}=8\left(q_{1\mu}q_{2\nu}+q_{1\nu}q_{2\mu}-g_{\mu\nu}q_1\cdot q_2\right)+L_{\mu\nu}^{\mathrm{antisym}}.
$$

The [Levi-Civita symbol](../../../../../levi-civita-symbol.md) term is antisymmetric and drops out when contracted with $p^\mu p^\nu$. Thus

$$
\sum_{\mathrm{spins}}|\mathcal M|^2=16G_F^2|V_{us}|^2|f_+(s)|^2
\left[2(p\cdot q_1)(p\cdot q_2)-m_K^2(q_1\cdot q_2)\right].
$$

There is no initial-spin average because the kaon is spinless. For the [integrated massless leptonic tensor](../../../../../integrated-massless-leptonic-tensor.md), keep every factor of $2\pi$ explicit and define the unnormalized two-lepton [Lorentz-invariant phase space](../../../../../lorentz-invariant-phase-space.md)

$$
I_{\mu\nu}=\int\frac{d^3q_1}{q_1^0}\frac{d^3q_2}{q_2^0}
\delta^{(4)}(q-q_1-q_2)q_{1\mu}q_{2\nu}
=\frac\pi3 q_\mu q_\nu+\frac\pi6 g_{\mu\nu}s.
$$

The leptons are massless, so $q_i^0=|\boldsymbol q_i|$. Its trace is $g^{\mu\nu}I_{\mu\nu}=\pi s$. Therefore

$$
2p^\mu p^\nu I_{\mu\nu}-m_K^2g^{\mu\nu}I_{\mu\nu}
=\frac{2\pi}{3}\left[(p\cdot q)^2-m_K^2s\right].
$$

The three [Lorentz-invariant phase-space measures](../../../../../lorentz-invariant-phase-space-measure.md) and their momentum delta function contribute $1/[8(2\pi)^5]$, in addition to $1/(2m_K)$ in the [decay rate](../../../../../decay-width.md). Combining them with the spin sum gives

$$
\boxed{\Gamma=\frac{G_F^2|V_{us}|^2}{48\pi^4m_K}
\int\frac{d^3k}{k^0}\left[(p\cdot q)^2-m_K^2q^2\right]|f_+(q^2)|^2,\quad
A=\frac{G_F^2|V_{us}|^2}{48\pi^4m_K}.}
$$

This [massless semileptonic pseudoscalar decay rate](../../../../../massless-semileptonic-pseudoscalar-decay-rate.md) uses a two-lepton integral over future-timelike $q$ and the pion integral is restricted to the physically allowed region. The null endpoint follows by continuity. The coefficient has mass dimension $-5$, so the complete expression has mass dimension one, as a [decay rate](../../../../../decay-width.md) must in natural units.

In the kaon [centre-of-momentum frame](../../../../../center-of-momentum-frame.md), put $E=k^0$ and $\kappa=|\boldsymbol k|$. Then

$$
s=m_K^2+m_\pi^2-2m_KE,\qquad
(p\cdot q)^2-m_K^2s=m_K^2(E^2-m_\pi^2)=m_K^2\kappa^2.
$$

The dimensionally consistent [Källén function](../../../../../kallen-function.md) is

$$
\lambda(s,m_K^2,m_\pi^2)=s^2+m_K^4+m_\pi^4-2sm_K^2-2sm_\pi^2-2m_K^2m_\pi^2,
\qquad \kappa=\frac{\sqrt\lambda}{2m_K}.
$$

The pion-only mass term must have fourth power: the second power printed in the PDF is dimensionally inconsistent. This repair also follows directly from squaring $E=(m_K^2+m_\pi^2-s)/(2m_K)$. Angular integration and the change of variable give

$$
\frac{d^3k}{k^0}=4\pi\frac{\kappa^2}{E}\,d\kappa
=-\frac{2\pi\kappa}{m_K}\,ds
=-\frac{\pi\sqrt\lambda}{m_K^2}\,ds,
$$

where the negative sign reverses the endpoints. Combining this with the bracket $\lambda/4$ yields

$$
\boxed{\Gamma=\frac{G_F^2|V_{us}|^2}{192\pi^3m_K^3}
\int_0^{(m_K-m_\pi)^2} ds\,\lambda(s,m_K^2,m_\pi^2)^{3/2}|f_+(s)|^2.}
$$

Thus $\boxed{B=G_F^2|V_{us}|^2/(192\pi^3m_K^3),\ a=0,\ b=(m_K-m_\pi)^2}$. The lower limit is the minimum invariant mass of two massless leptons; at the upper limit the pion is at rest. The coefficient has mass dimension $-7$, while $ds\,\lambda^{3/2}$ has dimension eight. The [Källén function](../../../../../kallen-function.md) also shows why the differential [decay rate](../../../../../decay-width.md) vanishes at zero pion momentum.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
