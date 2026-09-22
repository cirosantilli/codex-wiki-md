<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maintain an [integer](../../../../../integer-split.md) `len`, initially zero, with `len = length xs`:
```
PROCEDURE Add(x: INTEGER);
BEGIN
  ASSERT(len < N);
  u[len] := x;
  len := len+1
END Add;
```
The [precondition](../../../../../precondition.md) is the abstract capacity condition. Appending at the first unused [array index](../../../../../array-index.md) establishes $u[0..\mathrm{len})=xs'$ in constant [running time](../../../../../running-time.md).

If `get(k)` first applies a [comparison sort](../../../../../comparison-sort.md) to all $n=\mathrm{len}$ entries, the [comparison sorting lower bound](../../../../../comparison-sorting-lower-bound.md) gives at least $\lceil\log_2(n!)\rceil=\Omega(n\log n)$ comparisons in the worst case. A [merge sort](../../../../../merge-sort.md) or [heapsort](../../../../../heapsort.md) meets that order, after which indexing costs constant time:

$$
\boxed{\operatorname{add}:\Theta(1),\qquad\operatorname{get}\text{ by comparison sorting}:\Theta(n\log n)\text{ optimally in the worst case}.}
$$

This is a logarithmic factor worse than linear. The qualification to [comparison sorting](../../../../../comparison-sort.md) is necessary: merely saying that keys are [integers](../../../../../integer-split.md) does not prohibit [counting sort](../../../../../counting-sort.md) for a bounded small range or [radix sort](../../../../../radix-sort.md) under suitable machine-key assumptions. The printed assertion of an unavoidable superlinear bound needs the comparison model.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
