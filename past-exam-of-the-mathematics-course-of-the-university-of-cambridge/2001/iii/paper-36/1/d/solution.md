<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $P(x)$ for the outer [pressure](../../../../../../pressure.md) extrapolated to the wall. The normal balance in the thin [boundary layer](../../../../../../boundary-layer.md) is $p_y=\overline F_y$, giving

$$
p(x,y)=P(x)-\frac{C(x)^2}{4\mu_0}e^{-2y/\delta}.
$$

The spatially varying [magnetic pressure](../../../../../../magnetic-pressure.md) deficit drives a tangential [pressure gradient](../../../../../../pressure-gradient.md). For fixed forcing as $\omega\to\infty$, layer inertia is small compared with [viscous dissipation](../../../../../../viscous-dissipation.md); explicitly the ratio is $U\delta^2/(\nu b)$. The leading tangential balance is

$$
\rho\nu u_{yy}=p_x=-\frac{CC'}{2\mu_0}e^{-2y/\delta}.
$$

The outer gradient $P'$ contributes only at higher inner order. Matching the leading outer shear gives $u_y\to0$, and the physical [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) gives $u(x,0)=0$. Two integrations yield the [magnetic skin-layer streaming slip](../../../../../../magnetic-skin-layer-streaming-slip.md):

$$
\boxed{u(x,y)=U(x)(1-e^{-2y/\delta}),\qquad U(x)=\frac{\delta^2CC'}{8\mu_0\rho\nu}=\frac{\delta^2}{16\mu_0\rho\nu}\frac{d(C^2)}{dx}.}
$$

For the present field amplitude,

$$
\boxed{U(x)=-\frac{\mu_0J^2b^2\delta^2}{4\pi^2\rho\nu}\frac{x}{(x^2+b^2)^3}.}
$$

Using [incompressibility](../../../../../../incompressible-flow.md) and $v(x,0)=0$ also gives

$$
v(x,y)=-U'(x)\left[y-\frac\delta2(1-e^{-2y/\delta})\right].
$$

Hence $v/u=O(\delta/b)$ in the layer, except at symmetry zeros where a componentwise ratio is inappropriate. In the matching region $\delta\ll y\ll b$, $u\sim U$ and $v\sim-yU'$, up to the smaller displacement term $\delta U'/2$.

**The effective outer boundary conditions are tangential slip $u_{\rm bulk}(x,0)=U(x)$ and zero leading normal velocity $v_{\rm bulk}(x,0)=0$.** These describe the bulk flow extrapolated through the unresolved [magnetic skin layer](../../../../../../magnetic-skin-layer.md); the actual wall remains at rest. For $x>0$ the slip is negative, and for $x<0$ it is positive. Fluid converges along the wall toward the wire, turns upward near $x=0$, and returns outward farther above the wall.

The following original [streamline](../../../../../../streamline.md) sketch uses the small-[Reynolds number](../../../../../../reynolds-number.md) bulk [Stokes flow](../../../../../../stokes-flow-split.md) for this slip. It illustrates that circulation without claiming that the unspecified bulk [Reynolds number](../../../../../../reynolds-number.md) fixes a unique complete flow. With $X=x/b$, $Y=y/b$, $Z=X+iY$, a dimensionless [stream function](../../../../../../stream-function.md) is

$$
\Psi=Y\operatorname{Re}\left[\frac1{4(Z+i)^3}-\frac{i}{8(Z+i)^2}\right].
$$

Its factor in brackets is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) in $Y>0$, so $\Psi$ solves the [biharmonic equation](../../../../../../biharmonic-equation.md); its wall derivative is $\Psi_Y(X,0)=-X/(1+X^2)^3$. Thus it satisfies both effective wall conditions and gives an exact creeping-flow illustration of the derived slip.

<a id="1/d/image-bulk-stokes-flow-streamlines-driven-by-magnetic-skin-layer-slip-converging-along-the-wall-and-rising-above-the-wire"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36-streamlines.png)

**[Figure 1](#1/d/image-bulk-stokes-flow-streamlines-driven-by-magnetic-skin-layer-slip-converging-along-the-wall-and-rising-above-the-wire). Bulk Stokes-flow streamlines driven by magnetic skin-layer slip, converging along the wall and rising above the wire**.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
