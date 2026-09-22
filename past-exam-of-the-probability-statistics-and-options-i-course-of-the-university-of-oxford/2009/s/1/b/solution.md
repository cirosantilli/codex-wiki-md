<h1 id="s/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the prior itself as an [independence](../../../../../independent-random-variables.md) proposal: draw $J\geq1$ with $\mathbb P(J=j)=2^{-j}$ and propose $s=2^{-J}$. This indeed samples $p(s)=s$, since the geometric series sums to one. Starting from any allowed current value $r$, accept the proposal with probability

$$
\boxed{\min\left\{1,\left(\frac sr\right)^x
\left(\frac{1-s}{1-r}\right)^{n-x}\right\}.}
$$

The Hastings proposal ratio cancels the prior ratio in the posterior, leaving exactly the binomial [likelihood](../../../../../likelihood-function.md) ratio; its binomial coefficient also cancels. All allowed states communicate, and proposing the current state gives a self-loop. Detailed balance therefore gives the specified posterior as the stationary law, and the chain converges to it. Its normalizing constant is finite and positive because it is a prior average of a nonnegative, nonzero [likelihood](../../../../../likelihood-function.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
