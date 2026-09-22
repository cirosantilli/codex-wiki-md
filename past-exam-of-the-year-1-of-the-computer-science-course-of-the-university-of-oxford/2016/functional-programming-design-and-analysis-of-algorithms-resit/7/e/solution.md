<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use [greedy coin change for powers of an integer](../../../../../greedy-coin-change-for-powers-of-an-integer.md), with integer $p\geq2$. In any optimal solution, there can be no $p$ or more stamps of denomination $p^j$ for $j<k$: replacing $p$ of them by one stamp $p^{j+1}$ preserves value and reduces the stamp count by $p-1$.

Consequently each lower-denomination count lies in $\{0,\ldots,p-1\}$, and their total value is at most

$$
(p-1)(1+p+\cdots+p^{k-1})=p^k-1<p^k.
$$

The number of largest stamps must therefore be $\lfloor m/p^k\rfloor$, leaving a residual below $p^k$. Apply the same argument successively to lower powers. This forces exactly the greedy quotients, proving optimality. For $k=0$, only unit stamps are available and the conclusion is immediate. Integer $p$ is essential to the carry argument and follows from the stated integer denominations whenever denomination $p$ is present.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
