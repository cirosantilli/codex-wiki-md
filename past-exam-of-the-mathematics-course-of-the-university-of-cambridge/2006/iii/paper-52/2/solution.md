<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A useful model of [spontaneous breaking of a Z2 scalar symmetry](../../../../../spontaneous-breaking-of-a-z2-scalar-symmetry.md) is the four-dimensional real scalar theory

$$
\mathcal L=\frac12(\partial\phi)^2-\frac\lambda4(\phi^2-v^2)^2,\qquad\lambda>0,quad v>0.
$$

The action is invariant under the [Z2 symmetry](../../../../../z2-symmetry.md) $\phi\mapsto-\phi$. Its classical [vacuum manifold](../../../../../vacuum-manifold.md) consists of the two values $\phi=\pm v$. In the broken quantum phase, choose a pure vacuum with $\langle\phi\rangle=v$; the symmetry maps it to a different vacuum with opposite expectation value, although it leaves the action unchanged. To distinguish quantum symmetry breaking from simply minimizing a classical potential, introduce a small source $J\phi$ and take the infinite-volume limit before $J\to0^+$. A finite-volume symmetry-preserving ground state can remain an even superposition because of tunneling, whereas the selected infinite-volume pure vacua have nonzero [vacuum expectation values](../../../../../vacuum-expectation-value.md). The parameter $v$ below is the tree-level expectation, with its quantum value determined by renormalized parameters.

Writing $\phi=v+h$ gives

$$
V=\lambda v^2h^2+\lambda vh^3+\frac\lambda4h^4,\qquad
\boxed{m_h^2=2\lambda v^2.}
$$

The original sign symmetry relates expansions about the two vacua; in one expansion it acts as $h\mapsto-2v-h$. It is not a symmetry that fixes the chosen vacuum. Since the broken group is discrete, there is no continuous broken generator and no required [Goldstone boson](../../../../../goldstone-boson.md).

With relativistically normalized external states, the general two-body partial [decay width](../../../../../decay-width.md) is

$$
\boxed{\Gamma_{1\to2}=\frac1{2m}\frac1{\mathcal S}\int d\Phi_2\,\overline{|\mathcal M|^2},\qquad
d\Phi_2=(2\pi)^4\delta^{(4)}(P-p_1-p_2)\prod_{i=1}^2\frac{d^3p_i}{(2\pi)^3,2E_i}.}
$$

Here the bar sums final spins and averages initial spins only if the initial ensemble is unpolarized. The [identical final-state symmetry factor](../../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md) is $\mathcal S=2!$ for two identical daughters and one for distinguishable daughters. Integrating the three-momentum delta function in the parent rest frame leaves $\mathbf p_2=-\mathbf p_1$. The energy delta function fixes $k=|\mathbf p_1|$ and has radial Jacobian $k(1/E_1+1/E_2)$. Hence the [two-body decay phase space](../../../../../two-body-decay-phase-space.md) is

$$
d\Phi_2=\frac{k}{16\pi^2m}d\Omega,\qquad
k=\frac{\sqrt{[m^2-(m_1+m_2)^2][m^2-(m_1-m_2)^2]}}{2m}.
$$

Consequently

$$
\frac{d\Gamma}{d\Omega}=\frac{k}{32\pi^2m^2\mathcal S}\overline{|\mathcal M|^2},\qquad
\Gamma=\frac{k}{8\pi m^2\mathcal S}\overline{|\mathcal M|^2}
$$

when the spin-summed amplitude is angle independent.

For [Higgs decay to two W bosons](../../../../../higgs-decay-to-two-w-bosons.md), the scalar parent has no spin average and the amplitude, up to an irrelevant phase, is $\mathcal M=gM_W\varepsilon_1^*\cdot\varepsilon_2^*$. Use the [massive vector polarization sum](../../../../../polarization-sum-for-a-massive-vector-boson.md) with $p_i^2=M_W^2$:

$$
\begin{aligned}
\sum_{\lambda_1,\lambda_2}|\mathcal M|^2
&=g^2M_W^2\left(-g_{\mu\nu}+\frac{p_{1\mu}p_{1\nu}}{M_W^2}\right)
\left(-g^{\mu\nu}+\frac{p_2^\mu p_2^\nu}{M_W^2}\right)\\
&=g^2M_W^2\left[4-1-1+\frac{(p_1\cdot p_2)^2}{M_W^4}\right].
\end{aligned}
$$

Momentum conservation gives $p_1\cdot p_2=(M_H^2-2M_W^2)/2$. With the PDF's ratio $x=M_W/M_H$, this becomes

$$
\sum|\mathcal M|^2=\frac{g^2M_H^4}{4M_W^2}(1-4x^2+12x^4),\qquad
k=\frac{M_H}{2}\sqrt{1-4x^2}.
$$

The charged daughters are distinguishable. Combining the last two equations with $g^2/M_W^2=4\sqrt2G_F$ gives

$$
\boxed{\Gamma(H\to W^+W^-)=\frac{G_FM_H^3}{8\pi\sqrt2}\sqrt{1-4x^2}\,(1-4x^2+12x^4).}
$$

For [Higgs decay to two Z bosons](../../../../../higgs-decay-to-two-z-bosons.md), the [Higgs boson coupling to Z bosons](../../../../../higgs-boson-coupling-to-z-bosons.md) is $2iM_Z^2g_{\mu\nu}/v=igM_Z^2g_{\mu\nu}/M_W$, using $v=2M_W/g$. This compensates the changed powers of $M_Z$ in the polarization contraction, giving the same normalization of the squared amplitude with $x$ replaced by $y=M_Z/M_H$. The two [Z bosons](../../../../../z-boson.md) are identical, so the phase-space symmetry factor supplies an additional half:

$$
\boxed{\Gamma(H\to ZZ)=\frac{G_FM_H^3}{16\pi\sqrt2}\sqrt{1-4y^2}\,(1-4y^2+12y^4).}
$$

Both expressions have mass dimension one, vanish at their two-body thresholds and approach the ratio $2:1$ for $M_H\gg M_Z$. The cubic large-mass behavior comes from longitudinal-vector polarizations. These are on-shell tree-level widths under the stated heavy-Higgs hypothesis; below threshold the physical off-shell multi-particle decays require a different calculation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
