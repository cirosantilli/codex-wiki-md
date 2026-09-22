<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [filter on a set](../../../../../filter-set-theory.md) $I$ means a proper family $\mathcal F\subseteq\mathcal P(I)$ with $I\in\mathcal F$, $\varnothing\notin\mathcal F$, closure under finite intersections, and upward closure under inclusion. An [ultrafilter](../../../../../ultrafilter.md) is a maximal proper filter; equivalently, for every $X\subseteq I$, exactly one of $X$ and $I\setminus X$ belongs to it. A [principal ultrafilter](../../../../../principal-ultrafilter.md) is $\{X\subseteq I:i\in X\}$ for some $i\in I$. A [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) is one not of that form, equivalently one containing no finite set.

To prove the [ultrafilter lemma](../../../../../ultrafilter-lemma.md) using [Zorn's lemma](../../../../../zorn-s-lemma.md), order all proper filters containing $\mathcal F$ by inclusion. The union of any chain is a proper filter: finitely many members lie together in one filter of the chain, and no chain member contains the empty set. Thus every chain has an upper bound, and Zorn's lemma gives a maximal member $\mathcal U$.

For completeness, its decision property follows from maximality. If $X\notin\mathcal U$, adjoining $X$ cannot generate a proper filter. Hence some $F\in\mathcal U$ has $F\cap X=\varnothing$. Upward closure gives $I\setminus X\in\mathcal U$. Both complements cannot be members, since their intersection is empty. Therefore $\boxed{\mathcal F\subseteq\mathcal U\text{ for an ultrafilter }\mathcal U}$. Properness is essential; a family containing the empty set cannot extend to an [ultrafilter](../../../../../ultrafilter.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
