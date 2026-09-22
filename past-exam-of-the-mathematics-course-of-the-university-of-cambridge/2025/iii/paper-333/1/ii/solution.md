<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With no $y$ dependence, the [linearized shallow water equations](../../../../../../linearized-shallow-water-equations.md) are

$$
u_t-fv=-g\eta_x,
\qquad v_t+fu=0,
\qquad \eta_t+H_0u_x=0.
$$

Their conserved linear potential-vorticity anomaly is

$$
v_x-\frac f{H_0}\eta
=2v_0\delta(x),
$$

because the initial velocity jump has derivative $2v_0\delta(x)$. The final steady state is in [geostrophic balance](../../../../../../geostrophic-balance.md), so $u=0$ and $fv=g\eta_x$. Hence

$$
\boxed{
\left(\frac{d^2}{dx^2}-\frac1{R_d^2}\right)\eta
=\frac{2fv_0}{g}\delta(x),
\qquad
R_d=\frac{\sqrt{gH_0}}{|f|}.}
$$

Taking $f>0$ for definiteness and requiring decay at infinity gives

$$
\boxed{
\eta=-v_0\sqrt{\frac{H_0}{g}}e^{-|x|/R_d},
\qquad
u=0,
\qquad
v=v_0\operatorname{sgn}(x)e^{-|x|/R_d}.}
$$

Initially, the potential energy is zero and, per unit length in $y$,

$$
E_{
m early}=\frac12\rho H_0v_0^2(2L)
=\rho H_0v_0^2L.
$$

For $L\gg R_d$, the final kinetic and potential energies are equal:

$$
E_{K,\rm steady}
=\frac12\rho H_0v_0^2R_d,
\qquad
E_{P,\rm steady}
=\frac12\rho g\int\eta^2dx
=\frac12\rho H_0v_0^2R_d.
$$

Thus $E_{
m steady}=\rho H_0v_0^2R_d$. During [geostrophic adjustment](../../../../../../geostrophic-adjustment.md), [inertia-gravity waves](../../../../../../inertia-gravity-wave.md) carry the excess energy out of $|x|<L$; energy in that finite region is therefore not conserved. Their long-wave speed is $c=\sqrt{gH_0}$, so the adjustment of the stated region takes

$$
\boxed{t_{\rm adj}=O\left(\frac{L}{\sqrt{gH_0}}\right)
=O\left(\frac{L}{|f|R_d}\right).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
