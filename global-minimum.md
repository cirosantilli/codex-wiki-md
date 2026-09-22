# Global minimum

↑ **Parent:** [Critical point](critical-point.md)

A [real-valued function](real-valued-function.md) $f:D\to\mathbb R$ attains a global minimum at $x_*$ when

$$
f(x_*)\leq f(x)\qquad\text{for every }x\in D.
$$

The point $x_*$ is a [global minimizer](global-minimizer.md); $f(x_*)$ is the minimum value. A [global maximum](global-maximum.md) reverses the inequality throughout the same [domain of a function](domain-of-a-function.md). Unlike a [local minimum](local-minimum.md) or [local maximum](local-maximum.md), a [global minimum](global-minimum.md) or [global maximum](global-maximum.md) compares every permitted input, however distant. The [domain of a function](domain-of-a-function.md) is part of the claim.

For $f(x)=x^4-2x^2$ on $\mathbb R$, completing the square gives

$$
f(x)=(x^2-1)^2-1\geq-1,
$$

with equality exactly at $x=\pm1$. This proves that $-1$ is the [global minimum](global-minimum.md) and that the two [global minimizers](global-minimizer.md) are $-1$ and $1$. Neither is a strict global minimizer, because the other attains the same value; both are [strict local minima](strict-local-minimum.md). There is no [global maximum](global-maximum.md) on $\mathbb R$, whereas on $[-1,1]$ the [global maximum](global-maximum.md) is $0$, attained at zero.

Finding [critical points](critical-point.md) supplies candidates rather than a global certificate. The squared expression above is beautiful because one inequality compares infinitely many inputs at once. A [global minimum](global-minimum.md) is always a [local minimum](local-minimum.md) under the relative-[neighbourhood](neighbourhood-mathematics.md) convention; the converse fails. For example, $f(x)=x^3-3x$ has a [strict local minimum](strict-local-minimum.md) at $x=1$, but $f(x)\to-\infty$ as $x\to-\infty$, so it has no [global minimum](global-minimum.md) on the [real line](real-line.md).

Existence also matters: $f(x)=x$ on $(0,1)$ has [infimum](infimum.md) zero and [supremum](supremum.md) one but attains neither a [global minimum](global-minimum.md) nor a [global maximum](global-maximum.md). By the [extreme value theorem](extreme-value-theorem.md), a [continuous function](continuous-function.md) on a nonempty [closed interval](closed-real-interval.md) $[a,b]$ attains both. To find those values, compare all [interior](interior-topology.md) critical numbers, including points where the [derivative](derivative.md) does not exist, and both endpoints. Checking only [stationary points](stationary-point.md) can miss a corner or an endpoint. [Gilbert Strang and Edwin Herman, OpenStax Calculus Volume 1, §4.3: locating absolute extrema](https://openstax.org/books/calculus-volume-1/pages/4-3-maxima-and-minima)

**Table of contents**

- [Global minimizer](global-minimizer.md)

## ↑ Ancestors (5)

1. [Critical point](critical-point.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (79)

- [Conic dual problem](conic-dual-problem.md)
- [Convex function](convex-function.md)
- [Convex KKT optimality certificate](convex-kkt-optimality-certificate.md)
- [Convex optimization](convex-optimization-split.md)
- [Cooling schedule for simulated annealing](cooling-schedule-for-simulated-annealing.md)
- [Critical point](critical-point.md)
- [Descent lemma](descent-lemma.md)
- [Equality slice of a feasible triangle](equality-slice-of-a-feasible-triangle.md)
- [Exponential-linear separable potential](exponential-linear-separable-potential.md)
- [Extreme value theorem](extreme-value-theorem.md)
- [Failure of multiplier stationarity at a singular constraint](failure-of-multiplier-stationarity-at-a-singular-constraint.md)
- [Feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md)
- [Finite-valued infimal convolution](finite-valued-infimal-convolution.md)
- [First-order transition in a cubic-quartic Landau potential](first-order-transition-in-a-cubic-quartic-landau-potential.md)
- [Five-state barrier example for simulated annealing](five-state-barrier-example-for-simulated-annealing.md)
- [Fixed-step gradient descent on a positive-definite quadratic](fixed-step-gradient-descent-on-a-positive-definite-quadratic.md)
- [Fixed-temperature law of simulated annealing](fixed-temperature-law-of-simulated-annealing.md)
- [Global minimum](global-minimum.md)
- [Gradient descent](gradient-descent-split.md)
- [Helmholtz free energy](helmholtz-free-energy.md)
- [Hessian matrix](hessian-matrix.md)
- [Higher-order test for separated extrema](higher-order-test-for-separated-extrema.md)
- [Hyperbolic cosine](hyperbolic-cosine.md)
- [KKT regularity at a local minimum](kkt-regularity-at-a-local-minimum.md)
- [Lagrange multiplier](lagrange-multiplier.md)
- [Lagrange multiplier for quadratic cost](lagrange-multiplier-for-quadratic-cost.md)
- [Lagrangian duality](lagrangian-duality.md)
- [Lagrangian duality for a quadratic threshold](lagrangian-duality-for-a-quadratic-threshold.md)
- [Local minimum](local-minimum.md)
- [Minimal surface](minimal-surface.md)
- [Multistart optimization](multistart-optimization.md)
- [Nonnegative-orthant optimality certificate](nonnegative-orthant-optimality-certificate.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2/a3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/5a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-56/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-56/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-43/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-49/1/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-43/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-303/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-303/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/12/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-b/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/13/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/14/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/19/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/20/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/18/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/19/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/19/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/12/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/9/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/9/a/ii/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1/4/e/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2019/4/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2019/4/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2019/4/d/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/3/g/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2014/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1/4/solution.md)
- [Radial Gaussian flat function](radial-gaussian-flat-function.md)
- [Sextic even Landau potential](sextic-even-landau-potential.md)
- [Simulated annealing](simulated-annealing.md)
- [Soap film pressure balance](soap-film-pressure-balance.md)
- [Stable minimal surface](stable-minimal-surface.md)
- [Stable zero-energy Polonyi vacuum](stable-zero-energy-polonyi-vacuum.md)
- [Stoner threshold for an interaction normalized per electron](stoner-threshold-for-an-interaction-normalized-per-electron.md)
- [Temperature-dependent cubic-quartic Landau free energy](temperature-dependent-cubic-quartic-landau-free-energy.md)
- [Thermodynamic free energy](thermodynamic-free-energy.md)
