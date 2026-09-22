<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Potential-vorticity inversion](../../../../../../potential-vorticity-inversion.md) is the diagnostic recovery of the balanced flow from the instantaneous PV distribution, together with appropriate boundary or far-field data. In the unbounded constant-$N$ case the mathematical problem is the [Poisson equation](../../../../../../poisson-equation.md)

$$
\boxed{\nabla_*^2\psi=Q-f\quad\text{in }\mathbb R^3,\qquad\psi\longrightarrow0\quad\text{as }|\mathbf X|\longrightarrow\infty.}
$$

Require a regular solution, with interface continuity in a piecewise-smooth case. For a compactly supported bounded anomaly, the unique decaying solution is the Newtonian-potential integral

$$
\boxed{\psi(\mathbf X)=-\frac1{4\pi}\int_{\mathbb R^3}\frac{Q(\mathbf X')-f}{|\mathbf X-\mathbf X'|}\,d^3X'.}
$$

The sign follows from $\nabla_*^2[-1/(4\pi r)]=\delta_0$. A nonzero total anomaly gives a $1/r$ far-field [streamfunction](../../../../../../stream-function.md), which is allowed by the stated decay condition. The measure is in stretched coordinates; converting to physical coordinates introduces their volume Jacobian.

Two regular solutions with these data differ by a [harmonic function](../../../../../../harmonic-function.md) tending to zero, which must vanish by the maximum principle. This also excludes imposed uniform currents or shear fields encoded by nondecaying harmonic additions and fixes the irrelevant additive [pressure](../../../../../../pressure.md) gauge. Once $\psi$ is found, $\mathbf u_g=(-\psi_y,\psi_x)$, $p'=f\psi$ and $b=f\psi_z$ follow. The smaller vertical and ageostrophic [velocities](../../../../../../velocity.md) require the next-order balance equations.

PV is not by itself an inversion variable for arbitrary unbalanced fluid motion: the [quasi-geostrophic approximation](../../../../../../quasi-geostrophic-approximation.md) supplies the diagnostic geostrophic and hydrostatic relations, filtering the independent inertia-gravity-wave motions. In bounded domains, boundary [buoyancy](../../../../../../buoyancy.md) or equivalent [pressure](../../../../../../pressure.md) data are additional indispensable inputs.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
