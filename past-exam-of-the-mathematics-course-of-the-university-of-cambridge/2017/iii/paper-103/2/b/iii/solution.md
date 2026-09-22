<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Induct on the distance between equal entries $a_i=a_j=a$ of a point of the [joint spectrum](../../../../../../../joint-spectrum.md). Consecutive equal entries are impossible by the [local spectral rules for Young–Jucys–Murphy elements](../../../../../../../local-spectral-rules-for-young-jucys-murphy-elements.md). It suffices to consider consecutive occurrences of $a$: proving the assertion for each such pair proves it for any wider pair.

Suppose $a-1$ is missing between them. There can be at most one occurrence of $a+1$ in the interval. Otherwise a pair of consecutive $a+1$ entries has a shorter gap, and the induction hypothesis forces an intervening $a$, contrary to our choice of the pair. Move the two endpoint entries $a$ inward past entries different from $a,a-1,a+1$. Every move is an admissible spectral interchange. If there is no $a+1$, this creates consecutive equal entries. If there is one, this creates $(a,a+1,a)$, already excluded by the [braid relation in a Coxeter group](../../../../../../../braid-relation-in-a-coxeter-group.md). Both are impossible.

Interchanging the roles of $a-1$ and $a+1$ excludes the omission of $a+1$ as well. Therefore

$$
\boxed{\{a-1,a+1\}\subseteq\{a_{i+1},\ldots,a_{j-1}\}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
