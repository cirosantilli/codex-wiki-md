<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At the change in [buoyancy frequency](../../../../../../buoyancy-frequency.md), continuity of vertical [velocity](../../../../../../velocity.md) and [fluid pressure](../../../../../../fluid-pressure.md) gives

$$
[W]_{H^-}^{H^+}=0,\qquad [P]_{H^-}^{H^+}=0.
$$

The background [mass density](../../../../../../density.md) is continuous, so there is no interfacial density jump or separate surface restoring [force](../../../../../../force.md). Since $P=i\omega W'/k^2$, these [internal-wave transmission across a stratification step](../../../../../../internal-wave-transmission-across-a-stratification-step.md) conditions are continuity of $W$ and $W'$. The [buoyancy perturbation](../../../../../../buoyancy-perturbation.md) need not be continuous, because the background density gradient jumps.

Let $W_0=-i\omega\eta_0$ and $\ell=k\sqrt{N_2^2/\omega^2-1}$. The lower unstratified layer obeys $W''-k^2W=0$ and the upper [radiation condition](../../../../../../radiation-condition.md) gives

$$
W(z)=C e^{-i\ell(z-H)}\quad(z>H),\qquad W'(H)=-i\ell C.
$$

Propagating these matching data downward gives

$$
W(z)=C\left[\cosh k(H-z)+i\frac{\ell}{k}\sinh k(H-z)\right]\quad(0\leq z\leq H).
$$

The [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) at the moving lower boundary therefore gives

$$
\boxed{C=\frac{-i\omega\eta_0}{\cosh(kH)+i(\ell/k)\sinh(kH)}}.
$$

The upper vertical-displacement [complex amplitude](../../../../../../complex-amplitude.md) at $H$ is

$$
\boxed{\eta_H=\frac{\eta_0}{\cosh(kH)+i(\ell/k)\sinh(kH)}},\qquad
(U,W)=\left(\frac\ell k,1\right)C e^{-i\ell(z-H)}.
$$

In particular, $|\eta_H/\eta_0|=[\cosh^2(kH)+(\ell/k)^2\sinh^2(kH)]^{-1/2}$. The unstratified layer attenuates and phase-shifts the transmitted [internal gravity wave](../../../../../../internal-wave.md). The matching height is $H$ in the original PDF; the TeX transcription's $H'$ is a typo.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
