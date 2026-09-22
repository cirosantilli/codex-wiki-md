<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the small [QR decomposition](../../../../../qr-decomposition.md), each of the $k$ [Givens rotations](../../../../../givens-rotation.md) eliminates one subdiagonal entry of the [upper Hessenberg matrix](../../../../../upper-hessenberg-matrix.md). At column $j$, apply the rotation to two rows in columns $j,\ldots,k$, costing $O(k-j+1)$ arithmetic operations. Summing gives $O(k^2)$, and applying the rotations to the right-hand side costs $O(k)$. [Backward substitution in a triangular system](../../../../../backward-substitution-in-a-triangular-system.md) costs $O(k^2)$.

Computing $\|b\|_2$ costs $O(n)$ and the final dense [matrix multiplication](../../../../../matrix-multiplication.md) $Q_ky_k$ costs $O(nk)$. Thus the total, with the [Arnoldi decomposition](../../../../../arnoldi-decomposition.md) already supplied, is

$$
O(k^2+nk+n)=\boxed{O(nk)},\qquad \boxed{s=1,\quad t=1}.
$$

Here $1\leq k<n$, since $Q_{k+1}$ has [orthonormal](../../../../../orthonormal-set.md) columns in $\mathbb R^n$. In the standard dense arithmetic model, forming the general [matrix](../../../../../matrix.md)–[vector](../../../../../vector.md) product gives the sharp $\Theta(nk)$ cost. The pair above records that two-parameter bound; looser bounds such as $O(n^2)$ are also possible because $k<n$. Treating $\widetilde H_k$ as an unstructured dense [matrix](../../../../../matrix.md) would unnecessarily replace its $O(k^2)$ factorization by an $O(k^3)$ computation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
