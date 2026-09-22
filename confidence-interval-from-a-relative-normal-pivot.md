# Confidence interval from a relative normal pivot

↑ **Parent:** [Confidence interval](confidence-interval.md)

Suppose $\theta>0$ and a positive [estimator](estimator.md) $T_n$ satisfies $\sqrt n(T_n-\theta)/\theta\xrightarrow{d}N(0,1)$. Choose the [standard normal quantile](standard-normal-quantile.md) $c=\Phi^{-1}(1-\alpha/2)$. For $n>c^2$, an asymptotic [confidence interval](confidence-interval.md) of level $1-\alpha$ is

$$
\boxed{\left(\frac{T_n}{1+c/\sqrt n},\frac{T_n}{1-c/\sqrt n}\right).}
$$

**Proof.** [Convergence in distribution](convergence-in-distribution.md) gives $\mathbb P(-c<\sqrt n(T_n-\theta)/\theta<c)\to1-\alpha$. Multiplication by the positive $\theta$ and rearrangement makes this event equivalent to $\theta(1-c/\sqrt n)<T_n<\theta(1+c/\sqrt n)$. Both factors are positive when $n>c^2$, so division yields exactly the displayed interval. Thus its coverage [probability](probability.md) tends to $1-\alpha$. For $95\%$ coverage, $c\approx1.96$. This inversion retains the unknown scale $\theta$ in the normalized error, rather than replacing it by the observed [estimator](estimator.md) before inversion.

## ↑ Ancestors (6)

1. [Confidence interval](confidence-interval.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-iii/7/b/v/solution.md)
