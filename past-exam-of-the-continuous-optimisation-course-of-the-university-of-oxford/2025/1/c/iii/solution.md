<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Interpret boundedness above uniformly: there is an $M<\infty$ such that $B^k\preceq MI$ for every $k$. Since $B^k$ is a [positive-definite symmetric matrix](../../../../../symmetric-positive-definite-matrix.md), the [spectral theorem](../../../../../spectral-theorem.md) implies $(B^k)^{-1}\succeq M^{-1}I$. Therefore

$$
-\nabla f(x^k)^Ts^k=\nabla f(x^k)^T(B^k)^{-1}\nabla f(x^k)\geq\frac1M\|\nabla f(x^k)\|^2.
$$

Combining the [Armijo condition](../../../../../armijo-condition.md) with $\alpha^k\geq C>0$ yields

$$
f(x^k)-f(x^{k+1})\geq\frac{\beta_1C}{M}\|\nabla f(x^k)\|^2.
$$

If $f\geq L$, a [telescoping sum](../../../../../telescoping-sum.md) gives

$$
\frac{\beta_1C}{M}\sum_{k=0}^N\|\nabla f(x^k)\|^2\leq f(x^0)-f(x^{N+1})\leq f(x^0)-L.
$$

The nonnegative [series](../../../../../series-mathematics.md) converges, so its terms tend to zero:

$$
\boxed{\lim_{k\to\infty}\|\nabla f(x^k)\|=0}.
$$

This proves first-order global convergence in the sense of [stationarity from uniformly bounded quasi-Newton matrices](../../../../../stationarity-from-uniformly-bounded-quasi-newton-matrices.md). It does not imply that every nonconvex [objective function](../../../../../objective-function.md) reaches a [global minimum](../../../../../global-minimum.md), or that the iterates themselves converge. Every finite [limit point](../../../../../limit-point.md) is a [stationary point](../../../../../stationary-point.md), by [continuity](../../../../../continuous-function.md) of the [gradient](../../../../../gradient.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
