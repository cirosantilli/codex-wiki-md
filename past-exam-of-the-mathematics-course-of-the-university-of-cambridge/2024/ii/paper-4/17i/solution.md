<h1 id="17i/solution">Solution</h1>

↑ **Parent:** [17I](../17i.md)

A strongly regular graph with parameters $(k,a,b)$ is $k$-regular, with every adjacent pair having $a$ common neighbours and every distinct nonadjacent pair having $b$ common neighbours. Its adjacency [matrix](../../../../../matrix.md) satisfies

$$
A^2=(k-b)I+(a-b)A+bJ.
$$

On the orthogonal complement of the all-one [vector](../../../../../vector.md), the two possible [eigenvalues](../../../../../eigenvalue.md) are

$$
r,s=\frac{a-b\pm\sqrt{(a-b)^2+4(k-b)}}2.
$$

Using $1+m_r+m_s=n$ and $k+m_rr+m_ss=0$ gives exactly the two displayed expressions for $m_r,m_s$. They are eigenspace dimensions and hence integers, proving the rationality condition.

The Petersen graph has parameters $(3,0,1)$, so its [spectrum](../../../../../spectrum-functional-analysis.md) is

$$
3^{(1)},\qquad1^{(5)},\qquad(-2)^{(4)}.
$$

If three Petersen graphs partitioned $E(K_{10})$, their adjacency [matrices](../../../../../matrix.md) would satisfy $A+B+C=J-I$. The five-dimensional eigenvalue-one spaces of $A$ and $B$ inside the nine-dimensional space $\mathbf1^\perp$ intersect nontrivially. For a nonzero common [vector](../../../../../vector.md) $v$, $Av=Bv=v$ and therefore

$$
Cv=(J-I-A-B)v=-3v,
$$

contradicting the Petersen [spectrum](../../../../../spectrum-functional-analysis.md). No such partition exists.

## ↑ Ancestors (10)

1. [17I](../17i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
