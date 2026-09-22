# Finite volume method

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_volume_method)

The [finite volume method](finite-volume-method.md) follows the amount of a conserved quantity inside each [control volume](control-volume.md). Its unknowns are [cell averages](average-value-of-a-function.md), rather than values at isolated points: a cell's width times its stored average approximates that cell's total. A [numerical flux](numerical-flux.md) transfers an amount across a face. Using one shared transfer for both neighboring cells makes the loss from one exactly the gain of the other, as explained in [shared face flux cancellation](shared-face-flux-cancellation.md).[Approximate solvers, §Finite volume methods, equation FVupdate and the following cancellation argument](riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo.md)

For a one-dimensional [scalar conservation law](scalar-conservation-law.md) without sources, let $u_t+\partial_x f(u)=0$, with [conservation law flux](conservation-law-flux.md) $f$. Fix cells $I_j=[x_{j-1/2},x_{j+1/2}]$ of widths $h_j>0$. Define the exact [cell average](average-value-of-a-function.md) and its numerical approximation by

$$
\overline u_j(t)=\frac1{h_j}\int_{I_j}u(x,t)\,dx,\qquad U_j^n\approx\overline u_j(t_n).
$$

The integral balance over one cell and one time interval of length $k>0$ is

$$
h_j\bigl(\overline u_j(t_n+k)-\overline u_j(t_n)\bigr)=\int_{t_n}^{t_n+k}\bigl[f(u(x_{j-1/2},t))-f(u(x_{j+1/2},t))\bigr]\,dt.
$$

For a smooth solution this follows by [integration](integral.md) of the differential equation; with [jump discontinuities](jump-discontinuity.md), it expresses the [conservation law](conservation-law.md) in integral form, using appropriate face traces when they exist. Replacing each time-averaged face [conservation law flux](conservation-law-flux.md) by a [numerical flux](numerical-flux.md) gives

$$
U_j^{n+1}=U_j^n-\frac{k}{h_j}\bigl(F_{j+1/2}^n-F_{j-1/2}^n\bigr).
$$

Thus the [finite volume method](finite-volume-method.md) implements a balance directly, without needing a pointwise [derivative](derivative.md) at a jump. The tube balance in [Riemann Problems and Jupyter Solutions by David I. Ketcheson, Randall J. LeVeque, and Mauricio J. del Razo](riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo.md) (Advection, §Conservation of mass) motivates this construction from [conservation of mass](mass-conservation.md).

This is useful for [shock waves](shock-wave.md): their speed is constrained by the [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md), itself an integral balance. A nonconservative approximation can give a visibly plausible jump with the wrong speed. Conservation is one requirement; a nonlinear [scalar conservation law](scalar-conservation-law.md) also needs the correct [entropy solution](entropy-solution.md), and the chosen [numerical flux](numerical-flux.md) and update need their own [stability](stability-of-a-numerical-method.md) and accuracy analysis.[Approximate solvers, §§Finite volume methods, Godunov's method, High-resolution methods: wrong shock speeds, time-step restrictions and smeared jumps](riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo.md) The original [periodic upwind finite volume advection](periodic-upwind-finite-volume-advection.md) example isolates the shared-transfer mechanism in a problem with a known translated solution.

**Table of contents**

- [Shared face flux cancellation](shared-face-flux-cancellation.md)
- [Periodic upwind finite volume advection](periodic-upwind-finite-volume-advection.md)
- [Monotone conservative scheme](monotone-conservative-scheme.md)
  - [Total variation diminishing scheme](total-variation-diminishing-scheme.md)
  - [L1 contraction of a monotone conservative scheme](l1-contraction-of-a-monotone-conservative-scheme.md)
  - [Engquist-Osher method](engquist-osher-method.md)
    - [CFL necessity for explicit Engquist-Osher stability](cfl-necessity-for-explicit-engquist-osher-stability.md)
    - [Engquist-Osher flux](engquist-osher-flux.md)
      - [Sonic-point splitting of a convex Engquist-Osher flux](sonic-point-splitting-of-a-convex-engquist-osher-flux.md)
- [Numerical flux](numerical-flux.md)
  - [Godunov numerical flux](godunov-numerical-flux.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Engquist-Osher method](engquist-osher-method.md)
- [Finite volume method](finite-volume-method.md)
- [Numerical flux](numerical-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/6/solution.md)
- [Periodic upwind finite volume advection](periodic-upwind-finite-volume-advection.md)
- [Shared face flux cancellation](shared-face-flux-cancellation.md)
