<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Substitute the given [Stokes streamfunction](../../../../stokes-streamfunction.md) representation into the [divergence](../../../../divergence.md) in [spherical coordinates](../../../../spherical-coordinate-system.md). The mixed derivatives cancel:

$$
\begin{aligned}
\nabla\cdot\mathbf u
&=\frac1{r^2}\partial_r\left(\frac{\Psi_\theta}{\sin\theta}\right)
+\frac1{r\sin\theta}\partial_\theta\left(-\frac{\Psi_r}{r}\right)\\
&=\frac{\Psi_{r\theta}-\Psi_{\theta r}}{r^2\sin\theta}=0.
\end{aligned}
$$

Thus [incompressibility](../../../../incompressible-flow.md) is automatic for a smooth [Stokes streamfunction](../../../../stokes-streamfunction.md). Since this is an [axisymmetric flow](../../../../axisymmetric-flow.md) with no azimuthal [velocity](../../../../velocity.md), the only possibly nonzero component of its [vorticity](../../../../vorticity-split.md) is

$$
\begin{aligned}
(\nabla\times\mathbf u)_\varphi
&=\frac1r\left[\partial_r\left(-\frac{\Psi_r}{\sin\theta}\right)
-\partial_\theta\left(\frac{\Psi_\theta}{r^2\sin\theta}\right)\right]\\
&=-\frac1{r^3\sin\theta}\left[r^2\Psi_{rr}+\sin\theta\,\partial_\theta\left(\frac{\Psi_\theta}{\sin\theta}\right)\right].
\end{aligned}
$$

Define the differential operator in the [Stokes streamfunction equation for irrotational flow](../../../../stokes-streamfunction-equation-for-irrotational-flow.md)

$$
\mathcal L\Psi=r^2\Psi_{rr}+\Psi_{\theta\theta}-\cot\theta\,\Psi_\theta.
$$

The stated equation is $\mathcal L\Psi=0$, and therefore

$$
\boxed{\nabla\cdot\mathbf u=0,\qquad\nabla\times\mathbf u=\mathbf0.}
$$

The [irrotational flow](../../../../irrotational-flow.md) has a [velocity potential](../../../../velocity-potential.md) locally, and globally on a regular [simply connected domain](../../../../simply-connected-domain.md). Regularity of the physical [velocity field](../../../../velocity-field.md) supplies the limiting interpretation on the polar axis, where the coordinate expressions contain $\sin\theta$ in the denominator.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
