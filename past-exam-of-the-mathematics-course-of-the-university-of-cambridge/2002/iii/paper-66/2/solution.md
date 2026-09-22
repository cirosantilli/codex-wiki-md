<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take [metric](../../../../../metric.md) $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and write $M=M_W$. The outgoing electron and [antineutrino](../../../../../antineutrino.md) momenta are $k$ and $k'$. Up to an irrelevant overall phase, the [amplitude](../../../../../wave-amplitude.md) is

$$
\mathcal M=\frac{g}{2\sqrt2}\epsilon_\mu\bar u(k)\gamma^\mu(1-\gamma_5)v(k').
$$

A [fermion spin sum](../../../../../fermion-spin-sum.md) gives

$$
\sum_{\rm final}|\mathcal M|^2=\frac{g^2}{8}\epsilon_\mu\epsilon_\nu^*T^{\mu\nu},\qquad T^{\mu\nu}=\operatorname{Tr}\bigl[\not k\gamma^\mu(1-\gamma_5)\not k'\gamma^\nu(1-\gamma_5)\bigr].
$$

Anticommuting $\gamma_5$ through the massless [momentum](../../../../../momentum.md) and [gamma matrix](../../../../../gamma-matrices.md), and using $(1-\gamma_5)^2=2(1-\gamma_5)$, reduces the [trace](../../../../../matrix-trace.md) to twice the four-gamma [trace](../../../../../matrix-trace.md) minus twice its $\gamma_5$ counterpart. In particular its symmetric part is

$$
T_S^{\mu\nu}=8\bigl(k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'\bigr).
$$

The epsilon-tensor part is antisymmetric and contributes neither to the unpolarized polarization sum nor to the real linear polarization used below. There is no extra factor for selecting the [neutrino](../../../../../neutrino.md) [helicity](../../../../../helicity.md): the chiral vertex has already done so.

The external massless equations imply $p_\mu J^\mu=0$ for $p=k+k'$, so $p_\mu T^{\mu\nu}=0$. With $k\cdot k'=M^2/2$, averaging over the three initial [spin](../../../../../spin.md) states gives

$$
\overline{|\mathcal M|^2}=\frac{g^2}{24}\left(-g_{\mu\nu}+\frac{p_\mu p_\nu}{M^2}\right)T^{\mu\nu}=\boxed{\frac{g^2M^2}{3}}.
$$

Indeed $-g_{\mu\nu}T_S^{\mu\nu}=16k\cdot k'=8M^2$. This is a [massive-vector spin average](../../../../../massive-vector-spin-average.md), not an average over the final [spins](../../../../../spin.md).

In the rest frame, eliminating the [momentum](../../../../../momentum.md) delta function and integrating the remaining radial delta function $\delta(M-2|\mathbf k|)$ reduces the [two-body Lorentz-invariant phase space](../../../../../two-body-lorentz-invariant-phase-space.md) to $d\Phi_2=d\Omega/(32\pi^2)$. Therefore

$$
\frac{d\Gamma}{d\Omega}=\frac{|\mathcal M|^2}{64\pi^2M},\qquad\boxed{\Gamma_{\rm unpol}=\frac{g^2M}{48\pi}}.
$$

This derives the [massless leptonic W decay width](../../../../../massless-leptonic-w-decay-width.md) without invoking a precomputed decay formula.

For the specified polarization there is no initial [spin average](../../../../../spin-average.md). Put $\mathbf k=(M/2)\widehat{\mathbf n}$, $\mathbf k'=-(M/2)\widehat{\mathbf n}$ and $\widehat n_z=\cos\theta$. The contraction selects

$$
T_S^{33}=8\left(-\frac{M^2}{2}\cos^2\theta+\frac{M^2}{2}\right)=4M^2\sin^2\theta.
$$

It follows that

$$
\boxed{\sum_{\rm final}|\mathcal M_z|^2=\frac{g^2M^2}{2}\sin^2\theta,\quad\frac{d\Gamma_z}{d\Omega}=\frac{g^2M}{128\pi^2}\sin^2\theta,\quad\Gamma_z=\frac{g^2M}{48\pi}.}
$$

Here $\int\sin^2\theta\,d\Omega=8\pi/3$. The total rate agrees with the spin-averaged result, but its normalized polar distribution is $(1/\Gamma_z)d\Gamma_z/d\cos\theta=3(1-\cos^2\theta)/4$ instead of the isotropic unpolarized distribution. This is [polarized massless leptonic W decay](../../../../../polarized-massless-leptonic-w-decay.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
