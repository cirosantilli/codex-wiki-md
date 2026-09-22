<h1 id="section-a/a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

The [principal moments of inertia](../../../../../principal-moment-of-inertia.md) are the [eigenvalues](../../../../../eigenvalue.md) of the symmetric [inertia tensor](../../../../../inertia-tensor.md). In units of $\mathrm{kg\,m^2}$, its characteristic [determinant](../../../../../determinant.md) is

$$
\det(\mathsf I-\lambda\mathsf 1)
=(1-\lambda)[(2-\lambda)^2-1]
=(1-\lambda)^2(3-\lambda).
$$

Therefore the requested algebraic answer is

$$
\boxed{I_1=3\ \mathrm{kg\,m^2},\qquad I_2=I_3=1\ \mathrm{kg\,m^2}.}
$$

An [orthonormal basis](../../../../../orthonormal-basis.md) of [principal axes](../../../../../principal-axis.md) is $(1,1,0)/\sqrt2$, $(1,-1,0)/\sqrt2$, and $(0,0,1)$; the last two span the degenerate [eigenspace](../../../../../eigenspace.md) and may be replaced by any [orthonormal basis](../../../../../orthonormal-basis.md) of it.

There is a physical inconsistency in calling the supplied matrix a rigid body's [inertia tensor](../../../../../inertia-tensor.md). The [moment-of-inertia triangle inequalities](../../../../../moment-of-inertia-triangle-inequalities.md) require each principal moment to be no greater than the sum of the other two. Here $3>1+1$. In principal coordinates, $I_2+I_3-I_1=2\int x_1^2\,dm$ cannot be negative for a nonnegative [mass distribution](../../../../../mass-distribution.md). Thus the eigenvalue calculation is well defined, but no ordinary rigid mass distribution realizes this tensor. The [positive second-moment matrix test for an inertia tensor](../../../../../positive-second-moment-matrix-test-for-an-inertia-tensor.md) makes the same obstruction explicit.

## ↑ Ancestors (14)

1. [A2](../a2.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
