<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the time `print(n)` is called, `record` has evaluated `divisors(i)` once for every $1\leq i\leq n$. In the [unit-cost model](../../../../../unit-cost-model.md), the total number of remainder tests is

$$
\sum_{i=1}^{n}i=\frac{n(n+1)}2.
$$

The [record values](../../../../../record-value.md) comparisons add only $O(n)$ work, and output is cheap by assumption. **The elapsed time is $\Theta(n^2)$.** This measures time to reach a given [highly composite number](../../../../../highly-composite-number.md), rather than time as a function of the number of printed records.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
