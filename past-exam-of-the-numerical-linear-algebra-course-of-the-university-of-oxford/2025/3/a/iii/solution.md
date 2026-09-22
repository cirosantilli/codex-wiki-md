<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The claim is true**, with

$$
\boxed{M=A^TA}.
$$

It is a [symmetric positive-definite matrix](../../../../../symmetric-positive-definite-matrix.md): for every nonzero [vector](../../../../../vector.md) $z$, the fact that $A$ is an [invertible matrix](../../../../../invertible-matrix.md) gives $z^TMz=\|Az\|_2^2>0$. Since $Ax_*=b$, every candidate $x$ satisfies

$$
\|Ax-b\|_2^2=\|A(x-x_*)\|_2^2
=(x-x_*)^TA^TA(x-x_*)=\|x-x_*\|_M^2.
$$

The [generalized minimal residual method](../../../../../generalized-minimal-residual-method.md) therefore minimizes precisely this [weighted norm](../../../../../weighted-norm.md) of the error over the [linear span](../../../../../linear-span.md) of $Q_k$. The same [matrix](../../../../../matrix.md) $M$ works for every $k$ and does not depend on $b$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
