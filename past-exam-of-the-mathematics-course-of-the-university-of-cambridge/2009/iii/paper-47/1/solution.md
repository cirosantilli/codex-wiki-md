<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Minkowski metric](../../../../../minkowski-metric.md) signature $+---$ and natural units. With no lepton mixing, choose the [weak charged current](../../../../../charged-current.md) convention

$$
J^\alpha=\sum_{\ell=e,\mu,\tau}\overline\nu_\ell\gamma^\alpha(1-\gamma_5)\ell.
$$

Its conjugate convention exchanges $J$ and $J^\dagger$ without changing the interaction. The relevant [four-fermion interaction](../../../../../four-fermion-interaction.md) gives the [muon decay](../../../../../muon-decay.md) amplitude, up to an overall phase,

$$
\boxed{\mathcal M=\frac{G_F}{\sqrt2}
[\overline u(k)\gamma^\alpha(1-\gamma_5)v(q)]
[\overline u(q')\gamma_\alpha(1-\gamma_5)u(p)].}
$$

Here $G_F$ is the [Fermi constant](../../../../../fermi-constant.md); the factors $1-\gamma_5$ are twice the left [chiral projector](../../../../../chiral-projector.md), so there is no additional factor of two to insert.

For the final-spin sum let $\rho_\mu=(\not p+m)(1+\gamma_5\not s)/2$, where $m=m_\mu$. It already describes the specified initial polarization; there is no further initial-spin average. The two [gamma matrix](../../../../../gamma-matrices.md) traces are

$$
\sum_{\mathrm{final\ spins}}|\mathcal M|^2
=\frac{G_F^2}{2}L^{\alpha\beta}H_{\alpha\beta},
\qquad
L^{\alpha\beta}=\operatorname{tr}[(\not k+m_e)\gamma^\alpha(1-\gamma_5)\not q\gamma^\beta(1-\gamma_5)],
$$



$$
H_{\alpha\beta}=\operatorname{tr}[\not q'\gamma_\alpha(1-\gamma_5)\rho_\mu\gamma_\beta(1-\gamma_5)].
$$

The electron-mass term vanishes in its chiral trace. In the muon trace, anticommutation with $\gamma_5$ gives

$$
(1-\gamma_5)\rho_\mu\gamma_\beta(1-\gamma_5)
=(\not p-m\not s)\gamma_\beta(1-\gamma_5).
$$

For the [chiral fermion trace contraction](../../../../../chiral-fermion-trace-contraction.md), define

$$
K^{\alpha\beta}(a,b)=a^\alpha b^\beta+a^\beta b^\alpha-g^{\alpha\beta}a\cdot b
+i\epsilon^{\alpha\beta\rho\sigma}a_\rho b_\sigma.
$$

The supplied trace conventions imply $L^{\alpha\beta}=8K^{\alpha\beta}(k,q)$ and $H_{\alpha\beta}=4K_{\alpha\beta}(q',r)$, where $r=p-ms$. The factor four in the second trace follows from the polarization projector. The symmetric parts contract to $2[(a\cdot c)(b\cdot d)+(a\cdot d)(b\cdot c)]$. The [Levi-Civita symbol](../../../../../levi-civita-symbol.md) contraction, including $i^2=-1$, contributes $2[(a\cdot c)(b\cdot d)-(a\cdot d)(b\cdot c)]$. Mixed symmetric-antisymmetric contractions vanish. Thus $K^{\alpha\beta}(a,b)K_{\alpha\beta}(c,d)=4(a\cdot c)(b\cdot d)$, and

$$
\boxed{\sum|\mathcal M|^2=64G_F^2(k\cdot q')\,q\cdot(p-ms),
\qquad A=64,\quad B=-64.}
$$

Now neglect $m_e$ as well. Put $Q=p-k$ and $c=\widehat{\mathbf k}\cdot\mathbf s$. The given moment integral over two-neutrino [relativistic two-body phase space](../../../../../relativistic-two-body-phase-space.md) yields

$$
\int\frac{d^3q\,d^3q'}{|\mathbf q|\,|\mathbf q'|}
\delta^4(Q-q-q')\,(k\cdot q')(r\cdot q)
=\frac\pi3(k\cdot Q)(r\cdot Q)+\frac\pi6(k\cdot r)Q^2.
$$

In the [muon](../../../../../muon.md) rest frame, $k\cdot Q=mE$, $k\cdot r=mE(1+c)$, $r\cdot Q=m^2-mE(1+c)$ and $Q^2=m^2-2mE$. Substitution gives

$$
\frac{\pi m^3E}{6}\left[(3-2x)+(1-2x)c\right],\qquad x=2E/m.
$$

Combining this with the [Lorentz-invariant phase-space measure](../../../../../lorentz-invariant-phase-space-measure.md), whose one-particle denominator is $(2\pi)^3\,2E$, and $d^3k=E^2\,dE\,d\Omega$, gives the [polarized muon decay](../../../../../polarized-muon-decay.md) distribution

$$
\boxed{\frac{d\Gamma}{dx\,d\Omega}
=\frac{G_F^2m^5}{384\pi^4}x^2
\left[(3-2x)+(1-2x)\widehat{\mathbf k}\cdot\mathbf s\right],
\quad 0\leq x\leq1.}
$$

Consequently $C=-2$, $D=-2$, $E=1$. Integration over the electron direction removes the polarization term, and $\int_0^1x^2(3-2x)\,dx=1/2$, recovering $\Gamma=G_F^2m^5/(192\pi^3)$.

The [spin](../../../../../spin.md) vector is axial and the momentum direction is polar: under [parity](../../../../../parity.md), $\mathbf s$ stays unchanged while $\widehat{\mathbf k}$ reverses. Their scalar product therefore changes sign. Its nonzero coefficient demonstrates **[parity](../../../../../parity.md) violation in [polarized muon decay](../../../../../polarized-muon-decay.md)**, arising from the left-chiral [weak charged current](../../../../../charged-current.md). At the upper endpoint the negative muon's electron is preferentially emitted opposite the spin, providing a sign check on the result.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
