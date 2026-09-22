# Unique minimizer of a positive-definite quadratic function

↑ **Parent:** [Positive definiteness](positive-definiteness.md)

Let $A$ be a real [positive-definite matrix](positive-definite-matrix.md) and minimize the displayed [quadratic function](quadratic-function.md) over all of $\mathbb R^n$. Its [gradient](gradient.md) is $Ax-b$, so its only [stationary point](stationary-point.md) solves the [linear system](system-of-linear-equations.md) $Ax_*=b$. The [matrix](matrix.md) is an [invertible matrix](invertible-matrix.md), making this solution exist and be unique. [Completing the square](completing-the-square.md) around that solution proves the stronger global statement:

$$
f(x)=c-\frac12b^TA^{-1}b+\frac12(x-x_*)^TA(x-x_*),\qquad f(x)-f(x_*)>0\quad(x\ne x_*).
$$

The [quadratic function](quadratic-function.md) is [strictly convex](strictly-convex-function.md), and its [level sets](level-set.md) above the minimum are translated [ellipsoids](ellipsoid.md). Positivity therefore turns solving a [linear system](system-of-linear-equations.md) into locating the bottom of a bowl.[§3.1.4, Example 3.2, p. 71: a quadratic function is strictly convex exactly when its symmetric coefficient matrix is positive definite](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

For the opening [matrix](matrix.md) $A=\begin{pmatrix}3&1\\1&3\end{pmatrix}$, take $b=(1,1)^T$ and $c=0$. Then $A^{-1}=\frac18\begin{pmatrix}3&-1\\-1&3\end{pmatrix}$, $x_*=(1/4,1/4)^T$, and $f(x_*)=-1/4$. Every displacement $h$ raises the value by $\tfrac12h^TAh$; along the unit [eigenvectors](eigenvector.md) $e_+$ and $e_-$ the increases are respectively $2s^2$ and $s^2$ for displacement $se_+$ or $se_-$.

For a singular [positive semidefinite matrix](positive-semidefinite-matrix.md), a solution of $Ax=b$ is still a global minimizer, but adding any [kernel](kernel-of-a-linear-map.md) [vector](vector.md) gives another. If $b$ is outside the [image of a linear map](image-of-a-linear-map.md) defined by $A$, some [kernel](kernel-of-a-linear-map.md) [vector](vector.md) $v$ has $b^Tv\ne0$, and $f(sv)=c-sb^Tv$ is unbounded below. For an [indefinite quadratic form](indefinite-quadratic-form.md), a negative [eigenvalue](eigenvalue.md) gives a direction along which the quadratic term tends to $-\infty$ regardless of $b$. Thus a [stationary point](stationary-point.md) alone does not establish a minimum. The same energy-difference identity extends to the [quadratic variational principle for a symmetric positive operator](quadratic-variational-principle-for-a-symmetric-positive-operator.md), with additional existence hypotheses in infinite [dimension](dimension-vector-space.md).

## ↑ Ancestors (9)

1. [Positive definiteness](positive-definiteness.md)
2. [Positive-definite bilinear form](positive-definite-bilinear-form.md)
3. [Symmetric bilinear form](symmetric-bilinear-form.md)
4. [Bilinear form](bilinear-form.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
