<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the once-per-bond Hamiltonian convention of part (a). Let each sublattice [magnetization](../../../../magnetization.md) be its [magnetic moment](../../../../magnetic-dipole-moment.md) _per total physical volume_, so the density of B-sublattice [spins](../../../../spin.md) is $1/(2a^3)$. Writing their moments as $\boldsymbol\mu=g\mu_B\mathbf S$ fixes

$$
\langle\mathbf S_B\rangle=\frac{2a^3}{g\mu_B}\mathbf M_B.
$$

The exchange [energy](../../../../energy-split.md) of one A [spin](../../../../spin.md) is $6J_1\mathbf S_A\cdot\langle\mathbf S_B\rangle=-\boldsymbol\mu_A\cdot\mathbf B_{\rm mf}$, giving

$$
\boxed{\mathbf B_{\rm mf}=-\lambda\mathbf M_B,\qquad
\lambda=\frac{12J_1a^3}{(g\mu_B)^2}>0.}
$$

A convention using $2J_1$ per bond would double this coefficient; defining [magnetization](../../../../magnetization.md) per sublattice volume instead changes its normalization. The definitions above make the total [magnetization](../../../../magnetization.md) $\mathbf M=\mathbf M_A+\mathbf M_B$.

For equal fixed sublattice magnitudes $M_0$, put $\mathbf M_A=M_0(\sin\theta,0,\cos\theta)$ and $\mathbf M_B=M_0(\sin\theta,0,-\cos\theta)$, with the external field along $+x$. The effective A-site field is $(B_\perp-\lambda M_0\sin\theta,0,\lambda M_0\cos\theta)$. Its alignment with $\mathbf M_A$ requires $B_\perp=2\lambda M_0\sin\theta$, so

$$
\boxed{\theta=\arcsin\frac{B_\perp}{2\lambda M_0}\simeq\frac{B_\perp}{2\lambda M_0},\quad
M_\perp=2M_0\sin\theta=\frac{B_\perp}\lambda,\quad
\chi_\perp=\frac{M_\perp}{H_\perp}=\frac{\mu_0}\lambda.}
$$

The last equality uses the externally imposed vacuum field $B_\perp=\mu_0H_\perp$ and neglects demagnetizing corrections. Canting costs exchange [energy](../../../../energy-split.md) but need not change the magnitude of either sublattice moment. The result holds before saturation and assumes the ordered axis is maintained when defining a transverse response.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
