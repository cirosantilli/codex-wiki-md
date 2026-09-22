<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a positive [integer](../../../../../integer-split.md) $x$, $p_G(x)$ counts proper vertex colorings using a labelled palette of $x$ colors. Choose an edge $e=uv$. Proper colorings of $G-e$ divide into those in which $u,v$ have different colors, counted by $p_G(x)$, and those in which they have the same color, counted by $p_{G/e}(x)$. Thus

$$
p_G(x)=p_{G-e}(x)-p_{G/e}(x),
$$

where parallel edges after contraction are suppressed. Induction, using $p_G(x)=x^{|V(G)|}$ for an edgeless [graph](../../../../../graph-split.md), produces a [polynomial](../../../../../polynomial-split.md) agreeing with every [integer](../../../../../integer-split.md) coloring count. The [polynomial](../../../../../polynomial-split.md) is unique because two polynomials agreeing at infinitely many integers are identical.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
