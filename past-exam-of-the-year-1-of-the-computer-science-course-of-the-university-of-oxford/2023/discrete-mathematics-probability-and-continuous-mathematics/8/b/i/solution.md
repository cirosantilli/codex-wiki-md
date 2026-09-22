<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take an [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md) sequence with **$X_i\sim\operatorname{Bernoulli}(r)$**, independent of $N$. Conditional on $N=n$, the [random sum](../../../../../../random-sum.md) $\sum_{i=1}^nX_i$ has [binomial distribution](../../../../../../binomial-distribution.md) with parameters $n,r$, including the [empty sum](../../../../../../empty-sum.md) at $n=0$. This construction therefore has exactly the prescribed joint law of $(N,Z)$ and represents $Z$ as the required [random sum](../../../../../../random-sum.md).

For a literal representation that retains an already given pair $(N,Z)$, enlarge the [probability space](../../../../../../probability-space-split.md) by auxiliary randomness. Conditional on $N=n,Z=z$, choose uniformly a size-$z$ subset of $\{1,\ldots,n\}$, put ones at those indices and zeros at the others, and append independent [Bernoulli](../../../../../../bernoulli-distribution.md) variables of parameter $r$. Given $N=n$, a specified length-$n$ pattern with $z$ ones has probability $\binom nzr^z(1-r)^{n-z}/\binom nz=r^z(1-r)^{n-z}$. Thus the entire sequence is [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md) and independent of $N$, while its first $N$ terms sum to the original $Z$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
