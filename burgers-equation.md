# Burgers' equation

↑ **Parent:** [Partial differential equation](partial-differential-equation-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burgers'_equation)

[Burgers' equation](burgers-equation.md) is the one-dimensional [partial differential equation](partial-differential-equation-split.md)

$$
u_t+uu_x=\nu u_{xx},\qquad \nu\geq0.
$$

The term $uu_x$ supplies nonlinear transport in a [transport equation](transport-equation-split.md): the transported value $u$ is also its own [characteristic speed](characteristic-speed.md) when $\nu=0$. Larger values catch up with smaller values ahead of them, steepening a decreasing profile. The [diffusion](diffusion.md) term $\nu u_{xx}$ opposes this steepening. Positive $\nu$ gives the [viscous Burgers equation](viscous-burgers-equation.md); setting $\nu=0$ gives the [Inviscid Burgers equation](inviscid-burgers-equation.md).

This small equation makes three different behaviors accessible in one model: [Burgers characteristic breaking](burgers-characteristic-breaking.md) from continuous decreasing data, an [entropy shock](entropy-shock.md) for a downward step, and a [rarefaction wave](rarefaction-wave.md) for an upward step. The [Burgers Riemann problem with positive flux](burgers-riemann-problem-with-positive-flux.md) and the [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md) below give exact examples. These are mathematical calculations with chosen data; the figures contain no experimental measurements.

Unless stated otherwise, take $x\in\mathbb R$, $t\geq0$, constant $\nu$, no [PDE source term](source-term-in-a-partial-differential-equation.md), and an [initial condition](initial-condition.md) $u(x,0)=u_0(x)$. There are no finite endpoints requiring [boundary conditions](boundary-condition.md). Where a profile has different limiting states at $x=\pm\infty$, those states are specified explicitly. On a finite [interval](interval-mathematics.md), [boundary conditions](boundary-condition.md) become part of the problem: positive [diffusion](diffusion.md) normally requires a condition at each endpoint, whereas the [Inviscid Burgers equation](inviscid-burgers-equation.md) requires appropriate [inflow transport boundary conditions](inflow-transport-boundary-condition.md). With dimensional variables, $u$ has units of [velocity](velocity.md) and $\nu$ of [kinematic viscosity](kinematic-viscosity.md); all numerical examples below use [dimensionless quantities](dimensionless-quantity.md).

**Table of contents**

- [Viscous Burgers equation](viscous-burgers-equation.md)
  - [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md)
  - [Modified Burgers equation with cubic flux](modified-burgers-equation-with-cubic-flux.md)
    - [Traveling front of the cubic-flux Burgers equation](traveling-front-of-the-cubic-flux-burgers-equation.md)
  - [Fay solution](fay-solution.md)
    - [Fay shock-layer asymptotics](fay-shock-layer-asymptotics.md)
  - [Burgers N-wave](burgers-n-wave.md)
    - [Cole-Hopf solution for a Burgers N-wave](cole-hopf-solution-for-a-burgers-n-wave.md)
  - [Viscous Burgers step solution with negative flux](viscous-burgers-step-solution-with-negative-flux.md)
    - [Midpoint symmetry of a viscous Burgers step](midpoint-symmetry-of-a-viscous-burgers-step.md)
  - [Cole-Hopf transformation](cole-hopf-transformation.md)
    - [Time normalization in the Cole-Hopf transformation](time-normalization-in-the-cole-hopf-transformation.md)
    - [Sinusoidal Cole-Hopf solution for negative-flux Burgers flow](sinusoidal-cole-hopf-solution-for-negative-flux-burgers-flow.md)
    - [Finite-exponential Cole-Hopf solution](finite-exponential-cole-hopf-solution.md)
      - [Extremal-state asymptotics of exponential Burgers solutions](extremal-state-asymptotics-of-exponential-burgers-solutions.md)

## ↑ Ancestors (5)

1. [Partial differential equation](partial-differential-equation-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Burgers' equation](burgers-equation.md)
- [Modified Burgers equation with cubic flux](modified-burgers-equation-with-cubic-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-50/4/a/solution.md)
