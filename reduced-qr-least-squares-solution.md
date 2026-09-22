# Reduced QR least-squares solution

↑ **Parent:** [QR decomposition](qr-decomposition.md)

Let $A=QR$ with $Q^TQ=I$ and square invertible upper triangular $R$. The [normal equations for linear least squares](normal-equations-for-linear-least-squares.md) reduce from $R^TRx=R^TQ^Tb$ to the system in the title. It is solved by [back substitution](back-substitution.md). The geometric identity $\|Ax-b\|_2^2=\|Rx-Q^Tb\|_2^2+\|(I-QQ^T)b\|_2^2$ proves existence and uniqueness of the minimizer. For tall $Q$, $QQ^T$ is an [orthogonal projection](orthogonal-projection.md), not the identity on the entire observation space.

## ↑ Ancestors (8)

1. [QR decomposition](qr-decomposition.md)
2. [Gram-Schmidt process](gram-schmidt-process.md)
3. [Inner product](inner-product-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/6/b/ii/solution.md)
