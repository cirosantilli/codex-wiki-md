<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Let the surface radius be $a$, let $\Delta$ denote epicentral angle in radians, and put $\eta(r)=r/v(r)$. The [spherical elastic ray invariant](../../../../../spherical-elastic-ray-invariant.md) gives $\sin i=p/\eta$. Along either radial leg, if $l$ is arclength and $\theta$ polar angle in the ray plane,

$$
\left|\frac{dr}{dl}\right|=\cos i,\qquad
r\frac{d\theta}{dl}=\sin i.
$$

For a turning ray with minimum radius $r_p$ defined by $\eta(r_p)=p$, the outgoing and incoming legs therefore give

$$
\boxed{\Delta(p)=2\int_{r_p}^a
\frac{p}{r\sqrt{\eta(r)^2-p^2}}\,dr,}
\qquad
T(p)=2\int_{r_p}^a
\frac{\eta(r)^2}{r\sqrt{\eta(r)^2-p^2}}\,dr.
$$

The square-root turning singularity is integrable for a regular turning point.

Introduce the reduced travel time

$$
\tau(p)=T(p)-p\Delta(p)
=2\int_{r_p}^a\frac{\sqrt{\eta(r)^2-p^2}}r\,dr.
$$

Its integrand vanishes at the moving lower endpoint, so differentiation gives $\tau'(p)=-\Delta(p)$. Consequently

$$
T'(p)=p\Delta'(p),\qquad
\boxed{\frac{dT}{d\Delta}=p}
$$

on every regular travel-time branch. This is also the endpoint variation of travel time: the tangential endpoint [slowness](../../../../../slowness.md) multiplied by the surface radius is $p$. Angles expressed in degrees would introduce the corresponding conversion factor; the displayed equality uses radians.

For [Herglotz–Wiechert inversion](../../../../../herglotz-wiechert-inversion.md), assume $\eta$ is strictly increasing so that $r=r(\eta)$ is single-valued, and set $\eta_a=a/v(a)$ and $h(\eta)=d\log r/d\eta$. The angular integral becomes an [Abel integral equation](../../../../../abel-integral-equation.md):

$$
\Delta(p)=2p\int_p^{\eta_a}
\frac{h(\eta)}{\sqrt{\eta^2-p^2}}\,d\eta.
$$

For any $0<\mu<\eta_a$, multiply by $(p^2-\mu^2)^{-1/2}$ and integrate. Interchanging the triangular region $\mu<p<\eta<\eta_a$ gives

$$
\begin{aligned}
\int_\mu^{\eta_a}\frac{\Delta(p)}{\sqrt{p^2-\mu^2}}\,dp
&=2\int_\mu^{\eta_a}h(\eta)
\left[\int_\mu^\eta
\frac{p\,dp}{\sqrt{p^2-\mu^2}\sqrt{\eta^2-p^2}}\right]d\eta\\
&=\pi\int_\mu^{\eta_a}h(\eta)\,d\eta
=\pi\log\frac{a}{r(\mu)}.
\end{aligned}
$$

The inner integral equals $\pi/2$: the substitution $p^2=\mu^2+(\eta^2-\mu^2)\sin^2\theta$ reduces it to $\int_0^{\pi/2}d\theta$. Thus the full constructive inversion is

$$
\boxed{r(\mu)=a\exp\left[-\frac1\pi
\int_\mu^{\eta_a}\frac{\Delta(p)}{\sqrt{p^2-\mu^2}}\,dp\right],
\qquad v(r(\mu))=\frac{r(\mu)}{\mu}.}
$$

The surface radius and surface [slowness](../../../../../slowness.md) fix the normalization. Varying $\mu$ reconstructs radius and speed parametrically; the centre is recovered by a limit when the data extend that far. The calculation assumes smooth regular turning rays and complete branch data, not merely the first arrival at each epicentral angle.

For a check, a constant speed $v_0$ gives $\eta_a=a/v_0$, $\Delta(p)=2\arccos(p/\eta_a)$ and $T(p)=2\sqrt{a^2-p^2v_0^2}/v_0$. These satisfy $dT/d\Delta=p$, and the inversion returns $r(\mu)=v_0\mu$.

If $\eta$ decreases outwards on an interval, then it increases as a surface ray travels inward through that interval. Such a ray cannot turn there, since turning requires the decreasing inward value of $\eta$ to reach $p$. Rays that penetrate this interval can traverse it and turn deeper, but the map $\eta\mapsto r$ now has several branches. The angular data constrain combinations of those branch contributions, rather than the single function $h(\eta)$ used above. This is a [hidden turning-ray zone from nonmonotone spherical slowness](../../../../../hidden-turning-ray-zone-from-nonmonotone-spherical-slowness.md). **The stated single-valued inversion fails and does not uniquely locate the speed profile in that interval without additional information.** Missing turning rays and possible multiple travel-time branches are the obstruction, not a failure of the algebraic Abel-kernel identity.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
