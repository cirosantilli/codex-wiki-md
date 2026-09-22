# Quantile proof of the Glivenko-Cantelli theorem

↑ **Parent:** [Glivenko-Cantelli theorem](glivenko-cantelli-theorem.md)

For a [cumulative distribution function](cumulative-distribution-function.md) $G$, let $Q(u)=\inf\{x:G(x)\geq u\}$, $0<u<1$. Right continuity gives $Q(u)\leq x$ exactly when $u\leq G(x)$, including at atoms. Thus applying $Q$ to independent uniform variables $U_i$ constructs an independent sample with distribution function $G$. Its [empirical distribution function](empirical-distribution-function.md) is $G_n(x)=F_n(G(x))$, where $F_n$ is the uniform-sample empirical distribution function. Consequently $\sup_x|G_n(x)-G(x)|\leq\sup_{t\in[0,1]}|F_n(t)-t|$. For the uniform sample, monotonicity and a grid of mesh $1/m$ bound the last supremum by the largest error at grid points plus $1/m$. The [strong law of large numbers](strong-law-of-large-numbers.md) on the countable union of all such grids proves the almost-sure limit. This construction proves the theorem for distributions with atoms as well as continuous distributions.

## ↑ Ancestors (10)

1. [Glivenko-Cantelli theorem](glivenko-cantelli-theorem.md)
2. [Uniform law of large numbers](uniform-law-of-large-numbers.md)
3. [Weak law of large numbers](weak-law-of-large-numbers.md)
4. [Convergence in probability](convergence-in-probability.md)
5. [Convergence of random variables](convergence-of-random-variables-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/2/a/iii/solution.md)
