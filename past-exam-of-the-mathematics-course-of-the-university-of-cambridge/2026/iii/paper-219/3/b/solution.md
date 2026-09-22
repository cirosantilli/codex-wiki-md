<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $D=(y_1,y_2,t)$ and $\nu=(\Delta m,c,A,\tau)$,

$$
p(\theta\mid D)\propto
p(y_1,y_2\mid t,\theta)
\exp\left(-\frac{\Delta t^2}{2\sigma_{\mathrm{prior}}^2}\right)p(\nu).
$$

A [Random-walk Metropolis algorithm](../../../../../../random-walk-metropolis-algorithm.md) proposes $\theta'=\theta+Z$ from a symmetric multivariate normal increment, conveniently using logarithmic coordinates for $A,\tau>0$, and accepts with probability

$$
\min\left\{1,
\frac{p(\theta'\mid D)}{p(\theta\mid D)}
\right\}.
$$

After burn-in, retain a suitably long chain and assess convergence and [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
