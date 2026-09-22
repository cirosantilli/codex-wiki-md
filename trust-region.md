# Trust region

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trust_region)

A [trust region](trust-region.md) restricts a local approximation to a neighborhood where it is expected to model the [objective function](objective-function.md) accurately. A quadratic model is $m(s)=f(x)+g^Ts+\tfrac12s^THs$, where $g=\nabla f(x)$ and $H$ is a [symmetric matrix](symmetric-matrix.md) approximating the [Hessian matrix](hessian-matrix.md). Minimizing this [quadratic function](quadratic-function.md) over a [Euclidean ball](euclidean-ball.md) of radius $\Delta>0$ is the [trust-region subproblem](trust-region-subproblem.md). The [trust-region acceptance ratio](trust-region-acceptance-ratio.md) then checks the model against the actual [objective function](objective-function.md).

**Table of contents**

- [Trust-region method](trust-region-method.md)
- [Trust-region subproblem](trust-region-subproblem.md)
  - [Cauchy point](cauchy-point.md)
    - [Cauchy decrease bound](cauchy-decrease-bound.md)
      - [Fraction of Cauchy decrease](fraction-of-cauchy-decrease.md)
- [Trust-region acceptance ratio](trust-region-acceptance-ratio.md)

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/i/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/5/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/6/c/iii/solution.md)
- [Sequential quadratic programming](sequential-quadratic-programming.md)
- [Sl1QP](sl1qp.md)
- [Trust region](trust-region.md)
- [Trust-region acceptance ratio](trust-region-acceptance-ratio.md)
