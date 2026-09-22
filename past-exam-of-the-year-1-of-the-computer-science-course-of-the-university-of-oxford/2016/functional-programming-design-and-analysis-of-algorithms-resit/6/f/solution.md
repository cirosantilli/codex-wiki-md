<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Precompute the 26 cumulative counts $C[j]=\#\{i:a_i\leq j\}$ using [prefix sums](../../../../../prefix-sum.md). Then

$$
\boxed{\#\{i:c<a_i\leq d\}=C[d]-C[c]\quad\text{if }c<d,}
$$

and the answer is zero if $c\geq d$. Counting and prefix summation take $O(n+26)=O(n)$ preprocessing time and constant storage for this fixed alphabet. Each query uses two indexed reads and one subtraction, hence $O(1)$ time. The guard for $c>d$ prevents a negative answer for an empty interval.

## ↑ Ancestors (12)

1. [F](../f.md)
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
