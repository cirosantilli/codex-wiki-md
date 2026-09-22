<h1 id="r/r2/v/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First choose the $l$ absent labels, which will be the [leaves of a graph](../../../../../../leaf-of-a-graph.md), in $\binom nl$ ways. Every other label must occur exactly $r-1$ times in the [Prüfer sequence](../../../../../../prufer-sequence.md). There are $n-l$ such labels and their total multiplicity is $n-2$ by (a). The number of orderings of this [multiset](../../../../../../multiset.md) is $(n-2)!/((r-1)!)^{n-l}$. The [bijection](../../../../../../bijection.md) in (i) turns each ordering into one distinct [labelled tree](../../../../../../labelled-tree.md) and exhausts all possibilities. Therefore

$$
\boxed{\binom nl\frac{(n-2)!}{((r-1)!)^{n-l}}.}
$$

The formula is used with the feasible integer parameters from (a), and gives one for the two-[vertex](../../../../../../vertex-graph-theory.md) [edge](../../../../../../edge-of-a-graph.md) with no internal labels.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [V](../../v.md)
3. [R2](../../../r2.md)
4. [R](../../../../r.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
