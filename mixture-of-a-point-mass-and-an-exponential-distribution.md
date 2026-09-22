# Mixture of a point mass and an exponential distribution

↑ **Parent:** [Mixed probability distribution](mixed-probability-distribution.md)

Let $c>0$, $0\leq p\leq1$ and $\lambda>0$. With probability $p$, take $Y=-c$; otherwise draw an [exponential distribution](exponential-distribution.md) of rate $\lambda$. This [mixed probability distribution](mixed-probability-distribution.md) has a negative atom and a continuous nonnegative component. Its moments are $\mathbb E[Y]=-pc+(1-p)/\lambda$ and $\mathbb E[Y^2]=pc^2+2(1-p)/\lambda^2$. The [law of total variance](law-of-total-variance.md) equivalently gives $\operatorname{Var}(Y)=(1-p)/\lambda^2+p(1-p)(c+1/\lambda)^2$.

When $p<1$, conditioning on $Y\geq0$ selects exactly the exponential component, so $P(Y\geq t\mid Y\geq0)=e^{-\lambda t}$ for $t\geq0$. An ordinary [probability density function](probability-density-function.md) for the continuous component integrates to $1-p$, not one; the missing mass is the atom, not a normalization error.

## ↑ Ancestors (7)

1. [Mixed probability distribution](mixed-probability-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/5/b/i/solution.md)
