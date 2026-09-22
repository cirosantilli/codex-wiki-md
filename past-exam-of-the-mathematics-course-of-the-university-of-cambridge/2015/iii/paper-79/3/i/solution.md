<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md) convention $u_n=-\psi_{n,y}$, $v_n=\psi_{n,x}$, and write $F=k_I^2$, $f=f_0+\beta y$. In a steady, large-scale basin interior, neglect the [material derivatives](../../../../../../material-derivative.md) of relative [vorticity](../../../../../../vorticity.md) and interfacial stretching compared with advection of [planetary vorticity](../../../../../../planetary-vorticity.md). With small [Rossby number](../../../../../../rossby-number.md), weak nonlinear eddy terms, no significant interior friction or topographic forcing, and the specified forcing confined to layer 1, [Sverdrup balance](../../../../../../sverdrup-balance.md) is

$$
\boxed{\beta\bar v_1=W,\qquad \beta\bar v_2=0.}
$$

For equal depths $h$, the depth-integrated meridional transport is $h(\bar v_1+\bar v_2)=hW/\beta$. Here $W$ is the normalized [potential vorticity](../../../../../../potential-vorticity.md) source appearing in the evolution equation. If the dimensional [wind stress curl](../../../../../../wind-stress-curl.md) is used, its usual layer forcing is $W=(\nabla_h\times\boldsymbol\tau)_z/(\rho_0h)$, so $\beta h(\bar v_1+\bar v_2)=(\nabla_h\times\boldsymbol\tau)_z/\rho_0$.

For $\beta>0$ and $W<0$, the upper-layer interior transport is **southward**. In a closed subtropical basin, negative [wind stress curl](../../../../../../wind-stress-curl.md) also corresponds to downwelling [Ekman pumping](../../../../../../ekman-pumping.md) for $f_0>0$ and an anticyclonic gyre. A northward return transport is needed to close the circulation; its narrow western boundary current requires processes outside the frictionless [Sverdrup balance](../../../../../../sverdrup-balance.md). The local interior equations by themselves do not specify the detailed boundary-current structure.

Expanding the layer equation shows the physical budget:

$$
\beta v_n+\frac{D_n}{Dt}\nabla_h^2\psi_n-F\frac{D_n}{Dt}(\psi_n-\psi_m)=\begin{cases}W,&n=1,\\0,&n=2,\end{cases}\qquad m\ne n.
$$

The first term is the change of [planetary vorticity](../../../../../../planetary-vorticity.md) as a fluid parcel moves north or south. The second is the change of relative [vorticity](../../../../../../vorticity.md). The last is [vortex stretching in layered quasi-geostrophic flow](../../../../../../vortex-stretching-in-layered-quasi-geostrophic-flow.md): displacement of the interface changes layer thickness and thus the stretching contribution to [potential vorticity](../../../../../../potential-vorticity.md). Its opposite signs in the two layer definitions express their thickness changes in opposite directions. The [wind stress curl](../../../../../../wind-stress-curl.md) supplies or removes upper-layer [potential vorticity](../../../../../../potential-vorticity.md). Each $D_n/Dt$ follows its own layer velocity, rather than a common velocity for both layers.

For uniform $W$, choose the local [two-layer Sverdrup interior](../../../../../../two-layer-sverdrup-interior.md)

$$
\boxed{\bar\psi_1=Vx,\qquad \bar\psi_2=0,\qquad V=\frac W\beta.}
$$

Unforced background zonal currents and arbitrary additive interface offsets have been set to zero. This choice is also an exact uniform-flow solution of the stated forced equations, not just a leading balance: $\bar q_1=f_0+\beta y-FVx$, $\bar q_2=f_0+\beta y+FVx$, and $\bar v_1\bar q_{1,y}=V\beta=W$. The local interface slope can be nonzero even though its stretching contribution is constant along each basic-state trajectory. A streamfunction linear in $x$ is an interior-patch description, not a complete globally bounded basin solution.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
