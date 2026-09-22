<h1 id="2/a/iv/solution">Solution</h1>

↑ **Parent:** [iv](../iv.md)

The [transpose](../../../../../../../transpose.md) is a [linear map](../../../../../../../linear-map.md), so $T(A)=A+A^T$ is a [linear map](../../../../../../../linear-map.md) on the $n^2$-dimensional [vector space](../../../../../../../vector-space-split.md) $M_{n\times n}(F)$. Let $E_{ij}$ denote a [matrix unit](../../../../../../../matrix-unit.md). The answer depends on the [characteristic of a field](../../../../../../../characteristic-of-a-field.md).

If $\operatorname{char}F\ne2$, then $T(A)=0$ means $A^T=-A$. Such [skew-symmetric matrices](../../../../../../../skew-symmetric-matrix.md) have zero diagonal, and their entries above the diagonal can be chosen freely. A [basis](../../../../../../../basis.md) of the [kernel of a linear map](../../../../../../../kernel-of-a-linear-map-split.md) is $E_{ij}-E_{ji}$ for $i<j$, giving [nullity](../../../../../../../nullity-of-a-linear-map.md) $n(n-1)/2$. The [image of a linear map](../../../../../../../image-of-a-linear-map.md) consists of all [symmetric matrices](../../../../../../../symmetric-matrix.md): $T(A)$ is symmetric, and every [symmetric matrix](../../../../../../../symmetric-matrix.md) $S$ is $T(S/2)$. Its [basis](../../../../../../../basis.md) comprises $E_{ii}$ and $E_{ij}+E_{ji}$ for $i<j$, giving [rank of a linear map](../../../../../../../rank-of-a-linear-map.md) $n(n+1)/2$.

If $\operatorname{char}F=2$, then $-A=A$, so $\ker T$ consists of all [symmetric matrices](../../../../../../../symmetric-matrix.md), with [dimension](../../../../../../../dimension-vector-space.md) $n(n+1)/2$. Every $T(A)$ is symmetric with zero diagonal, and every symmetric zero-diagonal [matrix](../../../../../../../matrix.md) $S$ arises by taking $A_{ij}=S_{ij}$ for $i<j$ and all other entries zero. The [image of a linear map](../../../../../../../image-of-a-linear-map.md) therefore has [basis](../../../../../../../basis.md) $E_{ij}+E_{ji}$ for $i<j$, and [dimension](../../../../../../../dimension-vector-space.md) $n(n-1)/2$. This is the [symmetrization map in characteristic two](../../../../../../../symmetrization-map-in-characteristic-two.md).

In both cases the [rank-nullity theorem](../../../../../../../rank-nullity-theorem.md) is verified explicitly:

$$
\boxed{\begin{array}{c|cc}
&\dim\ker T&\dim\operatorname{im}T\\\hline
\operatorname{char}F\ne2&\dfrac{n(n-1)}2&\dfrac{n(n+1)}2\\
\operatorname{char}F=2&\dfrac{n(n+1)}2&\dfrac{n(n-1)}2
\end{array}\qquad
\dim\ker T+\dim\operatorname{im}T=n^2.}
$$

## ↑ Ancestors (13)

1. [iv](../iv.md)
2. [a](../../a.md)
3. [2](../../../2.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
