<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The supporting inequality in part 2(a) bounds $f$ below by an [affine function](../../../../affine-function.md) plus a positive squared [Euclidean norm](../../../../euclidean-norm.md), making it a [coercive function](../../../../coercive-function.md). Its [continuity](../../../../continuous-function.md) gives a [global minimizer](../../../../global-minimizer.md) $x^*$, which is unique by [strict convexity](../../../../strictly-convex-function.md). Let $L_{\max}=\max_iL_i$, $\ell=n/m$ and $\Delta_0=f(x^0)-f(x^*)$. Here $m$ is the block size, so its role differs from the number of component [functions](../../../../function-split.md) in Question 2. Use [randomized block coordinate descent](../../../../randomized-block-coordinate-descent.md) with uniformly sampled blocks of size $m$, independently at each update. Sampling uniformly from a fixed partition into $\ell$ equal-sized blocks gives the same calculation, since each coordinate has inclusion [probability](../../../../probability.md) $1/\ell=m/n$.

Let $\beta$ be a common upper bound on the block [Lipschitz constants](../../../../lipschitz-constant.md). Part (c) permits $\beta=mL_{\max}$. With [step size](../../../../step-size.md) $1/\beta$, part (a) gives

$$
f\left(x-\frac1\beta\nabla_{\mathcal B}f(x)\right)\leq f(x)-\frac1{2\beta}\|\nabla_{\mathcal B}f(x)\|^2.
$$

Summing squared [partial derivatives](../../../../partial-derivative.md) according to their inclusion [probabilities](../../../../probability.md),

$$
\mathbb E_{\mathcal B}\|\nabla_{\mathcal B}f(x)\|^2=\frac1\ell\|\nabla f(x)\|^2.
$$

For a [strongly convex function](../../../../strongly-convex-function.md), part 2(a) also yields the [strong convexity gradient inequality](../../../../strong-convexity-gradient-inequality.md)

$$
\|\nabla f(x)\|^2\geq2\gamma\big(f(x)-f(x^*)\big).
$$

Indeed, substitute $y=x^*$ into the supporting inequality and complete the square in $x^*-x$: the expression $\nabla f(x)^Td+\gamma\|d\|^2/2$ is at least $-\|\nabla f(x)\|^2/(2\gamma)$ for every $d$.

Combining the last three estimates gives a contraction in [conditional expectation](../../../../conditional-expectation.md):

$$
\mathbb E[f(X^{t+1})-f(x^*)\mid X^t]
\leq\left(1-\frac\gamma{\ell\beta}\right)\big(f(X^t)-f(x^*)\big).
$$

By the [tower property](../../../../law-of-total-expectation.md) and repeated application,

$$
\mathbb E[f(X^t)-f(x^*)]\leq\left(1-\frac\gamma{\ell\beta}\right)^t\Delta_0
\leq\exp\left(-\frac{\gamma t}{\ell\beta}\right)\Delta_0.
$$

An [optimization epoch](../../../../optimization-epoch.md) counts $n$ coordinate [partial derivative](../../../../partial-derivative.md) evaluations: it comprises $\ell$ block updates or one full [gradient](../../../../gradient.md) update. With sampling with replacement, an [optimization epoch](../../../../optimization-epoch.md) is this work measure; it need not visit every coordinate. Consequently the block method needs

$$
\boxed{\begin{gathered}
O\left(\frac\beta\gamma\log\frac{\Delta_0}{\varepsilon}\right)\text{ epochs},\\
O\left(\frac{mL_{\max}}\gamma\log\frac{\Delta_0}{\varepsilon}\right)\text{ using }\beta=mL_{\max}.
\end{gathered}}
$$

to bring the expected [objective function](../../../../objective-function.md) gap below $\varepsilon$, for $0<\varepsilon<\Delta_0$, up to integer rounding.

For the [steepest descent method](../../../../gradient-descent-split.md), use a global [Lipschitz gradient](../../../../lipschitz-gradient.md) constant $L_f$. Part (c) with the full block permits $L_f=\sum_iL_i\leq nL_{\max}$. The [descent lemma](../../../../descent-lemma.md) with [step size](../../../../step-size.md) $1/L_f$, together with the [strong convexity gradient inequality](../../../../strong-convexity-gradient-inequality.md), gives

$$
f(x^{t+1})-f(x^*)\leq\left(1-\frac\gamma{L_f}\right)\big(f(x^t)-f(x^*)\big).
$$

An [exact line search](../../../../exact-line-search.md) along the negative [gradient](../../../../gradient.md) does at least as well in [objective function](../../../../objective-function.md) decrease per update. Ignoring its additional work, the resulting [epoch complexity](../../../../epoch-complexity.md) is

$$
\boxed{\begin{gathered}
O\left(\frac{L_f}\gamma\log\frac{\Delta_0}{\varepsilon}\right)\text{ epochs},\\
O\left(\frac{nL_{\max}}\gamma\log\frac{\Delta_0}{\varepsilon}\right)\text{ using }L_f=nL_{\max}.
\end{gathered}}
$$

**The common coordinate-based guarantees favour blocks by a factor $n/m=\ell$ in epochs.** In fact, with the conservative constants $\beta=mL_{\max}$ and $L_f=nL_{\max}$, both methods have the same guaranteed contraction per update, while a block update uses only $m$ coordinate [partial derivatives](../../../../partial-derivative.md).

This compares the bounds justified by the given constants. For a particular [objective function](../../../../objective-function.md), sharper constants give the comparison $\beta/\gamma$ against $L_f/\gamma$; an actual speedup of $\ell$ is not universal. Computing a [block coordinate gradient](../../../../block-coordinate-gradient.md) also need not cost exactly $m/n$ of a full [gradient](../../../../gradient.md) evaluation. The [epoch complexity](../../../../epoch-complexity.md) comparison assumes that coordinate [partial derivative](../../../../partial-derivative.md) counts are a useful measure of work, and does not itself establish a wall-clock comparison.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
