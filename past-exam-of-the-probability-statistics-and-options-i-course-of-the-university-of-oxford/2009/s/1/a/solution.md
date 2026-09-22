<h1 id="s/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $0<r<1$, start at any $x\in\{0,\ldots,n\}$. Propose $Y$ uniformly from this same finite set and accept it with probability

$$
\boxed{\min\left\{1,\frac{\binom nY}{\binom nx}\left(\frac r{1-r}\right)^{Y-x}\right\}.}
$$

Otherwise retain $x$. The uniform proposal is symmetric, so this is the [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) with target $\pi(\cdot\mid r)$. Detailed balance follows because accepted probability flow is proportional to $\min\{\pi(x),\pi(Y)\}$. The chain is irreducible and has positive self-transition probability, hence converges to that binomial equilibrium law. At the degenerate parameters zero or one, the target is simply a point mass and can be simulated as a constant chain.

## ↑ Ancestors (13)

1. [A](../a.md)
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
