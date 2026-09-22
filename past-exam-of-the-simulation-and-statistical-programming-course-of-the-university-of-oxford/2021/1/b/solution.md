<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [moment-generating function](../../../../moment-generating-function.md) of a [standard normal distribution](../../../../standard-normal-distribution.md) gives $\mathbb E[e^{tX_j}]=e^{t^2/2}$. Using [independence](../../../../independent-random-variables.md) of the coordinates,

$$
\theta=\mathbb E_p[\phi(X)]=\prod_{j=1}^d\mathbb E[e^{-X_j}]=e^{d/2},\qquad
\mathbb E_p[\phi(X)^2]=\prod_{j=1}^d\mathbb E[e^{-2X_j}]=e^{2d}.
$$

The accepted draws are [independent and identically distributed random variables](../../../../independent-and-identically-distributed-random-variables.md), so their [sample mean](../../../../sample-mean.md) is an [unbiased estimator](../../../../unbiased-estimator.md) and has [variance](../../../../variance-split.md)

$$
\boxed{\operatorname{Var}(\widehat\theta_n^{\mathrm{RS}})=\frac{e^{2d}-e^d}{n}.}
$$

This counts $n$ accepted draws, requiring $n\sigma^d$ proposals in [expectation](../../../../expected-value-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../split.md)
5. [Simulation and statistical programming course of the University of Oxford](../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
