# Lagrangian duality

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)

A [feasible point](feasible-point.md) gives an upper bound on a [minimization problem](minimization-problem.md)'s best value; a suitable [Lagrange multiplier](lagrange-multiplier.md) gives a lower bound. [Lagrangian duality](lagrangian-duality.md) searches for the strongest bound obtainable this way. Matching bounds certify a [global minimum](global-minimum.md).

Let $X$ be a nonempty decision domain on which the [objective function](objective-function.md) $f$ and the constraint [functions](function-split.md) $g_i,h_j$ are finite. Write the [primal problem](primal-problem.md) and its [optimization Lagrangian](optimization-lagrangian.md) as

$$
p_* = \inf\{f(x):x\in X,\ g_i(x)\leq0,\ h_j(x)=0\},
\qquad
L(x,\lambda,\nu)=f(x)+\sum_{i=1}^m\lambda_i g_i(x)+\sum_{j=1}^r\nu_j h_j(x).
$$

The inequality [Lagrange multipliers](lagrange-multiplier.md) obey $\lambda_i\geq0$; the equality [Lagrange multipliers](lagrange-multiplier.md) $\nu_j$ are unrestricted [real numbers](real-number.md). Define the [Lagrange dual function](lagrange-dual-function.md) and dual optimal value by

$$
q(\lambda,\nu)=\inf_{x\in X}L(x,\lambda,\nu),\qquad
d_* = \sup_{\lambda\geq0,\ \nu\in\mathbb R^r}q(\lambda,\nu).
$$

The inner [infimum](infimum.md) keeps $X$, but releases the displayed [optimization constraints](optimization-constraint.md). It can be $-\infty$, giving an uninformative lower bound. A different domain changes the bound.[§§5.1.1–5.1.3, printed pp. 215–216: domain, Lagrangian, dual function and lower bounds](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

Here is the entire [weak duality](weak-duality.md) argument. For any [feasible point](feasible-point.md) $z$ and allowable [Lagrange multipliers](lagrange-multiplier.md),

$$
q(\lambda,\nu)\leq L(z,\lambda,\nu)\leq f(z).
$$

The first [inequality](inequality-mathematics.md) is the definition of an [infimum](infimum.md); the second uses $\lambda_i g_i(z)\leq0$ and $h_j(z)=0$. Taking the [infimum](infimum.md) over feasible $z$, then the [supremum](supremum.md) over allowable [Lagrange multipliers](lagrange-multiplier.md), gives $d_*\leq p_*$. No [convexity](convex-function.md) is used.

The [Lagrange dual function](lagrange-dual-function.md) is a [concave function](concave-function.md), since each fixed decision makes $L$ an [affine function](affine-function.md) of the [Lagrange multipliers](lagrange-multiplier.md).[§5.1.2, printed p. 216: pointwise infimum of affine functions](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md) Explicitly, write $y=(\lambda,\nu)$ and choose two points where $q$ is finite. For $0\leq t\leq1$ and every $x\in X$,

$$
L(x,ty_1+(1-t)y_2)
=tL(x,y_1)+(1-t)L(x,y_2)
\geq tq(y_1)+(1-t)q(y_2).
$$

Taking the [infimum](infimum.md) over $x$ proves the defining [concavity](concave-function.md) [inequality](inequality-mathematics.md). Thus even a difficult [primal problem](primal-problem.md) supplies a dual with useful geometry, although evaluating $q$ can itself be difficult.

For finite optimal values, [strong duality](strong-duality.md) means $d_*=p_*$, or zero [duality gap](duality-gap.md). It need not imply [dual attainment](dual-attainment.md). For [convex optimization](convex-optimization-split.md), [Slater's condition](slater-s-condition.md) is a sufficient [constraint qualification](constraint-qualification.md) for both when $p_*$ is finite.[§§5.2.2–5.2.3, printed pp. 225–227: gap, strong duality and Slater dual attainment](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md) The [Strong Lagrangian property](strong-lagrangian-property.md) requires an actual finite [Lagrange multiplier](lagrange-multiplier.md) achieving equality. [Convex perturbation duality](convex-perturbation-duality.md) interprets such a bound as a supporting slope of the perturbed [value function](value-function.md).

**Table of contents**

- [Lagrangian duality for a quadratic threshold](lagrangian-duality-for-a-quadratic-threshold.md)
- [Positive Lagrangian duality gap on a finite domain](positive-lagrangian-duality-gap-on-a-finite-domain.md)
- [Strong duality without dual attainment](strong-duality-without-dual-attainment.md)
- [Strong Lagrangian property](strong-lagrangian-property.md)
- [Primal problem](primal-problem.md)

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Convex optimization](convex-optimization-split.md)
- [Envelope theorem](envelope-theorem.md)
- [Lagrangian duality](lagrangian-duality.md)
- [Lagrangian duality for a quadratic threshold](lagrangian-duality-for-a-quadratic-threshold.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/20h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/20h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38/2/b/solution.md)
