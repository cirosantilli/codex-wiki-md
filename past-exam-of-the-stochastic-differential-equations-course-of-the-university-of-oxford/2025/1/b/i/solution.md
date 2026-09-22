<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The existence assertion is false under the hypotheses printed in the source.** No measurability of $\theta$ is specified. Even requiring $\theta$ to be a [Borel measurable function](../../../../../borel-measurable-function.md) does not suffice: a coefficient can be positive at every point while approaching zero too rapidly near the starting point. This is the obstruction described by [pointwise positivity does not ensure weak existence](../../../../../pointwise-positivity-does-not-ensure-weak-existence.md).

Here is a counterexample in dimension one, with $\Theta=1$:

$$
\theta(0)=1,\qquad \theta(x)=\min(x^2,1)\quad(x\ne0).
$$

Suppose that a solution to the [martingale problem](../../../../../martingale-problem.md) with domain $C_c^\infty(\mathbb R)$ existed. The cutoff argument from part (a)(ii), now with $\mathcal L=\theta\Delta$, makes $X$ a [continuous local martingale](../../../../../continuous-local-martingale.md) with

$$
[X]_t=2\int_0^t\theta(X_s)\,ds\leq2t.
$$

The criterion for a [continuous local martingale with bounded quadratic variation](../../../../../continuous-local-martingale-with-bounded-quadratic-variation.md) makes it a [square-integrable](../../../../../square-integrable-function.md) [martingale](../../../../../martingale-split.md), and the [Itô isometry](../../../../../ito-isometry.md) gives $\mathbb EX_t^2=\mathbb E[X]_t$.

Apply the [occupation-times formula](../../../../../occupation-times-formula.md) with the indicator of the singleton $\{0\}$. Since that singleton has zero [Lebesgue measure](../../../../../lebesgue-measure.md),

$$
0=\int_0^t\mathbf1_{\{X_s=0\}}\,d[X]_s
=2\int_0^t\mathbf1_{\{X_s=0\}}\,ds.
$$

Thus $X$ spends zero ordinary time at zero. Away from zero, $\theta(x)\leq x^2$, so

$$
0\leq\mathbb EX_t^2
=2\mathbb E\int_0^t\theta(X_s)\,ds
\leq2\int_0^t\mathbb EX_s^2\,ds.
$$

The [Gronwall inequality](../../../../../gronwall-inequality.md) forces $\mathbb EX_t^2=0$ for every $t$. Continuity then forces $X\equiv0$ [almost surely](../../../../../almost-sure-convergence.md), contradicting either the zero occupation time just proved or $[X]_t=2t$ for that constant path. Consequently

$$
\boxed{0<\theta\leq\Theta\text{, even Borel measurable, does not ensure existence}.}
$$

For completeness, the intended construction works if $\theta$ is a [Borel measurable function](../../../../../borel-measurable-function.md) and bounded away from zero on every compact set. In particular, it works for continuous strictly positive $\theta$. Let $B$ be standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md), and define a clock and its inverse by

$$
A_u=\int_0^u\frac{dr}{2\theta(B_r)},\qquad
\tau_t=\inf\{u\geq0:A_u>t\},\qquad X_t=B_{\tau_t}.
$$

The Brownian path on each finite interval has compact range, so the added hypothesis makes $A_u$ finite. The clock is continuous and strictly increasing, and $A_u\geq u/(2\Theta)$, so $A_u\to\infty$. Its inverse is continuous and satisfies $\tau_t\leq2\Theta t$. Each $\tau_t$ is a [stopping time](../../../../../stopping-time.md) for the Brownian [filtration](../../../../../filtration-probability-theory.md).

For $f\in C_c^\infty(\mathbb R^d)$, the [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied at these bounded random times shows that

$$
f(B_{\tau_t})-\frac12\int_0^{\tau_t}\Delta f(B_r)\,dr
$$

is a true [martingale](../../../../../martingale-split.md) in the [filtration](../../../../../filtration-probability-theory.md) $\mathcal G_t=\mathcal F^B_{\tau_t}$. The inverse-clock substitution $d\tau_t=2\theta(X_t)dt$, valid almost everywhere, rewrites it as

$$
f(X_t)-\int_0^t\theta(X_s)\Delta f(X_s)\,ds.
$$

This proves the [Brownian time change for a variable diffusion speed](../../../../../brownian-time-change-for-a-variable-diffusion-speed.md):

$$
\boxed{X_t=B_{A^{-1}(t)}\text{ solves the corrected martingale problem}.}
$$

The factor $2$ in the clock is necessary because standard [Brownian motion](../../../../../brownian-motion-split.md) has [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) $\Delta/2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
