<h1 id="40a/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $q_1$ and $q_n$ be the first and last columns of $\widetilde Q_k$. Since $\widetilde R_k$ is upper triangular,

$$
A^ke_1=(\widetilde R_k)_{11}q_1.
$$

Thus $q_1$ is the normalized $k$th [power method](../../../../../../../power-method.md) iterate starting from $e_1$.

Taking the transpose of $A^k=\widetilde Q_k\widetilde R_k$ and using symmetry gives $A^k=\widetilde R_k^T\widetilde Q_k^T$. Therefore

$$
A^kq_n=(\widetilde R_k)_{nn}e_n,
\qquad
q_n=(\widetilde R_k)_{nn}A^{-k}e_n.
$$

So the last column is the normalized $k$th [inverse iteration](../../../../../../../inverse-iteration.md) iterate with shift zero and starting [vector](../../../../../../../vector.md) $e_n$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [40A](../../../40a.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
