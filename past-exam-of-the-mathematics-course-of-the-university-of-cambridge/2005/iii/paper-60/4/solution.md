<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The physical [spherical coordinates](../../../../../spherical-coordinate-system.md) cover $t\in\mathbb R$, $r\in[0,\infty)$, $\theta\in[0,\pi]$, and $\phi\in[0,2\pi)$ with periodic identification. The center and the polar axes are the usual [coordinate singularities](../../../../../coordinate-singularity.md), rather than physical [curvature singularities](../../../../../curvature-singularity.md); a regular polar chart restricts $r>0$ and $0<\theta<\pi$. For the [null coordinates](../../../../../null-coordinate.md),

$$
u=t-r,\quad v=t+r,\qquad t=\frac{u+v}{2},\quad r=\frac{v-u}{2},\qquad u,v\in\mathbb R,\ v\geq u.
$$

Thus the physical [metric tensor](../../../../../metric-tensor.md) is

$$
d\hat s^2=du\,dv-\frac{(v-u)^2}{4}d\Sigma^2.
$$

The [conformal transformation](../../../../../conformal-map.md) followed by $p=\arctan u$, $q=\arctan v$ gives $du=(1+u^2)dp$, $dv=(1+v^2)dq$, and

$$
\frac{v-u}{\sqrt{(1+u^2)(1+v^2)}}=\sin(q-p).
$$

Consequently $ds^2=4dp\,dq-\sin^2(q-p)d\Sigma^2$. Finally $T=p+q$, $R=q-p$ converts $4dp\,dq$ to $dT^2-dR^2$, yielding

$$
\boxed{ds^2=dT^2-dR^2-\sin^2R\,d\Sigma^2.}
$$

The ranges must retain their joint constraints:

$$
-\frac\pi2<p,q<\frac\pi2,\quad q\geq p;\qquad -\pi<T<\pi,\quad0\leq R<\pi,\quad |T|+R<\pi.
$$

Equivalently, $-\pi<T-R<\pi$ and $-\pi<T+R<\pi$, with $R\geq0$. The angles retain their original ranges and identifications. Extending $R$ to negative values would double-count the radial polar geometry. The [conformal factor](../../../../../conformal-factor.md) is

$$
\boxed{\Omega=2\cos p\cos q=\cos T+\cos R>0\ \text{in the physical region},\qquad g=\Omega^2\hat g.}
$$

The unphysical [metric tensor](../../../../../metric-tensor.md) extends onto the [Einstein static universe](../../../../../einstein-static-universe.md), while physical [Minkowski spacetime](../../../../../minkowski-spacetime.md) occupies the triangular region in its radial [Penrose diagram](../../../../../penrose-diagram.md). The edge $R=0$ is the regular center and belongs to the physical region away from its endpoints.

The [conformal boundary](../../../../../conformal-boundary.md) consists of the following infinities. [Future null infinity](../../../../../future-null-infinity.md) has $q=\pi/2$, hence $T+R=\pi$ with $0<R<\pi$, and corresponds to finite $u$ with $v\to+\infty$. [Past null infinity](../../../../../past-null-infinity.md) has $p=-\pi/2$, hence $T-R=-\pi$, and corresponds to finite $v$ with $u\to-\infty$. [Future timelike infinity](../../../../../future-timelike-infinity.md) is $(T,R)=(\pi,0)$, [past timelike infinity](../../../../../past-timelike-infinity.md) is $(-\pi,0)$, and [spacelike infinity](../../../../../spacelike-infinity.md) is $(0,\pi)$. Although angles label points on null infinity, their two-spheres collapse at these three endpoint locations in the compactified picture.

<a id="4/image-the-radial-minkowski-conformal-diagram-and-the-endpoints-of-timelike-null-and-spacelike-geodesics"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-60-minkowski-compactification.png)

**[Figure 2](#4/image-the-radial-minkowski-conformal-diagram-and-the-endpoints-of-timelike-null-and-spacelike-geodesics). The radial Minkowski conformal diagram and the endpoints of timelike, null and spacelike geodesics**.

For the [geodesic endpoints in Minkowski conformal compactification](../../../../../geodesic-endpoints-in-minkowski-conformal-compactification.md), one can check the limits directly. A timelike inertial trajectory is $\mathbf x=\mathbf b+\mathbf w t$ with $|\mathbf w|<1$. At $t\to+\infty$ both $t-r$ and $t+r$ tend to $+\infty$, so $p,q\to\pi/2$ and the trajectory ends at [future timelike infinity](../../../../../future-timelike-infinity.md). At $t\to-\infty$ both tend to $-\infty$, giving [past timelike infinity](../../../../../past-timelike-infinity.md). This includes a stationary inertial worldline with bounded $r$.

For a null inertial trajectory, $|\mathbf w|=1$. As $t\to+\infty$, $r=t+\mathbf w\cdot\mathbf b+o(1)$, so $u$ has a finite limit while $v\to+\infty$; its future endpoint lies on [future null infinity](../../../../../future-null-infinity.md). As $t\to-\infty$, $r=-t-\mathbf w\cdot\mathbf b+o(1)$, giving a finite limiting $v$ and $u\to-\infty$, hence a past endpoint on [past null infinity](../../../../../past-null-infinity.md). Radial [null geodesic](../../../../../null-geodesic.md) paths have $T\pm R$ constant. A ray passing through the center changes its angular direction; in the angle-suppressed radial diagram it reflects at $R=0$ rather than terminating there.

A [spacelike geodesic](../../../../../spacelike-geodesic.md) is also a straight line, now parametrized so that $|d\mathbf x/d\lambda|>|dt/d\lambda|$. At either end, $r>|t|$ asymptotically, $u\to-\infty$, $v\to+\infty$, and the endpoint is [spacelike infinity](../../../../../spacelike-infinity.md). A radial spacelike line at $t=0$ has two opposite-angle halves which project onto the same horizontal interval in the diagram.

The [conformal compactification](../../../../../conformal-compactification.md) endpoints occur at finite $T$ but at infinite physical [proper time](../../../../../proper-time.md) or [affine parameter](../../../../../affine-parameter.md); [Minkowski spacetime](../../../../../minkowski-spacetime.md) is [geodesically complete](../../../../../geodesic-completeness.md). The [conformal preservation of null geodesic paths](../../../../../conformal-preservation-of-null-geodesic-paths.md) does not preserve an [affine parameter](../../../../../affine-parameter.md): if $\lambda$ is physically affine, an unphysical [affine parameter](../../../../../affine-parameter.md) satisfies $d\widetilde\lambda/d\lambda=\Omega^2$ up to a constant. Along a complete null ray this can have a finite integral at infinity. Timelike and spacelike physical [geodesic](../../../../../geodesic.md) paths are not generally [geodesics](../../../../../geodesic.md) of the rescaled [metric tensor](../../../../../metric-tensor.md), so their drawn curves must not be interpreted as freely falling unphysical observers.

Finally, every physical event can send an outgoing null ray to [future null infinity](../../../../../future-null-infinity.md), so $J^-(\mathcal I^+)$ is all of [Minkowski spacetime](../../../../../minkowski-spacetime.md). Its [black-hole region](../../../../../black-hole.md) and intrinsic [event horizon](../../../../../event-horizon.md) are empty. The null edges in the diagram are infinity, not horizons concealing part of the physical manifold. Complete inertial observers likewise have no [observer event horizon](../../../../../observer-event-horizon.md). Accelerated observers restricted to a [Rindler wedge](../../../../../rindler-wedge.md) can have a [Rindler horizon](../../../../../rindler-horizon.md), but that is observer-dependent and does not contradict the [horizon-free Minkowski spacetime](../../../../../horizon-free-minkowski-spacetime.md). **The conformal diagram compactifies infinity; it does not introduce a physical horizon.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
