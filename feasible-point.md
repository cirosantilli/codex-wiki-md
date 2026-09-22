# Feasible point

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)

A [feasible point](feasible-point.md) satisfies every [optimization constraint](optimization-constraint.md) of an [optimization](mathematical-optimization-split.md) problem. For the [budget constraint](budget-constraint.md) example, the [feasible set](feasible-region.md) is exactly

$$
F=\{(x,10-x):0\leq x\leq10\}.
$$

It is the [line segment](line-segment.md) from $(0,10)$ to $(10,0)$, a [compact set](compact-space.md) and a [convex set](convex-set-split.md). The point $(2,8)$ is feasible, with product $16$; $(6,6)$ has a larger product $36$ but violates the [budget constraint](budget-constraint.md). Feasibility answers whether a decision is allowed; optimality asks whether any allowed decision is better. The [extreme value theorem](extreme-value-theorem.md) guarantees that this [continuous](continuous-function.md) [objective function](objective-function.md) attains its [maximum](maximum-of-a-subset-of-a-total-order.md) on this nonempty [compact set](compact-space.md).

Eliminating $y$ gives a one-variable [objective function](objective-function.md):

$$
q(x)=x(10-x)=25-(x-5)^2,\qquad0\leq x\leq10.
$$

By [completing the square](completing-the-square.md), $q(x)\leq25$, with equality exactly at $x=5$. Alternatively its [derivative](derivative.md) is $q'(x)=10-2x$, which vanishes at $5$; the endpoint values are both zero. [Completing the square](completing-the-square.md) proves global optimality directly, whereas the [first-order optimality condition](first-order-optimality-condition.md) only identifies a candidate. It also quantifies the cost of imbalance: moving to $(5+\delta,5-\delta)$ with $|\delta|\leq5$ loses exactly $\delta^2$ units of product. The [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md) gives another short certificate: $\sqrt{xy}\leq(x+y)/2=5$, with equality exactly when $x=y$.

For a [transportation problem](transportation-problem.md) with capacity inequalities, feasibility requires nonnegative shipments, row totals no greater than factory capacities and column totals equal to shop demands. Feasibility alone does not prove minimal cost: a matching [transportation dual certificate with capacity inequalities](transportation-dual-certificate-with-capacity-inequalities.md) provides an optimality proof. The [feasible set](feasible-region.md) can be empty, and a finite [infimum](infimum.md) need not be attained even when the set is nonempty.

**Table of contents**

- [Feasible region](feasible-region.md)
  - [Feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md)
  - [Equality slice of a feasible triangle](equality-slice-of-a-feasible-triangle.md)
  - [Empty and open feasible regions](empty-and-open-feasible-regions.md)

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Conic dual problem](conic-dual-problem.md)
- [Conic primal-dual gap](conic-primal-dual-gap.md)
- [Convex KKT optimality certificate](convex-kkt-optimality-certificate.md)
- [Convex optimization](convex-optimization-split.md)
- [Empty and open feasible regions](empty-and-open-feasible-regions.md)
- [Failure of multiplier stationarity at a singular constraint](failure-of-multiplier-stationarity-at-a-singular-constraint.md)
- [Farkas certificate for linear inequalities](farkas-certificate-for-linear-inequalities.md)
- [Farkas' lemma](farkas-lemma.md)
- [Feasible point](feasible-point.md)
- [Feasible region](feasible-region.md)
- [Feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md)
- [Five-state barrier example for simulated annealing](five-state-barrier-example-for-simulated-annealing.md)
- [Karmarkar standard form](karmarkar-standard-form.md)
- [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md)
- [Lagrangian duality](lagrangian-duality.md)
- [Lagrangian duality for a quadratic threshold](lagrangian-duality-for-a-quadratic-threshold.md)
- [Mathematical optimization](mathematical-optimization-split.md)
- [Nonnegative-orthant optimality certificate](nonnegative-orthant-optimality-certificate.md)
- [Objective function](objective-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-40/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-40/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/20c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/1/solution.md)
- [Positive Lagrangian duality gap on a finite domain](positive-lagrangian-duality-gap-on-a-finite-domain.md)
- [Quadratic minimization with a moving upper bound](quadratic-minimization-with-a-moving-upper-bound.md)
- [Robust infeasibility under uniform constraint relaxation](robust-infeasibility-under-uniform-constraint-relaxation.md)
- [Second-order-cone optimality certificate](second-order-cone-optimality-certificate.md)
- [Simulated annealing](simulated-annealing.md)
- [Strong duality without dual attainment](strong-duality-without-dual-attainment.md)
