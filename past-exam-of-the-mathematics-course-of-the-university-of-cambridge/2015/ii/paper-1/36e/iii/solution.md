<h1 id="36e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For constant viscosity, differentiating $\sigma=-pI+\mu(\nabla u+\nabla u^T)$ gives $\nabla\cdot\sigma=-\nabla p+\mu\nabla^2u$, since $\nabla\cdot u=0$. This is zero by the body-force-free [Stokes equations](../../../../../../stokes-equation.md).

Apply the [divergence theorem](../../../../../../divergence-theorem.md) to the annular fluid. Its outer normal is $+n_R$, but its inner normal is minus the sphere's outward normal. Therefore $0=\int_{S_R}\sigma n_RdS-\int_{S_a}\sigma n_adS$. The second integral is the hydrodynamic force on the inner sphere, $-F$, because that sphere exerts $F$ on the fluid. Thus again **$G=-F$**, without differentiating the far field. Local momentum conservation carries the same total force through every enclosing surface.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [36E](../../36e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
