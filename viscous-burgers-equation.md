# Viscous Burgers equation

↑ **Parent:** [Burgers' equation](burgers-equation.md)

The [viscous Burgers equation](viscous-burgers-equation.md) combines a nonlinear [transport equation](transport-equation-split.md) with [diffusion](diffusion.md) with constant $\nu>0$. On the infinite line, a bounded [initial condition](initial-condition.md) gives a [smooth function](smooth-function.md) solving the equation for every positive time; a jump in the [initial condition](initial-condition.md) is smoothed rather than retained as a discontinuity. Small $\nu$ can nevertheless produce a steep layer, as the [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md) illustrates. The [Cole-Hopf transformation](cole-hopf-transformation.md) $u=-2\nu\,\partial_x\log\phi$, with positive $\phi$, converts this equation to the [heat equation](heat-equation.md) $\phi_t=\nu\phi_{xx}$.[§9.1, Problem set-up, (9.1.1)–(9.1.2); Cole-Hopf transform, (9.1.11)–(9.1.13)](asymptotic-and-perturbation-methods-by-victor-ivrii/burgers-equation-1.md)

Positive [diffusion](diffusion.md) also explains the admissibility of the inviscid limit. For the [entropy flux for a scalar conservation law](entropy-flux-for-a-scalar-conservation-law.md) associated with $\eta(u)=u^2/2$, direct multiplication by $u$ gives

$$
\partial_t\frac{u^2}{2}+\partial_x\frac{u^3}{3}=\nu\partial_{xx}\frac{u^2}{2}-\nu u_x^2.
$$

The last term is nonpositive. With convergence sufficient to pass to the limit, the [vanishing viscosity approximation](vanishing-viscosity-approximation.md) therefore retains an entropy inequality rather than just the [weak solution](weak-solution.md) equation. For general bounded data, the full [Kruzhkov entropy inequalities](kruzhkov-entropy-inequality.md) specify the [entropy solution](entropy-solution.md); the quadratic identity is a useful illustration of dissipation.[§9.1, Case epsilon=0 as a limit, identity following (9.1.10)](asymptotic-and-perturbation-methods-by-victor-ivrii/burgers-equation-1.md)

**Table of contents**

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

## ↑ Ancestors (6)

1. [Burgers' equation](burgers-equation.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Burgers' equation](burgers-equation.md)
- [Burgers reduction of weakly nonlinear rightgoing acoustics](burgers-reduction-of-weakly-nonlinear-rightgoing-acoustics.md)
- [Cole-Hopf solution for a Burgers N-wave](cole-hopf-solution-for-a-burgers-n-wave.md)
- [Cole-Hopf transformation](cole-hopf-transformation.md)
- [Fay solution](fay-solution.md)
- [Finite-exponential Cole-Hopf solution](finite-exponential-cole-hopf-solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022/section-b/5/a/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022/section-b/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/31e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82/4/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/31e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-88/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-70/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-77/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/7a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/14/b/i/solution.md)
- [Time normalization in the Cole-Hopf transformation](time-normalization-in-the-cole-hopf-transformation.md)
- [Viscous Burgers equation](viscous-burgers-equation.md)
- [Viscous Burgers travelling shock](viscous-burgers-travelling-shock.md)
