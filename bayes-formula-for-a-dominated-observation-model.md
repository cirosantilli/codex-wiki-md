# Bayes formula for a dominated observation model

↑ **Parent:** [Bayesian inverse problem](bayesian-inverse-problem.md)

Suppose an unknown has [prior distribution](prior-probability.md) $\Pi$ and its conditional observation law $P_u$ has jointly measurable [Radon-Nikodym derivative](radon-nikodym-derivative.md) $L(u,m)$ relative to a fixed observation law $P_0$. If $L>0$ for $\Pi(du)P_0(dm)$-almost every pair, then

$$
Z(m)=\int L(u,m)\Pi(du),\qquad
\frac{d\Pi^m}{d\Pi}(u)=\frac{L(u,m)}{Z(m)}
$$

defines the [posterior distribution](bayesian-posterior.md) for almost every observation. Indeed, $\int L(u,m)P_0(dm)=1$ for almost every $u$, so [Tonelli theorem](tonelli-theorem.md) gives $\int Z(m)P_0(dm)=1$. Hence $Z$ is finite almost everywhere, and positivity of $L$ and [Fubini's theorem](fubini-s-theorem.md) give $Z>0$ almost everywhere. The data law is $ZP_0$, and integration of the proposed posterior against this data law recovers the joint law. This proves the [conditional distribution](conditional-distribution.md) property and also shows that the data law is an [equivalent probability measure](equivalent-probability-measure.md) to $P_0$.

## ↑ Ancestors (9)

1. [Bayesian inverse problem](bayesian-inverse-problem.md)
2. [Gaussian measure](gaussian-measure.md)
3. [Gaussian process](gaussian-process.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/3/b/solution.md)
