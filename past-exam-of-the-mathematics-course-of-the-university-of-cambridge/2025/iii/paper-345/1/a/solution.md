<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the velocity perturbation be $(u,w)$, pressure perturbation be $p$, and density perturbation be $\rho'$ about the hydrostatic background $\hat\rho(z)$. The linearized inviscid [Boussinesq approximation](../../../../../../boussinesq-approximation.md) gives

$$
u_x+w_z=0,\qquad
\rho'_t+w\hat\rho_z=0,\qquad
u_t=-p_x/\rho_0,\qquad
w_t=-p_z/\rho_0-g\rho'/\rho_0.
$$

Stable stratification means $\hat\rho_z<0$, and the [buoyancy frequency](../../../../../../buoyancy-frequency.md) is

$$
\boxed{N^2=-\frac g{\rho_0}\frac{d\hat\rho}{dz}>0}.
$$

Differentiate the momentum equations to eliminate $p$, use incompressibility, and then use the density equation to eliminate $\rho'$. This yields

$$
\boxed{\left[\left(\partial_x^2+\partial_z^2\right)\partial_t^2+N^2\partial_x^2\right]w=0}.
$$

For $w\propto e^{i(kx+mz-\omega t)}$, the [internal gravity wave](../../../../../../internal-wave.md) dispersion relation is $\omega^2=N^2k^2/(k^2+m^2)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
