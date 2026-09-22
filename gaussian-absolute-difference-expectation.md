# Gaussian absolute-difference expectation

↑ **Parent:** [Normal distribution](normal-distribution.md)

For independent errors $E_1,E_2\sim N(0,\sigma^2)$, their difference is normal with [variance](variance-split.md) $2\sigma^2$. Hence $\mathbb E|E_1-E_2|=2\sigma/\sqrt\pi$. To verify the constant, a standard normal variable $Z$ satisfies $\mathbb E|Z|=2\int_0^\infty z e^{-z^2/2}\,dz/\sqrt{2\pi}=\sqrt{2/\pi}$; multiply by $\sqrt2\sigma$. Thus an absolute difference of unbiased noisy ratings has a positive expectation even without a true difference.

## ↑ Ancestors (7)

1. [Normal distribution](normal-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
