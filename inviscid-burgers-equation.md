# Inviscid Burgers equation

↑ **Parent:** [Scalar conservation law](scalar-conservation-law.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inviscid_Burgers_equation)

The [Inviscid Burgers equation](inviscid-burgers-equation.md) is the [scalar conservation law](scalar-conservation-law.md)

$$
u_t+\left(\frac{u^2}{2}\right)_x=0.
$$

For a [classical solution](classical-solution.md), the [chain rule](chain-rule.md) makes this equivalent to $u_t+uu_x=0$, a nonlinear [transport equation](transport-equation-split.md) with [characteristic speed](characteristic-speed.md) $u$. The conservative form remains meaningful for a discontinuous [weak solution](weak-solution.md), whereas the product $uu_x$ cannot simply be evaluated pointwise at a jump. Its discontinuities obey the [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) $s=(u_L+u_R)/2$; this condition alone permits inadmissible expansion jumps. For bounded [initial conditions](initial-condition.md) on the infinite line, imposing the [Kruzhkov entropy inequalities](kruzhkov-entropy-inequality.md) and the initial trace selects a unique [entropy solution](entropy-solution.md). For step data, incoming [characteristic curves](characteristic-curve.md) select $u_L>s>u_R$, while $u_L<u_R$ produces a [rarefaction wave](rarefaction-wave.md).[Shock solution; Rarefaction wave; The entropy condition](riemann-problems-and-jupyter-solutions-by-david-i-ketcheson-randall-j-leveque-and-mauricio-j-del-razo/burgers-equation.md)

**Table of contents**

- [Burgers characteristic breaking](burgers-characteristic-breaking.md)
- [Burgers Riemann problem with positive flux](burgers-riemann-problem-with-positive-flux.md)
- [Periodic backward-sawtooth Burgers solution](periodic-backward-sawtooth-burgers-solution.md)
- [Burgers Riemann problem with negative flux](burgers-riemann-problem-with-negative-flux.md)
- [Entropy solution](entropy-solution.md)
  - [Kruzhkov entropy inequality](kruzhkov-entropy-inequality.md)
  - [Discrete entropy inequality](discrete-entropy-inequality.md)
  - [Averaged initial trace of an entropy solution](averaged-initial-trace-of-an-entropy-solution.md)
  - [Entropy flux for a scalar conservation law](entropy-flux-for-a-scalar-conservation-law.md)
    - [Kruzhkov entropy flux](kruzhkov-entropy-flux.md)
      - [Doubling of variables for scalar conservation laws](doubling-of-variables-for-scalar-conservation-laws.md)
        - [Kato inequality for scalar conservation laws](kato-inequality-for-scalar-conservation-laws.md)
          - [Local L1 contraction for scalar conservation laws](local-l1-contraction-for-scalar-conservation-laws.md)
            - [Order preservation for scalar entropy solutions](order-preservation-for-scalar-entropy-solutions.md)

## ↑ Ancestors (7)

1. [Scalar conservation law](scalar-conservation-law.md)
2. [Transport equation](transport-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Bounded-derivative Burgers flux](bounded-derivative-burgers-flux.md)
- [Burgers characteristic breaking](burgers-characteristic-breaking.md)
- [Burgers' equation](burgers-equation.md)
- [Burgers Riemann problem with negative flux](burgers-riemann-problem-with-negative-flux.md)
- [Burgers Riemann problem with positive flux](burgers-riemann-problem-with-positive-flux.md)
- [Engquist-Osher flux](engquist-osher-flux.md)
- [Inviscid Burgers equation](inviscid-burgers-equation.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022/section-b/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/31b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-62/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-70/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-75/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-77/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-314/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105/3/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-105/3/e/solution.md)
- [Perpendicular fast magnetosonic simple wave](perpendicular-fast-magnetosonic-simple-wave.md)
- [Simple wave in magnetohydrodynamics](simple-wave-in-magnetohydrodynamics.md)
