<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $p=x^{k+1}-x^k=\alpha^ks^k$ and $y=\nabla f(x^{k+1})-\nabla f(x^k)$. The [Quasi-Newton secant equation](../../../../../quasi-newton-secant-equation.md) is $B^{k+1}p=y$. If $B^{k+1}$ is a [positive-definite symmetric matrix](../../../../../symmetric-positive-definite-matrix.md) and $p\ne0$, it follows that

$$
p^Ty=p^TB^{k+1}p>0.
$$

The weak curvature part of the [Wolfe conditions](../../../../../wolfe-conditions.md) ensures precisely this necessary condition:

$$
p^Ty=\alpha^k\bigl(\nabla f(x^{k+1})^Ts^k-\nabla f(x^k)^Ts^k\bigr)\geq\alpha^k(\beta_2-1)\nabla f(x^k)^Ts^k>0.
$$

The last product is positive because $\alpha^k>0$, $\beta_2-1<0$, and $s^k$ is a [descent direction](../../../../../descent-direction.md). This explains why a [Quasi-Newton method](../../../../../quasi-newton-method.md) often uses the [Wolfe conditions](../../../../../wolfe-conditions.md) rather than only the [Armijo condition](../../../../../armijo-condition.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
