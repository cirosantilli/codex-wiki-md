<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The given map is the [unilateral shift operator](../../../../../../unilateral-shift-operator.md). Its [adjoint operator](../../../../../../adjoint-operator.md) is the [left shift operator](../../../../../../left-shift-operator.md), since

$$
\langle Ku,f\rangle=\sum_{j\geq1}u_j\overline{f_{j+1}},\qquad K^*f=(f_2,f_3,\ldots).
$$

The shift is an [isometry](../../../../../../isometry.md) with trivial [kernel](../../../../../../kernel-of-a-linear-map.md) and closed range $\{f:f_1=0\}$. Its range has [orthogonal complement](../../../../../../orthogonal-complement.md) $\operatorname{span}\{e_1\}$, so **every square-summable datum is admissible**. Consequently,

$$
\boxed{\mathcal D(K^\dagger)=\ell^2,\qquad K^\dagger(f_1,f_2,\ldots)=(f_2,f_3,\ldots)=K^*f.}
$$

Indeed $K^\dagger K=I$, while $KK^\dagger f=f-f_1e_1$ is the required [orthogonal projection](../../../../../../orthogonal-projection.md). The discarded first component is the residual of the [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md), not an obstruction to the existence of the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
