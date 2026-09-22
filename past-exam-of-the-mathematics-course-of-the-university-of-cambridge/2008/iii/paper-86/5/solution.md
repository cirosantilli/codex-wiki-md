<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $\rho$ be the liquid density and neglect atmospheric shear. The shallow-channel [lubrication approximation](../../../../../lubrication-theory.md) makes the surface nearly horizontal in each cross-section, at $z=h(x,t)$, with [hydrostatic pressure](../../../../../hydrostatic-pressure.md) $p=p_{\rm atm}+\rho g(h-z)$. At fixed $y$, the floor is $z_b=\alpha|y|$ and the local liquid thickness is $H_y=h-z_b$. Axial [momentum](../../../../../momentum.md) and [boundary conditions](../../../../../boundary-condition.md) are

$$
\mu u_{zz}=\rho g h_x,\qquad u(z_b)=0,\qquad u_z(h)=0.
$$

Writing $\zeta=z-z_b$, [integration](../../../../../integral.md) gives

$$
u=-\frac{\rho gh_x}{2\mu}(2H_y\zeta-\zeta^2),\qquad q(y)=\int_{z_b}^h u\,dz=-\frac{\rho g}{3\mu}H_y^3h_x.
$$

The wetted interval is $|y|<h/\alpha$. Its cross-sectional area and total axial flux are

$$
A=2\int_0^{h/\alpha}(h-\alpha y)dy=\frac{h^2}{\alpha},\qquad Q=-\frac{2\rho gh_x}{3\mu}\int_0^{h/\alpha}(h-\alpha y)^3dy=-\frac{\rho g}{6\mu\alpha}h^4h_x.
$$

The [shallow V-channel lubrication flux](../../../../../shallow-v-channel-lubrication-flux.md) and [volume conservation](../../../../../volume-conservation.md) $A_t+Q_x=0$ therefore give

$$
\boxed{(h^2)_t=C(h^4h_x)_x,\qquad C=\frac{\rho g}{6\mu},\qquad\frac1\alpha\int_{\mathbb R}h^2dx=V.}
$$

The slope $\alpha\ll1$ makes transverse shear small relative to vertical shear; the longitudinal current must also be slender for this reduction.

For typical height $H$ and axial length $L$, fixed volume gives $H^2L\sim\alpha V$, while the equation gives $L^2\sim CH^3t$. Eliminating either scale yields

$$
\boxed{H\sim\left(\frac{\alpha^2V^2}{Ct}\right)^{1/7},\qquad L\sim(Ct)^{2/7}(\alpha V)^{3/7}.}
$$

Thus the current grows in length like $t^{2/7}$ and thins like $t^{-1/7}$. Equivalently, the [porous-medium transformation of V-channel spreading](../../../../../porous-medium-transformation-of-v-channel-spreading.md) sets $w=h^2$ and gives $w_t=(C/5)(w^{5/2})_{xx}$ with constant mass $\alpha V$.

Seek a symmetric solution $h=t^{-1/7}f(\xi)$ with $\xi=x/t^{2/7}$. Substitution into the conservative depth equation gives

$$
-\frac27 f^2-\frac27\xi(f^2)'=C(f^4f')'.
$$

The left side is $-(2/7)(\xi f^2)'$. [Symmetry](../../../../../symmetry-physics.md) sets the [integration](../../../../../integral.md) constant to zero, so $Cf^4f'=-(2/7)\xi f^2$ within the [support](../../../../../support.md). Integrating $f^2f'=-2\xi/(7C)$ gives $f^3=3(\xi_0^2-\xi^2)/(7C)$. In physical variables the [constant-volume similarity in a V-shaped channel](../../../../../constant-volume-similarity-in-a-v-shaped-channel.md) is

$$
\boxed{h(x,t)=\left[\frac{3(X(t)^2-x^2)}{7Ct}\right]_+^{1/3},}
$$

where $X(t)$ is the half-length of its [support](../../../../../support.md) and the [positive part](../../../../../positive-part-of-a-real-valued-function.md) makes $h=0$ outside it.

Define the positive normalization

$$
J=\int_{-1}^1(1-s^2)^{2/3}ds=\int_0^\pi\sin^{7/3}\theta\,d\theta=\frac{\sqrt\pi\,\Gamma(5/3)}{\Gamma(13/6)}.
$$

The first substitution is $s=\cos\theta$; the gamma form follows from the [beta function](../../../../../beta-function.md) [integral](../../../../../integral.md). Conservation of volume now gives

$$
\alpha V=\left(\frac3{7Ct}\right)^{2/3}X^{7/3}J,
$$

and consequently

$$
\boxed{X(t)=\left(\frac{\alpha V}{J}\right)^{3/7}\left(\frac{7Ct}{3}\right)^{2/7},\qquad h(0,t)=\left(\frac{\alpha V}{J}\right)^{2/7}\left(\frac3{7Ct}\right)^{1/7}.}
$$

The full current length is $2X(t)$. Its flux vanishes at the two noses, since the integrated similarity equation gives $Ch^4h_x=-2xh^2/(7t)$ there, so no volume is lost at the [support](../../../../../support.md) boundary. A shifted origin or a positive shift of time gives the corresponding translated similarity family.

In an intended trigonometric $I(\beta)$ notation, $J=I(7/3)$ requires either cosine integrated over $[-\pi/2,\pi/2]$ or absolute cosine over $[0,\pi]$. The printed $\cos^\beta\theta$ on $[0,\pi]$ is not a positive real normalization for the required fractional exponent: with a real cube-root interpretation at $\beta=7/3$, its two halves cancel, while the principal complex power is not real. **The similarity normalization uses the positive sine [integral](../../../../../integral.md) $J$ above.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
