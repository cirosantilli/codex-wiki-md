<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the source convention $Q=T_3+Y$, with electric charge measured in units of the positron charge. Expanding the [covariant derivative](../../../../../covariant-derivative.md) in the [fermion](../../../../../fermion.md) [kinetic term](../../../../../kinetic-term.md) gives interaction $-\bar f\gamma_\mu(gT_3A_3^\mu+g'YB^\mu)f$. Substituting the given neutral-field rotation, the coefficient of $Z^\mu$ is

$$
gc_WT_3-g's_WY=\frac g{c_W}(T_3-s_W^2Q),\qquad s_W=\sin\theta_W,\quad c_W=\cos\theta_W.
$$

The photon coefficient is $gs_W(T_3+Y)=eQ$, with $e=gs_W=g'c_W$. For a [Dirac field](../../../../../dirac-field.md), $T_3$ acts only on its left-handed component. Thus

$$
T_3P_L-Qs_W^2=\frac12\bigl[(T_3-2Qs_W^2)-T_3\gamma^5\bigr].
$$

The [weak neutral current](../../../../../neutral-current.md) interaction consequently has the requested form, with

$$
\boxed{c_v=T_3-2Qs_W^2,\qquad c_a=T_3.}
$$

The [electroweak representation and hypercharge table](../../../../../electroweak-representation-and-hypercharge-table.md) gives the following values for one generation:

| Type | $T_3$ on left | $Q$ | $Y_L$ | $Y_R$ | $c_v$ | $c_a$ |
| --- | --- | --- | --- | --- | --- | --- |
| [Neutrino](../../../../../neutrino.md) | $1/2$ | $0$ | $-1/2$ | absent | $1/2$ | $1/2$ |
| Charged [lepton](../../../../../lepton.md) | $-1/2$ | $-1$ | $-1/2$ | $-1$ | $-1/2+2s_W^2$ | $-1/2$ |
| Up-type [quark](../../../../../quark.md) | $1/2$ | $2/3$ | $1/6$ | $2/3$ | $1/2-4s_W^2/3$ | $1/2$ |
| Down-type [quark](../../../../../quark.md) | $-1/2$ | $-1/3$ | $1/6$ | $-1/3$ | $-1/2+2s_W^2/3$ | $-1/2$ |

These [neutral-current vector and axial couplings](../../../../../neutral-current-vector-and-axial-couplings.md) use the source's vertex prefactor $g/(2c_W)$. They are twice the coefficients used with prefactor $g/c_W$; the latter convention must not be mixed into this calculation. For the neutrino, the [chiral projector](../../../../../chiral-projector.md) removes the inactive right-handed component automatically.

Set $G=g/(2c_W)$ and suppress the species label. For outgoing momenta $k_1,k_2$, the amplitude is, up to an irrelevant phase,

$$
\mathcal M=G\epsilon_\mu(p)\bar u(k_1)\gamma^\mu(c_v-c_a\gamma^5)v(k_2),\qquad p=k_1+k_2.
$$

The final-state [spin sum](../../../../../spin-sum.md) is the [Dirac trace](../../../../../gamma-matrix-trace.md) of $\not k_1\gamma^\mu(c_v-c_a\gamma^5)\not k_2\gamma^\nu(c_v-c_a\gamma^5)$. Anticommutation of $\gamma^5$ with the [gamma matrices](../../../../../gamma-matrices.md) makes its symmetric part

$$
T_{\mathrm{sym}}^{\mu\nu}=4(c_v^2+c_a^2)(k_1^\mu k_2^\nu+k_1^\nu k_2^\mu-g^{\mu\nu}k_1\cdot k_2).
$$

The vector-axial cross term is proportional to the antisymmetric [Levi-Civita symbol](../../../../../levi-civita-symbol.md), so it contracts to zero with the symmetric [massive vector polarization sum](../../../../../polarization-sum-for-a-massive-vector-boson.md) $-g_{\mu\nu}+p_\mu p_\nu/M_Z^2$. Since $k_1^2=k_2^2=0$, the symmetric tensor is transverse to $p$ as well. Only $-g_{\mu\nu}$ remains, and

$$
-g_{\mu\nu}T_{\mathrm{sym}}^{\mu\nu}=8(c_v^2+c_a^2)k_1\cdot k_2=4M_Z^2(c_v^2+c_a^2).
$$

Multiplying by $G^2$ proves the [massless fermion Z decay spin sum](../../../../../massless-fermion-z-decay-spin-sum.md):

$$
\boxed{\sum_{\lambda,s_1,s_2}|\mathcal M|^2=\frac{g^2M_Z^2}{c_W^2}(c_v^2+c_a^2).}
$$

For the [decay width](../../../../../decay-width.md), average over the three initial polarizations. Rotational invariance makes the integrated width the same for each initial spin state, so the [massive-vector spin average](../../../../../massive-vector-spin-average.md) is legitimate even for a single prepared polarization. In the rest frame, the delta functions in [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) leave

$$
d\Phi_2=\frac{d\Omega}{32\pi^2},\qquad\int d\Phi_2=\frac1{8\pi}.
$$

This follows by setting $\mathbf k_2=-\mathbf k_1$ and integrating $\delta(M_Z-2|\mathbf k_1|)$; the radial integration supplies a factor $1/2$. Hence

$$
\Gamma_f=\frac1{2M_Z}\frac13\sum|\mathcal M|^2\frac1{8\pi}=\boxed{\frac{g^2M_Z}{48\pi c_W^2}(c_v^2+c_a^2)}.
$$

For a [quark](../../../../../quark.md) species multiply by three colors, with strong-interaction radiative corrections when comparing with data. For one effectively massless active [neutrino](../../../../../neutrino.md), $c_v=c_a=1/2$, so $\Gamma_\nu=g^2M_Z/(96\pi c_W^2)=G_FM_Z^3/(12\sqrt2\pi)$.

The total resonance width contains visible charged-lepton and hadron decays plus $N_\nu\Gamma_\nu$. Thus the measured invisible contribution determines

$$
\boxed{N_\nu=\frac{\Gamma_Z-\Gamma_{\mathrm{visible}}}{\Gamma_\nu}.}
$$

Early resonance measurements supported three light active [neutrino](../../../../../neutrino.md) species, with experimental uncertainties; the [OPAL analysis of its 1989 data](https://inspirehep.net/files/afa87f449c4b3cb87894b53955b564da) explicitly compares the three- and four-species predictions. Under the question's assumption that every possible family has a massless [neutrino](../../../../../neutrino.md) with ordinary weak couplings, this constrains the number of such families. The inference does not exclude additional neutrinos heavier than $M_Z/2$ or [gauge singlet](../../../../../gauge-singlet.md) sterile states with no ordinary $Z$ coupling. This is [light-neutrino counting from the Z width](../../../../../light-neutrino-counting-from-the-z-width.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
