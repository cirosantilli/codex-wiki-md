<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Fix one common [eigenvector](../../../../../eigenvector.md) $v\ne0$, and write $AA^\top v=\lambda v$ and $BB^\top v=\mu v$. By (d),

$$
AA^\top BB^\top=A(A^\top B)B^\top=0,
$$

so $\lambda\mu v=0$ and **at least one of the two [eigenvalues](../../../../../eigenvalue.md) is zero**.

To exclude both being zero, use the [kernel of a Gram product](../../../../../kernel-of-a-gram-product.md) identity:

$$
v^\top AA^\top v=\|A^\top v\|^2,\qquad
v^\top BB^\top v=\|B^\top v\|^2.
$$

If both products annihilate $v$, then $A^\top v=B^\top v=0$. By (b), $v\in\operatorname{im}L$, and by (e), this is $\operatorname{im}B$. On the other hand, $B^\top v=0$ makes $v$ [orthogonal](../../../../../orthogonal-vectors.md) to every [vector](../../../../../vector.md) in $\operatorname{im}B$. In particular $v$ is [orthogonal](../../../../../orthogonal-vectors.md) to itself, so $\|v\|^2=0$ and $v=0$, a contradiction.

Therefore **each specified common [eigenvector](../../../../../eigenvector.md) belongs to exactly one of $\ker(AA^\top)$ and $\ker(BB^\top)$**. Both [eigenvalues](../../../../../eigenvalue.md) are nonnegative by the displayed squared-[norm](../../../../../norm.md) identities, so the other [eigenvalue](../../../../../eigenvalue.md) is strictly positive. This is the spectral mechanism behind [orthogonal null-space completion of a square matrix](../../../../../orthogonal-null-space-completion-of-a-square-matrix.md).

## ↑ Ancestors (13)

1. [G](../g.md)
2. [4](../../4.md)
3. [Linear algebra](../../linear-algebra.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
