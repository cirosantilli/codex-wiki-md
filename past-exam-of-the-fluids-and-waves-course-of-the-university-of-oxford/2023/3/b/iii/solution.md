<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Linearize about the resting state $\eta=0$, $\phi=0$. Introduce a dimensionless small parameter $\epsilon$ and write

$$
\eta=\epsilon\eta_1+O(\epsilon^2),\qquad
\phi=\epsilon\phi_1+O(\epsilon^2),
$$

holding the depth, [bending stiffness](../../../../../bending-stiffness.md) and variation scales fixed. Thus both boundary displacement and induced [velocity](../../../../../velocity.md) are small. For any first-order derivative $D\phi$, a [Taylor expansion](../../../../../taylor-expansion.md) at the moving surface gives

$$
(D\phi)(x,\eta,t)
=\epsilon(D\phi_1)(x,0,t)+O(\epsilon^2).
$$

The displacement correction to the leading field is $\epsilon^2\eta_1\partial_z(D\phi_1)(x,0,t)$, so evaluating it on $z=0$ changes it only at second order. Also $\phi_x\eta_x=O(\epsilon^2)$ and $|\nabla\phi|^2=O(\epsilon^2)$. The first-order [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) and dynamic boundary condition are therefore

$$
(\eta_1)_t=(\phi_1)_z(x,0,t),\qquad
(\phi_1)_t(x,0,t)+g\eta_1+\frac B\rho(\eta_1)_{xxxx}=0.
$$

Dropping the subscript, the [linearized boundary condition](../../../../../linearized-boundary-condition.md) pair is

$$
\boxed{\eta_t=\phi_z,\qquad
\phi_t+g\eta+\frac B\rho\eta_{xxxx}=0\quad\text{at }z=0}.
$$

The fixed-bed condition remains $\phi_z(x,-h,t)=0$. The source's shorthand $|\eta|\ll1$ requires a length scale: for the subsequent [plane wave](../../../../../plane-wave.md), small surface slope $k|\alpha|\ll1$ and displacement small compared with depth are sufficient conditions. Small height alone, with arbitrarily rapid spatial variation or a finite background disturbance, does not justify discarding the products.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
