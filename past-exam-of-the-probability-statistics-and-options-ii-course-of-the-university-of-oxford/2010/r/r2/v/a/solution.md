<h1 id="r/r2/v/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The sum of degrees is twice the number of [edges](../../../../../../edge-of-a-graph.md), so

$$
l+r(n-l)=2(n-1).
$$

For $r\ge2$ this gives

$$
\boxed{n-l=\frac{n-2}{r-1},\qquad l=n-\frac{n-2}{r-1}=\frac{n(r-2)+2}{r-1}.}
$$

Necessity of the divisibility condition follows. Conversely, when $r-1\mid n-2$, choose $k=(n-2)/(r-1)$ internal labels and form a [Prüfer sequence](../../../../../../prufer-sequence.md) in which each of them appears exactly $r-1$ times. Its length is $n-2$; all other labels are absent. The decoded [tree](../../../../../../tree-graph-theory-split.md) has [degree](../../../../../../degree-graph-theory.md) $r$ at the chosen labels and [degree](../../../../../../degree-graph-theory.md) one elsewhere. Thus the divisibility condition is sufficient, with the displayed [leaf of a graph](../../../../../../leaf-of-a-graph.md) count. For $n=2$ the code is empty and the sole [edge](../../../../../../edge-of-a-graph.md) works, with no internal [vertices](../../../../../../vertex-graph-theory.md).

The division assumes $r\ge2$. If $r=1$, all [vertices](../../../../../../vertex-graph-theory.md) would have [degree](../../../../../../degree-graph-theory.md) one, and the only [connected](../../../../../../connected-space.md) [tree](../../../../../../tree-graph-theory-split.md) with $n\ge2$ is the two-[vertex](../../../../../../vertex-graph-theory.md) [edge](../../../../../../edge-of-a-graph.md). This separate case is not expressed by division by $r-1$.

## ↑ Ancestors (14)

1. [A](../a.md)
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
