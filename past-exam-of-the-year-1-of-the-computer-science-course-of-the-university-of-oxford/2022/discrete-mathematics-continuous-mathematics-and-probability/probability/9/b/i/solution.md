<h1 id="probability/9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $M_n=\max_iE_i$. Each [exponential distribution](../../../../../../../exponential-distribution.md) has [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) $1-e^{-x}$ for $x\ge0$. Independence therefore gives the [maximum of independent exponential random variables](../../../../../../../maximum-of-independent-exponential-random-variables.md) formula

$$
\boxed{\mathbb P(M_n\le x)=\begin{cases}0,&x<0,\\(1-e^{-x})^n,&x\ge0.\end{cases}}
$$

For any fixed $y$, the threshold $y+\ln n$ is nonnegative for all sufficiently large $n$. Then

$$
\mathbb P(M_n-\ln n\le y)=\left(1-\frac{e^{-y}}n\right)^n\longrightarrow\boxed{\exp(-e^{-y})}.
$$

This is [convergence in distribution](../../../../../../../convergence-in-distribution.md) to the standard [Gumbel distribution](../../../../../../../gumbel-distribution.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Probability](../../../../probability.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
