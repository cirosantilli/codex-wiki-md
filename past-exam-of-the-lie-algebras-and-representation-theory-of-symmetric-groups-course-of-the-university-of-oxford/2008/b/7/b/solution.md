<h1 id="b/7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $v_{ij}$ for the [tabloid](../../../../../tabloid.md) with second-row entry $i$ and third-row entry $j$. Equivariance gives $\phi(v_{ij})=w_i+w_j$ for every distinct pair. For a tableau $t$, the only nontrivial column antisymmetrizer is on the three entries in its first column. In its alternating sum, pair each column permutation with the permutation obtained by interchanging the two singleton-row positions. Their images under $\phi$ are the same unordered sum of two $w$'s, while their signs are opposite. Hence $\phi(e_t)=0$ for every [polytabloid](../../../../../polytabloid.md), proving $\boxed{S^{(n-2,1,1)}\subseteq\ker\phi}$.

For distinct $i,j,k$,

$$
w_i=\frac12\big[(w_i+w_j)+(w_i+w_k)-(w_j+w_k)\big].
$$

Each summand is an image and two is invertible in [characteristic zero](../../../../../characteristic-zero.md). Thus every [basis](../../../../../basis.md) vector of $M^{(n-1,1)}$ is in the image, proving [surjectivity](../../../../../surjective-function.md). [rank-nullity theorem](../../../../../rank-nullity-theorem.md) then gives

$$
\boxed{\dim\ker\phi=n(n-1)-n=n(n-2).}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
