<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [geometrized units](../../../../../../geometrized-units.md) and [metric signature](../../../../../../metric-signature.md) $(-+++)$, with $M>0$. In the exterior of [Schwarzschild spacetime](../../../../../../schwarzschild-spacetime.md), put $f=1-2M/r$. The [Schwarzschild tortoise coordinate](../../../../../../schwarzschild-tortoise-coordinate.md) satisfies

$$
\frac{dr_*}{dr}=f^{-1},\qquad r_*=r+2M\log\left|\frac r{2M}-1\right|.
$$

The [retarded and advanced null coordinates](../../../../../../retarded-and-advanced-null-coordinates.md) $u=t-r_*$ and $v=t+r_*$ then give $ds^2=-f\,du\,dv+r^2d\Omega^2$. The logarithmic divergence of $r_*$ suggests exponentiating these [null coordinates](../../../../../../null-coordinate.md). In the right exterior define the [Kruskal–Szekeres coordinates](../../../../../../kruskal-szekeres-coordinates.md)

$$
U=-e^{-u/(4M)},\qquad V=e^{v/(4M)}.
$$

Their product eliminates $t$:

$$
UV=-e^{r_*/(2M)}=\left(1-\frac r{2M}\right)e^{r/(2M)}.
$$

Since $du=-4M\,dU/U$ and $dv=4M\,dV/V$, the [Schwarzschild metric](../../../../../../schwarzschild-spacetime.md) becomes

$$
\boxed{ds^2=-\frac{32M^3}{r}e^{-r/(2M)}\,dU\,dV+r^2d\Omega^2,\qquad UV=\left(1-\frac r{2M}\right)e^{r/(2M)}.}
$$

Here $r$ is an implicitly defined function of $UV$. The derivative of the right side with respect to $r$ is $-r e^{r/(2M)}/(4M^2)$, which is nonzero at $r=2M$. The [inverse function theorem](../../../../../../inverse-function-theorem.md) therefore makes $r(UV)$ smooth across that surface, and the coefficient of $dU\,dV$ tends to $-16M^2/e$. Thus the [Schwarzschild event horizon](../../../../../../schwarzschild-event-horizon.md) is a coordinate singularity of the original chart, while this [Lorentzian metric](../../../../../../lorentzian-metric.md) remains regular there.

Extend the [Kruskal–Szekeres coordinates](../../../../../../kruskal-szekeres-coordinates.md) to all real $U,V$ with $UV<1$. The signs give two exterior regions, $U<0<V$ and $V<0<U$, a future [black hole](../../../../../../black-hole.md) region $U,V>0$, and a past [white hole](../../../../../../white-hole.md) region $U,V<0$. The [event horizons](../../../../../../event-horizon.md) are $U=0$ or $V=0$, intersecting at the [bifurcation surface](../../../../../../bifurcation-surface.md). The boundary $UV=1$ has $r=0$ and is a genuine [Schwarzschild singularity](../../../../../../schwarzschild-singularity.md), as the [Kretschmann scalar](../../../../../../kretschmann-scalar.md) $48M^2/r^6$ diverges there.

Finally, $T=(V+U)/2$ and $X=(V-U)/2$ give $UV=T^2-X^2$ and a radial metric proportional to $-dT^2+dX^2$. Hence radial [null geodesics](../../../../../../null-geodesic.md) have slopes $\pm1$, the [event horizons](../../../../../../event-horizon.md) are $T=\pm X$, and the singular boundaries are $T^2-X^2=1$. **This constructs the maximal Kruskal extension**; a [black hole](../../../../../../black-hole.md) produced by collapse need not contain the second exterior or the [white hole](../../../../../../white-hole.md) of that eternal extension.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
