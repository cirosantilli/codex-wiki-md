<h1 id="s/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md), choose a proposal transition $q(x,y)$ and initialize at a state with $\pi(x)>0$. From current $x$, propose $Y\sim q(x,\cdot)$ and accept it with [probability](../../../../../probability.md)

$$
\boxed{\alpha(x,Y)=\min\left\{1,\frac{\pi(Y)q(Y,x)}{\pi(x)q(x,Y)}\right\}.}
$$

Otherwise stay at $x$. The accepted off-diagonal transition satisfies [detailed balance](../../../../../detailed-balance.md), since $\pi(x)q(x,y)\alpha(x,y)=\min\{\pi(x)q(x,y),\pi(y)q(y,x)\}$ is symmetric in $x,y$. Thus $\pi$ is stationary. For convergence from arbitrary starting states in the support, choose the proposal so the resulting chain is [irreducible](../../../../../irreducible-representation.md) and aperiodic. Only ratios of target probabilities are needed, so an unknown normalizing constant cancels.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
