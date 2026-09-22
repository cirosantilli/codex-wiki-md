<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the intended model of independent [Bernoulli trials](../../../../../bernoulli-trial.md), with the same scoring probability $p$ for every shot. Equal marginal scoring probabilities alone would not establish the stated formula without independence. Let $N_1,N_2$ count misses in the two groups of five. They are [independent random variables](../../../../../independent-random-variables.md) with [binomial distribution](../../../../../binomial-distribution.md) $\operatorname{Bin}(5,1-p)$. A tie occurs precisely when $N_1=N_2=n$ for one of the mutually exclusive possibilities $n=0,\ldots,5$. Therefore the [tie probability for independent binomial counts](../../../../../tie-probability-for-independent-binomial-counts.md) is

$$
\boxed{\alpha=\sum_{n=0}^5\binom5n^2(1-p)^{2n}p^{10-2n}.}
$$

At $p=1/2$, [Vandermonde's identity](../../../../../vandermonde-s-identity.md) gives $\sum_n\binom5n^2=\binom{10}5=252$, so

$$
\boxed{\alpha=\frac{252}{1024}=\frac{63}{256}.}
$$

Exchanging the two teams preserves the distribution and interchanges the two winning events. Their total probability is $1-\alpha$, so **the first team wins at the end of the initial period with probability $193/512$**. In this model the shooting order gives no advantage.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
