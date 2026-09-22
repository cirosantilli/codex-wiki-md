<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Complete the square in the [joint probability density function](../../../../../joint-probability-density.md):

$$
x^2-2\rho xy+y^2=(x-\rho y)^2+(1-\rho^2)y^2.
$$

The density therefore factors as the standard [normal distribution](../../../../../normal-distribution.md) density for $Y$ times a [normal distribution](../../../../../normal-distribution.md) density in $x$ with mean $\rho y$ and variance $1-\rho^2$. It follows that $\mathbb E[Y]=0$, $\mathbb E[Y^2]=1$, and $\mathbb E[X\mid Y]=\rho Y$. Symmetry gives $\mathbb E[X]=0$. By the [law of total expectation](../../../../../law-of-total-expectation.md),

$$
\mathbb E[XY]=\mathbb E\bigl[Y\mathbb E[X\mid Y]\bigr]=\rho\mathbb E[Y^2]=\rho.
$$

Consequently the [covariance](../../../../../covariance.md) of this [bivariate normal distribution](../../../../../bivariate-normal-distribution.md) is **$\operatorname{Cov}(X,Y)=\rho$**. This calculation derives the result from the given density.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
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
