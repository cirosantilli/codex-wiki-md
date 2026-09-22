<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Restrict attention to distinct keys; any [comparison sort](../../../../../comparison-sort.md) must handle these inputs. A deterministic [comparison sort](../../../../../comparison-sort.md) can be represented by a binary [decision tree](../../../../../decision-tree.md): an internal node records a comparison and its two possible outcomes, and a leaf records the final ordering of the input positions.

There are $n!$ possible relative orders. Two different orders cannot finish at the same leaf, since the [algorithm](../../../../../algorithm-split.md) would then output the same ordering of positions for both, making at least one result incorrect. A binary [decision tree](../../../../../decision-tree.md) of height $h$ has at most $2^h$ leaves. Hence

$$
2^h\geq n!,\qquad h\geq\lceil\log_2(n!)\rceil.
$$

Using the given bound, or just the last $\lfloor n/2\rfloor$ factors of $n!$, gives

$$
\boxed{h\in\Omega(n\log n).}
$$

This is a worst-case [comparison sorting lower bound](../../../../../comparison-sorting-lower-bound.md), and [merge sort](../../../../../merge-sort.md) achieves the same order. The result concerns [comparison sorting](../../../../../comparison-sort.md); a procedure that uses numerical digits or bounded integer values has a different computational model.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
