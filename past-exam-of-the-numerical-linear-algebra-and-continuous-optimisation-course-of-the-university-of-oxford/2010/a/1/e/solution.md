<h1 id="a/1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $r$ be the [matrix rank](../../../../../matrix-rank.md), and partition the right singular vectors as $V=(V_r\ V_0)$, with $V_0\in\mathbb R^{n\times(n-r)}$ consisting of the columns associated with zero [singular values](../../../../../singular-value.md). From $Ax=0\iff\Sigma V^Tx=0$, these columns form an [orthonormal basis](../../../../../orthonormal-basis.md) of the [nullspace](../../../../../kernel-of-a-linear-map-split.md). Therefore its [orthogonal projector](../../../../../orthogonal-projection.md) is

$$
\boxed{P_{\ker A}=V_0V_0^T=I_n-V_rV_r^T.}
$$

It acts on the input space $\mathbb R^n$. Symmetry and idempotence follow from $V_0^TV_0=I_{n-r}$. At full column rank it is zero, and at rank zero it is the identity.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
