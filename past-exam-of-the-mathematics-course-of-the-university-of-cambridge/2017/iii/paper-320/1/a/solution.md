<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [stellar relaxation time](../../../../../../stellar-relaxation-time.md) is the [time](../../../../../../time-in-physics.md) on which accumulated discrete gravitational encounters change a typical [star](../../../../../../star.md)'s [velocity](../../../../../../velocity.md) by an amount comparable to its original [velocity](../../../../../../velocity.md). It concerns [two-body relaxation](../../../../../../two-body-relaxation.md), rather than the much faster orbital evolution in a smooth [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md). A [collisionless stellar system](../../../../../../collisionless-stellar-system.md) requires this [time](../../../../../../time-in-physics.md) to greatly exceed the duration being studied.

In the straight-line [impulse approximation](../../../../../../impulse-approximation.md), an encounter at relative [speed](../../../../../../speed.md) $u$ has transverse [acceleration](../../../../../../acceleration.md) $Gmb/(b^2+u^2t^2)^{3/2}$. Thus

$$
\Delta v_\perp=\int_{-\infty}^{\infty}\frac{Gmb\,dt}{(b^2+u^2t^2)^{3/2}}=\frac{2Gm}{bu}.
$$

A [small-angle gravitational encounter](../../../../../../small-angle-gravitational-encounter.md) needs $\Delta v_\perp\ll u$. The transition to order-one deflections is therefore $b\sim Gm/u^2$, ignoring factors such as the equal-mass relative deflection. For the spherical estimate $u\sim v$,

$$
\boxed{b_{\min}\sim\frac{Gm}{v^2}.}
$$

This is the lower cutoff of the weak-scattering estimate; closer encounters actually occur and require strong-scattering treatment.

The number of encounters in [time](../../../../../../time-in-physics.md) $T$ with [impact parameters](../../../../../../impact-parameter.md) in $[b,b+db]$ is $2\pi b\,db\,nuT$. Independent random transverse directions make mean kicks cancel while their [variances](../../../../../../variance-split.md) add. Consequently

$$
\frac{\langle|\Delta\mathbf v|^2\rangle}{T}=\int_{b_{\min}}^R\left(\frac{2Gm}{bu}\right)^2 2\pi bnu\,db=\frac{8\pi G^2m^2n}{u}\log\Lambda,\qquad\Lambda=\frac R{b_{\min}}.
$$

Each logarithmic interval contributes equally, giving the [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md). Defining a deflection [time](../../../../../../time-in-physics.md) by [variance](../../../../../../variance-split.md) $v^2$ and setting $u=v$ gives $v^3/(8\pi G^2m^2n\log\Lambda)$. The paper instead uses an order-one normalization three quarters of this estimate:

$$
\boxed{t_{\rm rel}\simeq\frac3{32\pi}\frac{v^3}{G^2m^2n\log\Lambda}.}
$$

Both have the same physical scaling. The specified characteristic [speed](../../../../../../speed.md), the word “comparable”, the velocity-distribution average and strong-encounter cutoff do not fix that numerical coefficient uniquely. The crude equal-speed impulse calculation must not be claimed to determine $3/(32\pi)$ exactly.

For a self-gravitating, approximately virialized system, the [virial theorem](../../../../../../virial-theorem.md) gives $v^2\sim GNm/R$. With $n=3N/(4\pi R^3)$, $\Lambda\sim N$ and the [stellar crossing time](../../../../../../stellar-crossing-time.md) $t_{\rm dyn}=R/v$, substitution into the paper's convention gives

$$
\boxed{t_{\rm rel}\simeq\frac{N}{8\log N}\,t_{\rm dyn}.}
$$

An externally dominated [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) or a different structural constant changes this substitution. For an [N-body simulation](../../../../../../n-body-simulation.md) lasting $T=K t_{\rm dyn}$, a tolerable fractional velocity-squared diffusion $\varepsilon\ll1$ requires $T/t_{\rm rel}\lesssim\varepsilon$, hence

$$
\boxed{\frac{N}{8\log N}\gtrsim\frac K\varepsilon.}
$$

There is no unique smallest $N$ without $K$, the error tolerance and the [force](../../../../../../force.md) prescription. For scale, equality at $t_{\rm rel}/t_{\rm dyn}=100$ occurs near $N=7.1\times10^3$; $N=10^5$ gives about $1.1\times10^3$ crossing times. A calculation lasting 100 crossing times therefore needs substantially more than the first threshold to have negligible relaxation. [Gravitational softening](../../../../../../gravitational-softening.md) can raise the effective cutoff and reduce artificial scattering, but it also sets the spatial [force](../../../../../../force.md) resolution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
