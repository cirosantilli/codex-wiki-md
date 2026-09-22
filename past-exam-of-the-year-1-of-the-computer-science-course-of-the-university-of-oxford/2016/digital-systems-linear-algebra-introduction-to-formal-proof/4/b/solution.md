<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Denote the columns by $c_1,\ldots,c_4$. The first two are [linearly independent](../../../../../linear-independence.md), because the top two coordinates have [determinant](../../../../../determinant.md) $3\cdot2-(-1)\cdot1=7$. Direct calculation gives

$$
c_3=\frac17c_1-\frac47c_2,\qquad c_4=\frac57c_1+\frac17c_2.
$$

Thus a [column-space basis](../../../../../column-space-basis.md) is **$\{(3,1,9)^T,(-1,2,4)^T\}$**, and

$$
\boxed{\operatorname{Col}(A)=\operatorname{span}\{c_1,c_2\}=\{(u,v,2u+3v)^T:u,v\in\mathbb R\}.}
$$

For the last description, the third row equals twice the first row plus three times the second, so every column lies in that plane. Since the two independent columns already span a two-dimensional [vector subspace](../../../../../vector-subspace.md), they fill the plane.

The target vector satisfies $5=2(-2)+3(3)$, so it is in the [column space](../../../../../column-space.md). An especially simple [linear combination](../../../../../linear-combination.md) is

$$
\boxed{\mathbf b=c_2-c_3=(-1,2,4)^T-(1,-1,-1)^T=(-2,3,5)^T.}
$$

In terms of the displayed [basis](../../../../../basis.md), the same vector is $-c_1/7+11c_2/7$. The [column space](../../../../../column-space.md) itself is unique; the freedom is in choosing its [basis](../../../../../basis.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
