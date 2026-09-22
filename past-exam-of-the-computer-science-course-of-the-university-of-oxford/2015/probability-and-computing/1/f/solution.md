<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For $X$ with [binomial distribution](../../../../../binomial-distribution.md) $B(n,p)$, where $n$ is a nonnegative [integer](../../../../../integer-split.md) and $0\leq p\leq1$, use its [probability mass function](../../../../../probability-mass-function.md) and the [binomial theorem](../../../../../binomial-theorem.md):

$$
\begin{aligned}
M_X(t)&=\mathbb E[e^{tX}]
=\sum_{k=0}^n e^{tk}\binom nk p^k(1-p)^{n-k}\\
&=\sum_{k=0}^n\binom nk (pe^t)^k(1-p)^{n-k}
=\boxed{(1-p+pe^t)^n},\qquad t\in\mathbb R.
\end{aligned}
$$

This [moment-generating function of a binomial distribution](../../../../../moment-generating-function-of-a-binomial-distribution.md) is finite for every real $t$, since the [random variable](../../../../../random-variable-split.md) has finite support. The formula also includes the degenerate cases $p=0$, $p=1$ and $n=0$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
