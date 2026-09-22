<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a discretized [ordinary differential equation](../../../../../ordinary-differential-equation.md), error control must distinguish the [local truncation error](../../../../../local-truncation-error.md) of one exact-start step from accumulated [global error](../../../../../global-discretization-error.md). For a smooth order-$p$ one-step method, these are usually $O(h^{p+1})$ and $O(h^p)$ respectively, provided perturbations propagate stably. A small local defect is useful only when the underlying problem and the numerical update do not amplify it excessively.

There are several practical [local error estimators](../../../../../local-error-estimator.md). In [step-doubling error estimation](../../../../../step-doubling-error-estimation.md), compute one step $Y_h$ and two half steps $Y_{h/2,h/2}$ from the same starting value. If the leading method error is $Ch^{p+1}$, the two-half-step error is $Ch^{p+1}/2^p$, up to higher terms. Their difference $D=Y_{h/2,h/2}-Y_h$ therefore gives

$$
e_{\rm fine}\simeq\frac{D}{2^p-1}
$$

for exact minus fine-step error. Adding that estimate is [Richardson extrapolation](../../../../../richardson-extrapolation.md). This costs extra evaluations but gives an independent check on a single-method implementation; nonsmooth events can invalidate the assumed expansion.

An [embedded Runge-Kutta pair](../../../../../embedded-runge-kutta-pair.md) shares stages and uses two output weight vectors to obtain orders $p$ and $q<p$. Their difference generally estimates the lower-order local error $O(h^{q+1})$, not the higher-order error directly. Stage reuse makes this much cheaper than independent integrations. [Predictor-corrector error estimation](../../../../../predictor-corrector-error-estimation.md) uses the appropriately calibrated difference of two formulas; raw predictor/corrector differences require their known error constants. For multistep schemes, changing the step size also changes interpolation coefficients and requires controlled step ratios and proper history updates, rather than reusing constant-step coefficients.

Component scales should reflect the requested physical accuracy. An example of [absolute and relative error tolerances](../../../../../absolute-and-relative-error-tolerances.md) is

$$
s_i={\rm atol}_i+{\rm rtol}_i\max(|y_{n,i}|,|Y_{n+1,i}|),
\qquad E=\max_i|\widehat e_i|/s_i.
$$

Positive absolute tolerances avoid singular scaling when a component vanishes, while relative tolerances track widely differing magnitudes. Accept the step if $E\leq1$; otherwise reject it without committing the new state or multistep history. If the estimated defect scales as $h^r$, a basic [adaptive step-size controller](../../../../../adaptive-step-size-controller.md) proposes

$$
h_{\rm new}=h\,\operatorname{clip}(f_{\min},f_{\max},\eta E^{-1/r}),
\qquad 0<\eta<1.
$$

Growth limits, a safety factor, and proportional-integral smoothing reduce erratic changes. The exponent must match the actual estimator: $r=p+1$ for a genuine order-$p$ local defect, but $r=p$ for the usual $p/(p-1)$ embedded difference. It is not always $1/p$ or always $1/(p+1)$. A zero estimate uses a finite maximum growth factor, not division by zero.

Local acceptance does not itself certify a global error tolerance. If a dense approximation $\eta(t)$ has residual $d(t)=\eta'(t)-f(t,\eta(t))$ and $f$ is [Lipschitz continuous](../../../../../lipschitz-continuity.md) with constant $L$ on the relevant trajectory region, [Gronwall's inequality](../../../../../gronwall-inequality.md) gives the [residual bound for global ODE error](../../../../../residual-bound-for-global-ode-error.md)

$$
\|y(t)-\eta(t)\|\leq e^{L(t-t_0)}\|y(t_0)-\eta(t_0)\|
+\int_{t_0}^t e^{L(t-s)}\|d(s)\|\,ds.
$$

The discrete analogue propagates and sums local defects. A posteriori defect correction, repeat integrations with tighter tolerances, and adjoint-weighted estimates for a chosen final functional provide stronger global checks. A smaller local target may be needed in an unstable flow; trajectory sensitivity should not be mislabeled as a code defect.

For a [stiff differential equation](../../../../../stiff-equation.md), [absolute stability](../../../../../linear-stability-domain.md) can constrain explicit steps far more tightly than accuracy alone. Use an appropriate implicit method and keep nonlinear stage/linear-solve errors below the discretization-error budget. [A-stability](../../../../../a-stability.md), [L-stability](../../../../../l-stability.md) and [B-stability](../../../../../b-stability.md) address different linear damping and nonlinear contractivity properties. An error controller cannot repair a method outside its stability domain. Tolerance-driven adaptation also does not automatically preserve positivity, conservation laws or a symplectic structure; these may require a suitable method or an additional acceptance test.

Finally, event detection and dense output have their own errors. Locate an event with a consistent interpolant and account for its state sensitivity; a discontinuous right side may require restarting the integrator. Refining indefinitely eventually exposes [roundoff error](../../../../../round-off-error.md) and conditioning limits. Reliable error control balances truncation, solution sensitivity, algebraic-solve error and floating-point error, while reporting failure to meet a target instead of endlessly shrinking a step.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [Section II](../section-ii.md)
3. [Paper 69](../../paper-69-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
