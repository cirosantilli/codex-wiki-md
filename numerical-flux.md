# Numerical flux

↑ **Parent:** [Finite volume method](finite-volume-method-split.md)

A [numerical flux](numerical-flux.md) estimates the rate of transfer across a cell face from nearby states. In the [finite volume method](finite-volume-method-split.md) update, $F_{j+1/2}^n$ approximates the [conservation law flux](conservation-law-flux.md) averaged over the time step; $kF_{j+1/2}^n$ is the transferred amount. For a two-state [numerical flux](numerical-flux.md) $F(L,R)$ approximating a [scalar conservation law](scalar-conservation-law.md) with [conservation law flux](conservation-law-flux.md) $f$, [consistency of a numerical method](consistency-of-a-numerical-method.md) requires $F(U,U)=f(U)$. Thus equal states recover the physical transfer rate. With constant equal-width cells, this also preserves a constant state because its incoming and outgoing [numerical fluxes](numerical-flux.md) agree.[Approximate solvers, §Finite volume methods, consistency paragraph after equation FVupdate](riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo.md)

Consistency and [shared face flux cancellation](shared-face-flux-cancellation.md) answer different questions: matching $f$ at equal states approximates the intended equation, while sharing one oriented face value preserves the total. The example [periodic upwind finite volume advection](periodic-upwind-finite-volume-advection.md) uses $F(L,R)=aL$ for $a>0$, so the arriving state comes from the left. The [Godunov numerical flux](godunov-numerical-flux.md) uses an [entropy solution](entropy-solution.md) of a local [Riemann problem](riemann-problem.md); the [Engquist-Osher flux](engquist-osher-flux.md) provides a different construction for a [scalar conservation law](scalar-conservation-law.md). A [monotone conservative scheme](monotone-conservative-scheme.md) uses a [numerical flux](numerical-flux.md) nondecreasing in its left state and nonincreasing in its right state, together with a time step that makes the complete update monotone. Neither two-state consistency nor conservation by itself supplies that time-step restriction or a general [stability](stability-of-a-numerical-method.md) or [order of a numerical method](order-of-a-numerical-method.md) guarantee.

**Table of contents**

- [Godunov numerical flux](godunov-numerical-flux.md)

## ↑ Ancestors (6)

1. [Finite volume method](finite-volume-method-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Engquist-Osher flux](engquist-osher-flux.md)
- [Finite volume method](finite-volume-method-split.md)
- [Numerical flux](numerical-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/6/solution.md)
- [Periodic upwind finite volume advection](periodic-upwind-finite-volume-advection.md)
- [Shared face flux cancellation](shared-face-flux-cancellation.md)
