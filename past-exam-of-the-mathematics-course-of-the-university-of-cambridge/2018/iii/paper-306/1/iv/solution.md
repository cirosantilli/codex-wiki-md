<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $q=\sigma/L$, with $L>0$, and let $Z=X^1+iX^2$. Direct differentiation gives $\ddot Z=Z''=-Z/L^2$, while the time coordinate also satisfies the [wave equation](../../../../../../wave-equation-split.md). Using the [Minkowski metric](../../../../../../minkowski-metric.md),

$$
\dot X\cdot X'=0,\qquad \dot X^2=-\cos^2q,\qquad X'^2=\cos^2q.
$$

Thus both [Virasoro constraints](../../../../../../virasoro-constraint.md) hold, and the [induced worldsheet metric](../../../../../../induced-worldsheet-metric.md) is $g_{\mu\nu}=\cos^2q\,\operatorname{diag}(-1,1)$. The configuration solves the [Nambu–Goto action](../../../../../../nambu-goto-action.md) equations in its interior.

Place the fixed end at $\sigma=0$. The first free endpoint has $Z'=e^{it/L}\cos q=0$ at $q=\pi/2$. For the usual single unfolded [rotating Nambu–Goto string](../../../../../../rotating-nambu-goto-string.md),

$$
\boxed{0\leq\sigma\leq\frac{\pi L}{2},\qquad
\ell_{\mathrm{proper}}=\int_0^{\pi L/2}|Z'|\,d\sigma=L.}
$$

This parameter interval need not equal the earlier interval $[0,\pi]$, since that interval was a coordinate convention. The [proper length](../../../../../../proper-length.md) is measured on a constant-$X^0$ slice; the local motion is perpendicular to the string, so there is no longitudinal [Lorentz contraction](../../../../../../length-contraction.md).

All points have the same phase $t/L$, hence the segment rotates rigidly with [angular velocity](../../../../../../angular-velocity.md) $\Omega=1/L$. At radius $r=L\sin q$, its [speed](../../../../../../speed.md) is $v=r/L$. Therefore **the free tip moves at the [speed of light](../../../../../../speed-of-light.md)**. This is consistent with its [Neumann boundary condition](../../../../../../neumann-boundary-condition.md): $X'=0$ and the [Virasoro constraints](../../../../../../virasoro-constraint.md) imply $\dot X^2=0$ at the free tip. The null endpoint is a boundary limit, not a nondegenerate interior point.

In this [conformal gauge](../../../../../../conformal-gauge.md), $P_m=T\dot X_m$, so the [energy density](../../../../../../energy-density.md) per $\sigma$ is $-P_0=T$. Equivalently, the [energy density](../../../../../../energy-density.md) per [proper length](../../../../../../proper-length.md) is $T/\sqrt{1-r^2/L^2}$. Thus

$$
E=T\int_0^{\pi L/2}d\sigma=\frac{\pi TL}{2},\qquad
E_{\mathrm{rest}}=TL,
$$

and the [rotational kinetic energy](../../../../../../rotational-kinetic-energy.md) is

$$
\boxed{E_{\mathrm{rot}}=\left(\frac\pi2-1\right)TL
=\left(1-\frac2\pi\right)E.}
$$

The [angular momentum](../../../../../../angular-momentum.md) about the fixed point is

$$
J=\int d\sigma\,(X^1P_2-X^2P_1)
=TL\int_0^{\pi L/2}\sin^2(\sigma/L)\,d\sigma
=\frac{\pi TL^2}{4}.
$$

Therefore the [Regge trajectory](../../../../../../regge-trajectory.md) is

$$
\boxed{E=\frac{\pi TL}{2},\qquad J=\frac{E^2}{\pi T},\qquad\beta=\frac1{\pi T}.}
$$

The endpoint conditions alone also admit folded extensions with parameter length $(n+\tfrac12)\pi L$, $n\geq0$. Their [proper length](../../../../../../proper-length.md), [energy](../../../../../../energy.md) and [angular momentum](../../../../../../angular-momentum.md) are $(2n+1)$ times the values above, and $\beta=1/[(2n+1)\pi T]$. The displayed answer uses the implicit unfolded-segment convention.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
