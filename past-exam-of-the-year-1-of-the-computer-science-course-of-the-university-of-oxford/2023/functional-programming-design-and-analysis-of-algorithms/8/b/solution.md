<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**$\Theta(n^{\log_2 7})$, approximately $\Theta(n^{2.8074})$, arithmetic operations.** [Strassen's algorithm](../../../../../strassen-s-algorithm.md) replaces an $n\times n$ [matrix multiplication](../../../../../matrix-multiplication.md) by seven products of half-size blocks and a constant number of block additions and subtractions. Consequently

$$
T(n)=7T(n/2)+\Theta(n^2),\qquad T(1)=\Theta(1).
$$

The [Master theorem](../../../../../master-theorem.md) applies with $a=7$, $b=2$, since $2<\log_2 7$. Padding an arbitrary matrix dimension to the next power of two changes the dimension by less than a factor of two and preserves this asymptotic bound. The cost model counts scalar arithmetic as constant time; it is not a bit-complexity claim for arbitrarily large integer entries.

## ↑ Ancestors (12)

1. [B](../b.md)
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
