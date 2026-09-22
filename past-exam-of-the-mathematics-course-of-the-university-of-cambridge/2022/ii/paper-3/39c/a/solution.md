<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the medium varies on scales much longer than the wavelength and period, so the leading-order [WKB method](../../../../../../wkb-method.md) gives the local [eikonal equation](../../../../../../eikonal-equation.md). For the phase $\theta$ in the stated ansatz, define

$$
\mathbf k=\nabla\theta,
\qquad
\omega=-\partial_t\theta.
$$

The local [dispersion relation](../../../../../../dispersion-relation.md) becomes the Hamilton--Jacobi equation

$$
-\partial_t\theta
=\Omega(\nabla\theta;\mathbf x,t).
$$

Differentiating it with respect to $x_i$, using equality of mixed derivatives, and choosing a ray whose velocity is

$$
\dot x_i=\frac{\partial\Omega}{\partial k_i}
$$

gives

$$
\dot k_i
=\partial_tk_i+\dot x_j\partial_{x_j}k_i
=-\frac{\partial\Omega}{\partial x_i}.
$$

Here the dot, or $d/dt$, is the [total derivative along a ray](../../../../../../total-derivative-along-a-ray.md),

$$
\frac d{dt}
=\frac{\partial}{\partial t}
+\dot{\mathbf x}\cdot\nabla_{\mathbf x},
$$

and not merely a partial time derivative at fixed position.

Finally, differentiate $\omega=\Omega(\mathbf k;\mathbf x,t)$ along the same trajectory:

$$
\frac{d\omega}{dt}
=\frac{\partial\Omega}{\partial t}
+\frac{\partial\Omega}{\partial x_i}\dot x_i
+\frac{\partial\Omega}{\partial k_i}\dot k_i
=\frac{\partial\Omega}{\partial t},
$$

because the last two terms cancel. The [Hamiltonian ray-tracing equations](../../../../../../hamiltonian-ray-tracing-equations.md) are therefore

$$
\boxed{
\frac{dx_i}{dt}=\frac{\partial\Omega}{\partial k_i},
\qquad
\frac{dk_i}{dt}=-\frac{\partial\Omega}{\partial x_i},
\qquad
\frac{d\omega}{dt}=\frac{\partial\Omega}{\partial t}
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
