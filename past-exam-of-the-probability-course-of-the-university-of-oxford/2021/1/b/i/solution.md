<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $\delta>0$. Once $|c_n-c|<\delta$, the following event inclusions hold outside $\{|X_n-X|>\delta\}$:

$$
\{X\leq c-2\delta\}\subseteq\{X_n\leq c_n\}\subseteq\{X\leq c+2\delta\}.
$$

Taking [probabilities](../../../../../probability.md) gives the explicit bounds

$$
F(c-2\delta)-\mathbb P(|X_n-X|>\delta)\leq F_n(c_n)\leq F(c+2\delta)+\mathbb P(|X_n-X|>\delta).
$$

By the assumed [convergence in probability](../../../../../convergence-in-probability.md), the error tends to zero. Therefore

$$
F(c-2\delta)\leq\liminf_nF_n(c_n)\leq\limsup_nF_n(c_n)\leq F(c+2\delta).
$$

The [continuity](../../../../../continuous-function.md) of the [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F$ at $c$ lets $\delta$ decrease to zero, proving $\boxed{F_n(c_n)\to F(c).}$ This proves the needed implication directly, without invoking any theorem comparing [convergence of random variables](../../../../../convergence-of-random-variables-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
