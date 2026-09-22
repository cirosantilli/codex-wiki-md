<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<\omega<\epsilon$, let $x=\theta-\theta_s$ and $\kappa=\sqrt{\epsilon^2-\omega^2}$. In a single well, sufficiently small fluctuations obey the linear [overdamped Langevin dynamics](../../../../../../overdamped-langevin-dynamics.md)

$$
\dot x=-\kappa x+\xi(t),\qquad \langle\xi(t)\xi(t')\rangle=2T_{\rm eff}\delta(t-t').
$$

This is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md). Its solution is

$$
x(t)=e^{-\kappa t}x(0)+\int_0^t e^{-\kappa(t-s)}\xi(s)\,ds.
$$

The mean decays, while the noise integral gives $\langle x(t)^2\rangle\to T_{\rm eff}/\kappa$. For $\tau\geq0$, the future-noise contribution is independent of $x(t)$, so $\langle x(t)x(t+\tau)\rangle=e^{-\kappa\tau}\langle x(t)^2\rangle$. The [intrawell phase autocorrelation](../../../../../../intrawell-phase-autocorrelation.md) is therefore

$$
\boxed{\langle\theta(t)\theta(t+\tau)\rangle\simeq\arcsin^2(\omega/\epsilon)+\frac{T_{\rm eff}}{\sqrt{\epsilon^2-\omega^2}}\exp[-\sqrt{\epsilon^2-\omega^2}\,|\tau|].}
$$

The connected [unnormalized time autocorrelation](../../../../../../unnormalized-time-autocorrelation.md) is just the exponentially decaying second term. The constant first term is necessary because the requested raw correlation is not centered at the [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md). This is the harmonic-well approximation. If a full first-order expansion in $T_{\rm eff}$ is wanted, the quadratic term in the drift is $\omega x^2/2$. Local stationarity gives $\langle x\rangle=\omega T_{\rm eff}/(2\kappa^2)+O(T_{\rm eff}^2)$, so the raw correlation gains a constant $\alpha\omega T_{\rm eff}/\kappa^2$ at that order. The connected correlation is unchanged to first order; the boxed formula is the conventional linearized result rather than a complete nonlinear first-order raw-correlation expansion.

The required time window is long compared with $\kappa^{-1}$ but short compared with the escape time, with the lag also short compared with escape. Fluctuations of size $\sqrt{T_{\rm eff}/\kappa}$ must be small compared with the distance to a neighboring maximum, and the relevant barriers must greatly exceed $T_{\rm eff}$. For a fixed nonzero noise strength, the unwrapped phase eventually makes [phase slips](../../../../../../phase-slip.md); its raw correlation does not have this stationary infinite-time limit. Thus “large time” here refers to local relaxation within the occupied well, not to the limit after arbitrarily many barrier crossings.

For [thermally activated phase slips](../../../../../../thermally-activated-phase-slip.md), the forward saddle is at $\pi-\alpha$ and the backward saddle at $-\pi-\alpha$. Their barriers above the same minimum are

$$
\Delta V_+=2\kappa-\omega(\pi-2\alpha),\qquad \Delta V_-=2\kappa+\omega(\pi+2\alpha),\qquad \boxed{\Delta V_--\Delta V_+=2\pi\omega.}
$$

In the [Kramers escape rate](../../../../../../kramers-escape-rate.md) approximation, both saddles have curvature $-\kappa$ and the minimum has curvature $+\kappa$, so the prefactors agree:

$$
p_\pm\propto\frac{\kappa}{2\pi}e^{-\Delta V_\pm/T_{\rm eff}},\qquad \boxed{\frac{p_+}{p_-}=\exp\left(\frac{2\pi\omega}{T_{\rm eff}}\right).}
$$

This is the [forward-backward bias of phase slips](../../../../../../forward-backward-bias-of-phase-slips.md). It favors forward motion because each forward step lowers the tilted potential by $2\pi\omega$. For $\omega\ll\epsilon$, $\Delta V_\pm=2\epsilon\mp\pi\omega+O(\omega^2/\epsilon)$, which gives the same ratio; the exact barrier difference is independent of $\epsilon$. These probabilities may be read as rates in a common short observation interval, or as normalized competing exit probabilities. The $T_{\rm eff}$ in the exponent is the noise scale as defined in the [Langevin equation](../../../../../../langevin-dynamics.md); no additional $k_B$ factor is inserted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
