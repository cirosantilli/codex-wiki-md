<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Denote a matrix by $A(x,y,z)$, with $y$ the upper-right entry. Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
\boxed{A(x,y,z)A(x',y',z')=A(x+x',\ y+y'+xz',\ z+z').}
$$

This proves closure. Associativity is inherited from matrix multiplication. The identity is $A(0,0,0)$, and the inverse is

$$
\boxed{A(x,y,z)^{-1}=A(-x,xz-y,-z).}
$$

Both products with this matrix are the identity. Thus these real matrices form the [Heisenberg group](../../../../../heisenberg-group.md), in the coordinate convention with central coordinate $y$.

Let $N=\{A(0,b,0):b\in\mathbb R\}$. Its multiplication adds $b$, its identity is $b=0$ and its inverse negates $b$, so it is a [subgroup](../../../../../subgroup.md). Moreover

$$
A(x,y,z)A(0,b,0)=A(x,y+b,z)=A(0,b,0)A(x,y,z).
$$

Thus every element of $N$ is central, and $gNg^{-1}=N$. Therefore **$N$ is a normal subgroup**. In fact it is the full [center of a group](../../../../../center-of-a-group.md), as described by the [center quotient of the real Heisenberg group](../../../../../center-quotient-of-the-real-heisenberg-group.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
