# Euler-Heun embedded pair

↑ **Parent:** [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)

The Euler-Heun 1(2) pair combines the [explicit Euler method](euler-method.md) and [Heun's method](heun-s-method.md). Here 1(2) names their respective [order of a numerical method](order-of-a-numerical-method.md); the accepted endpoint in this article is the second-order one. Its shared [Runge-Kutta stages](runge-kutta-stage.md) and endpoints are

$$
\begin{aligned}
k_1&=f(t_n,y_n),&k_2&=f(t_n+h,y_n+hk_1),\\
Y^{[1]}&=y_n+hk_1,&Y^{[2]}&=y_n+\frac h2(k_1+k_2),\\
d&=Y^{[2]}-Y^{[1]}=\frac h2(k_2-k_1).
\end{aligned}
\qquad
\begin{array}{c|cc}
0&0&0\\
1&1&0\\\hline
&\tfrac12&\tfrac12\\
&1&0
\end{array}
$$

The first output row in this [Butcher tableau](butcher-tableau.md) is [Heun's method](heun-s-method.md); the second is the [explicit Euler method](euler-method.md). Both outputs cost two evaluations of $f$ together, rather than one for [Euler method](euler-method.md) plus two for a separately computed [Heun's method](heun-s-method.md).

For the [initial value problem](initial-value-problem.md) $y'=y$, $y(0)=1$, take $h=0.2$. The first slope is $k_1=1$; the stage state is $1+0.2k_1=1.2$, giving $k_2=1.2$. Therefore

$$
Y^{[1]}=1.2,\qquad Y^{[2]}=1.22,\qquad d=0.02,\qquad y(0.2)=e^{0.2}\approx1.22140275816.
$$

The exact [exponential function](exponential-function.md) gives signed local defects approximately $0.02140275816$ for the [explicit Euler method](euler-method.md) and $0.00140275816$ for [Heun's method](heun-s-method.md). Their difference is exactly $0.02$. Thus the pair difference estimates the larger Euler defect; calling it the actual Heun defect would miss by a factor about fourteen here.

More generally, a step from $y_n$ on $y'=y$ has

$$
\begin{aligned}
\ell_1&=y_n(e^h-1-h)=y_n\left(\frac{h^2}{2}+\frac{h^3}{6}+O(h^4)\right),\\
\ell_2&=y_n(e^h-1-h-h^2/2)=y_n\left(\frac{h^3}{6}+O(h^4)\right),\\
d&=y_n\frac{h^2}{2}.
\end{aligned}
$$

These original [Taylor expansions](taylor-expansion.md) separate three quantities: the accepted [Heun's method](heun-s-method.md) has [local truncation error](local-truncation-error.md) $O(h^3)$ and [global error](global-discretization-error.md) $O(h^2)$ under suitable [numerical stability](stability-of-a-numerical-method.md), while the tested [local error estimator](local-error-estimator.md) is $O(h^2)$. For $E=|d|/s$ with $s$ held approximately fixed, use $h_{\rm new}=\eta h E^{-1/2}$. A cube-root update would model a different quantity, the actual higher-order local defect.

**Table of contents**

- [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md)

## ↑ Ancestors (8)

1. [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
2. [Local error estimator](local-error-estimator.md)
3. [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
- [Heun's method](heun-s-method.md)
