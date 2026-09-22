# Linear differential equation

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_differential_equation)

A scalar [linear differential equation](linear-differential-equation.md) of order $n\geq1$ has the form

$$
L[y](t)=a_n(t)y^{(n)}(t)+a_{n-1}(t)y^{(n-1)}(t)+\cdots+a_1(t)y'(t)+a_0(t)y(t)=g(t).
$$

Here the [coefficients](coefficient.md) $a_j$ and the [forcing term](forcing-term.md) $g$ are prescribed [functions](function-split.md) of the independent variable $t$. A classical [solution of a differential equation](solution-of-a-differential-equation.md) is an $n$-times [differentiable function](differentiable-function.md) satisfying the identity at every point of its [interval](interval-mathematics.md). The unknown [function](function-split.md) $y$ and its [derivatives](derivative.md) enter to the first power, without products between them or [coefficients](coefficient.md) depending on $y$. Equivalently, the [differential operator](differential-operator.md) $L$ is a [linear map](linear-map.md): for constant [scalars](scalar.md) $\alpha,\beta$,

$$
L[\alpha u+\beta v]=\alpha L[u]+\beta L[v].
$$

The [forcing term](forcing-term.md) may be zero, giving a [homogeneous linear differential equation](homogeneous-linear-differential-equation.md), or nonzero, giving an [inhomogeneous linear differential equation](inhomogeneous-linear-differential-equation.md). [Linearity](linearity.md) of $L$ does not mean that every [function graph](graph-of-a-function.md) of a [solution of a differential equation](solution-of-a-differential-equation.md) is a straight line.

To use the usual order-$n$ [initial value problem](initial-value-problem.md) theory on an [interval](interval-mathematics.md) $I$, assume that $a_n(t)\ne0$ throughout $I$ and that all $a_j$ and $g$ are [continuous functions](continuous-function.md) there. Dividing by $a_n$ normalizes the highest [derivative](derivative.md); specifying $y(t_0),y'(t_0),\ldots,y^{(n-1)}(t_0)$ at $t_0\in I$ then selects one [solution of a differential equation](solution-of-a-differential-equation.md) throughout $I$. A zero of $a_n$ needs separate analysis: one cannot divide through it and retain these conclusions. The first-order normalization appears in [OpenStax's definition and standard form of linear equations](https://openstax.org/books/calculus-volume-2/pages/4-5-first-order-linear-equations); the corresponding system theorem is in [MIT's existence and uniqueness notes for linear systems](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/8ae57eb392d85ce692965b97dda608fc_MIT18_03SCF11_s35_4text.pdf).

The [coefficients](coefficient.md) need not be [linear functions](linear-function.md) of $t$. For example, $t^2y'+y=0$ is a [linear differential equation](linear-differential-equation.md) on $t>0$, although $t^2$ is quadratic. Its [solution of a differential equation](solution-of-a-differential-equation.md) with [initial condition](initial-condition.md) $y(1)=1$ is $y(t)=e^{1/t-1}$: its [derivative](derivative.md) is $y'=-y/t^2$, so substitution gives $t^2y'+y=0$, and $y(2)=e^{-1/2}\approx0.60653$. The zero of the highest [coefficient](coefficient.md) at $t=0$ explains the domain restriction. In contrast, $y'+y^2=0$, $yy'+y=0$ and $y'+\sin y=0$ are [nonlinear ordinary differential equations](nonlinear-ordinary-differential-equation.md) because of their dependence on the unknown [function](function-split.md). Variable [coefficients](coefficient.md) and [nonlinear ordinary differential equations](nonlinear-ordinary-differential-equation.md) are different issues; see [MIT's definitions and examples of first-order linear equations](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/acc65618b35025a2e9db939ec35b1de5_MIT18_03SCF11_s4_1text.pdf).

The practical benefit of [linearity](linearity.md) is that it separates the effect of the [initial condition](initial-condition.md) from the effect of the [forcing term](forcing-term.md). Once one [particular solution](particular-solution.md) $y_p$ satisfies $L[y_p]=g$, every [solution of a differential equation](solution-of-a-differential-equation.md) is

$$
y=y_p+h,\qquad h\in\ker L.
$$

Here $\ker L$ is the [kernel of a linear map](kernel-of-a-linear-map-split.md), consisting of [solutions of a differential equation](solution-of-a-differential-equation.md) to the associated [homogeneous linear differential equation](homogeneous-linear-differential-equation.md). Indeed, $L[y-y_p]=g-g=0$, and conversely $L[y_p+h]=g+0=g$. Thus the family for a fixed [forcing term](forcing-term.md) is an [affine space](affine-space.md) obtained by translating $\ker L$. If $g$ is not identically zero, the zero [function](function-split.md) is absent, so this family is not a [vector space](vector-space-split.md) under the usual operations on [functions](function-split.md). This short argument explains why a [general solution](general-solution.md) is a [particular solution](particular-solution.md) plus a [homogeneous solution](homogeneous-solution.md).

**Table of contents**

- [Fuchsian linear differential system](fuchsian-linear-differential-system.md)
  - [Analytic solution at a maximal integer Fuchsian exponent](analytic-solution-at-a-maximal-integer-fuchsian-exponent.md)
  - [Residue and monodromy of a constant Fuchsian system](residue-and-monodromy-of-a-constant-fuchsian-system.md)
- [Fundamental matrix of a linear differential equation](fundamental-matrix-of-a-linear-differential-equation.md)
  - [Gauge transformation of a linear differential system](gauge-transformation-of-a-linear-differential-system.md)
    - [Formal cubic-exponential two-by-two system](formal-cubic-exponential-two-by-two-system.md)
  - [Liouville formula for a fundamental matrix](liouville-formula-for-a-fundamental-matrix.md)
- [Floquet theory](floquet-theory.md)
  - [Floquet exponent](floquet-exponent.md)
  - [Floquet growth rate](floquet-growth-rate.md)
  - [Monodromy matrix of a periodic linear system](monodromy-matrix-of-a-periodic-linear-system.md)
- [Characteristic root of a constant-coefficient differential equation](characteristic-root-of-a-constant-coefficient-differential-equation.md)
- [Laplace contour-integral method for a linear differential equation](laplace-contour-integral-method-for-a-linear-differential-equation.md)
- [Homogeneous linear differential equation](homogeneous-linear-differential-equation.md)
  - [Solution space of a homogeneous linear differential equation](solution-space-of-a-homogeneous-linear-differential-equation.md)
- [Linearized equation](linearized-equation.md)
- [Inhomogeneous linear differential equation](inhomogeneous-linear-differential-equation.md)
  - [Forcing term](forcing-term.md)

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (47)

- [Addition closure of Siegel E-functions](addition-closure-of-siegel-e-functions.md)
- [Airy half-line solution with prescribed boundary derivative](airy-half-line-solution-with-prescribed-boundary-derivative.md)
- [Characteristic root of a constant-coefficient differential equation](characteristic-root-of-a-constant-coefficient-differential-equation.md)
- [Exact linear Foucault pendulum trajectory](exact-linear-foucault-pendulum-trajectory.md)
- [Floquet growth rate](floquet-growth-rate.md)
- [Floquet multiplier](floquet-multiplier.md)
- [Forcing term](forcing-term.md)
- [Fuchsian linear differential system](fuchsian-linear-differential-system.md)
- [Fundamental matrix of a linear differential equation](fundamental-matrix-of-a-linear-differential-equation.md)
- [Homogeneous linear differential equation](homogeneous-linear-differential-equation.md)
- [Infrared](infrared.md)
- [Initial value problem](initial-value-problem.md)
- [Laplace transform](laplace-transform.md)
- [Latitude law of Foucault precession](latitude-law-of-foucault-precession.md)
- [Linear differential equation](linear-differential-equation.md)
- [Mathieu equation](mathieu-equation.md)
- [Monodromy matrix of a periodic linear system](monodromy-matrix-of-a-periodic-linear-system.md)
- [Neumann boundary-forcing formula](neumann-boundary-forcing-formula.md)
- [Nonlinear ordinary differential equation](nonlinear-ordinary-differential-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-20/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-29/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2/5b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-12/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/3b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-41/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/23i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-331/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-b/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/8/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/8/a/solution.md)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2021/paper-ne1/4/c/solution.md)
- [Periodic solution](periodic-solution.md)
- [Power transformation of a complete-market investment equation](power-transformation-of-a-complete-market-investment-equation.md)
- [Resonant exponential particular solution](resonant-exponential-particular-solution.md)
- [Square-root reduction of a regular-singular differential equation](square-root-reduction-of-a-regular-singular-differential-equation.md)
- [Symmetric part of a matrix](symmetric-part-of-a-matrix.md)
- [Two-size fragmentation cascade](two-size-fragmentation-cascade.md)
- [Uniqueness](uniqueness.md)
