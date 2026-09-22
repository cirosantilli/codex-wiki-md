# Convex KKT optimality certificate

↑ **Parent:** [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md)

For [differentiable functions](differentiable-function.md) $f,g_i$ that are [convex functions](convex-function.md) on an open [convex set](convex-set-split.md) and [affine functions](affine-function.md) $h_j$, the [KKT conditions](karush-kuhn-tucker-conditions.md) certify a [global minimum](global-minimum.md). Once [Lagrange multipliers](lagrange-multiplier.md) satisfy them, no extra [Slater condition](slater-s-condition.md) is needed.[§5.5.3, printed p. 244: sufficiency under convexity and affine equalities](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

The certificate is a short chain of [inequalities](inequality-mathematics.md). Nonnegative [Lagrange multipliers](lagrange-multiplier.md) and affine equalities make $L(\cdot,\lambda,\mu)$ a [convex function](convex-function.md). Its zero [gradient](gradient.md) gives a [global minimum](global-minimum.md) at $x_*$ by the [first-order optimality condition](first-order-optimality-condition.md). For every [feasible point](feasible-point.md) $z$,

$$
f(x_*)=L(x_*,\lambda,\mu)\leq L(z,\lambda,\mu)\leq f(z).
$$

The first equality uses feasibility and [complementary slackness](complementary-slackness.md); the last inequality uses $g_i(z)\leq0$ and $\lambda_i\geq0$. Equivalently, the [Lagrange dual function](lagrange-dual-function.md) attains the same value as the primal [objective function](objective-function.md), proving [strong duality](strong-duality.md). A [strictly convex function](strictly-convex-function.md) $f$ makes the primal optimum unique, although the [Lagrange multipliers](lagrange-multiplier.md) need not be unique.

Affine equality [optimization constraints](optimization-constraint.md) matter: an arbitrary signed multiple of a nonlinear equality can destroy [convexity](convex-function.md) of the [optimization Lagrangian](optimization-lagrangian.md). For example, minimizing $(x-2)^2$ subject to the affine equality $x=b$ gives $x_*=b$ and $\mu=2(2-b)$ for $L=(x-2)^2+\mu(x-b)$. This equality [Lagrange multiplier](lagrange-multiplier.md) is positive for $b<2$, zero at $b=2$, and negative for $b>2$. [Completing the square](completing-the-square.md) gives the certificate $L=(x-b)^2+(b-2)^2$ for every [real number](real-number.md) $b$.

Outside [convex optimization](convex-optimization-split.md), [KKT](karush-kuhn-tucker-conditions.md) stationarity alone does not certify an optimum: minimizing $-x^2$ with no [optimization constraints](optimization-constraint.md) gives the stationary candidate $x=0$, which is a [global maximum](global-maximum.md). The [Lagrangian sufficiency theorem](lagrange-sufficiency-theorem.md) remains applicable whenever a global minimum of the [optimization Lagrangian](optimization-lagrangian.md) can be proved directly.

## ↑ Ancestors (5)

1. [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Lagrangian duality for a quadratic threshold](lagrangian-duality-for-a-quadratic-threshold.md)
