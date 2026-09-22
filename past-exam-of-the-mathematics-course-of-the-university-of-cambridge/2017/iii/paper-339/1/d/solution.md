<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [pointed cone](../../../../../../pointed-cone.md) has no nonzero line through the origin: equivalently $K\cap(-K)=\{0\}$. If $A\in K\cap(-K)$, its [quadratic form](../../../../../../quadratic-form.md) vanishes on the [nonnegative orthant](../../../../../../nonnegative-orthant.md). Testing the coordinate [vectors](../../../../../../vector.md) gives $A_{ii}=0$. Testing $e_i+e_j$ then gives

$$
0=(e_i+e_j)^TA(e_i+e_j)=2A_{ij}.
$$

Since $A$ is a [symmetric matrix](../../../../../../symmetric-matrix.md), every entry is zero. Thus $\boxed{K\cap(-K)=\{0\}}$.

The [identity matrix](../../../../../../identity-matrix.md) gives an [interior](../../../../../../interior-topology.md) point. For a symmetric perturbation $E$ with [operator norm](../../../../../../operator-norm.md) $\|E\|_2<1$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
x^T(I+E)x\geq(1-\|E\|_2)\|x\|_2^2>0\quad(x\ne0).
$$

This open [norm](../../../../../../norm.md) ball around $I$ lies even in the [positive semidefinite cone](../../../../../../positive-semidefinite-cone.md), hence in $K$. Consequently $\boxed{I\in\operatorname{int}K}$ and the [interior](../../../../../../interior-topology.md) is nonempty.

More generally, the [interior of the copositive cone](../../../../../../interior-of-the-copositive-cone.md) consists exactly of [strictly copositive matrices](../../../../../../strictly-copositive-matrix.md). Positivity on the [compact](../../../../../../compact-space.md) nonnegative [unit sphere](../../../../../../unit-sphere.md) has a positive minimum and persists under small perturbations; a zero there is destroyed by an arbitrarily small negative multiple of $I$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
