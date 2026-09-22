<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $A_k=N_{2k}-N_k$ and $B_k=N_k$. The [stationary increments](../../../../../stationary-increments.md) and [independent increments](../../../../../independent-increments.md) of the [Poisson process](../../../../../poisson-process-split.md) make $A_k$ and $B_k$ [independent random variables](../../../../../independent-random-variables.md), each with [Poisson distribution](../../../../../poisson-distribution.md) of parameter $k$. Thus

$$
\frac{N_{2k}-2N_k}{\sqrt{k}}=\frac{A_k-B_k}{\sqrt{k}}.
$$

Multiplication of the two [moment-generating functions](../../../../../moment-generating-function.md) gives

$$
M_k(t)=\exp\!\left\{k\left(e^{t/\sqrt{k}}+e^{-t/\sqrt{k}}-2\right)\right\}.
$$

The odd terms cancel in [Taylor's theorem](../../../../../taylor-s-theorem.md), so $\log M_k(t)=t^2+O(k^{-1})$. The limit $e^{t^2}$ is the [moment-generating function of a normal distribution](../../../../../moment-generating-function-of-a-normal-distribution.md) with [mean](../../../../../expected-value-split.md) zero and [variance](../../../../../variance-split.md) two. The same [continuity theorem for moment-generating functions](../../../../../convergence-theorem-for-moment-generating-functions.md) therefore yields

$$
\boxed{\frac{N_{2k}-2N_k}{\sqrt{k}}\xrightarrow{\mathrm d}N(0,2).}
$$

In particular, the two equal-length increments must be separated before using [independence](../../../../../independent-random-variables.md): $N_{2k}$ and $N_k$ themselves are dependent.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
