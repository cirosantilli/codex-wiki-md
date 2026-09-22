<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On nonnegative states the characteristic speed is $f'(u)=1+pu^{p-1}>0$, so [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) uses the left spatial difference. With $\lambda=\Delta t/\Delta x$, the conservative [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) is

$$
\boxed{U_j^{m+1}=U_j^m-\lambda\bigl[f(U_j^m)-f(U_{j-1}^m)\bigr],\qquad U_j^0=u_0(j\Delta x).}
$$

Explicitly the flux difference is $(U_j^m-U_{j-1}^m)+[(U_j^m)^p-(U_{j-1}^m)^p]$. Preservation of nonnegativity under the given Courant restriction, proved next, justifies the same left-upwind direction at every step.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
