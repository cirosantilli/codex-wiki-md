<h1 id="m/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Poisson process](../../../../poisson-process-split.md) of rate $\lambda>0$ starts from zero, has independent stationary increments, has unit jumps, and satisfies $N_t-N_s\sim\operatorname{Poisson}(\lambda(t-s))$ for $t>s$. Its inter-arrival times are independent with the [exponential distribution](../../../../exponential-distribution.md) of rate $\lambda$: any finite joint density is $\prod_i\lambda e^{-\lambda x_i}$ on positive coordinates.

The second arrival is a sum of two such variables. Convolution gives

$$
f_{T_2}(t)=\int_0^t\lambda e^{-\lambda s}\lambda e^{-\lambda(t-s)}\,ds
=\boxed{\lambda^2t e^{-\lambda t}\quad(t>0).}
$$

This is a gamma distribution of shape two and rate $\lambda$. If $S$ is the first arrival of the independent rate-$\mu$ process, exponential independence gives

$$
\boxed{\mathbb P(S<T_1)=\int_0^\infty\mu e^{-\mu s}e^{-\lambda s}\,ds
=\frac{\mu}{\lambda+\mu}.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [M](../../m.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
