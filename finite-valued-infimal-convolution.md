# Finite-valued infimal convolution

↑ **Parent:** [Infimal convolution](infimal-convolution.md)

If two nonnegative finite-valued [convex functions](convex-function.md) are defined on all of a finite-dimensional space, their [infimal convolution](infimal-convolution.md) is finite, [convex](convex-function.md) and continuous everywhere. [Convex perturbation duality](convex-perturbation-duality.md) then gives [strong duality](strong-duality.md) and dual attainment at every argument. It does not require or imply attainment of the primal decomposition infimum.

More precisely, let $f,g:\mathbb R^n\to[0,\infty)$ be finite everywhere and write $h=f\mathbin\square g$. Nonnegativity supplies a lower bound, while the two trial splits $(x,0)$ and $(0,x)$ give

$$
0\leq h(x)\leq\min\{f(x)+g(0),\ f(0)+g(x)\}<\infty.
$$

Mixing nearly optimal splits proves [convexity](convex-function.md), and [continuity of a convex function](continuity-of-a-convex-function.md) applies because the [effective domain](effective-domain.md) is the entire [finite-dimensional vector space](finite-dimensional-vector-space.md). These statements concern the optimized value, rather than existence of an optimal split. For the continuity theorem and dual attainment under the equality constraint $u+v=x$, see [Bertsekas, Convex Optimization Theory: A Summary, Propositions 1.3.11 and 5.3.3(a)](https://ocw.mit.edu/courses/6-253-convex-analysis-and-optimization-spring-2012/db7bde2cd43e8dbaba11f6911311b87c_MIT6_253S12_summary.pdf#page=40). The equality has a feasible point in the whole space for every $x$, and the displayed bound makes its optimal value finite.

**A finite value without any optimal split.** On $\mathbb R$, take the [convex functions](convex-function.md) $f(u)=e^u$ and $g(v)=0$. Both are nonnegative and finite everywhere, but

$$
(f\mathbin\square g)(x)=\inf_{u\in\mathbb R}e^u=0
$$

for every $x$. The splits $(u,v)=(-k,x+k)$ have costs $e^{-k}\to0$, yet the [exponential function](exponential-function.md) is strictly positive at every finite $u$. No split attains the [infimum](infimum.md). The value function is even constant and [differentiable](differentiable-function.md); regularity of the value function does not prevent optimizing splits from escaping to infinity. For example, $k=1,3,6$ gives costs approximately $0.367879$, $0.049787$ and $0.002479$.

A sufficient extra condition for attainment at a fixed $x$ is that $u\mapsto f(u)+g(x-u)$ be a [coercive function](coercive-function.md), meaning it tends to $+\infty$ as $\|u\|\to\infty$. Under the finite-valued assumptions it is a [continuous function](continuous-function.md), so a sufficiently large closed ball contains a [global minimum](global-minimum.md) by the [extreme value theorem](extreme-value-theorem.md). If this cost is also a [strictly convex function](strictly-convex-function.md), the optimal split is unique. The quadratic example above satisfies both conditions; the [exponential function](exponential-function.md) example does not satisfy [coercivity](coercive-function.md).

Nonnegativity is sufficient, not necessary: finite lower bounds $f\geq A$, $g\geq B$ would give $h\geq A+B$ by the same argument. Removing all lower-bound control can lose finiteness even for finite [convex functions](convex-function.md): $f(u)=u$ and $g(v)=-v$ give $f(u)+g(x-u)=2u-x$, hence $h(x)=-\infty$. Nor does finiteness alone guarantee [differentiability](differentiability.md): choosing $f=g=|\cdot|$ gives $h(x)=|x|$ by the [triangle inequality](triangle-inequality.md) and the split $(x,0)$.

**Table of contents**

- [Infimal-convolution dual subgradients](infimal-convolution-dual-subgradients.md)

## ↑ Ancestors (7)

1. [Infimal convolution](infimal-convolution.md)
2. [Convex analysis](convex-analysis.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/2/b/solution.md)
