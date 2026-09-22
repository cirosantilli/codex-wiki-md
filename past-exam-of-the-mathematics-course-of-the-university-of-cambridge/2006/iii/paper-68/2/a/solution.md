<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h=\Delta x$, $k=\Delta t$, with fixed positive $\mu=k/h$. Insert a smooth exact solution and divide the residual by $2k$:

$$
\frac{u(t+k)-u(t-k)}{2k}
-\frac{u(x+h,y)-u(x-h,y)+u(x,y+h)-u(x,y-h)}{2h}.
$$

[Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
u_t-u_x-u_y+\frac{k^2}{6}u_{ttt}-\frac{h^2}{6}(u_{xxx}+u_{yyy})+O(k^4+h^4).
$$

The [differential equation](../../../../../../differential-equation-split.md) cancels the leading part, leaving normalized [local truncation error](../../../../../../local-truncation-error.md) $O(k^2+h^2)$. Since $u_{ttt}=(\partial_x+\partial_y)^3u$ contains mixed [derivatives](../../../../../../derivative.md), there is no fixed positive [Courant number](../../../../../../courant-number.md) canceling this leading error for every smooth solution. Thus **the method is second order in time and space**. Global second-order convergence also requires [stability](../../../../../../stability-of-a-numerical-method.md) and initial values at both time levels accurate enough to retain this order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
