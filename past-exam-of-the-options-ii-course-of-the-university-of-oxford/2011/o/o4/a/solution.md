<h1 id="o/o4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Ignoring a factor independent of the parameters, the [likelihood function](../../../../../likelihood-function.md) is

$$
L(\theta)=\prod_{i,j}\theta_{ij}^{n_{ij}},\qquad
\ell(\theta)=\sum_{i,j}n_{ij}\log\theta_{ij}.
$$

Since every count is positive, a boundary value $\theta_{ij}=0$ has zero likelihood. At an interior optimum, a [Lagrange multiplier](../../../../../lagrange-multiplier.md) for $\sum\theta_{ij}=1$ gives $n_{ij}/\theta_{ij}=\lambda$. Summing the resulting $\theta_{ij}=n_{ij}/\lambda$ gives $\lambda=N$, so

$$
\boxed{\widehat\theta_{ij}=\frac{n_{ij}}N.}
$$

The log [likelihood function](../../../../../likelihood-function.md) is strictly concave on the positive simplex, because its [Hessian matrix](../../../../../hessian-matrix.md) is diagonal with entries $-n_{ij}/\theta_{ij}^2<0$. Hence this critical point is the unique global [maximum-likelihood estimate](../../../../../maximum-likelihood-estimation-split.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
