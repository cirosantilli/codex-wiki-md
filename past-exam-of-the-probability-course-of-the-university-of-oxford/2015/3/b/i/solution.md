<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $q=1-p$ and $\xi_i=Y_i-Y_{i-1}$. The [Markov property](../../../../../markov-property.md) and the state-independent transition probabilities show that, conditional on the whole previous history, $\xi_i$ is $+1$ with [probability](../../../../../probability.md) $p$ and $-1$ with [probability](../../../../../probability.md) $q$. Multiplying these conditional probabilities for any finite step sequence proves that the $\xi_i$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md), with

$$
\mathbb E\xi_i=p-q=2p-1>0.
$$

Because $Y_n=k+\sum_{i=1}^n\xi_i$, the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives

$$
\boxed{\frac{Y_n}{n}=\frac kn+\frac1n\sum_{i=1}^n\xi_i
\xrightarrow{\mathrm{a.s.}}\mu=2p-1.}
$$

In particular, $Y_n\to+\infty$ [almost surely](../../../../../almost-sure-convergence.md). This stronger pathwise consequence will determine both eventual crossings and the asymptotic [first-passage times](../../../../../first-passage-time.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
