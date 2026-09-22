<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $q\ne0$ and $\alpha>0$, each [Fourier mode](../../../../../../fourier-mode.md) is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md) with decay rate $r_q=\alpha q^2$. Its [explicit Ornstein-Uhlenbeck solution](../../../../../../explicit-ornstein-uhlenbeck-solution.md) is

$$
h_q(t)=e^{-r_qt}h_q(0)+\sigma\int_0^t e^{-r_q(t-s)}\,dW_q(s),
$$

so the [Itô isometry](../../../../../../ito-isometry.md) gives

$$
\langle h_q(t)^2\rangle
=e^{-2r_qt}\langle h_q(0)^2\rangle
+\frac{\sigma^2}{2r_q}(1-e^{-2r_qt}).
$$

To identify the [overdamped Langevin dynamics](../../../../../../overdamped-langevin-dynamics.md), choose a friction $\zeta_q>0$, a [harmonic oscillator](../../../../../../simple-harmonic-motion.md) potential $V_q=\zeta_q\alpha q^2h_q^2/2$, and force noise $f_q=\zeta_q\eta_q$. The [fluctuation-dissipation relation for a Langevin particle](../../../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md) then defines $k_BT_{\rm eff}=\zeta_q\sigma^2/2$. Its [Boltzmann distribution](../../../../../../boltzmann-distribution.md) is

$$
P_q(h)=\sqrt{\frac{\alpha q^2}{\pi\sigma^2}}
\exp\!\left(-\frac{\alpha q^2h^2}{\sigma^2}\right),
\qquad \boxed{\langle h_q^2\rangle_{\rm st}=\frac{\sigma^2}{2\alpha q^2}\propto q^{-2}}.
$$

This is the [stationary spectrum of a linear fluctuating interface](../../../../../../stationary-spectrum-of-a-linear-fluctuating-interface.md), also following from the [equipartition theorem](../../../../../../equipartition-theorem.md). The numerical prefactor uses exactly the mode-noise normalization given in the paper. The nonzero modes can therefore have a stationary [Gaussian distribution](../../../../../../normal-distribution.md) even though the unpinned zero mode cannot.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
