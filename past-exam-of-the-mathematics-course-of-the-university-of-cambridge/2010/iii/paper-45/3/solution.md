<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The product of leptonic [weak charged currents](../../../../../charged-current.md) in the [Fermi interaction](../../../../../fermi-interaction.md) contains four-fermion cross terms such as

$$
-\frac{G_F}{\sqrt2}[\bar e\gamma^\alpha(1-\gamma_5)\nu_e][\bar\nu_\mu\gamma_\alpha(1-\gamma_5)\mu]+\mathrm{h.c.}
$$

This produces $\mu^-\to e^-+\bar\nu_e+\nu_\mu$, and the same interaction permits neutrino-electron scattering and inverse muon decay. Pure electromagnetic interactions have no neutrino coupling and preserve the separate charged-lepton species, so cannot produce these processes by themselves. The factor $1-\gamma_5=2P_L$ fixes the chiral structure of the [weak charged current](../../../../../charged-current.md).

The pion is a [pseudoscalar](../../../../../pseudoscalar.md) with negative parity, while the strong-interaction vacuum is parity even. [Lorentz covariance](../../../../../lorentz-covariance.md) restricts a vacuum-to-pion vector-current matrix element to $a p^\alpha$. In the pion rest frame only its temporal component could be nonzero, but a vector current's temporal component is parity even, whereas the pion is parity odd. The matrix element therefore equals its negative and vanishes. The temporal component of an [axial current](../../../../../axial-current.md) is parity odd, so its matrix element is allowed and Lorentz covariance fixes it to a constant times $p^\alpha$. Defining the [pion decay constant](../../../../../pion-decay-constant.md) in the printed normalization gives

$$
\langle0|J_{\rm hadrons}^\alpha|\pi^-(p)\rangle=-i\sqrt2F_\pi p^\alpha.
$$

This proves both the vector-current exclusion and the axial-current form; $F_\pi$ itself is a strong-interaction parameter, not fixed by symmetry.

The cross term $J_{\rm leptons}^{\alpha\dagger}J_\alpha^{\rm hadrons}$ gives, up to an irrelevant overall phase, the [decay amplitude](../../../../../decay-amplitude.md)

$$
\mathcal M=G_FF_\pi p_\alpha\bar u_e(k)\gamma^\alpha(1-\gamma_5)v_\nu(q).
$$

Take the antineutrino mass to be zero. Since $p=k+q$, $\bar u_e\not k=m_e\bar u_e$, and $\not qv_\nu=0$, anticommutation with $\gamma_5$ gives

$$
\boxed{\mathcal M=G_FF_\pi m_e\bar u_e(k)(1-\gamma_5)v_\nu(q).}
$$

The amplitude has [helicity suppression](../../../../../helicity-suppression.md) by one power of the charged-lepton mass.

Using the external spin sums, with no initial spin average for a spin-zero pion,

$$
\begin{aligned}
\sum_{\rm spins}|\mathcal M|^2
&=G_F^2F_\pi^2m_e^2\operatorname{Tr}[(\not k+m_e)(1-\gamma_5)\not q(1+\gamma_5)]\\
&=8G_F^2F_\pi^2m_e^2\,k\cdot q\\
&=4G_F^2F_\pi^2m_e^2(M_\pi^2-m_e^2).
\end{aligned}
$$

The middle equality follows from $(1-\gamma_5)\not q=\not q(1+\gamma_5)$, $(1+\gamma_5)^2=2(1+\gamma_5)$, and the [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md). Summing a full massless neutrino spin basis introduces no factor of two: the current projector annihilates the inactive helicity.

For completeness, evaluate the [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) in the pion rest frame. Its three-momentum delta function sets $\mathbf q=-\mathbf k$, and the energy delta function is $\delta(M_\pi-\sqrt{|\mathbf k|^2+m_e^2}-|\mathbf k|)$. The radial root is

$$
|\mathbf k|=\frac{M_\pi^2-m_e^2}{2M_\pi}.
$$

Combining its derivative with $1/(4E_k|\mathbf k|)$ and integrating solid angle gives

$$
\int d\Phi_2=\frac{|\mathbf k|}{4\pi M_\pi}=\frac1{8\pi}\left(1-\frac{m_e^2}{M_\pi^2}\right).
$$

The invariant squared amplitude is independent of direction, so the supplied decay formula yields the [leptonic pseudoscalar decay width](../../../../../leptonic-pseudoscalar-decay-width.md)

$$
\boxed{\Gamma_{\pi^-\to e^-\bar\nu_e}=\frac{G_F^2F_\pi^2}{4\pi}M_\pi m_e^2\left(1-\frac{m_e^2}{M_\pi^2}\right)^2.}
$$

The denominator is $4\pi$ because the matrix element contains $\sqrt2F_\pi$. With the alternative definition $f_\pi=\sqrt2F_\pi$, the same width is $G_F^2f_\pi^2M_\pi m_e^2(1-m_e^2/M_\pi^2)^2/(8\pi)$. In either convention it vanishes as $m_e\to0$.

Replacing the electron by a muon gives the same hadronic factor and weak coupling. Hence the [pion electron-to-muon decay ratio](../../../../../pion-electron-to-muon-decay-ratio.md) is

$$
\boxed{\frac{\Gamma_{\pi^-\to e^-\bar\nu_e}}{\Gamma_{\pi^-\to\mu^-\bar\nu_\mu}}=\frac{m_e^2}{m_\mu^2}\left(\frac{1-m_e^2/M_\pi^2}{1-m_\mu^2/M_\pi^2}\right)^2.}
$$

This is a tree-level result with massless neutrinos. The cancellation of $F_\pi$ and $G_F$ makes the ratio a clean test of the predicted [helicity suppression](../../../../../helicity-suppression.md) and electron–muon universality in the chiral [weak charged current](../../../../../charged-current.md). For example, scalar or pseudoscalar four-fermion interactions could remove the charged-lepton mass factor and substantially enhance the electron mode. Radiative corrections are required for a precision experimental comparison.

With two quark generations, the charged hadronic current contains

$$
\bar u\gamma_\alpha(1-\gamma_5)(\cos\theta_C\,d+\sin\theta_C\,s).
$$

A $K^-$ contains $s\bar u$, so its annihilation into the lepton pair selects the term proportional to $\sin\theta_C$. Strong strangeness conservation excludes the $d$ term from its vacuum matrix element. Its amplitude is thus multiplied by $\sin\theta_C$ and its width by $\sin^2\theta_C$:

$$
\boxed{\Gamma_{K^-\to\ell^-\bar\nu_\ell}=\frac{G_F^2F_K^2}{4\pi}\sin^2\theta_C\,M_Km_\ell^2\left(1-\frac{m_\ell^2}{M_K^2}\right)^2.}
$$

Here $F_K$ is the pure strong-interaction decay constant in the same square-root-of-two convention. If the pion current's quark mixing coefficient is also shown explicitly, its width carries $\cos^2\theta_C$; it is already absorbed if the stated pion matrix element uses the full weak current. Thus the isolated weak-factor ratio is $\tan^2\theta_C$, while the kaon suppression relative to unit weak coupling is the requested [Cabibbo suppression](../../../../../cabibbo-suppression.md) factor $\sin^2\theta_C$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
