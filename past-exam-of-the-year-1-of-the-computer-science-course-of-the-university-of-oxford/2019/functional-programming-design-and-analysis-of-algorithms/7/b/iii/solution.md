<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $M_i[t]$ use only the first $i$ available coins. Initialize $M_0[0]=0$, $M_0[t]=\infty$ for $t>0$, and use

$$
M_i[t]=\min\{M_{i-1}[t],\ 1+M_{i-1}[t-x_i]\},
$$

omitting the second term when $t<x_i$. The alternatives exclude the current coin or use it once; both refer to the previous row, so it cannot be used twice. [Induction](../../../../../../mathematical-induction.md) on $i$ proves correctness, and **$M_n[v]$** is the required answer, including $\infty$ when no selection works.

The [running time](../../../../../../running-time.md) is **$O(nv)$**. A single amount [array](../../../../../../array-data-structure.md) reduces [auxiliary space](../../../../../../auxiliary-space.md) to **$O(v)$** if each coin updates amounts in _descending_ order, $t=v,v-1,\ldots,x_i$. Then $M[t-x_i]$ still describes the previous row. Ascending updates would reuse the same coin and solve a different, unlimited-supply problem.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
