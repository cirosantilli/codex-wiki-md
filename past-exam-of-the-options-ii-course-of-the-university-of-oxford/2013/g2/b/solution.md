<h1 id="g2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The autonomous [Lagrangian](../../../../lagrangian.md) has the [Beltrami identity](../../../../beltrami-identity.md)

$$
\sum_i\dot q_iL_{\dot q_i}-L=\text{constant}.
$$

Here $L$ is homogeneous of degree two in the velocities, so $\dot uL_{\dot u}+\dot vL_{\dot v}=2L$. Thus **$L$ itself is constant**, say $C\geq0$.

For $C>0$, put $\ell=\sqrt L$. Its Euler-Lagrange expression along the curve is

$$
\frac{d}{dt}\ell_{\dot q_i}-\ell_{q_i}
=\frac1{2\sqrt L}\left(\frac{d}{dt}L_{\dot q_i}-L_{q_i}\right)
-\frac{\dot L}{4L^{3/2}}L_{\dot q_i}=0.
$$

The first term vanishes by stationarity for $L$, and the second by constancy of $L$. Thus the same path is stationary for its length functional $\int\sqrt L\,dt$.

On a regular segment described as a graph $v=v(u)$, reparametrize by $u$. Since $\dot v=v_u\dot u$,

$$
\sqrt L\,dt=\sqrt{E+2Fv_u+Gv_u^2}\,|du|.
$$

Choose the orientation with increasing $u$; reversing it does not change stationarity. Invariance of length under regular reparametrization therefore gives

$$
\boxed{\delta\int\sqrt{E+2Fv_u+Gv_u^2}\,du=0.}
$$

This is the principle of [length extremals from a constant quadratic energy](../../../../length-extremals-from-a-constant-quadratic-energy.md). The stated nonnegativity also permits the degenerate case $C=0$. Then the length is zero, its absolute minimum since the integrand is nonnegative, so it is an extremal in the minimizing sense. The differentiated square-root Euler-Lagrange equation above is only used where $L>0$; it would not be legitimate to divide by $\sqrt L$ on a null curve. For a genuine surface metric and a regular nonconstant path, $C>0$ automatically.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [G2](../../g2.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
