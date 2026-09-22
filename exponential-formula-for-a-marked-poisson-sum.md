# Exponential formula for a marked Poisson sum

↑ **Parent:** [Poisson process](poisson-process.md)

Let $J_i$ be the points of a rate-$\lambda$ Poisson process and let independent identically distributed marks $X_i$ be independent of the process. Then

$$
\mathbb E\exp\left(\theta\sum_{i=1}^{N_t}g(J_i,X_i)\right)
=\exp\left\{\lambda\int_0^t
\left(\mathbb E e^{\theta g(s,X_1)}-1\right)ds\right\}.
$$

Condition on $N_t$, use uniform order statistics, and sum the resulting exponential series.

## ↑ Ancestors (6)

1. [Poisson process](poisson-process.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/28j/c/solution.md)
