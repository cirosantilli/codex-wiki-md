<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the one-step [local truncation error](../../../../../../local-truncation-error.md) as the defect obtained by inserting the exact solution into an update:

$$
\delta_{n+1}=y(x_n+h)-y(x_n)-h f(x_n,y(x_n)).
$$

For a smooth solution, [Taylor's theorem](../../../../../../taylor-s-theorem.md) and $y'=f(x,y)$ give

$$
\boxed{\delta_{n+1}=\frac{h^2}{2}y''(x_n)+O(h^3)=O(h^2).}
$$

Thus **$m=2$ for the one-step defect convention**. The leading derivative can also be written $y''=f_x+f_yf$ by the chain rule.

Some conventions instead call $\tau_{n+1}=\delta_{n+1}/h$ the truncation error. That [normalized local truncation error](../../../../../../normalized-local-truncation-error.md) is $O(h)$, so **$m=1$ under the normalized convention**. Both describe the same [Euler one-step defect](../../../../../../euler-one-step-defect.md); neither should be confused with an unqualified global error claim.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
