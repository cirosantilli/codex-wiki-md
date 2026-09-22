<h1 id="3/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Unroll the [recurrence relation](../../../../../../recurrence-relation.md) down to its [initial condition](../../../../../../initial-condition.md):

$$
T(n)=T(0)+\sum_{j=1}^{n}j=1+\frac{n(n+1)}2.
$$

Thus

$$
\boxed{T(n)=1+\frac{n(n+1)}2=O(n^2)}.
$$

Indeed $T(n)/n^2\to1/2$, so the sharper growth classification is $\Theta(n^2)$ in [big theta notation](../../../../../../big-theta-notation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
