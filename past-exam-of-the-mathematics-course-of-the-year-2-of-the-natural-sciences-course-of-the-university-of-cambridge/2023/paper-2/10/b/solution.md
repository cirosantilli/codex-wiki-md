<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The relations in (a) reduce every word in the generators to $U^aV^b$, with $0\leq a<4$ and $b\in\{0,1\}$. These eight [matrices](../../../../../matrix.md) are distinct: the $b=0$ elements have third diagonal entry $1$ and the $b=1$ elements have entry $-1$, while the four planar blocks are distinct in each family. Their multiplication is

$$
\boxed{(U^aV^b)(U^cV^d)=U^{a+(-1)^bc}V^{b+d},}
$$

with exponents reduced modulo four and two. This proves closure. The [identity element](../../../../../identity-element.md) is $U^0V^0$, the inverse of $U^a$ is $U^{-a}$, and each $U^aV$ is its own inverse. [Associativity](../../../../../associative-property.md) is inherited from matrix multiplication, proving the [group axioms](../../../../../group-axioms.md). This is the eight-element [dihedral group](../../../../../dihedral-group.md) $D_8$.

Set $g_j=U^j$ and $g_{j+4}=U^jV$ for $j=0,1,2,3$, consistently with the two labels specified in the question. The row-times-column [multiplication table](../../../../../multiplication-table.md) is

$$
\boxed{\begin{array}{c|cccccccc}
&g_0&g_1&g_2&g_3&g_4&g_5&g_6&g_7\\\hline
g_0&g_0&g_1&g_2&g_3&g_4&g_5&g_6&g_7\\
g_1&g_1&g_2&g_3&g_0&g_5&g_6&g_7&g_4\\
g_2&g_2&g_3&g_0&g_1&g_6&g_7&g_4&g_5\\
g_3&g_3&g_0&g_1&g_2&g_7&g_4&g_5&g_6\\
g_4&g_4&g_7&g_6&g_5&g_0&g_3&g_2&g_1\\
g_5&g_5&g_4&g_7&g_6&g_1&g_0&g_3&g_2\\
g_6&g_6&g_5&g_4&g_7&g_2&g_1&g_0&g_3\\
g_7&g_7&g_6&g_5&g_4&g_3&g_2&g_1&g_0
\end{array}}
$$

The rotation powers commute with one another, and $U^a$ commutes with $U^cV$ exactly when $a$ is even. Two elements $U^aV,U^cV$ commute exactly when $a-c$ is even. These statements also check the symmetric portions of the table.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
