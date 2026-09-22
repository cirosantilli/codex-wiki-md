# Averaged stationarity bound for stochastic gradient descent

↑ **Parent:** [Stochastic gradient descent](stochastic-gradient-descent.md)

Suppose a fixed-[step size](step-size.md) [stochastic gradient descent](stochastic-gradient-descent.md) iteration satisfies

$$
\mathbb E[f(X^{j+1})\mid X^j]\leq f(X^j)-\frac1{2L}\|\nabla f(X^j)\|^2+\frac M{2L},
$$

and $f$ has a [global minimizer](global-minimizer.md) $x^*$. Taking [expectations](expected-value-split.md) and forming a [telescoping sum](telescoping-sum.md) proves the displayed bound with $\Delta_0=f(X^0)-f(x^*)$ and deterministic $X^0$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) then bounds the averaged, or the best, expected [gradient](gradient.md) [Euclidean norm](euclidean-norm.md) by $\sqrt{M+2L\Delta_0/k}$. This is a guarantee of stationarity in the indicated senses, rather than a last-iterate convergence assertion. The additive $M$ is a [stochastic gradient noise floor](stochastic-gradient-noise-floor.md).

```
Target: real-analysis.bigb, under Strongly convex function.
```

## ↑ Ancestors (7)

1. [Stochastic gradient descent](stochastic-gradient-descent.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/2/d/solution.md)
