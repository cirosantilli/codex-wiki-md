<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

For constant [mass density](../../../../../density.md) and [incompressible flow](../../../../../incompressible-flow.md), use $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$ in the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md). Taking the [curl](../../../../../curl.md) removes the [pressure](../../../../../pressure.md) and [kinetic energy](../../../../../kinetic-energy.md) [gradients](../../../../../gradient.md), giving $\boldsymbol\omega_t=\nabla\times(\mathbf u\times\boldsymbol\omega)$. The supplied vector identity, with $\nabla\cdot\mathbf u=0$ and $\nabla\cdot\boldsymbol\omega=0$, yields the [vorticity equation](../../../../../vorticity-equation.md)

$$
\boxed{\frac{D\boldsymbol\omega}{Dt}=\boldsymbol\omega_t+(\mathbf u\cdot\nabla)\boldsymbol\omega=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

In a two-dimensional flow $\mathbf u=(u,v,0)$ is independent of $z$, and $\boldsymbol\omega=\omega\mathbf e_z$. The right side vanishes, so $D\omega/Dt=0$: each material element retains its [vorticity](../../../../../vorticity.md). The [vortex lines](../../../../../vortex-line.md) are parallel to $z$ and are carried by the planar velocity. Also planar incompressibility preserves the area of a material cross-section; integrating its conserved [vorticity](../../../../../vorticity.md) over that area shows that its [circulation](../../../../../circulation-physics.md), or vortex strength, stays constant. Thus the [vortex lines](../../../../../vortex-line.md) move with the fluid without changing strength.

Place a [line vortex](../../../../../line-vortex.md) of [circulation](../../../../../circulation-physics.md) $\Gamma$ at $(0,b)$ above the wall $y=0$. Its [velocity field](../../../../../velocity-field.md) is $\Gamma\mathbf e_z\times(\mathbf r-\mathbf r_0)/(2\pi|\mathbf r-\mathbf r_0|^2)$. The [method of images](../../../../../method-of-images.md) puts a vortex of [circulation](../../../../../circulation-physics.md) $-\Gamma$ at $(0,-b)$. With $\mathbf u=(\psi_y,-\psi_x)$, the resulting [stream function](../../../../../stream-function.md) is

$$
\psi(x,y)=-\frac\Gamma{2\pi}\log\sqrt{x^2+(y-b)^2}+\frac\Gamma{2\pi}\log\sqrt{x^2+(y+b)^2}.
$$

It is identically zero on the wall, so $u_y=-\psi_x=0$ there. In the fluid half-plane it has just the required vortex singularity, with no other singularities, and its velocity decays at infinity. This is the no-background-flow solution with the wall: the difference from another such solution is a regular irrotational, divergence-free decaying field with zero normal [velocity](../../../../../velocity.md). Reflect its tangential component evenly and its normal component oddly across the wall. The reflected components are bounded harmonic functions on the whole plane, so they are constant by [harmonic Liouville theorem](../../../../../harmonic-liouville-theorem.md), and decay forces both constants to be zero. Thus replacing the wall by the image gives the same flow. The real vortex moves under the image velocity, excluding its own singular velocity, so

$$
\dot{\mathbf r}_0=\frac{-\Gamma}{2\pi}\frac{\mathbf e_z\times(0,2b)}{4b^2}=\left(\frac\Gamma{4\pi b},0\right).
$$

Its **signed velocity parallel to the wall is $\Gamma/(4\pi b)$**, and its speed is $|\Gamma|/(4\pi b)$.

For the quarter-plane, place images of [circulation](../../../../../circulation-physics.md) $-\Gamma$ at $(-x,y)$ and $(x,-y)$, and $+\Gamma$ at $(-x,-y)$. The paired [stream functions](../../../../../stream-function.md) make both walls [streamlines](../../../../../streamline.md). Summing their velocities at the real vortex gives

$$
\dot x=\frac\Gamma{4\pi}\left(\frac1y-\frac{y}{x^2+y^2}\right)=\frac{\Gamma x^2}{4\pi y(x^2+y^2)},\qquad\dot y=\frac\Gamma{4\pi}\left(-\frac1x+\frac{x}{x^2+y^2}\right)=-\frac{\Gamma y^2}{4\pi x(x^2+y^2)}.
$$

In [polar coordinates](../../../../../polar-coordinates.md),

$$
\dot r=\frac{x\dot x+y\dot y}{r}=\frac\Gamma{2\pi r}\cot2\theta,\qquad\dot\theta=\frac{x\dot y-y\dot x}{r^2}=-\frac\Gamma{4\pi r^2}.
$$

It follows directly that

$$
\frac d{dt}(r\sin2\theta)=\dot r\sin2\theta+2r\dot\theta\cos2\theta=0.
$$

Thus the [line-vortex trajectory in a quarter-plane](../../../../../line-vortex-trajectory-in-a-quarter-plane.md) is **$r\sin2\theta=\text{constant}$**.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
