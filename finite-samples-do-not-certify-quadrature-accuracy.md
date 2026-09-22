# Finite samples do not certify quadrature accuracy

↑ **Parent:** [Numerical integration](numerical-integration-split.md)

For any finite set of [quadrature nodes](quadrature-node.md) $x_1,\ldots,x_m$ in $[a,b]$, $a<b$, consider the [polynomial](polynomial-split.md)

$$
p(x)=\prod_{j=1}^m(x-x_j)^2,\qquad A=\int_a^bp(x)\,dx>0.
$$

Every sample is zero, so every [quadrature rule](quadrature-rule.md) at these [quadrature nodes](quadrature-node.md) gives $Q(p)=0$. Yet $p$ is nonnegative and strictly positive away from its finitely many [polynomial roots](root-of-a-polynomial.md); its [continuity](continuous-function.md) makes the [integral](integral-split.md) positive. Consequently the [smooth functions](smooth-function.md) $0$ and $g(x)=p(x)/A$ have identical samples but [definite integrals](definite-integral.md) $0$ and $1$. Multiplying $g$ by any positive constant makes the difference arbitrarily large. This is an information limit, even with exact arithmetic; merely assuming smoothness without quantitative bounds does not remove it. The related [degree ceiling for quadrature exactness](degree-ceiling-for-quadrature-exactness.md) uses the same squared nodal [polynomial](polynomial-split.md) to limit [polynomial](polynomial-split.md) exactness.

For example, the endpoint [quadrature nodes](quadrature-node.md) $0,1$ give $p(x)=x^2(1-x)^2$, $A=1/30$, and $g(x)=30x^2(1-x)^2$. Both the zero [function](function-split.md) and $g$ produce zero under the one-panel [trapezoidal rule](trapezoidal-rule.md), although $I(g)=1$. More generally, any estimate based only on their shared samples has [absolute error](absolute-error.md) at least $1/2$ for one of these two [integrands](integrand.md), by the [triangle inequality](triangle-inequality.md).

The obstruction also applies to a deterministic adaptive procedure that terminates after finitely many evaluations on the zero [function](function-split.md): form $p$ using every [quadrature node](quadrature-node.md) it visited. On $g$, the same zero responses lead to the same choices and answer. Certified [quadrature error](quadrature-error.md) control therefore needs additional information, such as a known bound on relevant [derivatives](derivative.md), rather than agreement among sampled approximations alone.

## ↑ Ancestors (6)

1. [Numerical integration](numerical-integration-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Numerical integration](numerical-integration-split.md)
