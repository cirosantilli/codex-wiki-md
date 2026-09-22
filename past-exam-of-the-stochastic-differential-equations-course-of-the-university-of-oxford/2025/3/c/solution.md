<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K=\sup_x f(x)<\infty$ and let $C$ be a [Lipschitz constant](../../../../lipschitz-constant.md) for $f$. Since

$$
|f(x)^2-f(y)^2|\leq2KC|x-y|,
$$

both coefficients $f$ and $-f^2/2$ are bounded and [globally Lipschitz](../../../../globally-lipschitz-function.md). The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) gives a unique global [strong solution of a stochastic differential equation](../../../../strong-solution-of-a-stochastic-differential-equation.md).

The same [Itô formula](../../../../ito-s-lemma.md) cancellation as before gives

$$
d(e^{X_t})=e^{X_t}f(X_t)\,dB_t,\qquad
[e^X]_t=\int_0^te^{2X_s}f(X_s)^2\,ds.
$$

For $S=T_{-a}\wedge T_b$, the stopped exponential is bounded between $e^{-a}$ and $e^b$. Continuity and strict positivity of $f$ give

$$
c_{a,b}:=\min_{x\in[-a,b]}e^{2x}f(x)^2>0.
$$

The [Itô isometry](../../../../ito-isometry.md) therefore yields

$$
1+c_{a,b}\mathbb E[t\wedge S]
\leq\mathbb E e^{2X_{t\wedge S}}\leq e^{2b}.
$$

The [monotone convergence theorem](../../../../monotone-convergence-theorem.md) proves $\mathbb ES<\infty$. The bounded [optional stopping](../../../../optional-sampling-theorem-for-a-supermartingale.md) argument is now identical to part (b)(iii), and gives

$$
\mathbb P(T_b<T_{-a})=\frac{1-e^{-a}}{e^b-e^{-a}},\qquad
\mathbb P(T_b<\infty)=e^{-b}.
$$

Passing from level hitting to strict exceedances as in part (b)(iv),

$$
\boxed{X^\star\sim\operatorname{Exp}(1).}
$$

No global positive lower bound on $f$ was needed: compact-interval positivity suffices for each exit argument. The law is independent of the particular $f$ because the [scale function](../../../../scale-function-stochastic-processes.md) is always $s(x)=e^x$: its [infinitesimal generator](../../../../infinitesimal-generator-stochastic-processes.md) satisfies

$$
\mathcal Ls=\frac{f^2}{2}(s''-s')=0.
$$

This is the [exponential scale function for a drift tied to diffusivity](../../../../exponential-scale-function-for-a-drift-tied-to-diffusivity.md). Changing $f$ changes how quickly the path is traversed, but leaves these boundary probabilities and the maximum law unchanged.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
