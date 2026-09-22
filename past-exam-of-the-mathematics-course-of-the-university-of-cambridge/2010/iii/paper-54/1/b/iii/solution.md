<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $M=-a^2$ with $a>0$. On a constant-time slice, the proper distance from the axis to radius $r$ and the circumference at that radius are

$$
s(r)=\int_0^r\frac{dR}{\sqrt{a^2+R^2/\ell^2}}=\frac r a+O(r^3),
\qquad C(r)=2\pi r.
$$

Hence $C/s\to2\pi a$. A smooth axis in a [Riemannian metric](../../../../../../../riemannian-metric.md) requires the Euclidean limit $C/s\to2\pi$, so regularity forces $a=1$, or $M=-1$. For $a\ne1$ the [conical singularity of negative-mass BTZ geometry](../../../../../../../conical-singularity-of-negative-mass-btz-geometry.md) has deficit angle $2\pi(1-a)$; for $a>1$ this is an angular excess. Even integer $a>1$ is singular with the stipulated angular period $2\pi$: a multiple covering does not make the tip a smooth point.

At $M=-1$, set $r=\ell\sinh\chi$. The [metric tensor](../../../../../../../metric-tensor.md) becomes

$$
ds^2=-\cosh^2\chi\,dt^2+\ell^2(d\chi^2+\sinh^2\chi\,d\phi^2),
$$

which is regular at $\chi=0$ and describes [Anti-de Sitter spacetime](../../../../../../../anti-de-sitter-spacetime.md) with nonperiodic time. For every $M<0$, $f=a^2+r^2/\ell^2$ stays positive. An outward [radial null geodesic](../../../../../../../radial-null-geodesic.md) obeys $dt/dr=1/f$, and reaches the timelike conformal boundary in finite coordinate time, since $\int_0^\infty dr/f=\pi\ell/(2a)$. Thus no [event horizon](../../../../../../../event-horizon.md) hides the conical axis. **The geometry is nakedly singular except at $M=-1$.** Its local curvature away from the axis is that of [Anti-de Sitter spacetime](../../../../../../../anti-de-sitter-spacetime.md); the argument is a global angular-identification test, not curvature blowup.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 54](../../../../paper-54-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
