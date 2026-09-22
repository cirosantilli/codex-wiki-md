<h1 id="s/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Start at any integer $x\geq2$, for example two. Propose $x+1$ or $x-1$ with [probability](../../../../../probability.md) $1/2$ each; if the proposal is one, reject it immediately. Between distinct valid neighboring states the proposal is symmetric. The [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md) for an upward proposal is

$$
\boxed{\alpha_+(x)=\min\{1,\tfrac{x}{x-1}(1-p)\}.}
$$

For a downward proposal from $x\geq3$, it is

$$
\boxed{\alpha_-(x)=\min\{1,\tfrac{x-2}{(x-1)(1-p)}\}.}
$$

These are exactly the ratios of the supplied [negative binomial distribution](../../../../../negative-binomial-distribution.md) probabilities; the factor $p^2$ cancels. The rejection at the boundary supplies a self-loop at two. All neighboring positive states communicate, so the chain is [irreducible](../../../../../irreducible-representation.md) and aperiodic. Detailed balance gives the desired stationary law. Rejecting the invalid move, rather than forcing an upward move at two, preserves the proposal symmetry used in these ratios.

## ↑ Ancestors (13)

1. [B](../b.md)
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
