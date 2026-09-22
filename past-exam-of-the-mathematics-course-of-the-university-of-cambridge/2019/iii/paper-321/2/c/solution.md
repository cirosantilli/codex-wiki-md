<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Initially every particle has $A=B=0$, so its [Jacobi energy in a shearing sheet](../../../../../../jacobi-energy-in-a-shearing-sheet.md) is $-3\Omega_0^2x_0^2/8$. During an [inelastic collision](../../../../../../inelastic-collision.md), positions are fixed at the instant of impact, while [momentum conservation](../../../../../../momentum-conservation.md) preserves the sum of the tangential velocities. Hence the sum of $p_y=\dot y+2\Omega_0x$, and therefore the sum of the [epicyclic guiding center](../../../../../../epicyclic-guiding-center.md) positions $x_0=2p_y/\Omega_0$, is unchanged. Between collisions, these quantities are individually conserved.

The collision dissipates kinetic energy without changing the instantaneous tidal potential. Consequently the total [Jacobi energy in a shearing sheet](../../../../../../jacobi-energy-in-a-shearing-sheet.md) decreases. At any later time, writing $x_{0j}$ for the particles' current [epicyclic guiding center](../../../../../../epicyclic-guiding-center.md) positions gives

$$
E=E_{\rm osc}-\frac38\Omega_0^2\sum_jx_{0j}^2,\qquad
E_{\rm osc}=\frac12\Omega_0^2\sum_j(|A_j|^2+|B_j|^2)\geq0.
$$

If $D\geq0$ is the accumulated energy dissipated in the [inelastic collisions](../../../../../../inelastic-collision.md), comparison with the initial circular orbits gives

$$
\boxed{\sum_jx_{0j}^2
=\sum_jx_{0j,\rm initial}^2+\frac{8}{3\Omega_0^2}(D+E_{\rm osc})}.
$$

Thus the mean guiding-center position stays fixed, while its variance grows. The initial ensemble has no preference for positive or negative $x$, and the local equations and collision law preserve the symmetry $(x,y,z)\mapsto(-x,-y,z)$. The spreading is therefore symmetric in the ensemble average: [angular momentum transport](../../../../../../angular-momentum-transport.md) moves some particles inward and others outward. A particular finite random realization need not be exactly symmetric. This is the microscopic energy argument for [dissipative spreading of a planetary ring](../../../../../../dissipative-spreading-of-a-planetary-ring.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
