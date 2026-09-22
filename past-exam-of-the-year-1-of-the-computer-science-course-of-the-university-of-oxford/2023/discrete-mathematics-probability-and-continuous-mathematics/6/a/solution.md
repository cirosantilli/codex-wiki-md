<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md) is

$$
\boxed{g(x)=x-\frac{f(x)}{f'(x)}.}
$$

It requires $f$ and its [derivative](../../../../../derivative.md) to be defined at the current point, and requires $f'(x)\ne0$. A step can leave the domain, making a subsequent iteration undefined. In [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), division by zero, overflow or non-finite function evaluations can also prevent a usable step. At a root where $f'$ is zero the displayed quotient itself remains undefined unless the implementation stops before evaluating it.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
