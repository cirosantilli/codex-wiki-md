<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [minimum spanning tree cut property](../../../../../minimum-spanning-tree-cut-property.md) says: if a [cut of a graph](../../../../../cut-graph-theory.md) respects an edge set $A$ contained in some [minimum spanning tree](../../../../../minimum-spanning-tree.md), a minimum-weight edge across that cut is safe to add to $A$, meaning that some minimum spanning tree contains $A$ together with that edge. Respecting $A$ means no edge of $A$ crosses the cut. In particular, any lightest cut edge belongs to some minimum spanning tree; a uniquely lightest cut edge belongs to every minimum spanning tree.

For the [exchange argument](../../../../../exchange-argument.md), take a minimum spanning tree $T$ containing $A$. If it lacks the chosen edge $e$, add $e$ to create its [fundamental cycle](../../../../../fundamental-cycle.md). The remaining route between $e$'s endpoints crosses the cut at some edge $e'$, with $w(e')\geq w(e)$. Since the cut respects $A$, $e'\notin A$. Replacing $e'$ by $e$ preserves a spanning tree, retains $A$, and cannot increase weight. Hence it is also minimum. Strict inequality would contradict minimality, which gives the unique-lightest assertion.

For an illustration, take a triangle with weights $w(ab)=1$, $w(ac)=2$, $w(bc)=3$. Across the cut $\{a\}\mid\{b,c\}$, $ab$ is the unique lightest edge and must be in every minimum spanning tree. The minimum tree is $\{ab,ac\}$, of weight $3$. With tied light edges, the existence assertion need not mean that every minimum spanning tree contains the particular tied edge chosen.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
