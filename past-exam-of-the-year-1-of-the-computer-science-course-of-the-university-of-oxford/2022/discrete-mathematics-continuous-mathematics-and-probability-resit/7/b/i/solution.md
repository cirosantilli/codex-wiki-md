<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Summing the two nonzero entries with $X=1$ gives

$$
\mathbb P(X=1)=p(1-e^{-p})+pe^{-p}=p.
$$

The remaining [probability](../../../../../../probability.md) is $\mathbb P(X=0)=1-p$, so **$X$ has the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) with parameter $p$**.

For the other marginal, the two entries at $Y=0$ add to $e^{-p}$, the entry at $Y=1$ is $pe^{-p}$, and for $k\geqslant2$ the only nonzero entry is already $e^{-p}p^k/k!$. Thus

$$
\boxed{\mathbb P(Y=k)=e^{-p}\frac{p^k}{k!},\qquad k=0,1,2,\ldots,}
$$

and **$Y$ has the [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $p$**. This also checks normalization of the [joint probability mass function](../../../../../../joint-probability-mass-function.md) by summing the marginal.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
