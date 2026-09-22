<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $q=n/k$. After each linear-time [selection algorithm](../../../../../selection-algorithm.md) and partition, exactly $k$ elements are removed, so the successive input sizes are $n,n-k,\ldots,k$. Thus the standard efficient implementation takes

$$
\Theta\left(\sum_{j=1}^{q}jk\right)
=\Theta\left(k\frac{q(q+1)}2\right)
=\boxed{\Theta(n^2/k)}.
$$

Here selection can use [median of medians](../../../../../median-of-medians.md) for worst-case linear time; a suitable randomised linear-time selection routine gives the same bound in expectation. Merely sorting each remaining array would introduce an avoidable logarithmic factor.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
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
