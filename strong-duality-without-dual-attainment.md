# Strong duality without dual attainment

↑ **Parent:** [Lagrangian duality](lagrangian-duality.md)

Consider an [objective function](objective-function.md) that is a [quadratic polynomial](quadratic-polynomial.md), with a singular [optimization constraint](optimization-constraint.md):

$$
\min_{x\in\mathbb R}(x-3)^2\qquad\text{subject to }x^2\leq0.
$$

Its only [feasible point](feasible-point.md) is $x_*=0$, giving $p_*=9$. For $\lambda\geq0$, [completing the square](completing-the-square.md) yields

$$
L(x,\lambda)=(1+\lambda)\left(x-\frac3{1+\lambda}\right)^2
+\frac{9\lambda}{1+\lambda},\qquad
q(\lambda)=\frac{9\lambda}{1+\lambda}=9-\frac9{1+\lambda}.
$$

Every finite [Lagrange multiplier](lagrange-multiplier.md) gives $q(\lambda)<9$, but $q(\lambda)\to9$ as $\lambda\to\infty$. Thus $d_*=p_*=9$: [strong duality](strong-duality.md) holds, and the primal optimum is attained, yet [dual attainment](dual-attainment.md) fails. The inner minimizers $3/(1+\lambda)$ approach $0$ without ever becoming feasible at finite $\lambda$.

Both the [objective function](objective-function.md) and the constraint [function](function-split.md) are [convex functions](convex-function.md). However, [Slater's condition](slater-s-condition.md) fails because $x^2<0$ is impossible. At the optimum, stationarity would require $-6+\lambda\cdot0=0$, which no finite [Lagrange multiplier](lagrange-multiplier.md) satisfies. Compare [KKT regularity at a local minimum](kkt-regularity-at-a-local-minimum.md): a zero [gradient](gradient.md) of an [active constraint](active-constraint.md) can prevent a multiplier certificate. This example has zero [duality gap](duality-gap.md) without the [Strong Lagrangian property](strong-lagrangian-property.md).

## ↑ Ancestors (5)

1. [Lagrangian duality](lagrangian-duality.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
