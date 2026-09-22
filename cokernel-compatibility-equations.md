# Cokernel compatibility equations

↑ **Parent:** [Cokernel](cokernel.md)

For a [matrix](matrix.md) $A$ over the [complex numbers](complex-number.md) with the standard [Hermitian inner product](hermitian-inner-product.md), the [linear system](system-of-linear-equations.md) $Ax=b$ is solvable exactly when

$$
y^*b=0\qquad\text{for every }y\in\ker A^*.
$$

The star is the [conjugate transpose](conjugate-transpose.md); for [matrices](matrix.md) over the [real numbers](real-number.md), use the [transpose](transpose.md). Necessity follows from $y^*Ax=(A^*y)^*x=0$. For sufficiency, $(\operatorname{im}A)^\perp=\ker A^*$, and taking the [orthogonal complement](orthogonal-complement.md) again recovers $\operatorname{im}A$ in finite [dimension](dimension-vector-space.md). This is the [cokernel](cokernel.md) obstruction expressed as scalar equations. [Gilbert Strang, MIT 18.06, Lecture 10: the four fundamental subspaces](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/resources/lecture-10-the-four-fundamental-subspaces/)

For $A=\begin{pmatrix}1&2\\0&0\end{pmatrix}$, $\ker A^T=\operatorname{span}\{(0,1)\}$, so the single compatibility equation is $b_2=0$. If it holds, the [kernel](kernel-of-a-linear-map.md) supplies the remaining input freedom; if it fails, changing the input cannot remove the obstruction.

## ↑ Ancestors (6)

1. [Cokernel](cokernel.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cokernel](cokernel.md)
