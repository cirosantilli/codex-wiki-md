<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**No uniform absolute error bound of order $\epsilon$ follows.** Take the [Jordan block](../../../../../jordan-block.md)

$$
B=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
E=\begin{pmatrix}0&0\\\epsilon&0\end{pmatrix}.
$$

Here $\|B\|_2=1$ and $\|E\|_2=\epsilon$. The exact [eigenvalues](../../../../../eigenvalue.md) of $B$ are both zero, whereas

$$
\det(\lambda I_2-B-E)=\lambda^2-\epsilon,
\qquad \boxed{\lambda_\pm(B+E)=\pm\sqrt\epsilon}.
$$

These are admissible outputs under a [backward error](../../../../../backward-error.md) guarantee of size $\epsilon$, yet their [forward errors](../../../../../forward-error.md) are $\sqrt\epsilon$. This is the [square-root splitting of a defective double eigenvalue](../../../../../square-root-splitting-of-a-defective-double-eigenvalue.md). More generally, [eigenvalue sensitivity](../../../../../eigenvalue-sensitivity.md) depends on the [matrix](../../../../../matrix.md); [backward stability](../../../../../backward-stability.md) alone does not control it. The [singular value perturbation bound](../../../../../singular-value-perturbation-bound.md) used in part (ii) has no equally uniform counterpart for the [eigenvalues](../../../../../eigenvalue.md) of arbitrary nonsymmetric [matrices](../../../../../matrix.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
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
