<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $q(x,y)=p(y)$, with fresh proposal randomness independent of the past. For $x,y\in S$, the [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md) is

$$
\alpha(x,y)=\min\left\{1,\frac{p(y)p(x)}{p(x)p(y)}\right\}=1.
$$

Thus $P(x,y)=p(y)$ is independent of $x$, and $X_1,\ldots,X_N$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with [probability distribution](../../../../../probability-distribution-split.md) $p$, even if $X_0$ was chosen arbitrarily in $S$. **The method becomes ordinary [Monte Carlo method](../../../../../monte-carlo-method-split.md) sampling from $p$.** The average of $f(X_1),\ldots,f(X_N)$ is an [unbiased estimator](../../../../../unbiased-estimator.md), with the [variance](../../../../../variance-split.md) stated in part (a). Including an arbitrary initial state would spoil this finite-sample property. This is the [independent stationary proposal lemma](../../../../../independent-stationary-proposal-lemma.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
