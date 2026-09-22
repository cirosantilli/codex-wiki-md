<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At momentum transfers small compared with $M_W$, the two [weak charged current](../../../../../charged-current.md) vertices each carry $g/(2\sqrt2)$ when written with $(1-\gamma_5)$, and the [W boson propagator](../../../../../w-boson-propagator.md) reduces to a local factor proportional to $1/M_W^2$. Matching their product to the [Fermi interaction](../../../../../fermi-interaction.md) gives, at tree level,

$$
\boxed{\frac{G_F}{\sqrt2}=\frac{g^2}{8M_W^2},\qquad G_F=\frac1{\sqrt2v^2}\quad(M_W=gv/2).}
$$

The [Fermi constant](../../../../../fermi-constant.md) is thus determined by the electroweak coupling and symmetry-breaking scale; the four-fermion description is a low-energy effective interaction.

Only the cross term $J_L^\dagger J_H$ can annihilate the pion and create the stated charged-lepton/antineutrino pair. Its leptonic [matrix element](../../../../../matrix-element.md) is $\bar u_e(k)\gamma^\mu(1-\gamma_5)v_\nu(q)$. [Lorentz covariance](../../../../../lorentz-covariance.md) permits a vacuum-to-[spin](../../../../../spin.md)-zero current [matrix element](../../../../../matrix-element.md) only proportional to $p^\mu$. At rest this has only a temporal component. The vacuum is parity-even and the pion is parity-odd, while $V_H^0$ is parity-even, so $\langle0|V_H^0|\pi\rangle$ equals its own negative and vanishes. [Lorentz covariance](../../../../../lorentz-covariance.md) then makes the full vector [matrix element](../../../../../matrix-element.md) vanish. The temporal [axial current](../../../../../axial-current.md) is parity-odd and is allowed: this is the [vacuum-to-pseudoscalar current selection rule](../../../../../vacuum-to-pseudoscalar-current-selection-rule.md).

The minus sign in $J_H=V_H-A_H$ cancels the interaction's minus sign, up to an irrelevant common S-matrix phase. Therefore

$$
\mathcal M=\frac{G_F}{\sqrt2}\bar u_e\gamma^\mu(1-\gamma_5)v_\nu\langle0|A_{H\mu}|\pi^-\rangle
=iG_FF_\pi\cos\theta_C\,p_\mu\bar u_e\gamma^\mu(1-\gamma_5)v_\nu.
$$

The [pion decay constant](../../../../../pion-decay-constant.md) convention here includes the given $\sqrt2$ in its current [matrix element](../../../../../matrix-element.md). Momentum conservation and the external [Dirac equations](../../../../../dirac-equation.md) give $p=k+q$, $\bar u_e\not k=m_e\bar u_e$, $\not qv_\nu=0$. Since $\not q(1-\gamma_5)=(1+\gamma_5)\not q$, the neutrino term vanishes and

$$
\boxed{\mathcal M=iG_FF_\pi\cos\theta_C\,m_e\bar u_e(1-\gamma_5)v_\nu.}
$$

This is [helicity suppression](../../../../../helicity-suppression.md): the amplitude vanishes in the zero charged-lepton-mass limit despite the larger available phase space.

For the [spin sum](../../../../../spin-sum.md), the Dirac adjoint of $1-\gamma_5$ is $1+\gamma_5$, and the completeness relations give

$$
\begin{aligned}
\sum_s|\mathcal M|^2
&=G_F^2F_\pi^2\cos^2\theta_C\,m_e^2
\operatorname{tr}[(\not k+m_e)(1-\gamma_5)\not q(1+\gamma_5)]\\
&=2G_F^2F_\pi^2\cos^2\theta_C\,m_e^2
\operatorname{tr}[(\not k+m_e)\not q(1+\gamma_5)]\\
&=8G_F^2F_\pi^2\cos^2\theta_C\,m_e^2\,k\cdot q
=4G_F^2F_\pi^2\cos^2\theta_C\,m_e^2(m_\pi^2-m_e^2).
\end{aligned}
$$

The chiral projectors automatically eliminate the unused neutrino helicity when the full massless completeness relation is inserted. There is no initial [spin](../../../../../spin.md) average for a [spin](../../../../../spin.md)-zero pion.

In the pion rest frame, let $r=|\boldsymbol k|=|\boldsymbol q|$, $E=\sqrt{r^2+m_e^2}$. After integrating the spatial delta function and angles, the [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) becomes

$$
\Phi_2=\frac1{4\pi}\int_0^\infty\frac{r^2}{Er}\,\delta(m_\pi-E-r)dr.
$$

The root is $r_*=(m_\pi^2-m_e^2)/(2m_\pi)$ and $E_*=(m_\pi^2+m_e^2)/(2m_\pi)$. The absolute derivative of the delta-function argument is $r_*/E_*+1=m_\pi/E_*$. Thus $\Phi_2=r_*/(4\pi m_\pi)$. Multiplying by the [spin sum](../../../../../spin-sum.md) and the initial factor $1/(2m_\pi)$ yields the [leptonic pseudoscalar decay width](../../../../../leptonic-pseudoscalar-decay-width.md)

$$
\boxed{\Gamma(\pi^-\to e^-\bar\nu_e)=\frac{G_F^2F_\pi^2\cos^2\theta_C}{4\pi}\,m_\pi m_e^2\left(1-\frac{m_e^2}{m_\pi^2}\right)^2.}
$$

If the decay constant were instead defined by a [matrix element](../../../../../matrix-element.md) $if_\pi p^\mu$ without $\sqrt2$, then $f_\pi=\sqrt2F_\pi$ and the width coefficient would be $f_\pi^2/(8\pi)$; mixing these conventions would introduce a factor-of-two error.

The same derivation for a muon cancels the common hadronic and weak factors in the [pion electron-to-muon decay ratio](../../../../../pion-electron-to-muon-decay-ratio.md):

$$
\boxed{R_{e/\mu}^{(0)}=\frac{m_e^2}{m_\mu^2}\left(\frac{1-m_e^2/m_\pi^2}{1-m_\mu^2/m_\pi^2}\right)^2\approx1.28\times10^{-4}.}
$$

The numerical value uses approximate masses $0.511,105.66,139.57$ MeV. Agreement with the corresponding [Standard Model](../../../../../standard-model-split.md) prediction tests [lepton universality](../../../../../lepton-universality.md) and the chiral, helicity-suppressing structure of the [weak charged current](../../../../../charged-current.md), rather than the poorly calculable hadronic decay constant. A difference in the electron and muon weak couplings would multiply the ratio by their squared coupling ratio. Precision agreement must be assessed after [radiative corrections](../../../../../radiative-correction.md), with matching [photon](../../../../../photon.md)-inclusive experimental definitions; the displayed tree-level ratio is not itself the radiatively corrected precision prediction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
