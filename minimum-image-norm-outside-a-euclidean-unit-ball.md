# Minimum image norm outside a Euclidean unit ball

↑ **Parent:** [Singular value](singular-value.md)

For a real [matrix](matrix.md) $A$, let $B=A^{\mathsf T}A$. It is [positive semidefinite](positive-semidefinite-matrix.md), and the [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md) gives $x^{\mathsf T}Bx\ge\lambda_{\min}\|x\|^2$. If $\lambda_{\min}>0$, rescaling any longer [vector](vector.md) to unit length decreases its image norm, so minimizers lie on the [unit sphere](unit-sphere.md). [Lagrange multipliers](lagrange-multiplier.md) applied to $x^{\mathsf T}Bx$ with $\|x\|=1$ give $Bx=\lambda x$. Thus the minimizers are exactly the unit [vectors](vector.md) in the least [eigenspace](eigenspace.md).

If $\lambda_{\min}=0$, the [minimum](minimum-of-a-subset-of-a-total-order.md) is zero and the full [argmin](argmin.md) consists of all $x\in\ker A$ with $\|x\|\ge1$. Indeed, $\ker(A^{\mathsf T}A)=\ker A$ because $x^{\mathsf T}A^{\mathsf T}Ax=\|Ax\|^2$. Restricting the minimizers to the sphere would omit longer [kernel](kernel-of-a-linear-map-split.md) vectors in this case. For a ball constraint $\|x\|\le1$, the [argmin](argmin.md) is always $\ker A$ intersected with the ball.

## ↑ Ancestors (7)

1. [Singular value](singular-value.md)
2. [Singular value decomposition](singular-value-decomposition.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/5/b/i/solution.md)
