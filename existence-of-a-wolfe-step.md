# Existence of a Wolfe step

↑ **Parent:** [Wolfe conditions](wolfe-conditions.md)

Suppose $f$ is [continuously differentiable](continuously-differentiable-function.md), $s$ is a [descent direction](descent-direction.md), and $f(x+\alpha s)$ is bounded below for $\alpha\geq0$. A positive [step size](step-size.md) satisfying the weak [Wolfe conditions](wolfe-conditions.md) exists. To prove this, put $\phi(\alpha)=f(x+\alpha s)$, $d=\phi'(0)<0$, and $h(\alpha)=\phi(\alpha)-\phi(0)-\beta_1\alpha d$. The [Armijo condition](armijo-condition.md) proof shows $h<0$ just to the right of zero. Boundedness below gives $h(\alpha)\to+\infty$. Consequently there is a first positive zero $A$, with $h\leq0$ on $[0,A]$. By the [mean value theorem](mean-value-theorem.md), some $t\in(0,A)$ satisfies

$$
\phi'(t)=\frac{\phi(A)-\phi(0)}A=\beta_1d>\beta_2d.
$$

At $t$, $h(t)\leq0$ gives the [Armijo condition](armijo-condition.md), and the displayed derivative gives the weak [Wolfe conditions](wolfe-conditions.md).

## ↑ Ancestors (6)

1. [Wolfe conditions](wolfe-conditions.md)
2. [Line search](line-search.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/b/solution.md)
