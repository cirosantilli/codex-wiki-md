# Vorticity of a linear shear flow

↑ **Parent:** [Vorticity](vorticity-split.md)

Use a [linear shear flow](linear-shear-flow.md) to see why straight [pathlines](pathline.md) can still carry local spin. Faster layers pull past slower ones, and a small symmetric paddle can turn clockwise while its center travels straight ahead.

<a id="image-straight-particle-paths-in-linear-shear-coexist-with-clockwise-local-spin-and-material-line-deformation"></a>
![](shear-flow-vorticity.png)

**[Figure 2](#image-straight-particle-paths-in-linear-shear-coexist-with-clockwise-local-spin-and-material-line-deformation). Straight particle paths in linear shear coexist with clockwise local spin and material-line deformation**.

For the planar [simple shear flow](simple-shear-flow.md) $\mathbf u=(\gamma y,0,0)$ with constant signed [shear rate](shear-rate.md) $\gamma$, direct [differentiation](differentiation.md) gives

$$
\omega_z=\partial_xu_y-\partial_yu_x=-\gamma,\qquad\Omega_{{\rm spin},z}=-\frac\gamma2.
$$

With $\gamma=1\ \mathrm{s^{-1}}$, these are $-1\ \mathrm{s^{-1}}$ and $-0.5\ \mathrm{s^{-1}}$: both signs indicate clockwise orientation under the [right-hand rule](right-hand-rule.md). Yet a particle initially at $(x_0,y_0)$ follows the straight [pathline](pathline.md) $x(t)=x_0+\gamma y_0t$, $y(t)=y_0$. The [curl](curl.md) measures differences of [velocity](velocity.md) between neighboring particles, rather than bending of one particle's [pathline](pathline.md).

The [velocity gradient](velocity-gradient.md) has $L_{xy}=\gamma$ as its only nonzero entry. Its [spin tensor](spin-tensor.md) supplies clockwise rotation, while its [rate-of-strain tensor](strain-rate-tensor.md) supplies simultaneous deformation. For a [material line](material-curve.md) making angle $\alpha$ to the horizontal, the equation $\dot{\delta\mathbf x}=L\delta\mathbf x$ gives $\dot\alpha=-\gamma\sin^2\alpha$. Initially horizontal and vertical [material lines](material-curve.md) therefore have [angular velocities](angular-velocity.md) $0$ and $-\gamma$; their mean is $-\gamma/2$. At $t=0.5\ \mathrm{s}$ with $\gamma=1\ \mathrm{s^{-1}}$, an initially vertical displacement becomes $(0.5,1)$ times its original length and has angle $\arctan 2\approx63.435^\circ$, a clockwise change of $26.565^\circ$. The plotted cross deforms; an actual paddle's response also depends on its shape and interaction with the fluid. The exact local spin statement concerns the [spin tensor](spin-tensor.md), rather than every tracer's orientation.

## ↑ Ancestors (5)

1. [Vorticity](vorticity-split.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
