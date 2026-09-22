<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the initial conditions $x(0,r)=1$, $y(0,r)=r$, $u(0,r)=g(r)$ in the [characteristic equations for a transport equation](../../../../../characteristic-equations-for-a-transport-equation.md). The resulting parametrized [solution surface](../../../../../solution-surface.md) is

$$
\boxed{\begin{aligned}
x(s,r)&=e^s,\\
y(s,r)&=(r+\beta)e^{2s}-\beta e^s,\\
u(s,r)&=\min\{r,0\}+e^s-1+2s,
\end{aligned}\qquad s\in\mathbb R,\ -1\leq r\leq1.}
$$

The [Jacobian determinant](../../../../../jacobian-determinant.md) of $(s,r)\mapsto(x,y)$ is $e^{3s}>0$. In fact the inverse is explicit:

$$
s=\log x,\qquad r=q(x,y):=\frac{y+\beta x}{x^2}-\beta.
$$

Consequently the explicit [solution of a differential equation](../../../../../solution-of-a-differential-equation.md) on the region reached from the data is

$$
\boxed{u(x,y)=x-1+2\log x+\min\left\{\frac{y+\beta x}{x^2}-\beta,0\right\}.}
$$

To verify it away from $q=0$, set $D=x\partial_x+(2y+\beta x)\partial_y$. Direct [differentiation](../../../../../differentiation.md) gives $Dq=0$ and $D(x-1+2\log x)=x+2$. At $x=1$ we have $q=y$, giving precisely the prescribed [boundary condition](../../../../../boundary-condition.md).

Across $q=0$ the formula remains [continuous](../../../../../continuous-function.md) and [locally Lipschitz](../../../../../locally-lipschitz-function.md), is a [smooth function](../../../../../smooth-function.md) on each side, and solves the [partial differential equation](../../../../../partial-differential-equation-split.md) along every [characteristic curve](../../../../../characteristic-curve.md). It is also a [weak solution](../../../../../weak-solution.md), since its first [distributional derivatives](../../../../../distributional-derivative.md) agree almost everywhere with its ordinary [derivatives](../../../../../derivative.md). It is not a [classical solution](../../../../../classical-solution.md) throughout the region because of the inherited corner.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
