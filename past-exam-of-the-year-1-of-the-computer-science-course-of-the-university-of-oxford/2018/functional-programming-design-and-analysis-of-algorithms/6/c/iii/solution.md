<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $c\geq2$, use largest-denomination-first [greedy algorithm](../../../../../../greedy-algorithm.md) steps: for $i=n,n-1,\ldots,1$, take $q_i=\lfloor r/c^i\rfloor$ coins and replace the residual amount $r$ by $r-q_ic^i$. A target is representable exactly when it is divisible by $c$, because the smallest denomination is $c$, not one.

To prove optimality whenever the target is representable, observe that an optimum can have fewer than $c$ coins of every denomination $c^i$ with $i<n$: replacing $c$ such coins by one $c^{i+1}$ coin preserves value and reduces the count by $c-1$. After all such carrying, the coefficients of $c,c^2,\ldots,c^{n-1}$ are the unique base-$c$ digits of $v/c$, while the coefficient of $c^n$ is the remaining quotient. Largest-first division produces exactly these coefficients. **The greedy coin count is optimal**, and can be computed with $O(n)$ quotient/remainder operations without listing every coin.

For $c=1$, distinct denominations permit only $n=1$; then all coins have value one and the answer is $v$. This handles the printed positive-integer condition without silently assuming $c>1$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
