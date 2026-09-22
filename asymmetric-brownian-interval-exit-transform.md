# Asymmetric Brownian interval-exit transform

↑ **Parent:** [Brownian exit from an interval](brownian-exit-from-an-interval.md)

For standard [Brownian motion](brownian-motion-split.md) started at zero and exit time $T$ from $(-b,a)$, $a,b>0$, stop the two [exponential Brownian martingales](exponential-brownian-martingale.md) with parameters $\lambda$ and $-\lambda$. Their stopped values are bounded by $e^{|\lambda|\max(a,b)}$. The [optional stopping theorem](optional-sampling-theorem-for-a-supermartingale.md) and [dominated convergence theorem](dominated-convergence-theorem.md) give $e^{\lambda a}p+e^{-\lambda b}q=1$ and $e^{-\lambda a}p+e^{\lambda b}q=1$, where $p,q$ are the discounted upper and lower exit probabilities. Solving gives the displayed formula and $q=\sinh(\lambda a)/\sinh(\lambda(a+b))$. Thus

$$
\mathbb E e^{-\lambda^2T/2}=\frac{\cosh(\lambda(a-b)/2)}{\cosh(\lambda(a+b)/2)}.
$$

At $\lambda=0$, the first ratio has its removable value $b/(a+b)$, and the second equals one. Finiteness of $T$ follows from a uniformly positive one-unit-time chance to leave any fixed bounded interval.

## ↑ Ancestors (9)

1. [Brownian exit from an interval](brownian-exit-from-an-interval.md)
2. [Brownian exit time](brownian-exit-time.md)
3. [Brownian motion](brownian-motion-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32/5/solution.md)
