<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Euclidean norm](../../../../../euclidean-norm.md) is invariant under an [orthogonal matrix](../../../../../orthogonal-matrix.md), so the full [singular value decomposition](../../../../../singular-value-decomposition.md) gives

$$
\begin{aligned}
\|Ax-b\|_2^2
&=\left\|\begin{pmatrix}\Sigma V^Tx-U^Tb\\-U_\perp^Tb\end{pmatrix}\right\|_2^2\\
&=\|\Sigma V^Tx-U^Tb\|_2^2+\|U_\perp^Tb\|_2^2.
\end{aligned}
$$

The second term is independent of $x$; the first attains its unique minimum zero because $\Sigma$ is an [invertible matrix](../../../../../invertible-matrix.md). The [linear least squares](../../../../../linear-least-squares.md) solution is therefore

$$
\boxed{x_*=V\Sigma^{-1}U^Tb=A^+b,\qquad
\min_x\|Ax-b\|_2=\|U_\perp^Tb\|_2.}
$$

Here $A^+=V\Sigma^{-1}U^T$ is the [Moore-Penrose inverse](../../../../../moore-penrose-inverse.md), and the fitted [vector](../../../../../vector.md) is the [orthogonal projection](../../../../../orthogonal-projection.md) $Ax_*=UU^Tb$ onto the [image of a linear map](../../../../../image-of-a-linear-map.md) defined by $A$.

With the [singular value decomposition](../../../../../singular-value-decomposition.md) supplied, forming $U^Tb$ costs $O(mn)$ [arithmetic operations](../../../../../arithmetic-operation.md), diagonal scaling costs $O(n)$, and multiplication by $V$ costs $O(n^2)$. Since $m\geq n$,

$$
\boxed{\text{Cost per right-hand side: }O(mn+n^2)=O(mn).}
$$

One need not form $U_\perp$, $A^+$ or $A^TA$ to calculate $x_*$. Computing the needed thin [singular value decomposition](../../../../../singular-value-decomposition.md) first has standard dense cost $O(mn^2)$; explicitly forming an entire $m\times m$ orthogonal completion can require additional work when $m$ is much larger than $n$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
