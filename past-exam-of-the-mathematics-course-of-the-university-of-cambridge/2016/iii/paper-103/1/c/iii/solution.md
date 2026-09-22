<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $e_1,\ldots,e_n$ be the coordinate vectors and choose

$$
v_j=e_1+\cdots+e_j-j e_{j+1},\qquad1\leq j\leq n-1.
$$

These vectors lie in the sum-zero [standard representation of the symmetric group](../../../../../../../standard-representation-of-the-symmetric-group.md). They are mutually orthogonal for the usual [Hermitian inner product](../../../../../../../hermitian-form.md), with $\|v_j\|^2=j(j+1)$, so they form a basis of its $(n-1)$-dimensional space.

If $i\leq j$, every [transposition](../../../../../../../transposition-permutation.md) in $X_i$ exchanges two coordinates equal to $1$, so each fixes $v_j$. If $i=j+1$, summing the $j$ [transpositions](../../../../../../../transposition-permutation.md) gives coordinate $-1$ in each of positions $1,\ldots,j$ and coordinate $j$ in position $j+1$, hence $X_{j+1}v_j=-v_j$. Finally, if $i>j+1$, the $i$th coordinate of $v_j$ is zero. In the sum of the $i-1$ [transpositions](../../../../../../../transposition-permutation.md), any coordinate in its support retains its original value in $i-2$ terms and becomes zero in the remaining term; the $i$th output coordinate is the sum of the original first $i-1$ coordinates, which is zero.

Thus **all actions are diagonal in this basis**:

$$
\boxed{
X_iv_j=
\begin{cases}
(i-1)v_j,&i\leq j,\\
-v_j,&i=j+1,\\
(i-2)v_j,&i\geq j+2.
\end{cases}}
$$

This supplies an explicit [Gelfand–Tsetlin basis of the standard representation](../../../../../../../gelfand-tsetlin-basis-of-the-standard-representation.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
