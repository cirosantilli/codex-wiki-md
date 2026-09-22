<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For freezing, the liquid [concentration](../../../../../../concentration.md) decreases away from the interface, so the [liquidus](../../../../../../liquidus.md) $T_L=-mC$ increases there. [Constitutional supercooling](../../../../../../constitutional-supercooling.md) means $T_l<T_L$ somewhere ahead of the interface. Since these [temperatures](../../../../../../temperature.md) agree at the interface, its local onset is

$$
T_{l,x}(a^+,t)<-m C_x(a^+,t).
$$

For the [similarity solution](../../../../../../similarity-solution.md) and [salt rejection](../../../../../../salt-rejection.md) condition, this is exactly

$$
\boxed{\frac{\epsilon(T_\infty-T_i)e^{-\epsilon^2\lambda^2}}{\sqrt\pi\operatorname{erfc}(\epsilon\lambda)}<m\lambda C_i.}
$$

It is also the global criterion for this freezing solution when $D<\kappa$ and $T_\infty>T_i$: the ratio $T_L'(x)/T_l'(x)$ is a positive constant times $\exp[-x^2(1/D-1/\kappa)/(4t)]$. For $x\ge a\ge0$ this ratio decreases with $x$. If the ratio is at most one at the interface, $T_l-T_L$ cannot become negative; if it is greater than one there, a supercooled interval appears immediately ahead. Equality marks onset, not a finite supercooled interval.

For fixed positive $\Delta\theta$ and $\lambda=O(1)>0$, the left side of the inequality is $O(\epsilon)$ and the right side is positive of order one, so freezing is constitutionally supercooled for sufficiently small $\epsilon$. To locate the boundary between the two regimes, resolve the smaller scale $\Delta\theta=O(\epsilon)$, $\lambda=O(\epsilon)$. The salt equation and [liquidus](../../../../../../liquidus.md) then give

$$
C_i-C_0=\sqrt\pi C_0\lambda+O(\lambda^2),\qquad m\lambda C_i=\frac{\Delta\theta}{2\sqrt\pi}+O(\epsilon^2).
$$

Here $\epsilon\lambda=O(\epsilon^2)$, so the thermal equation improves to $T_i=(T_\infty+T_{-\infty})/2+O(\epsilon^2)$; this justifies the second expansion including [latent heat](../../../../../../latent-heat.md). Also $T_\infty-T_i=\theta_++O(\epsilon)$ and the left side of the exact criterion is $\epsilon\theta_+/\sqrt\pi+O(\epsilon^2)$. Therefore the [small-diffusivity constitutional-supercooling threshold](../../../../../../small-diffusivity-constitutional-supercooling-threshold.md) is

$$
\Delta\theta>2\epsilon\theta_++O(\epsilon^2),\qquad \boxed{\theta_->\theta_+(1+2\epsilon)\ \text{to first order in }\epsilon.}
$$

This printed condition is an asymptotic onset condition, rather than an exact finite-$\epsilon$ inequality. In its $O(\epsilon^2)$ transition window the complete algebraic system and exact [gradient](../../../../../../gradient.md) criterion must be used.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
