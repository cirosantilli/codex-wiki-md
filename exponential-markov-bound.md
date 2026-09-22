# Exponential Markov bound

↑ **Parent:** [Markov's inequality](markov-s-inequality.md)

Applying [Markov's inequality](markov-s-inequality.md) to the positive [random variable](random-variable-split.md) $e^{tX}$ gives

$$
\Pr(X\geq x)\leq e^{-tx}M_X(t),
\qquad t>0.
$$

Here $M_X(t)=\mathbb E[e^{tX}]$ is the [moment-generating function](moment-generating-function.md), and the useful bound requires it to be finite at the chosen $t$. Optimizing over $t>0$ gives the [Chernoff bound](chernoff-bound.md) method: an [exponential function](exponential-function.md) weights large values more strongly before applying the same average-budget argument.

For example, let $N$ have the [Poisson distribution](poisson-distribution.md) with parameter one. Its [expected value](expected-value-split.md) and [variance](variance-split.md) are both one, and its [moment-generating function](moment-generating-function.md) is $M_N(t)=\exp(e^t-1)$. At threshold four, choosing $t=\log4$ gives

$$
\mathbb P(N\geq4)\leq\exp(3-4\log4)=\frac{e^3}{256}\approx0.0784591.
$$

This $t$ minimizes the exponent $e^t-1-4t$ because its [derivative](derivative.md) is $e^t-4$, with positive [second derivative](second-derivative.md). The direct [Markov's inequality](markov-s-inequality.md) bound is $1/4$, and the two-sided [Chebyshev's inequality](chebyshev-s-inequality.md) bound, applied to a deviation of at least three from the [mean](expected-value-split.md) one, is $1/9$. The exact [Poisson distribution](poisson-distribution.md) [tail probability](tail-probability.md) is $1-e^{-1}(1+1+1/2+1/6)\approx0.0189882$. These compare three valid bounds obtained from progressively different information; none is an exact [tail probability](tail-probability.md) formula for general [random variables](random-variable-split.md).

## ↑ Ancestors (7)

1. [Markov's inequality](markov-s-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Concentration of Lipschitz functions on the symmetric group](concentration-of-lipschitz-functions-on-the-symmetric-group.md)
- [Janson lower-tail bound by independent thinning](janson-lower-tail-bound-by-independent-thinning.md)
- [Markov's inequality](markov-s-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2/3f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2/3f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-122/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-122/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201/2/c/solution.md)
