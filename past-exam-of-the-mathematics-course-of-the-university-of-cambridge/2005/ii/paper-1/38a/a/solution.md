<h1 id="38a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h=\Delta x$, $k=\Delta t=\mu h$, and $D_0u=[u(x+h)-u(x-h)]/(2h)$. The scheme is the trapezoidal time rule with a centered spatial [derivative](../../../../../../derivative.md):

$$
u^{n+1}-u^n=\tfrac k2(D_0u^{n+1}+D_0u^n).
$$

Insert a smooth exact solution of $u_t=u_x$. Taylor expansion of the unnormalized one-step residual gives

$$
\begin{aligned}u(t+k)-u(t)&=ku_t+\tfrac12k^2u_{tt}+\tfrac16k^3u_{ttt}+O(h^4),\\\tfrac k2(D_0u(t+k)+D_0u(t))&=ku_x+\tfrac12k^2u_{xt}+\tfrac14k^3u_{xtt}+\tfrac16kh^2u_{xxx}+O(h^4).
\end{aligned}
$$

All repeated time [derivatives](../../../../../../derivative.md) equal the corresponding spatial [derivatives](../../../../../../derivative.md). The first two orders cancel, leaving

$$
\boxed{R=-\left(\frac{k^3}{12}+\frac{kh^2}{6}\right)u_{xxx}+O(h^4)=-\frac{\mu(\mu^2+2)}{12}h^3u_{xxx}+O(h^4).}
$$

Thus the one-step local error is $O(h^3)$ at fixed [Courant number](../../../../../../courant-number.md). If “[local truncation error](../../../../../../local-truncation-error.md)” is instead defined after division of the residual by $\Delta t$, its order is $O(h^2)$; these are two different normalizations of the same second-order method.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38A](../../38a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
