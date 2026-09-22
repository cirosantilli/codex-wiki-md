<h1 id="u/u2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For scalar minimization, apply Newton's root-finding method to the stationarity equation $f'(x)=0$. Linearize $f'$ at the current point to obtain

$$
\boxed{x_{k+1}=x_k-\frac{f'(x_k)}{f''(x_k)}.}
$$

The iteration requires $f''(x_k)\ne0$. Near a nondegenerate [local minimum](../../../../../../local-minimum.md), where $f'(x_*)=0$, $f''(x_*)>0$, suitable smoothness and a sufficiently close starting value give local convergence. A stationary limit must still be checked to be a [minimum](../../../../../../local-minimum.md). This undamped method is not globally convergent and need not decrease $f$ at every step.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [U2](../../../u2.md)
4. [U](../../../../u.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
