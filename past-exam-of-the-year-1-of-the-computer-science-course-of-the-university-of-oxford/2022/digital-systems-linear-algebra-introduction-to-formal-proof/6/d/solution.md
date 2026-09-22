<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) $g$ is precisely $U$, since

$$
g(u_1,u_2)=0\quad\Longleftrightarrow\quad u_2=-u_1\quad\Longleftrightarrow\quad (u_1,u_2)=(u,-u),\ u\in W_1\cap W_2.
$$

Part (c) gives $\operatorname{im}g=W_1+W_2$. Apply the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) to the [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md) $W_1\times W_2$, and then parts (a) and (b):

$$
\dim W_1+\dim W_2=\dim(W_1\times W_2)=\dim\ker g+\dim\operatorname{im}g=\dim(W_1\cap W_2)+\dim(W_1+W_2).
$$

This proves the [dimension formula for a sum of subspaces](../../../../../dimension-formula-for-a-sum-of-subspaces.md). The [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) records exactly the freedom to transfer a shared [vector](../../../../../vector.md) from one summand to the other without changing their [sum](../../../../../sum.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
