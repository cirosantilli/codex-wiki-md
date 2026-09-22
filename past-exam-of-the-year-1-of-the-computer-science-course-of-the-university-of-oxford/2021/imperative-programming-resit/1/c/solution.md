<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the time the candidate $n$ is emitted, every [positive integer](../../../../../positive-integer.md) $m\leq n$ has been examined. The straightforward [divisor](../../../../../divisor.md) routine makes exactly $m$ remainder tests on $m$. Consequently the total number is

$$
\sum_{m=1}^{n}m=\frac{n(n+1)}2,
$$

and the time is **$\Theta(n^2)$** when remainder tests and the other fixed-width operations have constant cost and printing is cheap. Emitting only record candidates does not avoid computing the [divisor](../../../../../divisor.md) count of the intervening candidates.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
