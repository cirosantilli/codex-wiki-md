<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the lower variational inequality choose reference conductivity $a_1$ and a trial polarization $q$ that vanishes in phase 1. Let $v_q\in H_0^1(\Omega)$ solve

$$
a_1\Delta v_q+\nabla\cdot q=0.
$$

The [Hashin-Shtrikman conductivity variational principle](../../../../../../hashin-shtrikman-conductivity-variational-principle.md) is

$$
\boxed{
J(u)\ge a_1|\Omega||\lambda|^2
+2\lambda\cdot\int_\Omega q\,dx
+\int_\Omega q\cdot\nabla v_q\,dx
-\int_{\mathrm{phase}\ 2}q\cdot(a-a_1I)^{-1}q\,dx .
}
$$

It holds for every admissible trial $q$; the exact principle takes the supremum of the right side. Writing the last integral only over phase 2 avoids applying an inverse to the zero contrast in the reference phase.

With $D=a_2-a_1>0$, the [isotropic](../../../../../../isotropy.md) phase trial $q=tD\lambda\chi_2$ gives the lower expression

$$
a_1+Dp_2\left[2t-t^2\left(1+\frac{Dp_1}{3a_1}\right)\right].
$$

Here the quadratic is concave, so maximize it at $t=[1+Dp_1/(3a_1)]^{-1}$. The lower member of the [Hashin-Shtrikman conductivity bounds](../../../../../../hashin-shtrikman-bounds-for-conductivity.md) is

$$
\boxed{
a^*\ge a_1+\frac{3a_1(a_2-a_1)p_2}{3a_1+p_1(a_2-a_1)}.
}
$$

Together with part (iii), this gives the required upper and lower interval. All denominators are positive for positive phase conductivities.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
