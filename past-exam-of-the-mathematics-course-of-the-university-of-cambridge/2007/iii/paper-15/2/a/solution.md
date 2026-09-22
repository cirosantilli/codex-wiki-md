<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed $p$, the [covariant derivative](../../../../../../covariant-derivative.md) is linear in its tangent-vector input, so $L_p:T_pM\to T_pM$, $v\mapsto(\nabla_vX)(p)$, is a well-defined linear map. Its [trace](../../../../../../matrix-trace.md) defines the [divergence of a Riemannian vector field](../../../../../../divergence-of-a-riemannian-vector-field.md). In the given [Riemannian orthonormal frame](../../../../../../riemannian-orthonormal-frame.md), write $X=\sum_j f_jE_j$. The [Levi-Civita connection](../../../../../../levi-civita-connection.md) product rule gives

$$
\nabla_{E_i}X=\sum_j E_i(f_j)E_j+\sum_j f_j\nabla_{E_i}E_j.
$$

At $p$, the second sum vanishes by the [normal orthonormal frame](../../../../../../normal-orthonormal-frame.md) hypothesis. Thus the $i$th diagonal coefficient of $L_p$ is $E_i(f_i)(p)$, and

$$
\boxed{\operatorname{div}X(p)=\operatorname{tr}L_p=\sum_{i=1}^nE_i(f_i)(p).}
$$

Equivalently one can take $\sum_i g(\nabla_{E_i}X,E_i)$; the [trace](../../../../../../matrix-trace.md) does not depend on the orthonormal [basis](../../../../../../basis.md) chosen.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
