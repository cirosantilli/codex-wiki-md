<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0\leq k\leq n$, the event $\{X=k,X+Y=n\}$ is $\{X=k,Y=n-k\}$. Use [independence](../../../../../../independent-random-variables.md) in its numerator and the [Poisson distribution](../../../../../../poisson-distribution.md) of the sum in its denominator:

$$
\begin{aligned}
\mathbb P(X=k\mid X+Y=n)
&=\frac{e^{-\lambda}\lambda^k/k!\;e^{-\mu}\mu^{n-k}/(n-k)!}{e^{-(\lambda+\mu)}(\lambda+\mu)^n/n!}\\
&=\boxed{\binom nk\left(\frac\lambda{\lambda+\mu}\right)^k\left(\frac\mu{\lambda+\mu}\right)^{n-k}}.
\end{aligned}
$$

Outside $0\leq k\leq n$ the conditional probability is zero. Consequently

$$
\boxed{X\mid(X+Y=n)\sim\operatorname{Bin}\!\left(n,\frac\lambda{\lambda+\mu}\right)}.
$$

This [binomial distribution](../../../../../../binomial-distribution.md) includes $n=0$, when it is concentrated at zero. Conditioning on the total converts the independent counts into an allocation of that total between the two rates.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
