# Finite volume method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_volume_method)

The [finite volume method](finite-volume-method.md) follows the amount of a conserved quantity inside each [control volume](fluid-mechanics.md#control-volume). Its unknowns are [cell averages](integral.md#average-value-of-a-function), rather than values at isolated points: a cell's width times its stored average approximates that cell's total. A [numerical flux](#numerical-flux) transfers an amount across a face. Using one shared transfer for both neighboring cells makes the loss from one exactly the gain of the other, as explained in [shared face flux cancellation](#shared-face-flux-cancellation).[Approximate solvers, §Finite volume methods, equation FVupdate and the following cancellation argument](mathematics-bibliography.md#riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo)

For a one-dimensional [scalar conservation law](transport-equation.md#scalar-conservation-law) without sources, let $u_t+\partial_x f(u)=0$, with [conservation law flux](transport-equation.md#conservation-law-flux) $f$. Fix cells $I_j=[x_{j-1/2},x_{j+1/2}]$ of widths $h_j>0$. Define the exact [cell average](integral.md#average-value-of-a-function) and its numerical approximation by

$$
\overline u_j(t)=\frac1{h_j}\int_{I_j}u(x,t)\,dx,\qquad U_j^n\approx\overline u_j(t_n).
$$

The integral balance over one cell and one time interval of length $k>0$ is

$$
h_j\bigl(\overline u_j(t_n+k)-\overline u_j(t_n)\bigr)=\int_{t_n}^{t_n+k}\bigl[f(u(x_{j-1/2},t))-f(u(x_{j+1/2},t))\bigr]\,dt.
$$

For a smooth solution this follows by [integration](integral.md) of the differential equation; with [jump discontinuities](calculus.md#jump-discontinuity), it expresses the [conservation law](mathematical-physics.md#conservation-law) in integral form, using appropriate face traces when they exist. Replacing each time-averaged face [conservation law flux](transport-equation.md#conservation-law-flux) by a [numerical flux](#numerical-flux) gives

$$
U_j^{n+1}=U_j^n-\frac{k}{h_j}\bigl(F_{j+1/2}^n-F_{j-1/2}^n\bigr).
$$

Thus the [finite volume method](finite-volume-method.md) implements a balance directly, without needing a pointwise [derivative](calculus.md#derivative) at a jump. The tube balance in [Riemann Problems and Jupyter Solutions by David I. Ketcheson, Randall J. LeVeque, and Mauricio J. del Razo](mathematics-bibliography.md#riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo) (Advection, §Conservation of mass) motivates this construction from [conservation of mass](continuum-mechanics.md#mass-conservation).

This is useful for [shock waves](transport-equation.md#shock-wave): their speed is constrained by the [Rankine-Hugoniot condition](transport-equation.md#rankine-hugoniot-conditions), itself an integral balance. A nonconservative approximation can give a visibly plausible jump with the wrong speed. Conservation is one requirement; a nonlinear [scalar conservation law](transport-equation.md#scalar-conservation-law) also needs the correct [entropy solution](transport-equation.md#entropy-solution), and the chosen [numerical flux](#numerical-flux) and update need their own [stability](numerical-analysis.md#stability-of-a-numerical-method) and accuracy analysis.[Approximate solvers, §§Finite volume methods, Godunov's method, High-resolution methods: wrong shock speeds, time-step restrictions and smeared jumps](mathematics-bibliography.md#riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo) The original [periodic upwind finite volume advection](#periodic-upwind-finite-volume-advection) example isolates the shared-transfer mechanism in a problem with a known translated solution.

**Table of contents**

- [Shared face flux cancellation](#shared-face-flux-cancellation)
- [Periodic upwind finite volume advection](#periodic-upwind-finite-volume-advection)
- [Monotone conservative scheme](#monotone-conservative-scheme)
  - [Total variation diminishing scheme](#total-variation-diminishing-scheme)
  - [L1 contraction of a monotone conservative scheme](#l1-contraction-of-a-monotone-conservative-scheme)
  - [Engquist-Osher method](#engquist-osher-method)
    - [CFL necessity for explicit Engquist-Osher stability](#cfl-necessity-for-explicit-engquist-osher-stability)
    - [Engquist-Osher flux](#engquist-osher-flux)
      - [Sonic-point splitting of a convex Engquist-Osher flux](#sonic-point-splitting-of-a-convex-engquist-osher-flux)
- [Numerical flux](#numerical-flux)
  - [Godunov numerical flux](#godunov-numerical-flux)

## Shared face flux cancellation

↑ **Parent:** [Finite volume method](finite-volume-method.md)

In a [finite volume method](finite-volume-method.md), orient every face [numerical flux](#numerical-flux) to the right. For cells $1,\ldots,N$, write the discrete total as $M^n=\sum_{j=1}^N h_jU_j^n$. If $u$ is a mass per unit length, this total approximates [mass](classical-mechanics.md#mass); for a different conserved field, it measures that field's [integral](integral.md). Multiplying the update by the cell width gives an amount balance, so adjacent cells contribute

$$
\begin{aligned}
h_j(U_j^{n+1}-U_j^n)&=kF_{j-1/2}^n-kF_{j+1/2}^n,\\
h_{j+1}(U_{j+1}^{n+1}-U_{j+1}^n)&=kF_{j+1/2}^n-kF_{j+3/2}^n.
\end{aligned}
$$

The interior face contributes $-kF_{j+1/2}^n+kF_{j+1/2}^n=0$. Summing all cells gives

$$
M^{n+1}-M^n=k\bigl(F_{1/2}^n-F_{N+1/2}^n\bigr).
$$

With [periodic boundary conditions](differential-equation.md#periodic-boundary-conditions), the two boundary labels denote the same physical face and must use the same [numerical flux](#numerical-flux); then $M^{n+1}=M^n$. On an open interval the total changes by the boundary transfers. Unequal widths require the weighted total $\sum h_jU_j$, not the unweighted [sum](arithmetic.md#sum) of [cell averages](integral.md#average-value-of-a-function).

<a id="image-one-oriented-face-transfer-leaves-the-left-cell-and-enters-the-right-cell-with-opposite-signs"></a>
![](finite-volume-shared-face-bookkeeping.png)

**[Figure 1](#image-one-oriented-face-transfer-leaves-the-left-cell-and-enters-the-right-cell-with-opposite-signs). One oriented face transfer leaves the left cell and enters the right cell with opposite signs**.

The diagram uses two unit-width cells, $k=1/4$, [cell averages](integral.md#average-value-of-a-function) $(2,1)$ and right-oriented [numerical fluxes](#numerical-flux) $(1,3,2)$ at their three faces. The updated [cell averages](integral.md#average-value-of-a-function) are $(3/2,5/4)$: the total changes from $3$ to $11/4$, exactly $k(1-2)=-1/4$. The shared interior transfer $k\cdot3=3/4$ cancels. If the receiving cell instead used $3+\varepsilon$ for that same face, the total would acquire the spurious term $k\varepsilon$. Conservation is therefore an algebraic property of sharing the transfer, even when the [numerical flux](#numerical-flux) is a poor approximation. In [floating-point arithmetic](floating-point-arithmetic.md), independently rounded cell updates may still leave small [roundoff errors](numerical-analysis.md#round-off-error) in the computed total.

## Periodic upwind finite volume advection

↑ **Parent:** [Finite volume method](finite-volume-method.md)

Consider the [advection equation](transport-equation.md) $u_t+a u_x=0$ with constant speed $a>0$, no sources, and [periodic boundary conditions](differential-equation.md#periodic-boundary-conditions) on $[0,1]$. Use $N$ equal cells of width $h=1/N$, time step $k>0$, and indices modulo $N$. The exact solution is the periodic translation $u(x,t)=u_0(x-at)$. At a face, the [Riemann problem](transport-equation.md#riemann-problem) transports the left state to the right, so the two-state upwind [numerical flux](#numerical-flux) is $F(L,R)=aL$, with $F(U,U)=aU$.[Advection, equations adv:advection and adv:solution, §The Riemann problem; Approximate solvers, §High-resolution methods: reduction to upwind advection](mathematics-bibliography.md#riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo)

The [finite volume method](finite-volume-method.md) with this [numerical flux](#numerical-flux) and an [explicit Euler method](numerical-analysis.md#euler-method) step gives

$$
F_{j+1/2}^n=aU_j^n,\qquad \nu=\frac{ak}{h},\qquad U_j^{n+1}=(1-\nu)U_j^n+\nu U_{j-1}^n.
$$

Here $U_j^n$ represents a [cell average](integral.md#average-value-of-a-function); the recurrence also occurs in the [upwind finite difference scheme](finite-difference.md#upwind-finite-difference-scheme). Impose the specific [CFL condition](finite-difference.md#courant-friedrichs-lewy-condition) $0<\nu\leq1$. Each updated [cell average](integral.md#average-value-of-a-function) is then a [convex combination](convex-set.md#convex-combination) of two old ones. This proves preservation of their initial minimum and maximum, including nonnegativity for nonnegative data, and contraction of the [maximum norm](normed-vector-space.md#supremum-norm) of the difference of two solutions on this periodic grid. These statements concern this constant-speed scalar update with this time step.

For an original synthetic example, take $N=8$, $a=1$, $h=1/8$, $k=1/16$, hence [Courant number](finite-difference.md#courant-number) $\nu=1/2$. Choose a [function](function.md) constant on each successive cell, with the following values, so these are exact initial [cell averages](integral.md#average-value-of-a-function). One step gives

$$
\begin{array}{c|rrrrrrrr}
j&0&1&2&3&4&5&6&7\\\hline
U_j^0&0&0&2&2&1&0&0&1\\
U_j^1&1/2&0&1&2&3/2&1/2&0&1/2
\end{array}
\qquad M^0=M^1=\frac18\cdot6=\frac34.
$$

For example, cell zero receives from cell seven across the periodic face: $U_0^1=(0+1)/2=1/2$. All eight face transfers cancel in the total by [shared face flux cancellation](#shared-face-flux-cancellation). More generally this periodic recurrence conserves the total algebraically for any $\nu$, even though the [CFL condition](finite-difference.md#courant-friedrichs-lewy-condition) is needed for the [convex combination](convex-set.md#convex-combination) argument. With the same initial data and $\nu=3/2$, one step gives $U_2^1=-1$ and $U_4^1=5/2$, despite preserving the total.

<a id="image-original-periodic-upwind-profile-at-zero-one-and-four-steps-the-integral-remains-three-quarters-while-jumps-spread"></a>
![](finite-volume-periodic-upwind-mass.png)

**[Figure 2](#image-original-periodic-upwind-profile-at-zero-one-and-four-steps-the-integral-remains-three-quarters-while-jumps-spread). Original periodic upwind profile at zero, one and four steps: the integral remains three quarters while jumps spread**.

After four steps, $t=1/4$, the exact translated profile has moved two cells to the right. Repeated averaging instead gives the explicit [binomial coefficient](binomial-coefficient.md) formula

$$
U_j^4=\frac1{16}\bigl(U_j^0+4U_{j-1}^0+6U_{j-2}^0+4U_{j-3}^0+U_{j-4}^0\bigr),
$$

with all indices modulo eight. The diagram compares these computed [cell averages](integral.md#average-value-of-a-function) with the exact translated [cell averages](integral.md#average-value-of-a-function). Their [integrals](integral.md) agree, but the numerical jumps spread across cells. The [finite volume method](finite-volume-method.md) is useful for [jump discontinuities](calculus.md#jump-discontinuity) because it retains the integral balance even at a jump; conservation alone does not guarantee a sharp profile. At $\nu=1$ this particular update is an exact one-cell shift, whereas for $0<\nu<1$ it mixes neighboring states. No accuracy conclusion at a jump follows just from the conserved total.

## Monotone conservative scheme

↑ **Parent:** [Finite volume method](finite-volume-method.md)

A scalar finite-volume update is monotone if increasing any input state cannot decrease any output state. A consistent conservative update preserves constants and has an invariant interval by comparison. On a periodic grid, or an infinite grid with summable perturbations, conservation and monotonicity imply [L1 contraction of a monotone conservative scheme](#l1-contraction-of-a-monotone-conservative-scheme). Translation invariance then implies the [total variation diminishing scheme](#total-variation-diminishing-scheme) property.

### Total variation diminishing scheme

↑ **Parent:** [Monotone conservative scheme](#monotone-conservative-scheme)

A translation-invariant conservative monotone update decreases discrete [total variation](sequence-and-series.md#total-variation). If $S$ is the one-cell shift, $TS=ST$, and [L1 contraction of a monotone conservative scheme](#l1-contraction-of-a-monotone-conservative-scheme) applied to $U,SU$ gives $\sum_j|(TU)_{j+1}-(TU)_j|\leq\sum_j|U_{j+1}-U_j|$. This prevents creation of new total variation, though it does not make every discontinuity sharply resolved.

### L1 contraction of a monotone conservative scheme

↑ **Parent:** [Monotone conservative scheme](#monotone-conservative-scheme)

Let $T$ be a monotone conservative scalar update on a periodic grid. Since $T(U\vee V)\geq TU,TV$, one has $(TU-TV)_+\leq T(U\vee V)-TV$. Conservation makes the sum of the right side equal to $\sum(U-V)_+$. Reverse $U,V$ and add to obtain $\|TU-TV\|_1\leq\|U-V\|_1$. On an infinite grid the same proof holds for summable differences with a Lipschitz flux on the state range.

### Engquist-Osher method

↑ **Parent:** [Monotone conservative scheme](#monotone-conservative-scheme)

The Engquist-Osher method is the [finite volume method](finite-volume-method.md) using the [Engquist-Osher flux](#engquist-osher-flux). Under $(k/d)\sup|f\prime|\leq1$ on the invariant state interval, its update is monotone. It preserves the state range, is contractive for summable perturbations in $L^1$, and decreases discrete [total variation](sequence-and-series.md#total-variation).

#### CFL necessity for explicit Engquist-Osher stability

↑ **Parent:** [Engquist-Osher method](#engquist-osher-method)

[Monotonicity](calculus.md#monotonic-function) of the explicit update requires $(k/h)\sup_{[m,M]}|f'|\le1$ on its invariant state interval. [Convexity](real-analysis.md#convex-function) and a unique [sonic point of a scalar flux](transport-equation.md#sonic-point-of-a-scalar-flux) do not remove this time-step restriction. For $f(u)=u^2/2$, linearization about a positive constant $U$ gives an [upwind finite difference scheme](finite-difference.md#upwind-finite-difference-scheme) for [advection equation](transport-equation.md): $v_j^{n+1}=(1-rU)v_j^n+rUv_{j-1}^n$, where $r=k/h$. At [Fourier frequency](discrete-fourier-transform.md#fourier-frequency) $\pi$ the multiplier is $1-2rU$, whose modulus exceeds one when $rU>1$. Thus a [CFL condition](finite-difference.md#courant-friedrichs-lewy-condition) is essential to the claimed nonlinear [stability](numerical-analysis.md#stability-of-a-numerical-method).

#### Engquist-Osher flux

↑ **Parent:** [Engquist-Osher method](#engquist-osher-method)

The Engquist-Osher [numerical flux](#numerical-flux) is $F(a,b)=f(0)+\int_0^a\max(f\prime(s),0)ds+\int_0^b\min(f\prime(s),0)ds$. It sends positive-speed contributions from the left state and negative-speed contributions from the right state. Its consistency $F(u,u)=f(u)$ and opposite monotonicities in the two arguments yield a [monotone conservative scheme](#monotone-conservative-scheme) under the appropriate [Courant–Friedrichs–Lewy condition](finite-difference.md#courant-friedrichs-lewy-condition). For the [Inviscid Burgers equation](transport-equation.md#inviscid-burgers-equation), it is $\tfrac12\max(a,0)^2+\tfrac12\min(b,0)^2$.

##### Sonic-point splitting of a convex Engquist-Osher flux

↑ **Parent:** [Engquist-Osher flux](#engquist-osher-flux)

For a flux that is a differentiable [convex function](real-analysis.md#convex-function) with unique minimum at $s_*$, define $f^+(u)=f(u)-f(s_*)$ for $u>s_*$ and zero otherwise, and $f^-(u)=f(u)-f(s_*)$ for $u<s_*$ and zero otherwise. The [Engquist-Osher flux](#engquist-osher-flux) is $F(a,b)=f(s_*)+f^+(a)+f^-(b)$. Thus transsonic [rarefaction wave](transport-equation.md#rarefaction-wave) states $a\le s_*\le b$ give $F=f(s_*)$, while reversed transsonic states give $F=f(a)+f(b)-f(s_*)$. This follows by integrating the positive and negative parts of $f'$.

## Numerical flux

↑ **Parent:** [Finite volume method](finite-volume-method.md)

A [numerical flux](#numerical-flux) estimates the rate of transfer across a cell face from nearby states. In the [finite volume method](finite-volume-method.md) update, $F_{j+1/2}^n$ approximates the [conservation law flux](transport-equation.md#conservation-law-flux) averaged over the time step; $kF_{j+1/2}^n$ is the transferred amount. For a two-state [numerical flux](#numerical-flux) $F(L,R)$ approximating a [scalar conservation law](transport-equation.md#scalar-conservation-law) with [conservation law flux](transport-equation.md#conservation-law-flux) $f$, [consistency of a numerical method](numerical-analysis.md#consistency-of-a-numerical-method) requires $F(U,U)=f(U)$. Thus equal states recover the physical transfer rate. With constant equal-width cells, this also preserves a constant state because its incoming and outgoing [numerical fluxes](#numerical-flux) agree.[Approximate solvers, §Finite volume methods, consistency paragraph after equation FVupdate](mathematics-bibliography.md#riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo)

Consistency and [shared face flux cancellation](#shared-face-flux-cancellation) answer different questions: matching $f$ at equal states approximates the intended equation, while sharing one oriented face value preserves the total. The example [periodic upwind finite volume advection](#periodic-upwind-finite-volume-advection) uses $F(L,R)=aL$ for $a>0$, so the arriving state comes from the left. The [Godunov numerical flux](#godunov-numerical-flux) uses an [entropy solution](transport-equation.md#entropy-solution) of a local [Riemann problem](transport-equation.md#riemann-problem); the [Engquist-Osher flux](#engquist-osher-flux) provides a different construction for a [scalar conservation law](transport-equation.md#scalar-conservation-law). A [monotone conservative scheme](#monotone-conservative-scheme) uses a [numerical flux](#numerical-flux) nondecreasing in its left state and nonincreasing in its right state, together with a time step that makes the complete update monotone. Neither two-state consistency nor conservation by itself supplies that time-step restriction or a general [stability](numerical-analysis.md#stability-of-a-numerical-method) or [order of a numerical method](numerical-analysis.md#order-of-a-numerical-method) guarantee.

### Godunov numerical flux

↑ **Parent:** [Numerical flux](#numerical-flux)

For a [scalar conservation law](transport-equation.md#scalar-conservation-law) whose flux is a [convex function](real-analysis.md#convex-function), the [Godunov numerical flux](#godunov-numerical-flux) is the physical flux at the origin of the [entropy solution](transport-equation.md#entropy-solution) of the [Riemann problem](transport-equation.md#riemann-problem) between states $a,b$. It is $\min_{u\in[a,b]}f(u)$ for $a\le b$ and $\max_{u\in[b,a]}f(u)$ for $a>b$. For a [rarefaction wave](transport-equation.md#rarefaction-wave), the [characteristic speed](transport-equation.md#characteristic-speed) is monotone across its states, so the origin sees either an endpoint or a zero-speed minimizing state. For a [shock wave](transport-equation.md#shock-wave), its speed is $(f(a)-f(b))/(a-b)$; the origin sees the left state if this speed is positive and the right state if negative, selecting the larger endpoint flux. Unlike the [Godunov flux](#godunov-numerical-flux), the [Engquist-Osher flux](#engquist-osher-flux) at reversed transsonic states may equal $f(a)+f(b)-f(s_*)$.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (8)

- [Engquist-Osher method](#engquist-osher-method)
- [Finite volume method](finite-volume-method.md)
- [Numerical flux](#numerical-flux)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63.md#6/solution)
- [Periodic upwind finite volume advection](#periodic-upwind-finite-volume-advection)
- [Shared face flux cancellation](#shared-face-flux-cancellation)
