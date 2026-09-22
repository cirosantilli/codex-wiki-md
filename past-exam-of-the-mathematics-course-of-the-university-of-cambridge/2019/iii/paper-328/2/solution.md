<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [weighted Neumann heat kernel with constant drift](../../../../../weighted-neumann-heat-kernel-with-constant-drift.md). The spatial operator has the [self-adjoint](../../../../../self-adjoint-operator.md) form

$$
\mathcal Lu=u_{xx}+\beta u_x=e^{-\beta x}(e^{\beta x}u_x)_x,
$$

so its homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) give a regular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) in the [weighted inner product](../../../../../weighted-inner-product.md)

$$
\langle f_1,f_2\rangle_\beta=\int_0^L e^{\beta x}\overline{f_1(x)}f_2(x)\,dx.
$$

The constant [eigenfunction](../../../../../eigenfunction.md) is $\phi_0=1$, with [eigenvalue](../../../../../eigenvalue.md) $\lambda_0=0$ and squared [norm](../../../../../norm.md) $N_0=(e^{\beta L}-1)/\beta$. For $k\geq1$, put $q_k=k\pi/L$. Substitution of $\phi=e^{-\beta x/2}v$ in $\mathcal L\phi=-\lambda\phi$ gives $v''+(\lambda-\beta^2/4)v=0$ and the [Robin boundary conditions](../../../../../robin-boundary-condition.md) $v'=\beta v/2$ at both endpoints. Hence

$$
\phi_k(x)=e^{-\beta x/2}\left[\cos(q_kx)+\frac{\beta}{2q_k}\sin(q_kx)\right],
\qquad \lambda_k=q_k^2+\frac{\beta^2}{4}.
$$

Indeed,

$$
\phi_k'(x)=-e^{-\beta x/2}\left(q_k+\frac{\beta^2}{4q_k}\right)\sin(q_kx),
\qquad
N_k=\int_0^Le^{\beta x}\phi_k(x)^2dx=\frac L2\left(1+\frac{\beta^2}{4q_k^2}\right).
$$

The [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) is complete and [orthogonal](../../../../../orthogonal-vectors.md). Its [heat kernel](../../../../../heat-kernel.md), relative to the measure $e^{\beta y}dy$, is

$$
K_\beta(x,y,t)=\frac1{N_0}+\sum_{k=1}^\infty\frac{e^{-\lambda_kt}}{N_k}\phi_k(x)\phi_k(y),\qquad t>0.
$$

For a coefficient $a_k(t)=\langle\phi_k,u(\cdot,t)\rangle_\beta/N_k$, two applications of [integration by parts](../../../../../integration-by-parts.md) yield

$$
a_k'+\lambda_ka_k=\frac{e^{\beta L}\phi_k(L)h(t)-\phi_k(0)g(t)}{N_k},
\qquad
a_k(0)=\frac1{N_k}\int_0^Le^{\beta y}\phi_k(y)u_0(y)\,dy.
$$

Solving these scalar [linear differential equations](../../../../../linear-differential-equation.md) and summing gives the [Neumann boundary-forcing formula](../../../../../neumann-boundary-forcing-formula.md):

$$
\boxed{u(x,t)=\int_0^LK_\beta(x,y,t)e^{\beta y}u_0(y)\,dy+\int_0^t\left[e^{\beta L}K_\beta(x,L,t-s)h(s)-K_\beta(x,0,t-s)g(s)\right]ds.}
$$

This depends only on the given data. In particular, the zero [eigenvalue](../../../../../eigenvalue.md) retains the changing weighted mean:

$$
\frac d{dt}\int_0^Le^{\beta x}u(x,t)\,dx=e^{\beta L}h(t)-g(t).
$$

The endpoint derivatives of the boundary integral are understood as interior limits. Differentiating each homogeneous [Neumann eigenfunction](../../../../../neumann-eigenfunction.md) at the endpoint before summing would incorrectly discard the prescribed boundary forcing: the short-time [heat kernel](../../../../../heat-kernel.md) makes that interchange invalid. The stated compatibility conditions give the classical boundary traces.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
