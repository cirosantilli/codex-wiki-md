# Integration error controlled by total variation

↑ **Parent:** [Total variation of a function](total-variation-of-a-function.md)

Let $f$ have [bounded variation](total-variation-of-a-function.md), and let $g,h$ be [continuous functions](continuous-function.md) on $[a,b]$. In any tagged sum for the [Riemann-Stieltjes integral](riemann-stieltjes-integral.md),

$$
\left|\sum_j(g(\xi_j)-h(\xi_j))(f(t_j)-f(t_{j-1}))\right|
\leq\|g-h\|_\infty\sum_j|f(t_j)-f(t_{j-1})|
\leq\|g-h\|_\infty V_a^b(f).
$$

Taking the [limit](limit-of-a-function.md) proves the displayed error bound. Thus approximating $g$ uniformly to accuracy $\varepsilon$ controls this integration error by $\varepsilon V_a^b(f)$, even when the integrator is not [differentiable](differentiable-function.md). For the [piecewise linear function](piecewise-linear-function.md) in [partition example of total variation](partition-example-of-total-variation.md), accuracy $0.001$ gives an error at most $0.011$. Total variation supplies exactly the movement budget that an endpoint difference would miss.

## ↑ Ancestors (7)

1. [Total variation of a function](total-variation-of-a-function.md)
2. [Riemann integration](riemann-integration.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
