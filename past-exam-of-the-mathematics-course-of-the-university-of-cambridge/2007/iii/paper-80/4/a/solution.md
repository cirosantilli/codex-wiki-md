<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hadamard well-posedness](../../../../../../well-posed-problem.md) requires existence of a solution for every admissible datum, uniqueness, and continuous dependence of the solution on the datum in the specified [normed spaces](../../../../../../normed-vector-space.md). **An [inverse problem](../../../../../../inverse-problem-split.md) is [ill-posed](../../../../../../ill-posed-problem.md) if any of these requirements fails.** The choice of spaces and [norms](../../../../../../norm.md) is part of this assertion: [continuity](../../../../../../continuous-function.md) in one [norm](../../../../../../norm.md) does not establish [continuity](../../../../../../continuous-function.md) in a stronger [norm](../../../../../../norm.md).

For a [bounded linear operator](../../../../../../continuous-linear-operator.md) $A$, existence requires $y\in\operatorname{ran}A$, and uniqueness requires $\ker A=\{0\}$. Even when both hold for exact data, inversion can be unstable. For example, if $\|x_N\|_X=1$ but $\|Ax_N\|_Y\to0$, data $Ax_N$ approach zero while their solutions do not approach zero. Thus $A^{-1}$ on its range is not continuous. Perturbed data can also leave the range entirely, so an exact solution need not exist after measurement error. These are distinct mechanisms of [ill-posedness](../../../../../../ill-posed-problem.md); the [inverse scattering problem](../../../../../../inverse-scattering-problem.md) below exhibits unstable continuation even on data for which an outgoing continuation exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
