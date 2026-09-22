<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For input length $n$, the successive [list concatenations](../../../../../list-concatenation.md) copy prefixes of lengths $0,1,\ldots,n-1$. Thus $T(n)=T(n-1)+\Theta(n)$ and $T(n)=\Theta(1+\sum_{j=0}^{n-1}(j+1))$. **The direct implementation takes $\Theta(n^2)$ time** for a fully produced nonempty reversal. The repeated copying, rather than the number of recursive calls alone, causes the quadratic cost.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
