<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $A=a+\sum_ix_i$ and $B=b+n$ as above. The future observation is independent of the old observations conditional on $\theta$, so the [posterior predictive probability](../../../../posterior-predictive-probability.md) is obtained by integrating its [Poisson distribution](../../../../poisson-distribution.md) against the [posterior distribution](../../../../bayesian-posterior.md) of $\theta$:

$$
\begin{aligned}
\Pr(X_{n+1}=k\mid x)
&=\int_0^\infty\frac{e^{-\theta}\theta^k}{k!}\frac{B^A}{\Gamma(A)}\theta^{A-1}e^{-B\theta}\,d\theta\\
&=\frac{B^A}{\Gamma(A)k!}\int_0^\infty\theta^{A+k-1}e^{-(B+1)\theta}\,d\theta\\
&=\boxed{\frac{\Gamma(A+k)}{\Gamma(A)k!}\left(\frac B{B+1}\right)^A
\left(\frac1{B+1}\right)^k,\quad k=0,1,\ldots.}
\end{aligned}
$$

The last integral is the normalizing [gamma function](../../../../gamma-function.md) integral, equal to $\Gamma(A+k)/(B+1)^{A+k}$. This is a [negative binomial distribution](../../../../negative-binomial-distribution.md) in the count-of-failures convention with shape $A$ and success probability $B/(B+1)$; the gamma-function expression remains valid for noninteger $A>0$. As checks, its [mean](../../../../expected-value-split.md) is $A/B$, and the [law of total variance](../../../../law-of-total-variance.md) gives [variance](../../../../variance-split.md) $A/B+A/B^2$. The additional term is the contribution of posterior uncertainty in $\theta$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
