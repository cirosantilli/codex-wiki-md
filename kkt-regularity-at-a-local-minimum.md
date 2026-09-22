# KKT regularity at a local minimum

↑ **Parent:** [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md)

At a [local minimum](local-minimum.md) of [continuously differentiable functions](continuously-differentiable-function.md), a suitable [constraint qualification](constraint-qualification.md) guarantees the existence of [Lagrange multipliers](lagrange-multiplier.md) satisfying the [KKT conditions](karush-kuhn-tucker-conditions.md). One sufficient local regularity assumption is that the [gradients](gradient.md) of the equality [optimization constraints](optimization-constraint.md) and the [active constraints](active-constraint.md) are jointly [linearly independent](linear-independence.md). This assumption concerns the description of the [feasible set](feasible-region.md), not just the smoothness of the [objective function](objective-function.md).[Lecture 7, §L7.1.3, Theorem L7.3, printed p. 4: continuous differentiability and independent active gradients](nonlinear-optimization-mit-6-7220-and-15-084-spring-2025/lecture-7-lagrange-multipliers-and-kkt-conditions.md)

To see why a hypothesis is needed, minimize $f(x)=x$ subject to $g(x)=x^2\leq0$. The [feasible set](feasible-region.md) is the [singleton](singleton-mathematics.md) $\{0\}$, so $x_*=0$ is a [global minimum](global-minimum.md). Yet $f'(0)+\lambda g'(0)=1$ for every finite [Lagrange multiplier](lagrange-multiplier.md) $\lambda$. Thus this [convex optimization](convex-optimization-split.md) problem has an attained optimum without a [KKT](karush-kuhn-tucker-conditions.md) multiplier. The zero [gradient](gradient.md) of the [active constraint](active-constraint.md) has hidden the actual restriction $x=0$ from its first-order equation. Rewriting it as the equality $h(x)=x=0$ yields the unrestricted [Lagrange multiplier](lagrange-multiplier.md) $\mu=-1$.

For [convex optimization](convex-optimization-split.md), [Slater's condition](slater-s-condition.md) requires strict inequalities and affine equalities at a point in the [relative interior](relative-interior.md) of the common [domain of a function](domain-of-a-function.md). A finite optimum value then gives [strong duality](strong-duality.md) and dual attainment. Primal attainment and [differentiability](differentiability.md) yield [KKT](karush-kuhn-tucker-conditions.md) multipliers. Affine inequalities may be nonstrict in the refined version.[§5.2.3, printed pp. 226–227, equations (5.26)–(5.27); §5.5.3, printed p. 244](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

[Slater's condition](slater-s-condition.md) is sufficient, and need not hold for an optimum to exist. The singular example above also shows that mere primal attainment is not a substitute for a [constraint qualification](constraint-qualification.md).

## ↑ Ancestors (5)

1. [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Constraint qualification](constraint-qualification.md)
- [Strong duality without dual attainment](strong-duality-without-dual-attainment.md)
