<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First exclude the short patterns $(a,a+1,a)$ and $(a,a-1,a)$ in the [joint spectrum](../../../../../../../joint-spectrum.md). In the first pattern, the [local spectral rules for Young–Jucys–Murphy elements](../../../../../../../local-spectral-rules-for-young-jucys-murphy-elements.md) make $s_r$ act by $+1$ and $s_{r+1}$ by $-1$ on the same simultaneous [eigenvector](../../../../../../../eigenvector.md). The two sides of the [braid relation in a Coxeter group](../../../../../../../braid-relation-in-a-coxeter-group.md) then act by opposite signs. The second pattern gives the same contradiction with signs reversed.

Now induct on the length of a spectral vector. A prefix of length $i-1$ is spectral for $S_{i-1}$: decompose the restricted [group representation](../../../../../../../group-representation.md) and retain a nonzero component of the simultaneous [eigenvector](../../../../../../../eigenvector.md). If $a_i$ differed by neither $+1$ nor $-1$ from every earlier entry, move it left using the allowed adjacent interchanges. Encountering an equal entry would contradict the distinctness of consecutive [eigenvalues](../../../../../../../eigenvalue.md). Otherwise it reaches the first position, forcing $a_i=0$. For $i>1$ the original first entry was also zero, so an equal entry would indeed have been encountered. Thus

$$
\boxed{\{a_i-1,a_i+1\}\cap\{a_1,\ldots,a_{i-1}\}\ne\varnothing.}
$$

This argument uses only the stated local rules. In particular, iterating the result from $a_1=0$ also shows that all coordinates are [integers](../../../../../../../integer.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
