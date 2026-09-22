<h1 id="38d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The linearized kinematic condition at the undisturbed surface is

$$
\partial_t\eta=\partial_z\phi\big|_{z=0}.
$$

For the given complex amplitudes this says

$$
-i\omega A=kB,
\qquad
\boxed{B=-\frac{i\omega}{k}A}.
$$

The velocity is $u=(\phi_x,0,\phi_z)$. Its nonzero complex strain amplitudes are

$$
e_{xx}=-k^2Be^{kz},\qquad
e_{zz}=k^2Be^{kz},\qquad
e_{xz}=e_{zx}=ik^2Be^{kz}.
$$

Using the stated rule for period averages,

$$
\langle e:e\rangle=2k^4|B|^2e^{2kz}.
$$

Thus the mean dissipation per unit horizontal area is

$$
\mathcal D
=2\mu\int_{-\infty}^0\langle e:e\rangle\,dz
=2\mu k^3|B|^2
=2\mu k\omega^2|A|^2
=\boxed{2\mu gk^2|A|^2}.
$$

The mean energy $E=\rho g|A|^2/2$ consequently obeys $dE/dt=-\mathcal D$. Writing $\nu=\mu/\rho$ gives the [viscous decay of a deep-water gravity wave](../../../../../../viscous-decay-of-a-deep-water-gravity-wave.md):

$$
\boxed{\frac{d|A|}{dt}=-2\nu k^2|A|},
\qquad
\boxed{|A(t)|=|A(0)|e^{-2\nu k^2t}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38D](../../38d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
