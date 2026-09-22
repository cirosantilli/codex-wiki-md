<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An allocation is a [tuple](../../../../../finite-tuple.md) $(x_1,\ldots,x_k)$ of nonnegative [integers](../../../../../integer-split.md) with $\sum_jx_j=n$, where $x_j$ is the number in labelled box $j$. Empty boxes are allowed. Encode the allocation by $n$ stars and $k-1$ bars: put $x_1$ stars before the first bar, $x_2$ between the first two bars, and so on. Adjacent bars represent an empty intermediate box; a bar at an end represents an empty end box.

Reading the group sizes recovers exactly one allocation from every such string, so this is a [bijection](../../../../../bijection.md). There are $n+k-1$ positions and we choose the $k-1$ bar positions. Hence [stars and bars](../../../../../stars-and-bars-combinatorics.md) gives

$$
\boxed{\binom{n+k-1}{k-1}.}
$$

No extra factor for ordering the objects is present, because the objects are indistinguishable. For $k=1$ the string has no bars and gives the single allocation of all objects to that box; for $n=0$ all boxes are empty, also a single allocation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
