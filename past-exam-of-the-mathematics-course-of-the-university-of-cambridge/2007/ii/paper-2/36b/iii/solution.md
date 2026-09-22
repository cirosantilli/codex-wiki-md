<h1 id="36b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $x$ increase away from the tip along the wall and $y$ point normally into the fluid. Put $u=u_x$, $v=u_y$ for velocity components and $U(x)=-A/x^2$ for the outer tangential velocity. The local Cartesian momentum and pressure equations are

$$
u\partial_xu+v\partial_yu=-\rho^{-1}p_x+\nu\partial_y^2u=UU'+\nu\partial_y^2u,
\qquad p_y=0.
$$

For a two-dimensional flat layer the usual [continuity equation](../../../../../../continuity-equation.md) is $\partial_xu+\partial_yv=0$. For this axisymmetric cone, however, the circumference is proportional to $x$, so its leading [continuity equation](../../../../../../continuity-equation.md) is

$$
\boxed{\partial_xu+\frac ux+\partial_yv=0,\quad\text{or}\quad\partial_x(xu)+\partial_y(xv)=0.}
$$

The circumference term is of the same order as $\partial_xu$ and cannot be omitted when deriving the cone's similarity equation. Conditions at the stationary wall are $u=v=0$; at the layer edge $u\to U$.

Balance $U^2/x\sim\nu |U|/\delta^2$. With $|U|=A/x^2$ this gives

$$
\boxed{\delta(x)=\sqrt{\frac\nu A}\,x^{3/2},\qquad\frac\delta x=\operatorname{Re}(x)^{-1/2}\ll1.}
$$

The choice of multiplicative constant fixes the normalization of the [similarity variable](../../../../../../similarity-variable.md). To enforce axisymmetric continuity set $xu=\Psi_y$, $xv=-\Psi_x$, with

$$
\Psi=-\sqrt{A\nu}\,x^{1/2}F(\eta),\qquad\eta=\frac y\delta.
$$

Then

$$
u=-\frac A{x^2}F'(\eta),\qquad
v=\sqrt{A\nu}\,x^{-3/2}\left(\frac12F-\frac32\eta F'\right).
$$

Differentiation gives $u\partial_xu+v\partial_yu=-(A^2/x^5)[2F'^2+FF''/2]$, whereas $UU'=-2A^2/x^5$ and $\nu u_{yy}=-A^2F'''/x^5$. Consequently the [conical sink boundary layer](../../../../../../conical-sink-boundary-layer.md) satisfies

$$
\boxed{F'''-\frac12FF''+2(1-F'^2)=0,\qquad
F(0)=0,\quad F'(0)=0,\quad F'(\infty)=1.}
$$

The first condition is no penetration, the second no slip, and the last matches the inward core flow. If one instead makes a strictly planar approximation and omits the circumference term, the [streamfunction](../../../../../../stream-function.md) is $-\sqrt{A\nu}x^{-1/2}F$ and the equation becomes $F'''+FF''/2+2(1-F'^2)=0$. The thickness exponent is the same, but that planar equation is not the axisymmetric cone equation.

Across a cap near $R=x$, the inward flux in a layer truncated at $y=Y$ is, to leading order,

$$
Q_{\mathrm{layer}}(R,Y)=2\pi R\sin\alpha\int_0^Y(-u)\,dy
=2\pi A\sin\alpha\frac{\delta(R)}R F(Y/\delta).
$$

To match to the core, use the finite displacement-flux deficit rather than integrate the uniform outer flow to infinite $Y$. If $I=\int_0^\infty(1-F')d\eta=\lim_{\eta\to\infty}(\eta-F)$, then

$$
\Delta Q=2\pi A\sin\alpha\frac{\delta(R)}R I
=2\pi\sin\alpha\,I\sqrt{A\nu}\,R^{1/2}.
$$

Conservation of the fixed total extraction rate requires an extra core flux of this order. Dividing by cap area, proportional to $R^2$, proves

$$
\boxed{u_{R,\mathrm{outer}}=-\frac A{R^2}+O(\sqrt{A\nu}\,R^{-3/2}).}
$$

The correction is a relative $O(\sqrt{\nu R/A})$ contribution. Its angular structure requires outer matching; the requested radial power follows from the displacement flux alone. Its cap-average direction increases the inward core speed to compensate for the wall deficit.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [36B](../../36b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
