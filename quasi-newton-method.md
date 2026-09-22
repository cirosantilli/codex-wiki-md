# Quasi-Newton method

↑ **Parent:** [Newton's method in optimization](newton-s-method-in-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-Newton_method)

A [Quasi-Newton method](quasi-newton-method.md) replaces the [Hessian matrix](hessian-matrix.md) in [Newton's method in optimization](newton-s-method-in-optimization.md) by a [matrix](matrix.md) $B_k$ learned from successive [gradients](gradient.md). Solving $B_ks_k=-\nabla f(x_k)$ gives a [descent direction](descent-direction.md) whenever $B_k$ is a [positive-definite symmetric matrix](symmetric-positive-definite-matrix.md) and the [gradient](gradient.md) is nonzero. After choosing a [step size](step-size.md), one updates $B_k$ to satisfy the [Quasi-Newton secant equation](quasi-newton-secant-equation.md), rather than calculating every second derivative again.

**Table of contents**

- [Dennis-Moré condition](dennis-more-condition.md)
- [BFGS method](bfgs-method.md)
  - [Limited-memory BFGS](limited-memory-bfgs.md)
- [Quasi-Newton secant equation](quasi-newton-secant-equation.md)
- [Stationarity from uniformly bounded quasi-Newton matrices](stationarity-from-uniformly-bounded-quasi-newton-matrices.md)

## 🏷️ Tagged (1)

- [Gauss-Newton algorithm](gauss-newton-algorithm.md)

## ↑ Ancestors (5)

1. [Newton's method in optimization](newton-s-method-in-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (13)

- [BFGS method](bfgs-method.md)
- [Charles George Broyden](charles-george-broyden.md)
- [Dennis-Moré condition](dennis-more-condition.md)
- [John E. Dennis](john-e-dennis.md)
- [Jorge Moré](jorge-more.md)
- [Limited-memory BFGS](limited-memory-bfgs.md)
- [Logarithmic gradient of an exponential squared-distance sum](logarithmic-gradient-of-an-exponential-squared-distance-sum.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/c/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/7/vii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/6/b/i/solution.md)
- [Quasi-Newton method](quasi-newton-method.md)
- [Quasi-Newton Methods by NEOS Guide](quasi-newton-methods-by-neos-guide.md)
