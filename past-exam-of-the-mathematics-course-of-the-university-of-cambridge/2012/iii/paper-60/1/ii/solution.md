<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md) relations $H=2/(3t)$ and $\bar\rho\propto t^{-2}$. Write $H_{\rm ta}=H(t_{\rm ta})$ and $R_{\rm ta}=R(t_{\rm ta})$. Since $M=(4\pi/3)\Delta_{\rm ta}\bar\rho_{\rm ta}R_{\rm ta}^3$,

$$
\frac{GM}{H_{\rm ta}^2R_{\rm ta}^3}=\frac{\Delta_{\rm ta}}2,\qquad \frac{d^2y}{d\tau^2}=-\frac{\Delta_{\rm ta}}{2y^2}.
$$

The dimensionless first integral with zero velocity at $y=1$ is $(dy/d\tau)^2=\Delta_{\rm ta}(1/y-1)$. On the expanding branch this gives

$$
\tau(y)=\frac1{\sqrt{\Delta_{\rm ta}}}\int_0^y\sqrt{\frac{u}{1-u}}\,du.
$$

Evaluating the integral gives the inverse-trigonometric expression in the source. Alternatively, differentiate it: $d\tau/dy=\Delta_{\rm ta}^{-1/2}\sqrt{y/(1-y)}$, so differentiation of the first integral gives exactly the required [equation of motion](../../../../../../equation-of-motion.md). At $y=1$, the integral equals $\pi/2$. Thus $\tau_{\rm ta}=2/3$ fixes $\sqrt{\Delta_{\rm ta}}=3\pi/4$. The collapsing branch is $\tau=4/3-\tau_{\rm expand}(y)$, not the same increasing inverse function.

For the early-time [density contrast](../../../../../../density-contrast.md), expand the integral directly:

$$
\boxed{\tau=\frac{8}{9\pi}y^{3/2}\left(1+\frac{3y}{10}+O(y^2)\right).}
$$

**The leading coefficient in the printed small-radius approximation needs correction to $8/(9\pi)$.** The printed coefficient is inconsistent with both the exact integral and approach to the homogeneous background. Indeed, the nonlinear [density contrast](../../../../../../density-contrast.md) satisfies

$$
1+\delta_{\rm NL}=\Delta_{\rm ta}\frac{(t/t_{\rm ta})^2}{y^3}=\Delta_{\rm ta}\frac{9\tau^2}{4y^3}=1+\frac35y+O(y^2).
$$

Hence $\delta_{\rm L}\sim3y/5$. In the [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md) the growing [linear cosmological density perturbation](../../../../../../linear-cosmological-density-perturbation-split.md) is proportional to $t^{2/3}$, so its extrapolation is

$$
\delta_{\rm L}(\tau)=\frac35\left(\frac{9\pi\tau}{8}\right)^{2/3}.
$$

The formal collapse occurs at $\tau_{\rm coll}=4/3$, giving the [linear spherical-collapse threshold](../../../../../../linear-spherical-collapse-threshold.md)

$$
\boxed{\delta_{\rm L}(t_{\rm coll})=\frac35\left(\frac{3\pi}{2}\right)^{2/3}\simeq1.686.}
$$

The actual nonlinear [density contrast](../../../../../../density-contrast.md) diverges at collapse; the finite number is the extrapolated linear amplitude. Equivalently, the full [spherical-collapse model](../../../../../../spherical-collapse-model.md) has $y=(1-\cos\theta)/2$ and $\tau=2(\theta-\sin\theta)/(3\pi)$, with turnaround at $\theta=\pi$ and formal collapse at $2\pi$. Combining the half-radius estimate with the background-density decrease up to $2t_{\rm ta}$ gives $\rho_{\rm vir}/\bar\rho(t_{\rm coll})=32\Delta_{\rm ta}=18\pi^2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
