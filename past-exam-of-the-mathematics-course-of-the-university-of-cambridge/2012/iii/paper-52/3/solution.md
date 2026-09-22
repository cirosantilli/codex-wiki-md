<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $s_W=\sin\theta_W$ and $c_W=\cos\theta_W$. The left-handed doublet has

$$
T_L^3=\begin{pmatrix}\frac12&0\\0&-\frac12\end{pmatrix},\qquad
Q_L=\begin{pmatrix}0&0\\0&-1\end{pmatrix},
$$

while the right-handed charged-[lepton](../../../../../lepton.md) singlet has $T_R^3=0$ and $Q_R=-1$. There is no weakly coupled right-handed [neutrino](../../../../../neutrino.md) in the stated field content. For a [fermion](../../../../../fermion.md) $f$, write $g_L^f=T_{3L}^f-Q_fs_W^2$ and $g_R^f=T_{3R}^f-Q_fs_W^2$, with $g_R^\nu=0$ here. Since $\bar f_L\gamma^\mu f_L=\bar f\gamma^\mu P_Lf$ and similarly for $R$,

$$
\bar f\gamma^\mu(g_L^fP_L+g_R^fP_R)f
=\bar f\gamma^\mu(c_V^f-c_A^f\gamma^5)f,
\quad c_V^f=\frac{g_L^f+g_R^f}{2},\quad c_A^f=\frac{g_L^f-g_R^f}{2}.
$$

Consequently the [neutral-current vector and axial couplings](../../../../../neutral-current-vector-and-axial-couplings.md) in the specified overall normalization are

$$
\boxed{c_V^\ell=-\frac14+s_W^2,\qquad c_A^\ell=-\frac14,\qquad
c_V^\nu=c_A^\nu=\frac14.}
$$

These coefficients accompany $g/c_W$. A convention with $g/(2c_W)$ uses twice these vector and axial coefficients; mixing the two conventions would make the widths wrong by a factor of four. For the [neutrino](../../../../../neutrino.md), $c_V-c_A\gamma^5=\frac12P_L$, so the chiral projection is already built into the vertex.

For either massless final pair with momenta $k_1,k_2$, $p=k_1+k_2$, the invariant amplitude is, up to an irrelevant overall phase,

$$
\mathcal M_f=\frac g{c_W}\epsilon_\mu(p)\bar u_f(k_1)\gamma^\mu(c_V^f-c_A^f\gamma^5)v_f(k_2).
$$

The [spin](../../../../../spin.md)-summed [fermion](../../../../../fermion.md) tensor is

$$
T_f^{\mu\nu}=\operatorname{tr}\!\left[\not k_1\gamma^\mu(c_V^f-c_A^f\gamma^5)
\not k_2\gamma^\nu(c_V^f-c_A^f\gamma^5)\right].
$$

The symmetric part, using the four-gamma [trace](../../../../../matrix-trace.md), is

$$
(T_f^{\mu\nu})_{\rm sym}=4[(c_V^f)^2+(c_A^f)^2]
\left(k_1^\mu k_2^\nu+k_1^\nu k_2^\mu-\eta^{\mu\nu}k_1\cdot k_2\right).
$$

The vector-axial interference is antisymmetric in $\mu,\nu$, so it drops out of the symmetric $Z$ polarization sum. Also $p_\mu T_f^{\mu\nu}=0$ for massless external [fermions](../../../../../fermion.md), by their [Dirac equations](../../../../../dirac-equation.md); hence the $p_\mu p_\nu/m_Z^2$ part contributes zero. Using $k_1\cdot k_2=m_Z^2/2$ gives

$$
\boxed{\overline{|\mathcal M_f|^2}
=\frac{g^2}{3c_W^2}(-\eta_{\mu\nu})T_f^{\mu\nu}
=\frac{4g^2m_Z^2}{3c_W^2}[(c_V^f)^2+(c_A^f)^2].}
$$

The [massive-vector spin average](../../../../../massive-vector-spin-average.md) supplies the factor $1/3$ for the three [spin](../../../../../spin.md) states of the massive $Z$. The massless [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) is $d\Phi_2=d\Omega/(32\pi^2)$, and so $\int d\Phi_2=1/(8\pi)$. The [spin](../../../../../spin.md)-averaged amplitude above is angle-independent in the rest frame, giving

$$
\boxed{\Gamma_f=\frac{g^2m_Z}{12\pi c_W^2}[(c_V^f)^2+(c_A^f)^2].}
$$

The [massless leptonic Z decay widths](../../../../../massless-leptonic-z-decay-width.md) for one charged-[lepton](../../../../../lepton.md) flavor and one active [neutrino](../../../../../neutrino.md) flavor respectively are

$$
\boxed{\Gamma(Z\to\ell\bar\ell)=\frac{g^2m_Z}{96\pi c_W^2}
(1-4s_W^2+8s_W^4),\qquad
\Gamma(Z\to\nu\bar\nu)=\frac{g^2m_Z}{96\pi c_W^2}.}
$$

There is no color factor for [leptons](../../../../../lepton.md) and no extra final-state identical-particle factor for a particle-antiparticle pair. The [neutrino](../../../../../neutrino.md) projectors already exclude sterile helicity states, so no additional factor of two is needed. These are tree-level massless widths; electroweak radiative corrections and charged-[lepton](../../../../../lepton.md) masses have not been included. If desired, using $G_F=g^2/(4\sqrt2m_W^2)$ and $m_W=c_Wm_Z$ converts the common prefactor to $G_Fm_Z^3/(12\sqrt2\pi)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
