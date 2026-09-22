<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $i$ and let $M_i=\overline{\operatorname{span}}\{x_j:j\ne i\}$. The hypothesis gives $M_i\ne X$. Moreover $x_i\notin M_i$, since otherwise the closed span of all the [vectors](../../../../vector.md) would be contained in $M_i$. Hence $d_i=\operatorname{dist}(x_i,M_i)>0$.

On $M_i+\mathbb Rx_i$, define $\phi_i(m+tx_i)=t$. It is well-defined because $x_i\notin M_i$. For $t\ne0$,

$$
\|m+tx_i\|=|t|\|x_i+m/t\|\geq|t|d_i,
$$

so $|\phi_i(m+tx_i)|\leq\|m+tx_i\|/d_i$; the inequality also holds for $t=0$. The [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) extends $\phi_i$ without increasing its [norm](../../../../norm.md) to $x_i^*\in X^*$. This gives $x_i^*(x_j)=\delta_{ij}$.

If two continuous functionals have these values, their difference vanishes on the [linear span](../../../../linear-span.md) of every $x_j$, which is dense in $X$. [Continuity](../../../../continuous-function.md) then makes the difference zero everywhere. Thus each functional is unique, proving the required **unique biorthogonal system**. In fact its [norm](../../../../norm.md) is $\|x_i^*\|=1/d_i$, by taking [vectors](../../../../vector.md) in $M_i$ approaching the distance infimum. This is the coordinate-functional construction for a [minimal total family in a normed space](../../../../minimal-total-family-in-a-normed-space.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the functional analysis course of the University of Oxford](../../../split.md)
5. [Functional analysis course of the University of Oxford](../../../../functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
