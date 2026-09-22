<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

In the instantaneous rest frame the total radiation has zero net three-momentum, so its emitted four-momentum is proportional to the [four-velocity](../../../../../four-velocity.md). A Lorentz boost multiplies its energy by $\gamma$, while the elapsed coordinate time for the source is also multiplied by $\gamma$. Their ratio, total instantaneous radiated power, is therefore invariant. This concerns total emitted power, not the directional flux or an observer's photon arrival rate.

Use the metric of signature $(+---)$ and dots for proper-time derivatives. From $\gamma=(1-v^2)^{-1/2}$ obtain $\dot\gamma=\gamma^3\alpha$, where $\alpha=\mathbf v\cdot\dot{\mathbf v}$. Differentiating $U=(\gamma,\gamma\mathbf v)$ gives

$$
\boxed{\dot U=(\gamma^3\alpha,\gamma^3\alpha\mathbf v+\gamma\dot{\mathbf v}).}
$$

Squaring in the [Minkowski metric](../../../../../minkowski-metric.md), using $1-v^2=\gamma^{-2}$, gives $\dot U\cdot\dot U=\gamma^6\alpha^2(1-v^2)-2\gamma^4\alpha^2-\gamma^2|\dot{\mathbf v}|^2$, hence

$$
\boxed{\dot U\cdot\dot U=-\gamma^4\alpha^2-\gamma^2|\dot{\mathbf v}|^2.}
$$

In the rest frame, $-\dot U^2$ is the squared ordinary acceleration, so invariance of power and the low-speed [Larmor formula](../../../../../larmor-formula.md) give $P=-(\mu_0q^2/6\pi)\dot U^2$. In terms of coordinate-time acceleration $\mathbf a=d\mathbf v/dt$, this is the [Lienard formula](../../../../../lienard-radiated-power-formula.md)

$$
\boxed{P=\frac{\mu_0q^2}{6\pi}\gamma^6\bigl(|\mathbf a|^2-|\mathbf v\times\mathbf a|^2\bigr),\qquad c=1.}
$$

For circular motion perpendicular to $\mathbf B$, $\mathbf a\perp\mathbf v$ and the [Lorentz force](../../../../../lorentz-force.md) gives $\gamma m|\mathbf a|=|q|v|\mathbf B|$. Thus

$$
\boxed{P=\frac{\mu_0q^4}{6\pi m^2}(\gamma^2-1)|\mathbf B|^2.}
$$

At low speed $\gamma^2-1\sim v^2$, reproducing ordinary Larmor radiation with magnetic acceleration $|q|vB/m$.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
