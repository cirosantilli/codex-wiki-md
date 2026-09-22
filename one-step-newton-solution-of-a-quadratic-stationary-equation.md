# One-step Newton solution of a quadratic stationary equation

↑ **Parent:** [Newton step](newton-step.md)

For a real symmetric [invertible matrix](invertible-matrix.md) $H$, the full undamped [Newton step](newton-step.md) for the displayed [quadratic function](quadratic-function.md) sends every starting point to the unique [stationary point](stationary-point.md):

$$
x_1=x_0-H^{-1}(Hx_0+c)=-H^{-1}c.
$$

This follows because the [gradient](gradient.md) is affine and its first-order expansion is exact. If $H$ is a [positive-definite matrix](positive-definite-matrix.md) the result is the unique [global minimum](global-minimum.md); a [negative-definite matrix](negative-definite-matrix.md) gives a [global maximum](global-maximum.md), and an [indefinite matrix](indefinite-matrix.md) $H$ gives a [saddle point](saddle-point.md). Thus exact arrival does not by itself show that a minimization method has minimized anything. A [line search](line-search.md), damping, or a [positive-definite matrix](positive-definite-matrix.md) replacing the [Hessian matrix](hessian-matrix.md) changes this exact one-step assertion.

## ↑ Ancestors (6)

1. [Newton step](newton-step.md)
2. [Newton's method in optimization](newton-s-method-in-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/5/a/iii/solution.md)
