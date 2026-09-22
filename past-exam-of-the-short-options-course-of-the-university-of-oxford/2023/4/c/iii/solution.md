<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The linear map $\pi(A)=(A+A^T)/2$ is the [projection](../../../../../projection-linear-algebra.md) onto the space $\mathcal S$ of [symmetric matrices](../../../../../symmetric-matrix.md), with kernel $\mathcal A$. Define $F=\pi\circ L$ on $V$. Since $DL$ is invertible everywhere on $V$ and $\pi$ is onto, $DF$ is onto everywhere. By part (ii),

$$
F^{-1}(0)=V\cap O(n).
$$

The [regular level set theorem](../../../../../regular-level-set-theorem.md) makes this a [submanifold](../../../../../submanifold.md) of codimension $\dim\mathcal S=n(n+1)/2$, and hence

$$
\boxed{\dim O(n)=n(n-1)/2}.
$$

This neighborhood is $V$ around $I$; the source's final occurrence of $U$ in this step is a neighborhood-label slip. For any $Q\in O(n)$, left multiplication by $Q$ is an invertible linear map of the ambient [matrix](../../../../../matrix.md) space and carries $V\cap O(n)$ onto $QV\cap O(n)$. These translated charts establish the [submanifold](../../../../../submanifold.md) property at every group element.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
