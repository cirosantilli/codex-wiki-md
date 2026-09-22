<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $d=\Delta x$, $k=\Delta t$ and use the diffusion [Courant number](../../../../../../courant-number.md) $r=k/d^2$. To discuss [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md), refine the mesh with a fixed positive $r$. With $\delta^2U_m=U_{m-1}-2U_m+U_{m+1}$, the printed update is $U^{n+1}-U^n=\alpha\delta^2U^{n+1}$. A [Taylor expansion](../../../../../../taylor-expansion.md) of a smooth exact solution, about the new time level, gives the residual divided by $k$:

$$
\frac{u(t+k,x)-u(t,x)-\alpha\delta^2u(t+k,x)}{k}
=\left(1-\frac{\alpha}{r}\right)u_{xx}
-\frac{k}{2}u_{xxxx}-\frac{\alpha d^4}{12k}u_{xxxx}
+O(k^2+\alpha d^6/k).
$$

Here the [heat equation](../../../../../../heat-equation.md) implies $u_t=u_{xx}$ and $u_{tt}=u_{xxxx}$. Since $\alpha$ depends only on $r$, the leading term can vanish for every smooth solution only if **$\alpha(r)=r$**. Thus the method is the [Backward Euler diffusion scheme](../../../../../../backward-euler-diffusion-scheme.md), with [local truncation error](../../../../../../local-truncation-error.md)

$$
\tau=-\left(\frac{k}{2}+\frac{d^2}{12}\right)u_{xxxx}
+O(k^2+kd^2+d^4).
$$

Its highest general accuracy is **first order in time and second order in space**, or **order two in $d$ under $k=rd^2$**. The coefficient of $d^2u_{xxxx}$ is $-(r/2+1/12)$, so it cannot cancel for any positive diffusion [Courant number](../../../../../../courant-number.md). This is a conclusion about the stencil actually printed: the new-time spatial difference fixes the sign of its temporal error. With sufficiently smooth compatible data, [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) below turns the $O(k+d^2)$ consistency estimate into an $O(k+d^2)$ [global error](../../../../../../global-discretization-error.md) bound on a fixed time interval.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
