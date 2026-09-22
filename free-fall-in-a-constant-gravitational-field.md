# Free fall in a constant gravitational field

↑ **Parent:** [Free fall](free-fall.md)

Take downward [displacement](displacement.md) $s$ as positive, assume a constant [gravitational acceleration](gravitational-acceleration.md) $g>0$, and release a [point mass](point-mass.md) from rest at $s=0$. Integrating $\ddot s=g$ twice gives

$$
v(t)=gt,\qquad s(t)=\frac12gt^2.
$$

For a downward distance $h>0$, the arrival time and [speed](speed.md) are

$$
t_{\mathrm{fall}}=\sqrt{\frac{2h}{g}},\qquad v_{\mathrm{arrival}}=\sqrt{2gh}.
$$

For the model values $h=20\,\mathrm m$ and $g=9.81\,\mathrm{m\,s^{-2}}$, these are approximately $2.0193\,\mathrm s$ and $19.8091\,\mathrm{m\,s^{-1}}$. Doubling the height multiplies both quantities by $\sqrt2$; it does not double them. The same [speed](speed.md) follows from the [work-energy theorem](work-energy-theorem.md), $mgh=mv^2/2$.

For intervals of length $\Delta t$, the successive downward [displacements](displacement.md) are

$$
s((j+1)\Delta t)-s(j\Delta t)=\frac12g(\Delta t)^2(2j+1),\qquad j=0,1,2,\ldots.
$$

Thus equal spacing in time produces increasingly separated positions. This is the odd-number pattern in Galileo's result. It assumes constant [acceleration](acceleration.md) and release from rest; a nonzero initial [velocity](velocity.md) adds a linear term to $s(t)$.

The approximation can be estimated for a spherical source of radius $R$ and [standard gravitational parameter](standard-gravitational-parameter.md) $\mu$. Writing $g_0=\mu/R^2$, the gravitational magnitude at height $h$ is

$$
\frac{g(R+h)}{g_0}=\left(1+\frac hR\right)^{-2}.
$$

For $h/R\ll1$, a [Taylor expansion](taylor-expansion.md) gives $g(R+h)/g_0=1-2h/R+O((h/R)^2)$. Small height relative to the source's radius makes nearly constant gravity plausible; negligible [drag force](drag-physics.md) remains a separate requirement.

## ↑ Ancestors (6)

1. [Free fall](free-fall.md)
2. [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
