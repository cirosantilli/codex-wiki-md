<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The three answers, in source order, are:
- **$T(n)=\Theta(n^2)$.** In the [Master theorem](../../../../../master-theorem.md), $a=6$, $b=3$, and $n^2$ grows polynomially faster than $n^{\log_3 6}$. The regularity condition holds because $6(n/3)^2=(2/3)n^2$. For powers of three, expansion even gives $T(n)=3n^2-2n^{\log_3 6}$.
- **$T(n)=n^2$, and hence $\Theta(n^2)$.** The [telescoping sum](../../../../../telescoping-sum.md) is $T(n)=1+\sum_{j=2}^n(2j-1)=\sum_{j=1}^n(2j-1)=n^2$.
- **$T(n)=\Theta(n^{\log_2 3})$.** Set $m=n-2$ and $U(m)=T(m+2)$. Then $U(m)=3U(m/2)+m+2$, with constant base cost for $m\leq2$. The [Master theorem](../../../../../master-theorem.md) with $a=3$, $b=2$ applies because $m+2=\Theta(m)$ is polynomially smaller than $m^{\log_2 3}$. Finally $m=n-2=\Theta(n)$.

The change of variable in the third case handles the additive shift in the recursive argument exactly; it is not an unjustified deletion of the `+1`. These [Big theta notation](../../../../../big-theta-notation.md) conclusions use the usual admissible input sizes, or bounded integer rounding of subproblem sizes.

## ↑ Ancestors (12)

1. [A](../a.md)
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
