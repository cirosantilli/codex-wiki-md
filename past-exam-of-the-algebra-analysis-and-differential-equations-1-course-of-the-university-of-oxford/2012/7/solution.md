<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Near $x=0$, [separation of variables](../../../separation-of-variables.md) gives $dy/y=dx/(1-x)$, so $\log|y|=-\log(1-x)+C$. The [initial condition](../../../initial-condition.md) selects

$$
\boxed{y(x)=\frac1{1-x},\qquad -\infty<x<1.}
$$

Direct substitution verifies both the [ordinary differential equation](../../../ordinary-differential-equation.md) and the [initial condition](../../../initial-condition.md). The endpoint $x=1$ is excluded because the coefficient and this solution are singular there; the displayed interval is the maximal connected real interval containing the initial point.

For $|x|\leq h<1$ and any two admissible values $y,\widetilde y$,

$$
|f(x,y)-f(x,\widetilde y)|
=\frac{|y-\widetilde y|}{|1-x|}
\leq\frac1{1-h}|y-\widetilde y|.
$$

This is a [Lipschitz condition](../../../lipschitz-continuity.md) in the dependent variable, uniform in $x$, with [Lipschitz constant](../../../lipschitz-constant.md) $L=(1-h)^{-1}$. Also $|f(x,y)|\leq(1+k)/(1-h)$ on the prescribed rectangle, so the usual local hypotheses of the [Picard-Lindelöf theorem](../../../picard-lindelof-theorem.md) hold.

Integrating from the initial point gives the [integral equation](../../../integral-equation.md)

$$
y(x)=1+\int_0^x\frac{y(t)}{1-t}\,dt.
$$

Conversely, differentiating this equation using the [fundamental theorem of calculus](../../../fundamental-theorem-of-calculus.md) recovers the [initial value problem](../../../initial-value-problem.md). Start [Picard iteration](../../../picard-iteration.md) with the constant initial approximation $y_0(x)=1$ and set

$$
y_{n+1}(x)=1+\int_0^x\frac{y_n(t)}{1-t}\,dt.
$$

The first three approximations are

$$
\boxed{y_0=1,\qquad y_1=1-\log(1-x),\qquad
y_2=1-\log(1-x)+\frac12\log^2(1-x).}
$$

To prove the general expression by [mathematical induction](../../../mathematical-induction.md), put $\ell(x)=\log(1-x)$. The initial approximation gives the formula for $n=0$. If it holds for $n$, then the [substitution rule](../../../integration-by-substitution.md)

$$
\int_0^x\frac{\ell(t)^k}{1-t}\,dt=-\frac{\ell(x)^{k+1}}{k+1}
$$

gives

$$
y_{n+1}(x)=1+\sum_{k=0}^n\frac{(-1)^{k+1}\ell(x)^{k+1}}{(k+1)!}
=\sum_{k=0}^{n+1}\frac{(-1)^k\ell(x)^k}{k!}.
$$

Thus the formula follows at every stage.

For every fixed real $x<1$, these are partial sums of the [exponential series](../../../exponential-series.md) evaluated at the finite real number $-\log(1-x)$. Therefore

$$
\boxed{\lim_{n\to\infty}y_n(x)=\exp(-\log(1-x))=\frac1{1-x}
\quad\text{for every }x<1.}
$$

This range is larger than $|x|<1$: the expansion is in powers of $\log(1-x)$, not a [Taylor series](../../../taylor-series.md) in $x$. For example it converges at $x=-2$. It also converges uniformly on every [compact interval](../../../compact-interval.md) contained in $(-\infty,1)$, because $|\log(1-x)|$ is bounded there and the [exponential series](../../../exponential-series.md) supplies a uniform summable bound. At $x=1$ the approximations are undefined, while for $x>1$ the real integral from zero crosses the singularity. This is [Picard iteration for a simple-pole linear differential equation](../../../picard-iteration-for-a-simple-pole-linear-differential-equation.md).

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2012](../../2012-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
