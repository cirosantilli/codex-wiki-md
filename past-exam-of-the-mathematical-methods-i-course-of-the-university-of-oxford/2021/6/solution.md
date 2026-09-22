<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the [Characteristic polynomials of AB and BA](../../../characteristic-polynomials-of-ab-and-ba.md), which also account for the zero [eigenvalue](../../../eigenvalue.md) and [algebraic multiplicities](../../../algebraic-multiplicity.md). The block [determinant](../../../determinant.md)

$$
\det\begin{pmatrix}I&tA\\-B&I\end{pmatrix}
$$

equals both $\det(I+tAB)$ and $\det(I+tBA)$, by taking the two [Schur complements](../../../schur-complement.md). For $\lambda\ne0$, set $t=-1/\lambda$ and multiply by $\lambda^n$ to obtain

$$
\boxed{\det(\lambda I-AB)=\det(\lambda I-BA).}
$$

Both sides are [polynomials](../../../polynomial-split.md), so agreement away from zero proves equality there as well. Their roots, with multiplicity, are the same. The familiar eigenvector argument $ABv=\mu v\Rightarrow BA(Bv)=\mu Bv$ works directly only when $\mu\ne0$, because then $Bv\ne0$; it should not be used to discard the zero case.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2021](../../2021-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
