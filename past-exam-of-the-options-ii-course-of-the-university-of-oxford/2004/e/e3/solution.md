<h1 id="e/e3/solution">Solution</h1>

↑ **Parent:** [E3](../e3.md)

The nested closed sets have the [finite intersection property](../../../../finite-intersection-property.md): the intersection of finitely many is the one with the largest index and is nonempty. Compactness gives $\boxed{Y_\infty\ne\varnothing}$.

For an open neighbourhood $W$ of the intersection, suppose no $Y_n$ were contained in $W$. Then $Z_n=Y_n\cap(X\setminus W)$ would be nested, nonempty and closed. The same argument gives a point in all $Z_n$, contradicting $Y_\infty\subseteq W$. Hence

$$
\boxed{Y_n\subseteq W\text{ for some }n.}
$$

For [connectedness](../../../../connected-space.md), suppose $Y_\infty=A\cup B$ were a separation into two nonempty relatively closed sets. Since $Y_\infty$ is [compact](../../../../compact-space.md), $A,B$ are disjoint [compact](../../../../compact-space.md) subsets of $X$. The supplied separation fact gives disjoint open neighbourhoods $U_A,U_B$. Their union contains $Y_\infty$, so some $Y_n$ lies in that union. But $Y_n$ meets both neighbourhoods, since it contains $A$ and $B$. Its intersections with the two neighbourhoods are then a separation, contradicting its [connectedness](../../../../connected-space.md). Thus **the nested intersection is [connected](../../../../connected-space.md)**.

## ↑ Ancestors (12)

1. [E3](../e3.md)
2. [E](../../e.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
