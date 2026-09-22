<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $Z=X-\mu$, so the [covariance operator](../../../../../../covariance-operator.md) is

$$
C_Xh=\mathbb E[\langle Z,h\rangle Z].
$$

For $g,h\in L^2[0,1]$,

$$
\langle C_Xh,g\rangle
=\mathbb E[\langle Z,h\rangle\langle Z,g\rangle]
=\langle h,C_Xg\rangle,
$$

so $C_X$ is [self-adjoint](../../../../../../self-adjoint-operator.md). Moreover,

$$
\langle C_Xh,h\rangle
=\mathbb E[\langle Z,h\rangle^2]\geq0,
$$

so it is a [positive operator](../../../../../../positive-operator.md).

Let $(e_j)$ be any [orthonormal basis](../../../../../../orthonormal-basis.md). [Tonelli theorem](../../../../../../tonelli-theorem.md) and [Parseval identity](../../../../../../parseval-identity.md) give

$$
\operatorname{tr}C_X
=\sum_j\langle C_Xe_j,e_j\rangle
=\mathbb E\sum_j|\langle Z,e_j\rangle|^2
=\mathbb E\lVert Z\rVert^2<\infty.
$$

A positive operator with finite trace is a [trace-class operator](../../../../../../trace-class-operator.md), completing the proof.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
