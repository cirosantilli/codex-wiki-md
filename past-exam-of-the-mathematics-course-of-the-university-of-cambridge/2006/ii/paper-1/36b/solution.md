<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

For a material interface with no mass transfer, the normal fluid [velocity](../../../../../velocity.md) on both sides equals the interface's normal [velocity](../../../../../velocity.md). For ordinary viscous fluids without interfacial slip, tangential [velocities](../../../../../velocity.md) also agree. The stress tensors $T_i=-p_iI+\mu_i(\nabla\mathbf u_i+\nabla\mathbf u_i^T)$ have continuous tangential traction when [surface tension](../../../../../surface-tension.md) is uniform; their normal traction jump balances surface-tension curvature. Nonuniform [surface tension](../../../../../surface-tension.md) instead supplies a tangential [Marangoni stress](../../../../../marangoni-effect.md). These conditions express conservation of mass, no slip between the contacting fluids and force balance at the interface. For a flat interface of constant tension the full traction is continuous.

Choose $x$ down the plane and $y$ perpendicular outward from it. A steady parallel solution has [velocity](../../../../../velocity.md) $(u(y),0)$ and equations

$$
0=-p_x+\mu u''+\rho g\sin\theta,\qquad0=-p_y-\rho g\cos\theta.
$$

For a uniform free layer, $p_x=0$, $u(0)=0$, $u'(h)=0$ and $p(h)=p_{\rm atm}$. [Integration](../../../../../integral.md) gives

$$
\boxed{p=p_{\rm atm}+\rho g\cos\theta(h-y),\quad u=\frac{\rho g\sin\theta}{\mu}\left(hy-\frac{y^2}{2}\right).}
$$

Its flux per unit cross-slope width is

$$
\boxed{\int_0^h u(y)dy=\frac{\rho g h^3\sin\theta}{3\mu}.}
$$

For the [two-layer falling film of equal-density viscous fluids](../../../../../two-layer-falling-film-of-equal-density-viscous-fluids.md) let $H=(1+\alpha)h$ and $A=\rho g\sin\theta/\mu$. Equal density gives the same continuous [hydrostatic pressure](../../../../../hydrostatic-pressure.md) in both, $p=p_{\rm atm}+\rho g\cos\theta(H-y)$. The wall condition is $u_1(0)=0$, the upper condition $u_2'(H)=0$, and at $h$ we require $u_1=u_2$, $\mu u_1'=\beta\mu u_2'$. Integrating the two [momentum](../../../../../momentum.md) equations with these conditions gives

$$
\boxed{u_1(y)=A\left(Hy-\frac{y^2}{2}\right),\quad0\leq y\leq h,}
$$



$$
\boxed{u_2(h+z)=Ah^2\left(\alpha+\frac12\right)+\frac A\beta\left(\alpha h z-\frac{z^2}{2}\right),\quad0\leq z\leq\alpha h.}
$$

The [shear stress](../../../../../shear-stress.md) transmitted to the lower layer is the upper layer's downslope weight per unit area, $\rho g\alpha h\sin\theta$, obtained by integrating the upper [momentum](../../../../../momentum.md) balance from its stress-free surface. It depends on thickness but not upper [viscosity](../../../../../dynamic-viscosity.md). Changing $\beta$ changes the upper shear rate needed to transmit that stress, while the lower profile depends on $\alpha$ alone.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
