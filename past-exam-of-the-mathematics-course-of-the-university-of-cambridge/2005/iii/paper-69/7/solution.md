<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

An ODE solver must distinguish the error made by one step started from exact data from the error accumulated along the computed trajectory. For an order-$p$ one-step map $\Phi_h$, define the exact-start defect $d_n=y(t_{n+1})-\Phi_{h_n}(t_n,y(t_n))=O(h_n^{p+1})$. If the step map is Lipschitz with factor $1+Lh_n$, its [global error](../../../../../global-discretization-error.md) obeys

$$
\|e_{n+1}\|\leq(1+Lh_n)\|e_n\|+C h_n^{p+1}.
$$

Iteration, using $1+Lh\leq e^{Lh}$, proves the [variable-step global ODE error bound](../../../../../variable-step-global-ode-error-bound.md)

$$
\boxed{\|e_N\|\leq e^{LT}\left(\|e_0\|+C\sum_nh_n^{p+1}\right)
\leq e^{LT}\left(\|e_0\|+CT h_{\max}^p\right).}
$$

It explains the difference between local defect order $p+1$ and global order $p$, and why local tolerance control alone does not certify a prescribed [global error](../../../../../global-discretization-error.md). Strong dynamical amplification can magnify many individually small defects.

A practical solver needs an inexpensive [local error estimator](../../../../../local-error-estimator.md). In [step-doubling error estimation](../../../../../step-doubling-error-estimation.md), compare one full step $Y_h$ with two half steps $Y_f$. Smoothness and propagation through the second half step give $Y_h=y_{\rm exact}+Ch^{p+1}+O(h^{p+2})$ and $Y_f=y_{\rm exact}+Ch^{p+1}/2^p+O(h^{p+2})$. Therefore

$$
\widehat e_f=\frac{Y_f-Y_h}{2^p-1}\simeq y_{\rm exact}-Y_f,
\qquad Y_{\rm ext}=Y_f+\widehat e_f.
$$

The difference estimates the finer local correction with the correct denominator and sign; adding it cancels the leading error by [Richardson extrapolation](../../../../../richardson-extrapolation.md). The common starting value and the smooth error expansion are essential, and the extra evaluations make this estimator relatively expensive.

An [embedded Runge-Kutta pair](../../../../../embedded-runge-kutta-pair.md) instead shares the stage computations and uses two output weight vectors. For orders $p$ and $p-1$, their difference is generally $O(h^p)$ and estimates the lower-order local defect, even when the higher-order output is accepted. Its controller exponent is therefore $1/p$, not $1/(p+1)$. For example the explicit Euler and Heun outputs share the first slope; their difference is $h(k_2-k_1)/2=O(h^2)$, while Heun's own defect is $O(h^3)$. Predictor-corrector differences can also estimate a defect when scaled by the appropriate leading error constants; an uncalibrated raw difference need not be the corrected method's error.

For a vector equation, choose positive component scales

$$
s_i={\rm atol}_i+{\rm rtol}_i\max(|y_{n,i}|,|Y_i|),\qquad
E=\max_i|\widehat e_i|/s_i.
$$

The [absolute and relative error tolerances](../../../../../absolute-and-relative-error-tolerances.md) allow meaningful tests both near zero and for large components with different physical scales. The max-norm criterion $E\leq1$ controls every scaled estimated component. A root-mean-square criterion is another common choice but has a weaker individual-component implication.

If the estimate scales like $E\simeq Ch^q$, an [adaptive step-size controller](../../../../../adaptive-step-size-controller.md) uses

$$
\boxed{h_{\rm new}=h\,\eta E^{-1/q},\qquad0<\eta<1,}
$$

with lower and upper bounds on the change factor. A rejected step leaves the old state and time unchanged and recomputes with a smaller step; an accepted step advances with the chosen output and adjusts the next step. A zero estimate receives capped finite growth rather than division by zero. The safety factor allows for variation in the error constant. Step doubling has $q=p+1$, whereas a $p/(p-1)$ embedded pair usually has $q=p$. If a solver instead controls defect per unit time, division by $h$ changes the scaling exponent and must be included in the controller design.

Using previous estimates can smooth the sequence of accepted steps. A proportional-integral controller can take $h_{n+1}/h_n=\eta E_n^{-a}E_{n-1}^{b}$ with $0<b<a$, appropriate scaling by the estimator order and bounded factors. It avoids overreacting to a single noisy estimate, but needs safeguards after rejected steps, changes of order and abrupt coefficient changes. Event locations and discontinuities require locating the event and restarting the error expansion; blindly applying a smooth-step estimator across a jump can be misleading.

For a [multistep method](../../../../../linear-multistep-method.md), adaptive step sizes change the interpolation history and coefficients. Constant-step coefficients cannot simply be reused with arbitrary step ratios. Variable-step formulas, compatible starting/restarting procedures and bounded ratios preserve the needed [stability](../../../../../stability-of-a-numerical-method.md); local error and sometimes order are selected together to balance evaluation cost against accuracy.

Stiffness imposes an additional requirement. On a rapidly decaying mode $y'=-\kappa y$, explicit Euler requires $h\kappa\leq2$ for [absolute stability](../../../../../linear-stability-domain.md). Once $y$ is small, a local absolute-tolerance test can propose a large step even though roundoff or a small perturbation would then be amplified. A stiff solver therefore also uses a suitable implicit [A-stable](../../../../../a-stability.md) or [L-stable](../../../../../l-stability.md) method and solves its algebraic equations accurately enough for the estimator to be meaningful. [A-stability](../../../../../a-stability.md) alone does not ensure stiff decay, as the Lobatto [stability function](../../../../../stability-function.md) in question 4 tends to one for large negative arguments.

Finally, over-tightening tolerance eventually encounters roundoff and algebraic-solve error rather than further truncation-error improvement. Inexact Newton or linear solves must have errors below the local budget; a tiny time step with an inaccurate stage solve does not deliver the formal order. [Global error](../../../../../global-discretization-error.md) assessment can use controlled refinements, defect propagation or adjoint weighting for a chosen output. Sensible error and step-size control therefore combines asymptotic estimators, tolerance scaling, [stability](../../../../../stability-of-a-numerical-method.md), event handling and implementation error, rather than treating the accepted local estimate as a complete guarantee about the trajectory.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
