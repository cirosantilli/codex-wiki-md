<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalize the symmetric $N$-particle [phase-space distribution function](../../../../phase-space-distribution-function.md) $D_N$ to one and write $z_i=(\mathbf x_i,\mathbf v_i)$, $dz_i=d^3x_i\,d^3v_i$. The number-normalized one- and [two-particle distribution functions](../../../../two-particle-distribution-function.md) are

$$
f(z_1,t)=N\int D_N\,dz_2\cdots dz_N,\qquad f_2(z_1,z_2,t)=N(N-1)\int D_N\,dz_3\cdots dz_N.
$$

Thus $\int f\,dz=N$ and $\int f_2(z,z_\star)\,dz_\star=(N-1)f(z)$. These conventions absorb the otherwise explicit factor $N-1$ in the first [BBGKY hierarchy](../../../../bbgky-hierarchy.md) equation.

Separate the [Hamiltonian](../../../../hamiltonian.md) into [kinetic energy](../../../../kinetic-energy.md), external [potential energy](../../../../potential-energy.md), and [pair potential](../../../../pair-potential.md) terms. Their [Hamilton's equations](../../../../hamilton-s-equations.md) give

$$
\dot{\mathbf x}_i=\mathbf v_i,\qquad \dot{\mathbf v}_i=-\nabla U(\mathbf x_i)-\sum_{j\ne i}\nabla_{\mathbf x_i}\phi(|\mathbf x_i-\mathbf x_j|).
$$

The sign follows directly from the stated [Poisson bracket](../../../../poisson-bracket.md): $\dot v_{i\alpha}=\{v_{i\alpha},H\}=-\partial_{x_{i\alpha}}H$. The [Hamiltonian Liouville equation](../../../../hamiltonian-liouville-equation.md) is consequently

$$
\partial_tD_N+\sum_i\left[\mathbf v_i\cdot\nabla_{\mathbf x_i}D_N-\left(\nabla U_i+\sum_{j\ne i}\nabla_{\mathbf x_i}\phi_{ij}\right)\cdot\nabla_{\mathbf v_i}D_N\right]=0.
$$

Integrate over $z_2,\ldots,z_N$ and multiply by $N$. Assume sufficient decay in [velocity space](../../../../velocity-space.md) and either decay or periodic [boundary conditions](../../../../boundary-condition.md) in position, so that [integration by parts](../../../../integration-by-parts.md) removes all transport terms with $i\geq2$. The surviving interaction term is

$$
N\sum_{j=2}^N\int \nabla_{\mathbf x_1}\phi_{1j}\cdot\nabla_{\mathbf v_1}D_N\,dz_2\cdots dz_N
=\int\nabla_{\mathbf x_1}\phi_{12}\cdot\nabla_{\mathbf v_1}f_2\,dz_2,
$$

where indistinguishability makes all $N-1$ terms equal. Relabeling $(z_1,z_2)$ as $(z,z_\star)$ yields the exact result

$$
\boxed{\partial_tf+\mathbf v\cdot\nabla f-\nabla U\cdot\nabla_{\mathbf v}f=\int d^3x_\star\,d^3v_\star\,\nabla_{\mathbf x}\phi(|\mathbf x-\mathbf x_\star|)\cdot\nabla_{\mathbf v}f_2.}
$$

No assumption of [molecular chaos for the Boltzmann equation](../../../../molecular-chaos-for-the-boltzmann-equation.md) has entered: the dependence on the [two-particle distribution function](../../../../two-particle-distribution-function.md) is still exact.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
