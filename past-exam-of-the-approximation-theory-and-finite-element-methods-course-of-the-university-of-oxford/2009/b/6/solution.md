<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Take linearly independent basis functions $\varphi_i\in H_0^1(0,1)$ and write $u_h(x,t)=\sum_jU_j(t)\varphi_j(x)$. The [weak formulation](../../../../weak-formulation.md) of the heat equation, tested against $\varphi_i$, is

$$
\int_0^1\partial_tu_h\,\varphi_i=-\int_0^1u_h'\varphi_i'.
$$

Thus the [semidiscrete finite element heat equation](../../../../semidiscrete-finite-element-heat-equation.md) is

$$
\boxed{M\dot U=KU,\qquad
M_{ij}=\int_0^1\varphi_i\varphi_j,\quad
K_{ij}=-\int_0^1\varphi_i'\varphi_j'.}
$$

The vector $U$ contains the basis coefficients. A natural initial vector $G$ is the $L^2$ projection of the initial data: $MG=b$, where $b_i=\int_0^1g\varphi_i$, and $U(0)=G$. Other consistent initial approximations can be specified, but exact representation of an arbitrary $g$ in the trial space is not implicit.

For a nonzero coefficient vector $a$, the function $v_h=\sum_ia_i\varphi_i$ is nonzero by basis independence. Hence $a^TMa=\|v_h\|_{L^2}^2>0$, proving that the [mass matrix](../../../../mass-matrix.md) is symmetric positive definite. Also $a^TKa=-\|v_h'\|_{L^2}^2<0$: if the derivative vanished, $v_h$ would be a constant, and its zero endpoint traces would make it zero. Therefore **$K$ is symmetric negative definite**, not merely semidefinite, for these homogeneous Dirichlet conditions.

The squared spatial norm is $U^TMU$. Differentiating and using the semidiscrete system gives the [energy identity](../../../../energy-identity.md)

$$
\frac d{dt}\|u_h(t)\|_{L^2}^2
=2U^TM\dot U=2U^TKU=-2\|u_h'(t)\|_{L^2}^2\leq0.
$$

Using the [trapezoidal rule](../../../../trapezoidal-rule.md) in time gives the [Crank-Nicolson method](../../../../crank-nicolson-method.md)

$$
\boxed{(M-\tfrac12\Delta t K)U^{k+1}
=(M+\tfrac12\Delta t K)U^k.}
$$

The left matrix is positive definite for every $\Delta t>0$, so every step exists uniquely. To prove stability, set $d=U^{k+1}-U^k$ and $s=U^{k+1}+U^k$. The update says $Md=(\Delta t/2)Ks$. Multiplying by $s^T$ gives

$$
(U^{k+1})^TMU^{k+1}-(U^k)^TMU^k
=\frac{\Delta t}{2}s^TKs\leq0.
$$

Consequently

$$
\boxed{\|u_h^{k+1}\|_{L^2}\leq\|u_h^k\|_{L^2}\quad
\text{for every }\Delta t>0.}
$$

The same inequality applied to the difference of two discrete solutions proves nonamplification of initial perturbations. This is unconditional stability in the mass-matrix norm, exactly the spatial $L^2$ norm of the finite element functions.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../split.md)
5. [Approximation theory and finite element methods course of the University of Oxford](../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
