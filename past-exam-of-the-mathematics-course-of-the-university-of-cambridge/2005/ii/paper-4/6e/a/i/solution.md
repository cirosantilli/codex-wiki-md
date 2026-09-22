<h1 id="6e/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $s=|w|^2$. The exact [Hebbian learning](../../../../../../../hebbian-learning.md) rule gives

$$
\tau\dot s=2w\cdot(yx)=2y^2\ge0.
$$

Thus the [norm](../../../../../../../norm.md) never decreases, and increases whenever the output is nonzero. Because learning is slow relative to input fluctuations, its averaged equation is $\tau\dot w=Cw$, where $C=\langle xx^T\rangle$ is the input second-moment [matrix](../../../../../../../matrix.md). It is a [covariance matrix](../../../../../../../covariance-matrix.md) only if the inputs have zero mean. Diagonalizing the [positive semidefinite matrix](../../../../../../../positive-semidefinite-matrix.md) $C$ gives components $w_j(t)=w_j(0)e^{\lambda_jt/\tau}$. Hence **weights grow without bound whenever the initial [vector](../../../../../../../vector.md) has a component in an excited positive-eigenvalue direction**. A [vector](../../../../../../../vector.md) entirely in $\ker C$, or identically zero input, is an important stationary exception.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [6E](../../../6e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
