# Explicit Ornstein-Uhlenbeck solution

↑ **Parent:** [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md)

The solution of

$$
dX_t=-\lambda X_t\,dt+dB_t,\qquad X_0=x,
$$

is

$$
X_t=xe^{-\lambda t}+\int_0^te^{-\lambda(t-s)}\,dB_s.
$$

It has variance $(1-e^{-2\lambda t})/(2\lambda)$. Starting from $N(0,(2\lambda)^{-1})$ makes it stationary with covariance $e^{-\lambda|t-s|}/(2\lambda)$.

**Table of contents**

- [Zero-start Ornstein-Uhlenbeck covariance](zero-start-ornstein-uhlenbeck-covariance.md)

## ↑ Ancestors (8)

1. [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md)
2. [Gaussian process](gaussian-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/1/e/solution.md)
- [Stationary spectrum of a linear fluctuating interface](stationary-spectrum-of-a-linear-fluctuating-interface.md)
