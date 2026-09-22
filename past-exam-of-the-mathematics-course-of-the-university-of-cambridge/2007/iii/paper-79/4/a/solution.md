<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use incompressible [Euler equations](../../../../../../euler-equations-for-an-inviscid-fluid.md) with pressure divided by the constant reference density. Writing $L=\partial_t+U(y)\partial_x$, their linearization about the parallel shear flow is

$$
Lu+U'v=-p_x,\qquad Lv=-p_y,\qquad Lw=-p_z,\qquad u_x+v_y+w_z=0.
$$

Taking the divergence requires the commutator $[\partial_y,L]=U'\partial_x$. Both this commutator and the divergence of $U'v$ contribute, so $\nabla^2p=-2U'v_x$. Applying the [Laplacian](../../../../../../laplacian.md) to $Lv=-p_y$ gives

$$
L\nabla^2v+2U'v_{xy}+U''v_x=-\partial_y\nabla^2p
=2U'v_{xy}+2U''v_x.
$$

Hence the wall-normal velocity equation is

$$
\boxed{L\nabla^2v-U''v_x=0.}
$$

Taking $\partial_z$ of the streamwise momentum equation minus $\partial_x$ of the spanwise equation cancels pressure and yields the inviscid [Squire equation](../../../../../../squire-equation.md),

$$
\boxed{L\eta=-U'v_z,\qquad\eta=u_z-w_x.}
$$

This is the vorticity component in the original PDF; the converted TeX corrupts its definition. Impermeable inviscid walls impose $v(\pm1,t)=0$. They do not impose a viscous no-slip condition on the tangential perturbation velocity.

For a [Fourier mode](../../../../../../fourier-mode.md), set $k^2=\alpha^2+\beta^2$, $D=d/dy$ and $q=(D^2-k^2)\widetilde v$. The equations become

$$
(\partial_t+i\alpha U)q-i\alpha U''\widetilde v=0,\qquad
(\partial_t+i\alpha U)\widetilde\eta=-i\beta U'\widetilde v.
$$

For [Couette flow](../../../../../../couette-flow.md) $U=\lambda y$, $U''=0$, so $q(y,t)=e^{-i\alpha\lambda yt}q_0(y)$ with $q_0=(D^2-k^2)\widetilde v_0$. Invert this using the [Dirichlet Green function](../../../../../../dirichlet-green-function.md) of $D^2-k^2$ on $[-1,1]$. If $y_< =\min(y,s)$ and $y_> =\max(y,s)$, it is

$$
G_k(y,s)=-\frac{\sinh[k(y_<+1)]\sinh[k(1-y_>)]}{k\sinh(2k)}.
$$

It vanishes at both walls and its first derivative has jump one at $y=s$. Thus

$$
\boxed{\widetilde v(y,t)=\int_{-1}^1G_k(y,s)e^{-i\alpha\lambda st}(D_s^2-k^2)\widetilde v_0(s)\,ds.}
$$

At $t=0$, uniqueness of the Dirichlet inversion recovers the compatible initial velocity. This [inviscid Couette initial-value Green function](../../../../../../inviscid-couette-initial-value-green-function.md) directly solves the initial-value problem without a [Laplace transform](../../../../../../laplace-transform.md).

The [Squire equation](../../../../../../squire-equation.md) is now a first-order forced equation in time. Its integrating factor gives

$$
\boxed{\widetilde\eta(y,t)=e^{-i\alpha\lambda yt}\widetilde\eta_0(y)-i\beta\lambda\int_0^t e^{-i\alpha\lambda y(t-s)}\widetilde v(y,s)\,ds.}
$$

For nonzero $\alpha$, the velocity formula contains shearing phases and the [inviscid Couette continuous spectrum](../../../../../../inviscid-couette-continuous-spectrum.md). Velocity cancellation can occur even though the transported $q$ has constant magnitude; it must not be confused with exponential modal instability.

For the separate case $\alpha=0$, $\beta\ne0$, the Dirichlet operator $D^2-\beta^2$ is invertible and $q_t=0$. Hence $\widetilde v=\widetilde v_0$ and

$$
\boxed{\widetilde\eta(y,t)=\widetilde\eta_0(y)-i\beta\lambda t\widetilde v_0(y).}
$$

Since $\widetilde\eta=i\beta\widetilde u$ in this case, $\widetilde u=\widetilde u_0-\lambda t\widetilde v_0$. This is the [lift-up effect](../../../../../../lift-up-effect.md): a transverse disturbance transports base-flow momentum and creates a streamwise perturbation growing linearly in time, with perturbation kinetic energy generically growing as $t^2$. The growth is algebraic and is possible without an exponentially unstable [normal mode](../../../../../../normal-mode.md). For nonzero initial normal velocity and nonzero shear, nonlinear effects eventually limit the validity of the linearized calculation. The same streamwise-independent result holds with $\lambda$ replaced by $U'(y)$ for a general parallel profile.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
