<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

By part (c) with $\lambda=1$, let $T_n=E_1+\cdots+E_n\sim\operatorname{Gamma}(n,1)$ for [independent and identically distributed](../../../../independent-and-identically-distributed-random-variables.md) [exponential random variables](../../../../exponential-distribution.md). The requested integral is $\mathbb P(T_n\leq n)$. Each summand has [expectation](../../../../expected-value-split.md) one and [variance](../../../../variance-split.md) one, so the [central limit theorem](../../../../central-limit-theorem.md) gives

$$
\frac{T_n-n}{\sqrt n}\xrightarrow{d}N(0,1).
$$

Zero is a [continuity](../../../../continuous-function.md) point of the [standard normal distribution](../../../../standard-normal-distribution.md), and consequently

$$
\boxed{\lim_{n\to\infty}\frac1{(n-1)!}\int_0^n x^{n-1}e^{-x}\,dx=\Phi(0)=\frac12.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
