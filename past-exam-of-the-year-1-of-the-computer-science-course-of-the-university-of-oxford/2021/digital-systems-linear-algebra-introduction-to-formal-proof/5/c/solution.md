<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $U=EE_5E_4E_3E_2E_1M$ and put $F_i=EE_iE$. Inserting $E^2=I$ between adjacent elimination [matrices](../../../../../matrix.md) gives

$$
U=F_5F_4F_3F_2F_1(EM),\qquad EM=F_1^{-1}F_2^{-1}F_3^{-1}F_4^{-1}F_5^{-1}U.
$$

Each $E_i^{-1}$ has the restricted lower triangular pattern in part (b)(v). Also $F_i^{-1}=EE_i^{-1}E$, as direct multiplication verifies. Hence every $F_i^{-1}$ is lower triangular. Their product is lower triangular by the allowed closure property, proving the required [Pivoted LU decomposition](../../../../../pivoted-lu-decomposition.md) with $L=F_1^{-1}\cdots F_5^{-1}$.

Explicitly,

$$
\boxed{L=\begin{pmatrix}1&0&0&0\\1&1&0&0\\-1&-1&1&0\\2&1&0&1\end{pmatrix},\qquad U=\begin{pmatrix}1&1&1&1\\0&2&-1&1\\0&0&3&5\\0&0&0&4\end{pmatrix},\qquad EM=LU.}
$$

The multipliers in rows three and four of $L$ are permuted along with the rows of $M$; simply keeping the unpermuted elimination multipliers would give the wrong product. This is the mechanism in [conjugating elimination matrices across a row permutation](../../../../../conjugating-elimination-matrices-across-a-row-permutation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
