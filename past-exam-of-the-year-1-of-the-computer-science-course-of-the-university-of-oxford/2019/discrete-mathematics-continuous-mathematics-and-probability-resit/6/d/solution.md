<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For iterates approaching $\mathbf x_*$, write $e_k=\|\mathbf x_k-\mathbf x_*\|$. Exact [order of convergence](../../../../../order-of-convergence.md) $p$ means $e_{k+1}/e_k^p\to C$ for a finite constant $C>0$, with nonzero errors. Thus **[quadratic convergence](../../../../../quadratic-convergence.md) has $p=2$, and [cubic convergence](../../../../../cubic-convergence.md) has $p=3$**. The weaker eventual bound $e_{k+1}\leq Ce_k^p$ means at least order $p$. Finite termination is a separate case.[§3.8(i), equation 3.8.3 and its order-of-convergence discussion](../../../../../nist-digital-library-of-mathematical-functions/3-8-nonlinear-equations.md)

The assertion about being always faster is **false**. For example, the [fixed-point iterations](../../../../../fixed-point-iteration.md) with errors $e_{k+1}=e_k^2$ and $d_{k+1}=50d_k^3$ have exact [quadratic convergence](../../../../../quadratic-convergence.md) and [cubic convergence](../../../../../cubic-convergence.md), respectively. Starting both at $0.1$, their next errors are $0.01$ and $0.05$: the [cubic convergence](../../../../../cubic-convergence.md) method is worse on that step, although both converge. Error constants, starting points, and work per step all matter. The higher [order of convergence](../../../../../order-of-convergence.md) describes asymptotic behavior within a convergence region, not a uniform comparison of all computations.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
