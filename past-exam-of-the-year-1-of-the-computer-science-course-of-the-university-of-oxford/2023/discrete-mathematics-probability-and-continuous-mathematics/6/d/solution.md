<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $h=x_{n+1}-x_n=-f(x_n)/f'(x_n)$. By [Taylor's theorem](../../../../../taylor-s-theorem.md),

$$
f(x_{n+1})=f(x_n)+hf'(x_n)+\frac{h^2}{2}f''(\xi).
$$

The first two terms cancel by the definition of the [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md). Thus

$$
\boxed{f(x_{n+1})=\frac{(x_{n+1}-x_n)^2}{2}f''(\xi),}
$$

with $\xi$ between the consecutive iterates. In particular, a nonzero step has negative new residual under the stated strict [concavity](../../../../../concave-function.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
