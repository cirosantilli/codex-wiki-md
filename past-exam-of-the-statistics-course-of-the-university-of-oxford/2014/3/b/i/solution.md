<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $s=\sum_ix_i$, $A=a+s$ and $B=b+n$. Conditional independence gives the [Poisson distribution](../../../../../poisson-distribution.md)'s [likelihood](../../../../../likelihood-function.md)

$$
L(\theta;x)=\frac{\theta^s e^{-n\theta}}{\prod_ix_i!}.
$$

Multiply by the prior [gamma distribution](../../../../../gamma-distribution.md)'s density and discard factors independent of $\theta$:

$$
\pi(\theta\mid x)\propto\theta^{a+s-1}e^{-(b+n)\theta}.
$$

Normalizing with the [gamma function](../../../../../gamma-function.md) identifies

$$
\boxed{\theta\mid x\sim\operatorname{Gamma}(A,B),\qquad
\pi(\theta\mid x)=\frac{B^A}{\Gamma(A)}\theta^{A-1}e^{-B\theta},\quad\theta>0.}
$$

Here $A=a+s$ is the shape and $B=b+n$ is the rate, not the scale. This is [conjugate prior](../../../../../conjugate-prior.md) updating for a [Poisson distribution](../../../../../poisson-distribution.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
