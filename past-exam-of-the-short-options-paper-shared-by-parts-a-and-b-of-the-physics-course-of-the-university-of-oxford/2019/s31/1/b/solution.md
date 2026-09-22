<h1 id="s31/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $h=\Delta x$, $k=\Delta t$ and $\delta_{xx}u_i=(u_{i+1}-2u_i+u_{i-1})/h^2$. Insert a smooth exact [heat equation](../../../../../heat-equation.md) solution into the [Crank-Nicolson method](../../../../../crank-nicolson-method.md). Expanding about the midpoint $(x_i,t_n+k/2)$ gives

$$
\frac{u(t+k/2)-u(t-k/2)}k=u_t+\frac{k^2}{24}u_{ttt}+O(k^4),
$$



$$
\frac D2[\delta_{xx}u(t-k/2)+\delta_{xx}u(t+k/2)]
=D\left[u_{xx}+\frac{h^2}{12}u_{xxxx}+\frac{k^2}{8}u_{xxtt}\right]+O(h^4+k^4+h^2k^2).
$$

Thus the residual, defined as left side minus right side, is

$$
\mathcal T=\frac{k^2}{24}u_{ttt}-\frac{Dk^2}{8}u_{xxtt}-\frac{Dh^2}{12}u_{xxxx}+O(h^4+k^4+h^2k^2).
$$

Since $u_t=Du_{xx}$ implies $u_{ttt}=Du_{xxtt}$,

$$
\boxed{\mathcal T=-\frac{k^2}{12}u_{ttt}-\frac{Dh^2}{12}u_{xxxx}+O(h^4+k^4+h^2k^2).}
$$

This proves second-order [numerical consistency](../../../../../consistency-of-a-numerical-method.md) in both space and time. About the old time level, uncombined Taylor remainders can include $O(k^3)$; the midpoint expression displays the symmetric leading errors most cleanly. Multiplying by $k$ gives the one-step defect $O(k^3+kh^2)$. Stable evolution with suitable initial and boundary data then gives global error $O(k^2+h^2)$; consistency alone does not prove global convergence.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
