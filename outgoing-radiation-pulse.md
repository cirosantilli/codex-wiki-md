# Outgoing radiation pulse

↑ **Parent:** [Electromagnetic radiation](electromagnetic-radiation-split.md)

An [outgoing radiation pulse](outgoing-radiation-pulse.md) carries a finite amount of [electromagnetic energy](electromagnetic-energy.md) through successively larger enclosing [spheres](sphere.md). In vacuum, far from a localized source and without absorption or additional reflections, let $P_{\rm emit}(t)$ be the emitted [power](power.md). The [retarded time](retarded-time.md) at [radius](radius.md) $r$ is $s=t-r/c$. Define $\overline S_r$ as the angular average of the radial [Poynting vector](poynting-vector.md) over the [sphere](sphere.md), not a cycle average:

$$
\overline S_r(r,t)=\frac{P_{\rm emit}(t-r/c)}{4\pi r^2},\qquad
\overline u(r,t)=\frac{\overline S_r(r,t)}{c},\qquad
\frac{dU}{dr}=4\pi r^2\overline u=\frac{P_{\rm emit}(t-r/c)}c.
$$

Here $\overline u$ is the angularly averaged [energy density](energy-density.md) in the leading [radiation zone](radiation-zone.md) approximation. Multiplying by shell [area](surface-area.md) removes geometric dilution: the [energy](energy-split.md) per unit radial thickness translates outward without losing its shape. These angular averages do not assume that an actual [electric dipole](electric-dipole.md) emits equally in all directions. Nor do they specify an exact spherically symmetric transverse solution of the [Maxwell equations](maxwell-equations-split.md).

For an explicitly stipulated model, emit

$$
P_{\rm emit}(s)=P_0g(s/\tau),\qquad
g(q)=\begin{cases}\sin^2(\pi q),&0\le q\le1,\\0,&\text{otherwise},\end{cases}
\qquad U=\int P_{\rm emit}(s)\,ds=\frac{P_0\tau}{2}.
$$

After emission ends, $t>\tau$, the pulse lies between $r=c(t-\tau)$ and $r=ct$, provided this shell is in the [radiation zone](radiation-zone.md). Its radial thickness remains $c\tau$. Substituting $s=t-r/c$ in the shell [integral](integral-split.md) $\int4\pi r^2\overline u\,dr$ gives $U=P_0\tau/2$ at every such time. The same substitution in the time [integral](integral-split.md) of $4\pi r^2\overline S_r$ at any enclosing [sphere](sphere.md) gives that same total crossing [energy](energy-split.md). This is [conservation of energy](conservation-of-energy.md) in two different views.

<a id="image-outgoing-pulse-increasing-shell-area-dilutes-local-energy-flux"></a>
![](outgoing-radiation-pulse-spherical-spreading.png)

**[Figure 2](#image-outgoing-pulse-increasing-shell-area-dilutes-local-energy-flux). Outgoing pulse: increasing shell area dilutes local energy flux**. Original calculated model with $L=c\tau$ and $P_{\rm emit}=P_0\sin^2(\pi s/\tau)$ during emission. The circle diagrams show shell support, not equally strong emission in all directions. The lower-left curves show angularly integrated [energy](energy-split.md) per radius and have equal areas. The lower-right curves compare [electric field](electric-field-split.md) and [energy flux](energy-flux.md) ratios at corresponding [retarded times](retarded-time.md) along a fixed direction. All values are model predictions, not historical measurements.

Along any fixed direction with nonzero outgoing [power](power.md), compare the same part of the pulse at two [radii](radius.md), hence at different arrival times. The leading [electric field](electric-field-split.md) amplitude falls as $1/r$, while its squared [wave intensity](intensity-physics.md) falls as $1/r^2$. At $2r$ the field is one half and the [energy flux](energy-flux.md) one quarter; the signal arrives $r/c$ later. A small fixed [area](surface-area.md) receiver therefore intercepts less [energy](energy-split.md) at greater distance even though every enclosing [sphere](sphere.md) receives the same total pulse [energy](energy-split.md). The [inverse-square law](inverse-square-law.md) expresses spreading over [area](surface-area.md), rather than destruction of [energy](energy-split.md). Close to the source, the neglected [near and far field](near-and-far-field.md) terms prevent extrapolating these formulas down to $r=0$.

## ↑ Ancestors (5)

1. [Electromagnetic radiation](electromagnetic-radiation-split.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Outgoing radiation pulse](outgoing-radiation-pulse.md)
