<h1 id="m/m5/solution">Solution</h1>

↑ **Parent:** [M5](../m5.md)

A homogeneous [Poisson process](../../../../poisson-process-split.md) of rate $\lambda>0$ is an integer-valued [counting process](../../../../counting-process.md) with $N_0=0$ almost surely, nondecreasing right-continuous paths with unit jumps, and [independent](../../../../independent-random-variables.md) [stationary increments](../../../../stationary-increments.md) satisfying

$$
\boxed{N_t-N_s\sim\operatorname{Poisson}(\lambda(t-s)),\qquad0\leq s<t.}
$$

Increments over disjoint time [intervals](../../../../interval-mathematics.md) are [independent](../../../../independent-random-variables.md). In particular,

$$
\mathbb P(N_t=k)=e^{-\lambda t}\frac{(\lambda t)^k}{k!},\qquad k=0,1,2,\ldots.
$$

The finite Poisson counts ensure that there is no explosion in finite time. The increment formula also gives [stochastic continuity](../../../../stochastic-continuity.md), since the [probability](../../../../probability.md) of any arrival in an [interval](../../../../interval-mathematics.md) of length $h$ is $1-e^{-\lambda h}\to0$.

## ↑ Ancestors (12)

1. [M5](../m5.md)
2. [M](../../m.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
