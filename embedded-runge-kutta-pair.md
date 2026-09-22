# Embedded Runge-Kutta pair

↑ **Parent:** [Local error estimator](local-error-estimator.md)

Two [Runge-Kutta methods](runge-kutta-method-split.md) share a stage matrix and nodes but use different output weights. An order-$p$ and order-$q$ pair with $q<p$ gives an output difference generally of order $h^{q+1}$, estimating the lower-order defect. Shared stage evaluations reduce the cost. The [adaptive step-size controller](adaptive-step-size-controller.md) exponent must reflect this estimator order, rather than blindly the higher reported solution order.

Using the slope convention for [Runge-Kutta stages](runge-kutta-stage.md), an [embedded Runge-Kutta pair](embedded-runge-kutta-pair.md) computes

$$
Y^{[p]}=y_n+h\sum_{i=1}^sb_i k_i,\qquad Y^{[q]}=y_n+h\sum_{i=1}^s\widehat b_i k_i,\qquad d=Y^{[p]}-Y^{[q]}=h\sum_{i=1}^s(b_i-\widehat b_i)k_i.
$$

Its [Butcher tableau](butcher-tableau.md) has two output rows, $b^T$ and $\widehat b^T$. Evaluating $f$ is often the expensive part of solving an [ordinary differential equation](ordinary-differential-equation.md); after the shared slopes have been computed, the extra row needs only another linear combination.[§6.5.2, embedded formulas and equation 6.5.5: common stages and two output rows](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/6-5-adaptive-runge-kutta.md)

Write $\Phi$ for the exact endpoint from the current numerical state, and define signed local defects $\ell_q=\Phi-Y^{[q]}$ and $\ell_p=\Phi-Y^{[p]}$. Then $d=\ell_q-\ell_p$. If $\ell_q=C_qh^{q+1}+O(h^{q+2})$ and $\ell_p=O(h^{p+1})$, with $C_q\ne0$, the difference reproduces the leading lower-order defect. It does not reproduce the leading higher-order defect. Here the powers use [big O notation](big-o-notation.md) and a smooth [Taylor expansion](taylor-expansion.md); a vanishing leading coefficient or accidental cancellation can make the estimate misleading.

A common choice accepts $Y^{[p]}$ after testing $d$ with [absolute and relative error tolerances](absolute-and-relative-error-tolerances.md). With the scale approximately unchanged on a retry, the [adaptive step-size controller](adaptive-step-size-controller.md) uses exponent $1/(q+1)$. Accepting a better endpoint does not change the power in the quantity being tested. The [Euler-Heun embedded pair](euler-heun-embedded-pair.md) makes this visible without a large coefficient table.[§6.5.1, equations 6.5.1–6.5.3 and Algorithm 6.5.1: lower-order local estimate and higher-order accepted output](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/6-5-adaptive-runge-kutta.md)

**Table of contents**

- [Euler-Heun embedded pair](euler-heun-embedded-pair.md)
  - [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md)

## ↑ Ancestors (7)

1. [Local error estimator](local-error-estimator.md)
2. [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Adaptive step-size controller](adaptive-step-size-controller.md)
- [Butcher tableau](butcher-tableau.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
- [Local error estimator](local-error-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
- [Runge-Kutta method](runge-kutta-method-split.md)
