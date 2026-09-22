# Differentiation of parameter integrals on compact rectangles

↑ **Parent:** [Dominated differentiation under the integral sign](dominated-differentiation-under-the-integral-sign.md)

Suppose $f$ and its [partial derivative](partial-derivative.md) $\partial_t f$ are jointly continuous on a compact rectangle $J\times[a,b]$. Then $F(t)=\int_a^bf(t,x)\,dx$ is continuously differentiable in the interior of $J$, and the displayed formula holds, with one-sided [derivatives](derivative.md) at parameter endpoints where the corresponding partial derivative is given.

To prove it, the [extreme value theorem](extreme-value-theorem.md) bounds $|\partial_t f|$ by $M_1$. For each fixed $x$, the [mean value theorem](mean-value-theorem.md) bounds the difference quotient $[f(t+h,x)-f(t,x)]/h$ by $M_1$. It converges pointwise to $\partial_t f(t,x)$, and the constant $M_1$ is integrable over $[a,b]$. [Dominated convergence](dominated-convergence-theorem.md) gives the derivative formula. Apply [continuity of parameter integrals on compact rectangles](continuity-of-parameter-integrals-on-compact-rectangles.md) to $\partial_t f$ to obtain continuity of $F'$. The proof works locally on unbounded parameter [intervals](interval-mathematics.md) as well.

## ↑ Ancestors (6)

1. [Dominated differentiation under the integral sign](dominated-differentiation-under-the-integral-sign.md)
2. [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2014/2/b/ii/solution.md)
