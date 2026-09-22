<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $s=a_{\min}$ be a small neck radius in the preceding sinusoidal shape. Expanding around a minimum gives $a\simeq s+(gk^2/\sqrt2)(z-z_*)^2$, so its local axial length is $\ell\sim[s/(gk^2)]^{1/2}$. The uniform-[pressure](../../../../../../pressure.md) model has $|a_t|\sim\gamma/\mu$ near the neck. Local [conservation of mass](../../../../../../mass-conservation.md) therefore demands axial inner flux $Q\sim s(\gamma/\mu)\ell$. Internal [Hagen-Poiseuille flow](../../../../../../hagen-poiseuille-equation.md) of viscosity $\lambda\mu$ would require a [pressure](../../../../../../pressure.md) difference

$$
\Delta P\sim\frac{\lambda\mu Q\ell}{s^4}\sim\frac{\lambda\gamma\ell^2}{s^3},\qquad
\frac{\Delta P}{\gamma/s}\sim\frac{\lambda}{gk^2s}.
$$

If $sk\ll\lambda$, while $gk\ll1$ by slenderness, this ratio is very large. Hence **internal [pressure](../../../../../../pressure.md) variation certainly cannot be neglected when $a_{\min}k\ll\lambda$**. This is a sufficient breakdown condition; appreciable variation can arise earlier, especially because the radial viscous and capillary terms nearly cancel in the uniform-[pressure](../../../../../../pressure.md) regime.

For the inner flow, the leading axial [pressure](../../../../../../pressure.md) is uniform across a section. Neglect the much smaller interfacial axial [velocity](../../../../../../velocity.md) relative to the internal [pressure](../../../../../../pressure.md)-driven motion. The [lubrication approximation](../../../../../../lubrication-theory.md) solves $\lambda\mu r^{-1}(ru_{z,r})_r=P_z$, with regularity at zero and $u_z(a)=0$ at leading order. Thus

$$
u_z=\frac{P_z}{4\lambda\mu}(r^2-a^2),\qquad Q=2\pi\int_0^a ru_z\,dr=-\frac{\pi a^4}{8\lambda\mu}P_z.
$$

The area balance $(\pi a^2)_t+Q_z=0$, combined with the exterior normal-stress relation, gives the [lubrication equation for a bubble with viscous exterior](../../../../../../lubrication-equation-for-a-bubble-with-viscous-exterior.md):

$$
\boxed{2aa_t=\frac1{8\lambda\mu}\partial_z\left[a^4\partial_z\left(\frac{2\mu a_t}a+\frac\gamma a\right)\right].}
$$

The neglected inner viscous [normal stress](../../../../../../normal-stress.md) is smaller by $\lambda$ in the similarity scales obtained next; the external axial interfacial speed is likewise smaller than the large [pressure](../../../../../../pressure.md)-driven inner speed.

Put $\tau=t_*-t$, $a\sim\tau^p$ and axial length $\ell\sim\tau^q$. The radial viscous [normal stress](../../../../../../normal-stress.md) scales as $\mu a_t/a\sim\tau^{-1}$ and capillary [pressure](../../../../../../pressure.md) as $\gamma/a\sim\tau^{-p}$. Retaining both requires $p=1$. The left side $aa_t$ scales as $\tau^{2p-1}$, while the axial-flux divergence scales as $a^4P/\ell^2\sim\tau^{4p-1-2q}$. Equating them gives $q=p=1$. Thus **both local radius and axial length shrink linearly in the remaining time**.

To obtain the specified dimensionless coefficients, choose the [linear pinch-off scaling of a slender viscous bubble](../../../../../../linear-pinch-off-scaling-of-a-slender-viscous-bubble.md)

$$
\boxed{a(z,t)=\frac\gamma\mu\tau A(\zeta),\qquad\zeta=\frac{\mu\sqrt\lambda(z-z_*)}{\gamma\tau}.}
$$

Then $a_t=(\gamma/\mu)(\zeta A'-A)$ and

$$
P=\frac\mu\tau\left[\frac{2\zeta A'+1}{A}-2\right].
$$

The constant $-2$ has no axial derivative. Substituting into the flux equation and cancelling its dimensional factor gives

$$
\boxed{\zeta AA'-A^2=\frac1{16}\left\{A^4\left[\frac{2\zeta A'+1}{A}\right]'\right\}'.}
$$

Both axial derivatives on the right are essential; the outer derivative is present in the PDF but lost in the converted TeX expression. The physical slope is $a_z=\sqrt\lambda A'$, so an order-one similarity profile remains slender for $\lambda\ll1$. No solution of this similarity ordinary differential equation is required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
