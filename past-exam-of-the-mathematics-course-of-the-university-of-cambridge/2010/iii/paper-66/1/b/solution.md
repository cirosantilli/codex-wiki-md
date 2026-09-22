<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathbf F$ denote the applied [force](../../../../../../force.md), and take the normal $\mathbf n_S$ outward from the solid. At leading order the [Stokes drag law](../../../../../../stokes-s-law.md) and the [torque](../../../../../../torque.md) on a [rotating sphere in Stokes flow](../../../../../../rotating-sphere-in-stokes-flow.md) give

$$
\boxed{\mathbf U_0=\frac{\mathbf F}{6\pi\mu a},\qquad\boldsymbol\Omega_0=\mathbf0.}
$$

The exact [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) and the exact resultant-load conditions are

$$
\begin{gathered}
\mathbf u(\mathbf x)=\mathbf U+\boldsymbol\Omega\times\mathbf x\quad(\mathbf x\in S),\qquad\mathbf u\to\mathbf0\quad(r\to\infty),\\
\int_S\boldsymbol\sigma\mathbf n_S\,dS=-\mathbf F,\qquad
\int_S\mathbf x\times(\boldsymbol\sigma\mathbf n_S)\,dS=\mathbf0.
\end{gathered}
$$

The [stress](../../../../../../stress.md) condition specifies the total [force](../../../../../../force.md) and [torque](../../../../../../torque.md), not a pointwise prescribed [traction](../../../../../../traction.md).

For the [boundary perturbation of a nearly spherical particle](../../../../../../boundary-perturbation-of-a-nearly-spherical-particle.md), evaluate the no-slip condition at $\mathbf x=(a+\varepsilon f)\mathbf n$. Taylor expansion gives

$$
\mathbf u_0(a\mathbf n)+\varepsilon\left[\mathbf u_1(a\mathbf n)+f\partial_r\mathbf u_0(a\mathbf n)\right]
=\mathbf U_0+\varepsilon\left[\mathbf U_1+\boldsymbol\Omega_1\times(a\mathbf n)\right]+O(\varepsilon^2).
$$

There is no $f\boldsymbol\Omega_0\times\mathbf n$ term because $\boldsymbol\Omega_0=0$. Therefore

$$
\boxed{\mathbf u_1=\mathbf U_1+\boldsymbol\Omega_1\times\mathbf x-f\partial_r\mathbf u_0\quad(r=a).}
$$

To expand the integral conditions correctly, use [surface independence of Stokes force and torque integrals](../../../../../../surface-independence-of-stokes-force-and-torque-integrals.md). The [Stokes equation](../../../../../../stokes-equation.md) implies $\nabla\cdot\boldsymbol\sigma=0$, and symmetry of the [stress tensor](../../../../../../cauchy-stress-tensor.md) implies that the angular-momentum flux is divergence-free as well. Evaluate the exact [force](../../../../../../force.md) and [torque](../../../../../../torque.md) on a fixed sphere of radius $R$ enclosing the perturbed particle. There are then no geometric terms: the $O(\varepsilon)$ integrals of $\boldsymbol\sigma_1$ on that fixed sphere vanish because the external [force](../../../../../../force.md) and [torque](../../../../../../torque.md) have no $O(\varepsilon)$ corrections. Each perturbation field solves the homogeneous exterior Stokes equations, so the [divergence theorem](../../../../../../divergence-theorem.md) transfers those integrals back to $r=a$. Hence

$$
\boxed{\int_{r=a}\boldsymbol\sigma_1\mathbf n\,dS=\mathbf0,\qquad
\int_{r=a}\mathbf x\times(\boldsymbol\sigma_1\mathbf n)\,dS=\mathbf0.}
$$

If the integrals are expanded directly on the displaced surface, terms involving the displaced evaluation of $\boldsymbol\sigma_0$, the changed normal and the changed area do appear individually. Their sum vanishes by the same surface-independence identity. Thus their absence in the final equations is a cancellation, not permission to omit geometric terms independently.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
