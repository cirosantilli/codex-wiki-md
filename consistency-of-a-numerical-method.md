# Consistency of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

For a one-step approximation $y_{n+1}=y_n+h\phi(t_n,y_n,h)$ to an [ordinary differential equation](ordinary-differential-equation.md), insert the exact solution and define the unscaled [local truncation error](local-truncation-error.md)

$$
\tau_{n+1}=y(t_n+h)-y(t_n)-h\phi(t_n,y(t_n),h).
$$

[Consistency of a numerical method](consistency-of-a-numerical-method.md) requires $\tau_{n+1}/h\to0$ uniformly on the finite interval being approximated, under the stated smoothness assumptions. Merely asking $\tau_{n+1}\to0$ is too weak: the useless update $y_{n+1}=y_n$ has defect $h y'(t_n)+O(h^2)$, which tends to zero but generally fails the scaled test. Here $O$ denotes [Big O notation](big-o-notation.md). MIT uses this division-by-step convention.[Laurent Demanet, MIT 18.330, Chapter 5, Definition 6, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/a9d2bd9be098f0ada172af40379a17cc_MIT18_330S12_Chapter5.pdf)

For the [Euler method](euler-method.md), [Taylor's theorem](taylor-s-theorem.md) gives $\tau_{n+1}=h^2y''(\xi_n)/2$. A bounded second [derivative](derivative.md) therefore gives [local truncation error](local-truncation-error.md) $O(h^2)$ and a scaled defect $O(h)$. Under a uniform [Lipschitz continuity](lipschitz-continuity.md) assumption on $f$ in $y$, within a region containing the exact and numerical solutions, [numerical stability](stability-of-a-numerical-method.md) controls accumulation over about $T/h$ steps. This yields [global error](global-discretization-error.md) $O(h)$ with exact starting data. [Consistency of a numerical method](consistency-of-a-numerical-method.md) checks each step; [numerical stability](stability-of-a-numerical-method.md) controls their combination.

**Table of contents**

- [Order of a numerical method](order-of-a-numerical-method.md)
  - [Local truncation error](local-truncation-error.md)
    - [Normalized local truncation error](normalized-local-truncation-error.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (39)

- [Butcher tableau](butcher-tableau.md)
- [Consistency of a numerical method](consistency-of-a-numerical-method.md)
- [Convergence of a numerical method](convergence-of-a-numerical-method.md)
- [Fourth-order two-step advection stencil](fourth-order-two-step-advection-stencil.md)
- [Harmonic superconvergence of the nine-point stencil](harmonic-superconvergence-of-the-nine-point-stencil.md)
- [Mehrstellen method](mehrstellen-method.md)
- [Numerical flux](numerical-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/39a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/6c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/6c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/18d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341/2/b/solution.md)
- [Sixth-order source correction of the nine-point Poisson stencil](sixth-order-source-correction-of-the-nine-point-poisson-stencil.md)
