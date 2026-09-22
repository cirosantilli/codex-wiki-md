<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Zero-stability](../../../../../zero-stability.md) means that perturbations of the starting values of the zero-step recurrence remain bounded by a fixed multiple of their initial size, uniformly as the number of steps tends to infinity on a fixed time interval. In particular solutions of $\sum_{j=0}^k\alpha_je_{n+j}=0$ obey $\max_{n\leq N}|e_n|\leq C\max_{j<k}|e_j|$ with $C$ independent of $N$.

The equivalent [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) is

$$
\boxed{\text{Every root of }\rho(\zeta)\text{ has }|\zeta|\leq1,\text{ and roots with }|\zeta|=1\text{ are simple}.}
$$

A root outside the unit circle gives exponential growth of a [recurrence relation](../../../../../recurrence-relation.md) mode; a repeated root on it gives polynomial growth. Repeated roots strictly inside it are harmless because their polynomial factor is dominated by decay.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
