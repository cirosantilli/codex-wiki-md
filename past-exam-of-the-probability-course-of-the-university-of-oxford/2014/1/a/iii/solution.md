<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The implication [convergence in probability implies convergence in distribution](../../../../../convergence-in-probability-implies-convergence-in-distribution.md) follows by comparing nearby [events](../../../../../event.md). Fix a [continuity](../../../../../continuous-function.md) point $x$ of the [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F_X$ and let $\varepsilon>0$. If $X\leq x-\varepsilon$ and $|X_n-X|\leq\varepsilon$, then $X_n\leq x$. Conversely, $X_n\leq x$ and $|X_n-X|\leq\varepsilon$ imply $X\leq x+\varepsilon$. Thus

$$
F_X(x-\varepsilon)-\mathbb P(|X_n-X|>\varepsilon)
\leq F_{X_n}(x)
\leq F_X(x+\varepsilon)+\mathbb P(|X_n-X|>\varepsilon).
$$

The error [probability](../../../../../probability.md) tends to zero by [convergence in probability](../../../../../convergence-in-probability.md). Taking lower and upper [limits](../../../../../limit-of-a-function.md) and then letting $\varepsilon\downarrow0$, [continuity](../../../../../continuous-function.md) at $x$ squeezes both bounds to $F_X(x)$. This is exactly [convergence in distribution](../../../../../convergence-in-distribution.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
