<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $m=r+s$ and $\beta=\lambda+n$. Conditional independence of the next count given $\theta$ allows us to average its [Poisson distribution](../../../../poisson-distribution.md) over the [posterior distribution](../../../../bayesian-posterior.md):

$$
\begin{aligned}
\mathbb P(X_{n+1}=k\mid\boldsymbol x)&=\int_0^\infty\frac{e^{-\theta}\theta^k}{k!}\frac{\beta^m}{\Gamma(m)}\theta^{m-1}e^{-\beta\theta}\,d\theta\\
&=\frac{\Gamma(k+m)}{\Gamma(m)k!}\frac{\beta^m}{(\beta+1)^{k+m}}\\
&=\binom{k+m-1}{k}\left(\frac\beta{\beta+1}\right)^m\left(\frac1{\beta+1}\right)^k.
\end{aligned}
$$

This [Poisson-gamma mixture](../../../../poisson-gamma-mixture.md) is the [posterior predictive distribution](../../../../posterior-predictive-distribution.md). In the stated [negative binomial distribution](../../../../negative-binomial-distribution.md) convention its parameters are

$$
\boxed{m=r+\sum_i x_i,\qquad p=\frac{\lambda+n}{\lambda+n+1}}.
$$

Its [expected value](../../../../expected-value-split.md) $m/\beta$ equals the [posterior mean](../../../../posterior-mean.md) of $\theta$, while its [variance](../../../../variance-split.md) $m/\beta+m/\beta^2$ includes both conditional Poisson variation and uncertainty in $\theta$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
