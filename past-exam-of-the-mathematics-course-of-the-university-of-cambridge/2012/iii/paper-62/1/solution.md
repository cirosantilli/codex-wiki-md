<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $u=u_x$ and $B=B_z$. In this geometry the [Lorentz force density](../../../../../lorentz-force-density.md) is purely longitudinal and equals $-\partial_x(B^2/2\mu_0)\mathbf e_x$. The [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) becomes $B_t+\partial_x(uB)=0$. Together with the [continuity equation](../../../../../continuity-equation.md) and adiabatic [pressure](../../../../../pressure.md) evolution, the four primitive-variable equations are

$$
\rho_t+u\rho_x+\rho u_x=0,\quad
p_t+up_x+\gamma p u_x=0,\quad
u_t+uu_x+\rho^{-1}p_x+\frac{B}{\mu_0\rho}B_x=0,\quad
B_t+uB_x+Bu_x=0.
$$

They have the required quasilinear form $\mathbf U_t+A\mathbf U_x=0$ with

$$
A=\begin{pmatrix}
u&0&\rho&0\\0&u&\gamma p&0\\0&1/\rho&u&B/(\mu_0\rho)\\0&0&B&u
\end{pmatrix}.
$$

Here the notation $u_x$ in derivatives means $\partial_xu$, whereas $u$ denotes the longitudinal [velocity](../../../../../velocity.md). Spatial dependence is one-dimensional; time dependence is allowed in the wave problem.

Put $c_f^2=\gamma p/\rho+B^2/(\mu_0\rho)$, and assume $\rho>0$ and $c_f>0$. Expansion of the [characteristic polynomial](../../../../../characteristic-polynomial.md) gives

$$
\det(A-\lambda I)=(u-\lambda)^2\bigl[(u-\lambda)^2-c_f^2\bigr],\qquad
\boxed{\lambda_0=u\text{ twice},\quad\lambda_\pm=u\pm c_f.}
$$

Two independent [eigenvectors](../../../../../eigenvector.md) for $\lambda_0$ can be chosen as $(1,0,0,0)^T$ and $(0,-B/\mu_0,0,1)^T$. For the two propagating branches, useful [eigenvectors](../../../../../eigenvector.md) are

$$
r_\pm=\left(1,\frac{\gamma p}{\rho},\frac{\pm c_f}{\rho},\frac B\rho\right)^T.
$$

The repeated branch advects an [entropy](../../../../../entropy.md) disturbance and a disturbance with unchanged total gas-plus-magnetic [pressure](../../../../../pressure.md). The $\pm$ branches are perpendicular [fast magnetosonic waves](../../../../../fast-magnetosonic-wave.md), with speed $c_f$ relative to the fluid.

On a uniform background, a Fourier amplitude $\widehat{\mathbf U}e^{i(kx-\omega t)}$ obeys $(kA-\omega I)\widehat{\mathbf U}=0$. Thus **the [eigenvalues](../../../../../eigenvalue.md) are the [phase velocities](../../../../../phase-velocity.md) $\omega/k$** for $k\ne0$, and the four dispersion branches are $\omega=ku$ twice and $\omega=k(u\pm c_f)$. The reduced geometry retains neither an independent transverse [velocity](../../../../../velocity.md) nor an additional propagating [Alfvén wave](../../../../../alfven-wave.md).

To construct each finite-amplitude [simple wave in magnetohydrodynamics](../../../../../simple-wave-in-magnetohydrodynamics.md), trace a state-space curve with tangent $r_\pm$, using $\rho$ as its parameter. Integrating the [pressure](../../../../../pressure.md) and magnetic components gives

$$
p=K\rho^\gamma,\qquad B=b\rho,\qquad
\frac{du}{d\rho}=\pm\frac{c_f(\rho)}{\rho},\qquad
c_f^2=\gamma K\rho^{\gamma-1}+\frac{b^2\rho}{\mu_0}.
$$

The constants $K$ and $b$ are the [entropy](../../../../../entropy.md) and transverse [magnetic flux freezing](../../../../../magnetic-flux-freezing.md) invariants along this state curve. Hence

$$
u(\rho)=u_*\pm\int_{\rho_*}^{\rho}\frac{c_f(r)}r\,dr.
$$

Since $A\mathbf U_\rho=\lambda_\pm\mathbf U_\rho$, substituting this curve into the original system reduces it to $\rho_t+\lambda_\pm(\rho)\rho_x=0$. By the [chain rule](../../../../../chain-rule.md),

$$
\boxed{\partial_t\lambda_\pm+\lambda_\pm\partial_x\lambda_\pm=0.}
$$

Thus the [characteristic speed](../../../../../characteristic-speed.md) itself satisfies the [Inviscid Burgers equation](../../../../../inviscid-burgers-equation.md). For initial speed $L(a)$, its smooth solution is $\lambda_\pm=L(a)$ along $x=a+tL(a)$, until the [characteristic curves](../../../../../characteristic-curve.md) intersect. This derivation supplies genuine state curves for [simple waves](../../../../../simple-wave.md), not merely a linear [dispersion relation](../../../../../dispersion-relation.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
