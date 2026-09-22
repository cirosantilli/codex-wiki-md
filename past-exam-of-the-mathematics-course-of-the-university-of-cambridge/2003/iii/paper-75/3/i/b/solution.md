<h1 id="3/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The weakly nonlinear, unsteady and dispersive core terms must enter at the same order. Axial nonlinearity first contributes at $O(\epsilon^2)$, while unsteadiness contributes $O(\epsilon\lambda St)$ and transverse-inertia [pressure](../../../../../../../pressure.md) variation contributes $O(\epsilon\lambda^{-2})$. Thus take the distinguished limit

$$
\boxed{\lambda St=\beta\epsilon,\qquad\lambda^{-2}=D\epsilon,\qquad\beta,D=O(1)>0}.
$$

Equivalently, $\lambda=O(\epsilon^{-1/2})$, $St=O(\epsilon^{3/2})$ and the wall-layer condition becomes $Re\gg\epsilon^{-7/2}$. These orderings imply the initially stipulated long wavelength, low [Strouhal number](../../../../../../../strouhal-number.md) and large [Reynolds number](../../../../../../../reynolds-number.md). In the core $\lambda/Re=o(\epsilon^3)$, so perturbation viscous terms are beyond the retained order.

Subtract the undisturbed fully developed state and scale [pressure](../../../../../../../pressure.md) by $\rho\hat U^2$. The inviscid core equations are

$$
u_x+\frac1r(rv)_y=0,\qquad\lambda St\,u_t+uu_x+vu_y=-p_x,\qquad p_y=-\lambda^{-2}(\lambda St\,v_t+uv_x+vv_y).
$$

Put $u=u_0+\epsilon u_1+\epsilon^2u_2+\cdots$ and $v=\epsilon v_1+\epsilon^2v_2+\cdots$. At first order $p_{1y}=0$ and

$$
u_0u_{1x}+v_1u_0'=-p_{1x},\qquad u_{1x}+\frac1r(rv_1)_y=0.
$$

The wall's normal movement first enters at second order in this scaling, so $v_1=0$ at both walls. Taking the regular wall limits, where $u_0=0$ and $u_0'\ne0$, gives $p_{1x}=0$. The arbitrary constant [pressure](../../../../../../../pressure.md) perturbation can be set to zero.

Define the first-order axisymmetric [stream function](../../../../../../../stream-function.md) by $u_1=\psi_{1y}/r$ and $v_1=-\psi_{1x}/r$. The axial equation becomes $u_0\psi_{1yx}-u_0'\psi_{1x}=0$, or $(\psi_{1x}/u_0)_y=0$. Consequently $\psi_1=A(x,t)u_0(y)$ after absorbing an $x$-independent profile into the background. This proves the [annular inviscid-core displacement](../../../../../../../annular-inviscid-core-displacement.md)

$$
\boxed{u_1=\frac{A}{R+y}u_0'(y),\qquad v_1=-\frac{A_x}{R+y}u_0(y)}.
$$

It gives exactly the stated core expansion without requiring an explicit calculation of $u_0(y)$. The factors $1/(R+y)$ arise from cylindrical [mass conservation](../../../../../../../mass-conservation.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [I](../../i.md)
3. [3](../../../3.md)
4. [Paper 75](../../../../paper-75-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
