# Periodic covariance function

↑ **Parent:** [Gaussian process](gaussian-process.md)

This [covariance function](covariance-function.md) is periodic with period $P>0$. Map time to the circle $u(t)=(\cos(2\pi t/P),\sin(2\pi t/P))$ and pull back a [Gaussian kernel](gaussian-kernel.md); since $\|u(t)-u(t')\|^2=4\sin^2(\pi(t-t')/P)$, this proves positive semidefiniteness. A [Gaussian process](gaussian-process.md) with this kernel has $\operatorname{Var}(f(t+P)-f(t))=0$ and therefore repeats at every fixed phase. Replacing the inner $\pi$ by $2\pi$ changes the actual period to $P/2$.

**Table of contents**

- [Periodic Gaussian process with zero period average](periodic-gaussian-process-with-zero-period-average.md)

## ↑ Ancestors (7)

1. [Gaussian process](gaussian-process.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/3/i/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/3/ii/solution.md)
- [Periodic Gaussian process with zero period average](periodic-gaussian-process-with-zero-period-average.md)
