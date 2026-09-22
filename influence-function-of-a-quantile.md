# Influence function of a quantile

↑ **Parent:** [Influence function](influence-function.md)

Let $q$ be the unique $p$th [quantile](quantile-function.md), with $0<p<1$, and suppose the [density](density.md) $f$ is continuous and positive at $q$. Define quantiles of contaminated distributions using the generalized inverse. For $z\ne q$, differentiating $(1-\varepsilon)F(q_\varepsilon)+\varepsilon\mathbf1_{z\le q_\varepsilon}=p$ gives

$$
\operatorname{IF}(z;q_p,F)=\frac{p-\mathbf1_{z\le q}}{f(q)}.
$$

At $z=q$, the generalized-inverse quantile stays exactly $q$ under this contamination, so its derivative is zero. The step formula thus holds $F$-almost everywhere and determines the [asymptotic variance](asymptotic-variance.md) $p(1-p)/(nf(q)^2)$. Its [gross-error sensitivity](gross-error-sensitivity.md) is $\max(p,1-p)/f(q)$, but its [local-shift sensitivity](local-shift-sensitivity.md) is infinite because of the jump.

## ↑ Ancestors (7)

1. [Influence function](influence-function.md)
2. [Robust statistics](robust-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/4/solution.md)
- [Rejection point of an influence function](rejection-point-of-an-influence-function.md)
