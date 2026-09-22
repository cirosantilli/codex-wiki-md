<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $x=X_0>0$ and $a>1/2$. For the construction take $0<\varepsilon<x$, the range relevant to localization at zero, and define

$$
g_\varepsilon(y)=\frac a{y\vee\varepsilon}\qquad(y\in\mathbb R).
$$

This drift is bounded by $a/\varepsilon$ and globally Lipschitz with constant at most $a/\varepsilon^2$. Together with the constant diffusion coefficient $1$, the [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) gives a unique [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md) $U^\varepsilon$ of

$$
dU_t^\varepsilon=dB_t+g_\varepsilon(U_t^\varepsilon)dt,\qquad U_0^\varepsilon=x,
$$

for the prescribed driving [Brownian motion](../../../../../../brownian-motion-split.md). Let $T_\varepsilon^\varepsilon=\inf\{t:U_t^\varepsilon=\varepsilon\}$ and choose $X_t^\varepsilon=U_{t\wedge T_\varepsilon^\varepsilon}^\varepsilon$ as the stopped continuation. Before this time the drift is exactly $a/X_t^\varepsilon$. Uniqueness here means uniqueness up to the [stopping time](../../../../../../stopping-time.md); the equation imposes no restriction on arbitrary continuations after it.

For $0<\delta<\varepsilon<x$, the two equations have the same coefficients while both solutions exceed $\varepsilon$. By local [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) they coincide until that level is reached. Thus the first hit of $\varepsilon$ by $X^\delta$ is $T_\varepsilon^\varepsilon$, and its later first hit of $\delta$ satisfies

$$
\boxed{T_\delta^\delta\geq T_\varepsilon^\varepsilon.}
$$

Patch along a deterministic sequence $\varepsilon_n\downarrow0$: for $t<T:=\lim_nT_{\varepsilon_n}^{\varepsilon_n}$, choose $n$ with $t<T_{\varepsilon_n}^{\varepsilon_n}$ and set $X_t=X_t^{\varepsilon_n}$. Compatibility makes the definition independent of $n$. It gives a continuous adapted positive process satisfying the original equation on every compact time interval before $T$. The same compatibility holds for other threshold choices, so the lifetime is the limit as $\varepsilon\downarrow0$, not a property of the chosen sequence.

To prove $T=\infty$, put $\nu=2a-1>0$ and $s(y)=y^{-\nu}$. Its generator vanishes. On each finite horizon, Itô's formula makes $s(X_{t\wedge T_\varepsilon^\varepsilon}^\varepsilon)$ a true [martingale](../../../../../../martingale-split.md), because its stochastic integrand is bounded by $\nu\varepsilon^{-\nu-1}$. Positivity therefore implies

$$
\varepsilon^{-\nu}\mathbb P(T_\varepsilon^\varepsilon\leq t)\leq\mathbb E s(X_{t\wedge T_\varepsilon^\varepsilon}^\varepsilon)=x^{-\nu},\qquad\mathbb P(T_\varepsilon^\varepsilon\leq t)\leq\left(\frac\varepsilon x\right)^\nu.
$$

Since $\{T\leq t\}$ is contained in each $\{T_\varepsilon^\varepsilon\leq t\}$, letting $\varepsilon\downarrow0$ gives $\mathbb P(T\leq t)=0$. Taking a countable union over integer $t$ proves $T=\infty$ almost surely. This is the [truncation construction of a positive Bessel strong solution](../../../../../../truncation-construction-of-a-positive-bessel-strong-solution.md).

For two positive solutions driven by the same [Brownian motion](../../../../../../brownian-motion-split.md), localize at their first hits of $\varepsilon$. The cutoff equations and [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) make them equal up to those times. On every finite interval both positive continuous paths have positive minima, so decreasing $\varepsilon$ removes the localization and proves indistinguishability. Thus

$$
\boxed{a>\tfrac12:\quad\text{a global positive strong solution exists for every driving Brownian motion, and pathwise uniqueness holds}.}
$$

The resulting global solution also supplies the stopped solution for any threshold $\varepsilon\geq x$, completing the literal all-threshold existence request. The monotonicity used to construct the zero-boundary lifetime concerns the thresholds $\varepsilon<x$ tending to zero; upper-threshold hitting times have the opposite ordering. Strong adaptation is preserved because every cutoff solution is strong and the patch uses their [stopping times](../../../../../../stopping-time.md) in the given filtration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
