<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

In vacuum without sources, [Maxwell equations](../../../../../maxwell-equations.md) are $\nabla\cdot E=\nabla\cdot B=0$, $\nabla\times E=-\dot B$, and $\nabla\times B=\dot E/c^2$. For $E'=cB$, $B'=-E/c$, both divergences remain zero, and

$$
\nabla\times E'=c\nabla\times B=\dot E/c=-\dot B',\qquad\nabla\times B'=-\nabla\times E/c=\dot B/c=\dot E'/c^2.
$$

This proves the quarter-turn [electromagnetic duality](../../../../../electromagnetic-duality.md) transformation.

A [perfect conductor](../../../../../perfect-conductor.md) has zero electric field in its bulk. Continuity of tangential electric field therefore gives $n\times E=0$ at its surface. Faraday's law makes a nonzero-frequency magnetic field vanish in that bulk, and continuity of its normal component gives $n\cdot B=0$ for the wave field. An independently trapped static magnetic flux is not excluded by perfect conductivity alone; the stated condition applies to the oscillating field under consideration.

For amplitudes with dependence $e^{i(kz-\omega t)}$, let $\gamma^2=\omega^2/c^2-k^2$ and suppose $(\Delta_\perp+\gamma^2)\psi=0$. With $k\ne0$ and $\omega\ne0$, define the transverse-magnetic family of [scalar-potential conducting waveguide modes](../../../../../scalar-potential-conducting-waveguide-modes.md) by

$$
\boxed{e_\perp=\nabla_\perp\psi,\quad e_z=-\frac{i\gamma^2}{k}\psi=i\left(k-\frac{\omega^2}{kc^2}\right)\psi,\quad b_\perp=\frac\omega{kc^2}\widehat z\times\nabla_\perp\psi,\quad b_z=0.}
$$

The electric divergence is $\Delta_\perp\psi+ike_z=0$; the magnetic divergence is zero because the transverse field is a rotated gradient. Direct differentiation gives $\nabla\times e=i\omega b$ and $\nabla\times b=-i\omega e/c^2$, where longitudinal differentiation means multiplication by $ik$. Thus all vacuum equations hold, with $\boxed{\gamma^2=\omega^2/c^2-k^2}$.

On a wall parallel to $z$, $\psi=0$ makes both $e_z$ and the boundary-tangential derivative of $\psi$ vanish. It also makes $n\cdot b$ proportional to that tangential derivative, hence zero. This proves the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) supplies both conductor conditions.

For a transverse-electric family, use duality and rescale the potential, or check directly that

$$
\boxed{e_\perp=\widehat z\times\nabla_\perp\psi,\quad e_z=0,\quad b_\perp=-\frac k\omega\nabla_\perp\psi,\quad b_z=\frac{i\gamma^2}{\omega}\psi}
$$

satisfies the same equations. If $t=\widehat z\times n$ is the cross-sectional wall tangent, then $t\cdot e=n\cdot\nabla_\perp\psi$ and $n\cdot b=-(k/\omega)n\cdot\nabla_\perp\psi$. Consequently $\boxed{\partial_n\psi=0}$, a [Neumann boundary condition](../../../../../neumann-boundary-condition.md), supplies both wall conditions. Duality exchanges the field constructions, but does not preserve electric-conductor boundary conditions without this new boundary test.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
