<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $x_i$ be the number in box $i$ and put $y_i=x_i-1$. We count [integer compositions](../../../../../composition-of-an-integer.md) satisfying $y_1+\cdots+y_4=6$ and $0\leq y_i\leq4$. Without the upper bounds, [stars and bars](../../../../../stars-and-bars-combinatorics.md) gives $\binom93=84$. If a specified $y_i\geq5$, subtract five from it; the remaining [nonnegative integer](../../../../../natural-number.md) variables sum to one, giving $\binom43=4$ possibilities. Two violations cannot occur because they would require a sum at least ten. The [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) therefore gives

$$
\boxed{\binom93-4\binom43=84-16=68.}
$$

The boxes are distinguished by their positions in the composition; individual objects are not distinguished.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
