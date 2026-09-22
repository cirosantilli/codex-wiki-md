<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

For a [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md), write $S_{ij}=(A_{ij}+A_{ji})/2$ and $W_{ij}=(A_{ij}-A_{ji})/2$. Under an orthogonal change of frame,

$$
A'_{ij}=R_{ik}R_{jl}A_{kl},\qquad
S'_{ij}=R_{ik}R_{jl}S_{kl},\qquad W'_{ij}=R_{ik}R_{jl}W_{kl},
$$

where the last two equalities follow by interchanging the dummy indices in $A'_{ji}$. Thus the symmetric and antisymmetric parts obey the same tensor transformation law. If $A=S+W$ with $S^T=S$, $W^T=-W$, adding or subtracting its transpose forces $S=(A+A^T)/2$ and $W=(A-A^T)/2$. This also proves uniqueness.

For the given matrix, the scalar part is $a=\operatorname{Tr}(A)/3=3$. The symmetric part is $S=\begin{pmatrix}1&3&2\\3&5&4\\2&4&3\end{pmatrix}$, so the [traceless second-rank tensor](../../../../../traceless-second-rank-tensor.md) is $B=S-3I$. The skew part is $W=\begin{pmatrix}0&-1&1\\1&0&2\\-1&-2&0\end{pmatrix}$. Comparing with the [cross product](../../../../../cross-product.md) matrix $[p]_\times=\begin{pmatrix}0&-p_3&p_2\\p_3&0&-p_1\\-p_2&p_1&0\end{pmatrix}$ gives

$$
\boxed{a=3,\qquad p=(-2,1,1)^T,\qquad B=\begin{pmatrix}-2&3&2\\3&2&4\\2&4&0\end{pmatrix}.}
$$

Then $A=aI+[p]_\times+B$ proves the decomposition for every vector. The vector dual to the antisymmetric tensor is an [axial vector](../../../../../pseudovector.md) under reflections, and an ordinary vector under proper rotations.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
