<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\widehat A=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$ and $v_i=P^{-1}e_i$, where $e_i$ are the [standard basis](../../../../../standard-basis.md) [vectors](../../../../../vector.md). Since $AP^{-1}=P^{-1}\widehat A$,

$$
Av_i=P^{-1}\widehat Ae_i=\lambda_iv_i.
$$

Thus **the columns of $P^{-1}$ form an [eigenbasis](../../../../../eigenbasis.md)**, and the requested [ordered basis](../../../../../ordered-basis.md) is $D=(P^{-1}e_1,\ldots,P^{-1}e_n)$. Its [basis matrix](../../../../../basis-matrix.md) is $P^{-1}$, giving $[t]_D=PAP^{-1}=\widehat A$. More completely, for each distinct [eigenvalue](../../../../../eigenvalue.md) $\lambda$, its [eigenspace](../../../../../eigenspace.md) is

$$
E_\lambda(A)=\operatorname{span}\{P^{-1}e_i:\lambda_i=\lambda\}.
$$

All nonzero [vectors](../../../../../vector.md) in these [eigenspaces](../../../../../eigenspace.md) are [eigenvectors](../../../../../eigenvector.md); when an [eigenvalue](../../../../../eigenvalue.md) repeats, they need not be individual columns of $P^{-1}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
