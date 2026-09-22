<h1 id="34b/solution">Solution</h1>

↑ **Parent:** [34B](../34b.md)

The asymptotic [scattering wavefunction](../../../../../scattering-wavefunction.md) is $\Psi\sim e^{ikz}+f(\theta)e^{ikr}/r$. For a real central potential, the [scattering phase shift](../../../../../scattering-phase-shift.md) $\delta_l$ multiplies the outgoing component of each [partial wave](../../../../../partial-wave.md) relative to the incoming one by $e^{2i\delta_l}$. Matching the incident-wave normalization gives

$$
\Psi\sim\frac1{2ikr}\sum_{l\geq0}(2l+1)\left[e^{2i\delta_l}e^{ikr}-(-1)^le^{-ikr}\right]P_l(\cos\theta).
$$

Subtract the given incident [plane wave](../../../../../plane-wave.md) expansion. Since $e^{2i\delta_l}-1=2ie^{i\delta_l}\sin\delta_l$, the [scattering amplitude](../../../../../scattering-amplitude.md) is

$$
\boxed{f(\theta)=\frac1k\sum_{l\geq0}(2l+1)e^{i\delta_l}\sin\delta_l\,P_l(\cos\theta)}.
$$

Orthogonality $\int_{-1}^1P_lP_j\,dx=2\delta_{lj}/(2l+1)$ eliminates cross terms in $\sigma=\int|f|^2\,d\Omega$, giving **$\boxed{\sigma=(4\pi/k^2)\sum_l(2l+1)\sin^2\delta_l}$.**

For the [spherical square well](../../../../../spherical-square-well.md), the regular reduced radial $l=0$ wave is $A\sin(\kappa r)$ inside and $B\sin(kr+\delta_0)$ outside, with $\kappa^2=k^2+\gamma^2$. Continuity of the wave and its derivative gives the [logarithmic-derivative matching](../../../../../logarithmic-derivative-matching.md) relation $\kappa\cot(\kappa a)=k\cot(ka+\delta_0)$, or

$$
\frac{\tan(ka+\delta_0)}{ka}=\frac{\tan(\kappa a)}{\kappa a}.
$$

At zeros of the denominators the original matching relation supplies the limiting interpretation.

Under the stated deep-well approximation, put $x=ka$ and $B_0=\tan(\gamma a)/(\gamma a)$. The condition $\delta_0\in\pi\mathbb Z$ is $\tan x/x=B_0$. If $B_0<0$, its first positive solution lies in $(\pi/2,\pi)$; if $B_0=0$, it is $\pi$. For $0<B_0\leq1$, a solution lies in $(\pi,3\pi/2)$ because there $\tan x/x$ rises continuously from zero to infinity. If $B_0>1$, the first positive solution lies in $(0,\pi/2)$, where $\tan x/x$ rises from one to infinity. The limiting pole case gives $x=\pi/2$ by the cotangent relation. Thus **$\boxed{0<k_0<3\pi/(2a)}$**, without calculating the integer phase index. The use of $\kappa\simeq\gamma$ presumes the located wave numbers remain small compared with $\gamma$.

## ↑ Ancestors (10)

1. [34B](../34b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
