<h1 id="p/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The elementary elimination step replaces row $i$ by row $i$ minus a multiple $m_{ij}$ of an earlier [pivot](../../../../pivotal-quantity.md) row $j$. With [coordinate vectors](../../../../coordinate-vector.md) $e_i$, its premultiplication [matrix](../../../../matrix.md) is

$$
E_{ij}=I-m_{ij}e_ie_j^T,\qquad i>j,
$$

and its inverse is $I+m_{ij}e_ie_j^T$, since $(e_ie_j^T)^2=0$. Choose $m_{ij}$ as the current entry below the [pivot](../../../../pivotal-quantity.md) divided by the current [pivot](../../../../pivotal-quantity.md). Required [pivots](../../../../pivotal-quantity.md) are assumed nonzero, consistently with elimination without [row interchanges](../../../../row-interchange.md).

For [dimension](../../../../dimension-vector-space.md) 4, first eliminate positions $(2,1),(3,1),(4,1)$, then $(3,2),(4,2)$, then $(4,3)$. Thus

$$
\boxed{U=E_{43}E_{42}E_{32}E_{41}E_{31}E_{21}A.}
$$

The rightmost operation acts first, and every multiplier is computed from the [matrix](../../../../matrix.md) at its own stage. For general $n$, the numbers of eliminations in successive columns are $n-1,n-2,\ldots,1$, totaling $n(n-1)/2$; a zero multiplier simply gives an identity operation.

The product $E$ is unit lower triangular and $U=EA$ is [upper triangular](../../../../upper-triangular-matrix.md). Its inverse $L=E^{-1}$ is unit lower triangular, so

$$
\boxed{A=LU.}
$$

The stored multiplier in position $(i,j)$ is the corresponding subdiagonal entry of $L$, as follows by reversing the pivot-row subtractions column by column.

If $A$ is upper Hessenberg, only the first subdiagonal can be nonzero below the diagonal. At stage $j$ only position $(j+1,j)$ needs elimination. Subtracting row $j$ cannot create lower entries further down because its entries before its [pivot](../../../../pivotal-quantity.md) are already zero. Hence only $n-1$ operations are needed. The inverse factors occur in increasing column order, and their [cross products](../../../../cross-product.md) vanish, giving

$$
L=I+\sum_{j=1}^{n-1}m_{j+1,j}e_{j+1}e_j^T,
$$

which is lower bidiagonal; $U$ is [upper triangular](../../../../upper-triangular-matrix.md), possibly dense above its diagonal.

If the [Hessenberg matrix](../../../../hessenberg-matrix.md) is also symmetric, it is tridiagonal. At each elimination step the [pivot](../../../../pivotal-quantity.md) row has no entries past its immediate superdiagonal, so the updated [matrix](../../../../matrix.md) retains that upper bandwidth. Thus **$L$ is lower bidiagonal and $U$ is upper bidiagonal**, with at most two nonzero entries in each row, as required.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [P](../../p.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
