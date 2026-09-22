<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $(\mathbf u^{(1)},\boldsymbol\sigma^{(1)})$ and $(\mathbf u^{(2)},\boldsymbol\sigma^{(2)})$ be two [Stokes flows](../../../../../stokes-flow-split.md) in the same fluid domain, with equal [dynamic viscosity](../../../../../dynamic-viscosity.md) and zero body [force](../../../../../force.md). The [Lorentz reciprocal theorem for Stokes flow](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) is

$$
\int_{\partial V}\mathbf u^{(1)}\cdot\boldsymbol\sigma^{(2)}\mathbf n\,dS=\int_{\partial V}\mathbf u^{(2)}\cdot\boldsymbol\sigma^{(1)}\mathbf n\,dS.
$$

To prove it, use the symmetric [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) $\boldsymbol\sigma^{(k)}=-p^{(k)}\mathbf I+2\mu\mathbf e^{(k)}$ and $\partial_j\sigma^{(k)}_{ij}=0$. [Incompressibility](../../../../../incompressible-flow.md) removes the [pressure](../../../../../pressure.md) contraction, while symmetry removes the antisymmetric [velocity](../../../../../velocity.md) gradient. Therefore

$$
\partial_j\bigl(u_i^{(1)}\sigma_{ij}^{(2)}-u_i^{(2)}\sigma_{ij}^{(1)}\bigr)=2\mu\bigl(\mathbf e^{(1)}:\mathbf e^{(2)}-\mathbf e^{(2)}:\mathbf e^{(1)}\bigr)=0.
$$

The [divergence theorem](../../../../../divergence-theorem.md) proves the boundary identity. It applies to an exterior domain by a limit at infinity; the boundary integral there vanishes for decaying rigid-body [Stokes flows](../../../../../stokes-flow-split.md).

Use a normal directed outward from the fluid, into the [rigid body](../../../../../rigid-body-dynamics.md). Then $\mathbf F=\int\boldsymbol\sigma\mathbf n\,dS$ and $\mathbf G=\int\mathbf r\times(\boldsymbol\sigma\mathbf n)\,dS$ are the [force](../../../../../force.md) and couple exerted by the body on the fluid. If $\mathbf q=(\mathbf U,\boldsymbol\Omega)$ and $(\mathbf F,\mathbf G)=\mathsf R\mathbf q$, inserting the rigid boundary [velocity](../../../../../velocity.md) $\mathbf U+\boldsymbol\Omega\times\mathbf r$ into the [Lorentz reciprocal theorem for Stokes flow](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) gives

$$
(\mathbf q^{(1)})^T\mathsf R\mathbf q^{(2)}=(\mathbf q^{(2)})^T\mathsf R\mathbf q^{(1)}.
$$

Arbitrary rigid velocities imply $\mathsf R=\mathsf R^T$. A separate integration by parts, using the [Stokes equation](../../../../../stokes-equation.md), gives

$$
\mathbf q^T\mathsf R\mathbf q=\mathbf F\cdot\mathbf U+\mathbf G\cdot\boldsymbol\Omega=2\mu\int_V\mathbf e:\mathbf e\,dV\ge0.
$$

Equality requires zero [rate-of-strain tensor](../../../../../strain-rate-tensor.md) everywhere. Such a [velocity](../../../../../velocity.md) is a rigid motion in the connected exterior fluid; decay at infinity forces it to vanish, and the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) then forces $\mathbf U=\boldsymbol\Omega=0$. Hence **the resistance matrix is symmetric positive definite**. Defining [force](../../../../../force.md) as fluid-on-body would reverse its sign, so the positive convention matters.

For the rods, choose body axes along $OA$, $OB$, and their normal. On the first rod, $\mathbf X=s\mathbf e_x$ for $0\le s\le2L$, and the [slender-body force density](../../../../../slender-body-force-density.md) is

$$
\mathbf f_x=C\left(\frac{U_x}{2},\ U_y+\Omega_zs,\ U_z-\Omega_ys\right).
$$

On the second rod, $\mathbf X=s\mathbf e_y$, and

$$
\mathbf f_y=C\left(U_x-\Omega_zs,\ \frac{U_y}{2},\ U_z+\Omega_xs\right).
$$

Integrate the [force](../../../../../force.md) densities and the moments $\mathbf X\times\mathbf f$, using $\int ds=2L$, $\int s\,ds=2L^2$, and $\int s^2ds=8L^3/3$. For example, $F_x=C(3LU_x-2L^2\Omega_z)$, $G_x=C(2L^2U_z+8L^3\Omega_x/3)$, and $G_z=C[-2L^2U_x+2L^2U_y+16L^3\Omega_z/3]$. In the ordering $(U_x,U_y,U_z,\Omega_x,\Omega_y,\Omega_z)$, the full [right-angle two-rod resistance matrix](../../../../../right-angle-two-rod-resistance-matrix.md) is

$$
\boxed{\mathsf R=C\begin{pmatrix}
3L&0&0&0&0&-2L^2\\
0&3L&0&0&0&2L^2\\
0&0&4L&2L^2&-2L^2&0\\
0&0&2L^2&8L^3/3&0&0\\
0&0&-2L^2&0&8L^3/3&0\\
-2L^2&2L^2&0&0&0&16L^3/3
\end{pmatrix}}.
$$

The planar subsystem is

$$
\begin{pmatrix}F_x\\F_y\\G_z/L\end{pmatrix}=CL\begin{pmatrix}3&0&-2\\0&3&2\\-2&2&16/3\end{pmatrix}\begin{pmatrix}U_x\\U_y\\\Omega_zL\end{pmatrix}.
$$

Inverting this symmetric matrix gives the [hydrodynamic mobility matrix](../../../../../hydrodynamic-mobility-matrix.md)

$$
\boxed{CL\begin{pmatrix}U_x\\U_y\\\Omega_zL\end{pmatrix}=\begin{pmatrix}1/2&-1/6&1/4\\-1/6&1/2&-1/4\\1/4&-1/4&3/8\end{pmatrix}\begin{pmatrix}F_x\\F_y\\G_z/L\end{pmatrix}}.
$$

The upper-right entry is positive, as printed in the PDF; the negative sign in the converted TeX would violate both this inversion and reciprocity.

Let laboratory $X$ point along the initial $OA$ and laboratory $Y$ point upward. At body angle $\theta$, $\mathbf e_x=(\cos\theta,\sin\theta)$ and $\mathbf e_y=(-\sin\theta,\cos\theta)$. The gravitational load, balanced by body-on-fluid resistance, has body components

$$
F_x=-(1+2\lambda)mg\sin\theta,\qquad F_y=-(1+2\lambda)mg\cos\theta,\qquad G_z=2\lambda mgL(\sin\theta-\cos\theta).
$$

The last expression follows by taking moments of the two endpoint weights about $O$. Substitution into the [hydrodynamic mobility matrix](../../../../../hydrodynamic-mobility-matrix.md) gives

$$
CL U_x=mg\left[\frac{1-\lambda}{6}\cos\theta-\frac{1+\lambda}{2}\sin\theta\right],\qquad CL U_y=mg\left[\frac{1-\lambda}{6}\sin\theta-\frac{1+\lambda}{2}\cos\theta\right],
$$



$$
\boxed{\dot\theta=\frac{(1-\lambda)mg}{4CL^2}(\cos\theta-\sin\theta)}.
$$

For $\lambda=1$, the initial condition $\theta=0$ persists, and $U_x=0$, $U_y=-mg/(CL)$: **vertical descent without rotation**. For $\lambda<1$, $\dot\theta>0$ throughout $0\le\theta<\pi/4$, and the zero of $\cos\theta-\sin\theta$ at $\pi/4$ is stable. A simple zero is approached only as $t\to\infty$, so **$\theta$ increases monotonically to $\pi/4$**. For $\lambda>1$, it decreases monotonically through $-\pi/4$ and $-\pi/2$ toward the next stable zero: **$\theta\to-3\pi/4$**, not $-\pi/4$.

The laboratory horizontal [velocity](../../../../../velocity.md) of $O$ is

$$
\dot X=U_x\cos\theta-U_y\sin\theta=\frac{(1-\lambda)mg}{6CL}\cos2\theta.
$$

For $\lambda\ne1$, divide by the angular equation to eliminate time:

$$
\frac{dX}{d\theta}=\frac{2L}{3}\frac{\cos2\theta}{\cos\theta-\sin\theta}=\frac{2L}{3}(\cos\theta+\sin\theta),\qquad X-X(0)=\frac{2L}{3}(1+\sin\theta-\cos\theta).
$$

At both limiting orientations the sine and cosine are equal, so the [sedimentation drift of a weighted two-rod body](../../../../../sedimentation-drift-of-a-weighted-two-rod-body.md) is

$$
\boxed{X(\infty)-X(0)=\frac{2L}{3}\quad\text{for both }\lambda<1\text{ and }\lambda>1.}
$$

For $\lambda>1$ the initial drift is negative. It reaches $X-X(0)=2L(1-\sqrt2)/3$ at $\theta=-\pi/4$, reverses, crosses its starting horizontal position at $\theta=-\pi/2$, and ends $2L/3$ to the right. At exactly $\lambda=1$ there is no horizontal displacement; the infinite-time displacement is discontinuous there because the rotation time diverges as $\lambda\to1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
