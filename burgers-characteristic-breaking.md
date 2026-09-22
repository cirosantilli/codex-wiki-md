# Burgers characteristic breaking

↑ **Parent:** [Inviscid Burgers equation](inviscid-burgers-equation.md)

Before [characteristic crossing](characteristic-crossing.md), the [method of characteristics](method-of-characteristics.md) for the [Inviscid Burgers equation](inviscid-burgers-equation.md) transports each initial value without changing it:

$$
\frac{dx}{dt}=u,\qquad \frac{du}{dt}=0,\qquad x=\xi+t u_0(\xi),\qquad u(x,t)=u_0(\xi).
$$

Here $\xi$ labels the starting position. Suppose $u_0$ is a bounded [continuously differentiable function](continuously-differentiable-function.md) with bounded [derivative](derivative.md). As long as $1+t u_0'(\xi)>0$ for every label, the [characteristic flow map](characteristic-flow-map.md) is invertible and differentiating it gives the displayed formula for $u_x$.[§2.1, Quasilinear equations, Example 7, (2.1.8)–(2.1.9)](partial-differential-equations-by-victor-ivrii/first-order-pdes.md)

If the negative minimum $m=\min_\xi u_0'(\xi)$ is attained, the first breaking time is $t_*=-1/m$. Two labels $\xi_1<\xi_2$ with $u_0(\xi_1)>u_0(\xi_2)$ have formal intersection time

$$
t=\frac{\xi_2-\xi_1}{u_0(\xi_1)-u_0(\xi_2)}>0.
$$

Their neighboring-label limit explains why the most negative initial slope breaks first. As $t\uparrow t_*$, the amplitude remains bounded but $u_x$ diverges: this is [gradient blow-up](gradient-blow-up.md). Continuing intersecting lines would assign incompatible values at one position; the post-breaking [entropy solution](entropy-solution.md) instead uses [shock waves](shock-wave.md). Nondecreasing data have no forward [characteristic crossing](characteristic-crossing.md) by this mechanism.

For a concrete calculation in [dimensionless quantities](dimensionless-quantity.md) on the infinite line, choose $u_0(\xi)=1-\tanh\xi$, with limiting states $2$ and $0$. Then $u_0'(\xi)=-(1-\tanh^2\xi)$ has minimum $-1$ at $\xi=0$, so $t_*=1$ and the breaking point is $(x,t)=(1,1)$. Along the central [characteristic curve](characteristic-curve.md) $x=t$, $u=1$ and $u_x=-1/(1-t)$ before breaking. The labels $\xi=\pm1$ give intersecting formal lines at $t=1/\tanh1\approx1.313$, after the [classical solution](classical-solution.md) has already broken.

<a id="image-decreasing-initial-data-steepen-the-first-gradient-blow-up-is-at-time-1-before-two-selected-characteristics-intersect"></a>
![](burgers-finite-time-characteristic-crossing.png)

**[Figure 2](#image-decreasing-initial-data-steepen-the-first-gradient-blow-up-is-at-time-1-before-two-selected-characteristics-intersect). Decreasing initial data steepen: the first gradient blow-up is at time 1, before two selected characteristics intersect**.

## ↑ Ancestors (8)

1. [Inviscid Burgers equation](inviscid-burgers-equation.md)
2. [Scalar conservation law](scalar-conservation-law.md)
3. [Transport equation](transport-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Burgers' equation](burgers-equation.md)
- [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md)
