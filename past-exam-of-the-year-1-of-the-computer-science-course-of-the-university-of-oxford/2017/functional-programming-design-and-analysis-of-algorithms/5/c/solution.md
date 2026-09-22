<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $a\geq1$, $b>1$ and $d\geq0$, a version of the [Master theorem](../../../../../master-theorem.md) states that, with bounded positive base costs,

$$
T(n)=aT(n/b)+\Theta(n^d),\quad p=\log_ba
\quad\Longrightarrow\quad
T(n)=\begin{cases}
\Theta(n^p),&d<p,\\
\Theta(n^p\log n),&d=p,\\
\Theta(n^d),&d>p.
\end{cases}
$$

Usual floors and ceilings preserve these bounds when a sufficiently large constant-size base case ensures strict size decrease.

- $A$: $T_A(n)=3T_A(\lceil2n/3\rceil)+\Theta(1)$, hence **$O(n^{\log_{3/2}3})$**, with exponent approximately $2.7095$. Base cases must include $n\leq2$ because the ceiling otherwise need not decrease.
- $B$: $T_B(n)=9T_B(\lceil n/3\rceil)+O(n^2)$, hence **$O(n^2\log n)$** by comparison with the equality recurrence having $\Theta(n^2)$ overhead. If that overhead is actually quadratic this is also tight; the stated upper bound alone does not establish a matching lower bound.
- $C$: $T_C(n)=3T_C(n-1)+\Theta(1)$, whose expansion is a [geometric series](../../../../../geometric-series.md), hence **$O(3^n)$**, in fact $\Theta(3^n)$ for nonzero base costs. The divide-by-a-constant Master theorem does not apply to a decrement by one.

**$B$ is asymptotically fastest; $C$ is slowest.** Even the quadratic-logarithmic upper bound for $B$ is smaller than the tight polynomial order of $A$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
