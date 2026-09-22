<h1 id="10a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\rho=a/\sqrt3$ be the distance from the origin to each fixed charge, and denote their position vectors by $\mathbf R_j$. For a small planar displacement $\mathbf r$, the [Taylor expansion](../../../../../../../taylor-expansion.md)

$$
\frac1{|\mathbf R_j-\mathbf r|}=\frac1\rho+\frac{\mathbf R_j\cdot\mathbf r}{\rho^3}+\frac{3(\mathbf R_j\cdot\mathbf r)^2-\rho^2|\mathbf r|^2}{2\rho^5}+O(|\mathbf r|^3)
$$

can be summed using the threefold [symmetry](../../../../../../../symmetry-physics.md) relations

$$
\sum_j\mathbf R_j=0,
\qquad
\sum_j\mathbf R_j\mathbf R_j^{\mathsf T}=\frac{3\rho^2}{2}I.
$$

The [electric potential](../../../../../../../electric-potential.md) due to the fixed charges is consequently

$$
\Phi(\mathbf r)=\frac{q}{4\pi\epsilon_0}\left(\frac3\rho+\frac{3|\mathbf r|^2}{4\rho^3}+O(|\mathbf r|^3)\right).
$$

The moving charge has [electrostatic potential energy of point charges](../../../../../../../electrostatic-potential-energy-of-point-charges.md) $U=q\Phi$. Because the quadratic coefficient is positive, the origin is a strict [local minimum](../../../../../../../local-minimum.md) of $U$, and the equilibrium is stable.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [10A](../../../10a.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
