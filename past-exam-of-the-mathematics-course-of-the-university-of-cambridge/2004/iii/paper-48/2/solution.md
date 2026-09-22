<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The derivative convention uses [hypercharge](../../../../../hypercharge.md) Y with $Q=T_3+Y$. For each [lepton](../../../../../lepton.md) family $l=e,\mu,\tau$, the left-handed fields form an [SU(2)](../../../../../su-2-group.md) doublet $L_l=(\nu_l,l)_L^T$, with $Y=-1/2$. Their [weak isospin](../../../../../weak-isospin.md) values are $T_3=+1/2,-1/2$ and their electric charges are $0,-1$. The right-handed charged [lepton](../../../../../lepton.md) $l_R$ is an [SU(2)](../../../../../su-2-group.md) singlet, with $T_3=0$, $Y=-1$ and charge $-1$. The minimal model used here has no right-handed [neutrino](../../../../../neutrino.md). A sterile right-handed [neutrino](../../../../../neutrino.md), if added as a singlet with $Y=0$, would have no [charged weak current](../../../../../charged-current.md) interaction. Antiparticles carry the conjugate representations and opposite electric charges.

Expanding $\bar L_l i\gamma^\mu D_\mu L_l$ supplies $-g\bar L_l\gamma^\mu A_\mu^a\sigma_aL_l/2$. The off-diagonal entries of $A^a\sigma_a$ are $\sqrt2W^+$ and $\sqrt2W^-$. With the [chiral projector](../../../../../chiral-projector.md) $P_L=(1-\gamma^5)/2$, one has $\bar\nu_L\gamma^\mu l_L=\bar\nu\gamma^\mu P_L l$. Thus the two [W boson](../../../../../w-boson.md) interactions are

$$
\boxed{\mathcal L_{W^+,l}=-\frac{g}{2\sqrt2}W_\mu^+\bar\nu_l\gamma^\mu(1-\gamma^5)l,\qquad\mathcal L_{W^-,l}=-\frac{g}{2\sqrt2}W_\mu^-\bar l\gamma^\mu(1-\gamma^5)\nu_l.}
$$

For [quarks](../../../../../quark.md), separate rotations diagonalize the up-type and down-type mass terms. If their left-handed rotations are $U_{uL}$ and $U_{dL}$, the charged interaction contains the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) $V=U_{uL}^\dagger U_{dL}$:

$$
J_{\rm had}^\mu=\sum_{i,j}\bar u_i\gamma^\mu(1-\gamma^5)V_{ij}d_j.
$$

There is an implicit sum over [color charge](../../../../../color-charge.md). This [quark mixing](../../../../../quark-mixing.md) permits transitions between different families, rather than just the paired fields in a single doublet.

Let $J^\mu=\sum_l\bar\nu_l\gamma^\mu(1-\gamma^5)l+J_{\rm had}^\mu$ and $\kappa=g/(2\sqrt2)$. At momenta much smaller than $m_W$, neglect derivatives in the heavy [W boson](../../../../../w-boson.md) equation. Its mass and source terms can be completed to a square:

$$
m_W^2W_\mu^+W^{-\mu}-\kappa(W_\mu^+J^\mu+W_\mu^-J^{\dagger\mu})=m_W^2\left(W_\mu^+-\frac\kappa{m_W^2}J_\mu^\dagger\right)\left(W^{-\mu}-\frac\kappa{m_W^2}J^\mu\right)-\frac{\kappa^2}{m_W^2}J_\mu^\dagger J^\mu.
$$

This explicitly performs [integrating out a charged vector boson](../../../../../integrating-out-a-charged-vector-boson.md). The resulting [Fermi interaction](../../../../../fermi-interaction.md) is

$$
\boxed{\mathcal L_{\rm eff}=-\frac{G_F}{\sqrt2}J_\mu^\dagger J^\mu,\qquad\frac{G_F}{\sqrt2}=\frac{g^2}{8m_W^2}.}
$$

The omitted terms contain derivatives and are relatively suppressed by momentum squared divided by $m_W^2$.

For the [leptonic pion decay](../../../../../leptonic-pion-decay.md), [Lorentz covariance](../../../../../lorentz-covariance.md) restricts a vacuum-to-spin-zero current matrix element to a constant times $p^\alpha$. In the rest frame, rotations eliminate the spatial components. Under [parity](../../../../../parity.md), the temporal vector current is even, whereas the vacuum is even and the [pion](../../../../../pion.md) is odd, so its temporal matrix element equals its negative and vanishes. The temporal axial current is odd and is allowed. This proves the [vacuum-to-pseudoscalar current selection rule](../../../../../vacuum-to-pseudoscalar-current-selection-rule.md), rather than merely assuming an axial current. Define the [pion decay constant](../../../../../pion-decay-constant.md) by

$$
\langle0|\bar u\gamma^\alpha\gamma^5d|\pi^-(p)\rangle=if_\pi p^\alpha.
$$

Then the vector-minus-axial [charged weak current](../../../../../charged-current.md) has matrix element $-if_\pi V_{ud}p^\alpha$, up to an irrelevant overall phase convention. Consequently the [scattering amplitude](../../../../../scattering-amplitude.md) for the decay can be written

$$
\mathcal M=\frac{iG_Ff_\pi V_{ud}}{\sqrt2}\,p_\alpha\bar u_e(k)\gamma^\alpha(1-\gamma^5)v_\nu(q).
$$

Use $p=k+q$, the momentum-space [Dirac equation](../../../../../dirac-equation.md) $\bar u_e\not k=m_e\bar u_e$, and $\not qv_\nu=0$ for a massless [neutrino](../../../../../neutrino.md). Since $\not q(1-\gamma^5)=(1+\gamma^5)\not q$, the neutrino contribution vanishes, leaving

$$
\mathcal M=\frac{iG_Ff_\pi V_{ud}m_e}{\sqrt2}\bar u_e(1-\gamma^5)v_\nu.
$$

The [fermion spin sum](../../../../../fermion-spin-sum.md) is, using the supplied [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md),

$$
\sum_{\rm spins}|\bar u_e(1-\gamma^5)v_\nu|^2=\operatorname{tr}\bigl[(\not k+m_e)(1-\gamma^5)\not q(1+\gamma^5)\bigr]=8k\cdot q=4(m_\pi^2-m_e^2).
$$

Here $(k+q)^2=m_\pi^2$, $k^2=m_e^2$, and $q^2=0$. The mass term in the trace vanishes; anticommuting $\gamma^5$ reduces the remaining trace to twice $\operatorname{tr}(\not k\not q)$. It follows that

$$
\boxed{\sum_{\rm spins}|\mathcal M|^2=2G_F^2f_\pi^2|V_{ud}|^2m_e^2(m_\pi^2-m_e^2).}
$$

Using [two-body decay phase space](../../../../../two-body-decay-phase-space.md), with final momentum magnitude $(m_\pi^2-m_e^2)/(2m_\pi)$, gives the [leptonic pseudoscalar decay width](../../../../../leptonic-pseudoscalar-decay-width.md)

$$
\Gamma(\pi^-\to e^-\bar\nu_e)=\frac{G_F^2f_\pi^2|V_{ud}|^2m_\pi m_e^2}{8\pi}\left(1-\frac{m_e^2}{m_\pi^2}\right)^2.
$$

Thus the requested $m_e^2(m_\pi^2-m_e^2)$ factor is already present in the squared amplitude, and the phase space supplies one more threshold factor.

The physical explanation is [helicity suppression](../../../../../helicity-suppression.md). In the [pion](../../../../../pion.md) rest frame the two momenta are opposite. The massless antineutrino has positive [helicity](../../../../../helicity.md); zero total angular momentum would require the electron to have positive [helicity](../../../../../helicity.md) too. The [charged weak current](../../../../../charged-current.md) instead creates a left-chiral electron, whose [helicity](../../../../../helicity.md) is negative when its mass vanishes. A nonzero electron mass admits the required opposite [helicity](../../../../../helicity.md) with an amplitude proportional to $m_e$. **The decay amplitude vanishes for $m_e=0$, and the rate is suppressed by $m_e^2$.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
