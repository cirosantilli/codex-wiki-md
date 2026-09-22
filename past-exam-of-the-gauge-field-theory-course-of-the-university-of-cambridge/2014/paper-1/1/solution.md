<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In [spontaneous symmetry breaking](../../../../spontaneous-symmetry-breaking.md), the [action](../../../../action.md) respects a [symmetry](../../../../symmetry-physics.md) while a selected [vacuum state](../../../../vacuum-state.md) is invariant only under a proper [subgroup](../../../../subgroup.md). A nonzero [vacuum expectation value](../../../../vacuum-expectation-value.md) can identify that choice. For a local [gauge theory](../../../../gauge-theory.md), gauge transformations are redundancies rather than transformations between physically different states; a gauge-fixed scalar expectation value describes the [Higgs mechanism](../../../../higgs-mechanism.md) and its massive excitations. It should not be interpreted as breaking an observable local redundancy.

Write the [adjoint scalar field](../../../../adjoint-scalar-field.md) as $\Phi=\Phi_0+\varphi$, with Hermitian [gauge generators](../../../../gauge-generator.md) normalized by $\operatorname{tr}(t^at^b)=\delta^{ab}/2$. Since $\Phi_0$ is constant, the part of the [covariant derivative](../../../../covariant-derivative.md) linear in the [gauge field](../../../../gauge-field.md) is $D_\mu\Phi_0=igA_\mu^a[t^a,\Phi_0]$. Both $t^a$ and $\Phi_0$ are Hermitian, so their [commutator](../../../../commutator.md) is anti-Hermitian. The scalar kinetic term therefore contributes

$$
\mathcal L_{\rm mass}
=-g^2A_\mu^aA^{b\mu}\operatorname{tr}([t^a,\Phi_0][t^b,\Phi_0])
=\frac12A_\mu^a(m^2)^{ab}A^{b\mu}.
$$

Matching coefficients gives the [adjoint scalar gauge-boson mass matrix](../../../../adjoint-scalar-gauge-boson-mass-matrix.md)

$$
\boxed{(m^2)^{ab}=-2g^2\operatorname{tr}([t^a,\Phi_0][t^b,\Phi_0]).}
$$

It is positive semidefinite: for real coefficients $x_a$, its [quadratic form](../../../../quadratic-form-split.md) is $2g^2\operatorname{tr}(C^\dagger C)\ge0$, where $C=[x_at^a,\Phi_0]$. Its null space consists of generators commuting with the vacuum, the [Lie algebra](../../../../lie-algebra-split.md) of its [centralizer](../../../../centralizer.md).

For a diagonal vacuum $\Phi_0=\operatorname{diag}(\lambda_1,\lambda_2,\lambda_3)$, the [matrix unit](../../../../matrix-unit.md) $E_{ij}$ obeys $[E_{ij},\Phi_0]=(\lambda_j-\lambda_i)E_{ij}$. The two normalized Hermitian generators built from $E_{ij},E_{ji}$ each acquire

$$
m_{ij}^2=g^2(\lambda_i-\lambda_j)^2.
$$

The diagonal generators $t^3,t^8$ commute with every such vacuum and remain massless. Orthogonality of these root generators also shows that the [mass](../../../../mass.md) matrix is diagonal in the supplied [Gell-Mann matrices](../../../../gell-mann-matrices.md) basis. Take $g>0$ and $v\ne0$ below; $v=0$ restores the full [SU(3)](../../../../su-3-group.md) group.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
