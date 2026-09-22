<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

For each point $(\Delta\phi_1,e)$, sample $\delta\in[-\Delta\phi_1,\Delta\phi_1]$ and the three conjunction branches

$$
M_{c,k}=\frac{\pi+\delta+2\pi k}{3}.
$$

For every branch, solve [Kepler's equation](../../../../../../kepler-s-equation.md) for the [eccentric anomaly](../../../../../../eccentric-anomaly.md), evaluate $r=a(1-e\cos E)$, and minimize the planet-planetesimal separation over $\delta$ and $k$. Mark the point as encounter-capable when this minimum is below a chosen $R_{\rm enc}$, naturally the [Hill radius](../../../../../../hill-radius.md) for strong scattering. Repeating this calculation on a grid traces the boundary in the $\Delta\phi_1$--$e$ plane.

Direct integrations of the [circular restricted three-body problem](../../../../../../circular-restricted-three-body-problem.md) can then refine the geometric map by allowing the [resonant argument](../../../../../../resonant-argument.md), eccentricity, and conjunction kicks to evolve self-consistently. The integrations distinguish merely orbit-crossing initial data from trajectories that actually enter the encounter region, and reveal chaotic layers near the boundary.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
