<h1 id="7/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Conditioning on $Z=z$ has positive [probability](../../../../../../probability.md) exactly when $z=2r+1$ for an [integer](../../../../../../integer-split.md) $r\geq0$. This is the same [event](../../../../../../event.md) as $X+Y=r$. The [addition of independent Poisson random variables](../../../../../../addition-of-independent-poisson-random-variables.md) gives a [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $\lambda+\mu$ for the sum. Therefore, for $0\leq t\leq r$,

$$
\begin{aligned}
\mathbb P(X=t\mid Z=2r+1)
&=\frac{e^{-(\lambda+\mu)}\lambda^t\mu^{r-t}/[t!(r-t)!]}
{e^{-(\lambda+\mu)}(\lambda+\mu)^r/r!}\\
&=\binom rt\left(\frac{\lambda}{\lambda+\mu}\right)^t
\left(\frac{\mu}{\lambda+\mu}\right)^{r-t}.
\end{aligned}
$$

Thus **$X\mid\{Z=2r+1\}\sim\operatorname{Binomial}(r,\lambda/(\lambda+\mu))$**. The case $r=0$ is a constant zero [random variable](../../../../../../random-variable-split.md). For even, nonpositive, or noninteger $z$, the conditioning [event](../../../../../../event.md) has zero [probability](../../../../../../probability.md), so an event-conditional [probability distribution](../../../../../../probability-distribution-split.md) is not specified by the quotient formula. This is a two-component case of [Poisson-multinomial conditioning](../../../../../../poisson-multinomial-conditioning.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
