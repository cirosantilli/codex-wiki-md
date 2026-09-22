# Threshold formula for the sum of the largest components

↑ **Parent:** [Sum of the largest components](sum-of-the-largest-components.md)

For $1\leq k\leq n$, [linear programming duality](linear-programming-duality.md) gives

$$
f_k(x)=\min_{t\in\mathbb R,\ s\geq0}\left\{kt+\sum_i s_i:s_i+t\geq x_i\right\}
=\min_{t\in\mathbb R}\left\{kt+\sum_i(x_i-t)_+\right\},
$$

where $(\cdot)_+$ is the [positive part of a real-valued function](positive-part-of-a-real-valued-function.md). To see equality directly, order the coordinates $x_{[1]}\geq\cdots\geq x_{[n]}$ and choose $x_{[k+1]}\leq t\leq x_{[k]}$ for $k<n$, or $t\leq x_{[n]}$ for $k=n$. The threshold expression then equals the [sum of the largest components](sum-of-the-largest-components.md). Introducing the variables $s_i$ turns this [convex](convex-function.md) piecewise-linear objective into a [linear program](linear-programming.md).

## ↑ Ancestors (7)

1. [Sum of the largest components](sum-of-the-largest-components.md)
2. [Support function](support-function.md)
3. [Convex set](convex-set.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/1/d/solution.md)
- [Threshold semidefinite program for the largest eigenvalues](threshold-semidefinite-program-for-the-largest-eigenvalues.md)
