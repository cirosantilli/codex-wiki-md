<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

For an $m\times n$ [matrix](../../../../../../../matrix.md), the corresponding [elementary matrices](../../../../../../../elementary-matrix.md) are $m\times m$, because the operation is implemented by left [matrix multiplication](../../../../../../../matrix-multiplication.md). Apply the desired [elementary row operation](../../../../../../../elementary-row-operation.md) to the [identity matrix](../../../../../../../identity-matrix.md) $I_m$. Writing $E_{ij}$ for the [matrix unit](../../../../../../../matrix-unit.md) with its only nonzero entry, $1$, in position $(i,j)$ gives:

$$
\begin{aligned}
P_{ij}&=I_m-E_{ii}-E_{jj}+E_{ij}+E_{ji},
& P_{ij}^{-1}&=P_{ij},\\
D_i(c)&=I_m+(c-1)E_{ii},
& D_i(c)^{-1}&=D_i(c^{-1})\quad(c\ne0),\\
L_{ij}(c)&=I_m+cE_{ij},
& L_{ij}(c)^{-1}&=L_{ij}(-c)\quad(i\ne j).
\end{aligned}
$$

Indeed, these [matrix products](../../../../../../../matrix-product.md) interchange rows $i,j$, scale row $i$, and add $c$ times row $j$ to row $i$, respectively. The displayed inverses undo precisely those operations. Algebraically, $E_{ij}^2=0$ when $i\ne j$, so $(I_m+cE_{ij})(I_m-cE_{ij})=I_m$; the other two inverse identities follow immediately from their row actions. Thus every [elementary matrix](../../../../../../../elementary-matrix.md) is an [invertible matrix](../../../../../../../invertible-matrix.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
