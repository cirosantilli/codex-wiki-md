<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A two-index [Cartesian tensor](../../../../cartesian-tensor.md) has components transforming as $T'_{ij}=R_{ik}R_{jl}T_{kl}$ under an orthogonal change of [orthonormal basis](../../../../orthonormal-basis.md). The tensor order here counts indices, rather than the [matrix rank](../../../../matrix-rank.md). Its [scalar, symmetric-traceless and axial tensor decomposition](../../../../scalar-symmetric-traceless-and-axial-tensor-decomposition.md) follows by setting

$$
Y=\frac{T_{kk}}3,\qquad\Omega_{ij}=\frac{T_{ij}-T_{ji}}2,\qquad S_{ij}=\frac{T_{ij}+T_{ji}}2-Y\delta_{ij}.
$$

Then $T_{ij}=Y\delta_{ij}+\Omega_{ij}+S_{ij}$, with $\Omega$ antisymmetric and $S$ symmetric and traceless. There are **three independent antisymmetric components** and **five independent symmetric traceless components**: three off-diagonal entries and two independent diagonal ones in the latter case.

For the symmetric tensor relative to a nonzero [vector](../../../../vector.md) $A$, put $q=A_iA_i>0$, $s=A_iT_{ij}A_j$, and $t=T_{ii}$. The [symmetric tensor decomposition relative to an axis](../../../../symmetric-tensor-decomposition-relative-to-an-axis.md) gives

$$
\boxed{\alpha=\frac12\left(t-\frac sq\right),\qquad\beta=\frac{3s/q-t}{2q},\qquad B_i=\frac{T_{ij}A_j}{q}-\frac{sA_i}{q^2}.}
$$

In particular $A_iB_i=s/q-s/q=0$. Define the [orthogonal projection](../../../../orthogonal-projection.md) $P_{ij}=\delta_{ij}-A_iA_j/q$ onto the plane perpendicular to $A$, and set

$$
\boxed{C_{ij}=P_{ik}T_{kl}P_{lj}-\alpha P_{ij}.}
$$

This [tensor](../../../../tensor.md) is symmetric and kills $A$. Its [trace](../../../../matrix-trace.md) is $t-s/q-2\alpha=0$. To verify the full decomposition, set $u=A/\sqrt q$ and split $T$ into its longitudinal component $(u^TTu)uu^T$, two mixed components, and $PTP$. The mixed terms are exactly $BA^T+AB^T$, and $\alpha+\beta q=s/q$ gives the longitudinal coefficient. Thus all requested constraints and the reconstruction hold.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
