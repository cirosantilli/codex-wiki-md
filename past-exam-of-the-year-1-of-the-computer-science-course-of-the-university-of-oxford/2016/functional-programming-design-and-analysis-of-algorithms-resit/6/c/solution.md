<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On $n$ distinct opaque keys, a [comparison sorting](../../../../../comparison-sort.md) algorithm must distinguish all $n!$ input orders. Its [binary decision tree](../../../../../binary-decision-tree.md) has at least $n!$ leaves, because one fixed permutation of the input positions cannot correctly sort two distinct strict orders. A tree of height $h$ has at most $2^h$ leaves. Therefore some input needs

$$
\boxed{h\geq\lceil\log_2(n!)\rceil=\Omega(n\log n)}.
$$

The bound is worst-case and specific to algorithms obtaining order information through binary comparisons; it does not apply to every possible representation of keys.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
