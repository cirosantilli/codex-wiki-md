<h1 id="6c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $e_1,\ldots,e_n$ be the standard [basis](../../../../../../basis.md) and define $a_j=f(e_j)$. By linearity,

$$
f(x)=f\!\left(\sum_{j=1}^n x_je_j\right)=\sum_{j=1}^n x_jf(e_j)=a\cdot x.
$$

Thus every [linear functional](../../../../../../linear-functional.md) has this form. Its representing vector is unique because evaluating $a\cdot x=b\cdot x$ at each $e_j$ gives $a_j=b_j$.

For the prescribed [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md), the third listed vector is the first minus the second, so it adds no independent constraint. The first two require

$$
a_1+a_2+a_3-a_4=0,\qquad2a_1-a_2-2a_4=0.
$$

Taking $a_1=s$ and $a_4=t$ gives $a_2=2s-2t$, $a_3=-3s+3t$. Consequently **all possible representing vectors** are

$$
\boxed{a=s(1,2,-3,0)^T+t(0,-2,3,1)^T,\qquad s,t\in\mathbb R.}
$$

Conversely, every such vector is perpendicular to each of the three prescribed vectors, so its [linear functional](../../../../../../linear-functional.md) vanishes on them. This also includes the zero [linear functional](../../../../../../linear-functional.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
