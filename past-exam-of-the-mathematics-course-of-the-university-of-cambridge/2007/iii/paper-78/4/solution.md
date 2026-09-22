<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose transverse $x$ along the cusp from the line of cylinder contact, and $y$ across its narrow gap. Expanding the two circular boundaries for $x\ll a$ gives $y=\pm x^2/(2a)$, so the local full gap is $d(x)=x^2/a$. At the meniscus, $x\simeq w$, a semicircle fits across this gap with radius $d(w)/2=w^2/(2a)$. Thus the leading area and transverse curvature in the [cusp flow between touching cylinders](../../../../../cusp-flow-between-touching-cylinders.md) are

$$
\boxed{\mathcal A=\int_0^w\frac{x^2}a\,dx=\frac{w^3}{3a},\qquad\kappa=\frac{2a}{w^2}.}
$$

The meniscus area correction is $O(w^4/a^2)$ and is small relative to $w^3/a$. The curvature is stated as a positive suction magnitude; the liquid [pressure](../../../../../pressure.md) relative to air is $p=-2\gamma a/w^2$. Axial curvature is negligible compared with this transverse curvature under the slow-variation approximation.

At fixed $x$, axial [lubrication theory](../../../../../lubrication-theory.md) gives a local slit [Poiseuille flow](../../../../../hagen-poiseuille-equation.md) between rigid walls $y=\pm d/2$:

$$
u_z=\frac{p_z}{2\mu}\left(y^2-\frac{d^2}4\right),\qquad
\int_{-d/2}^{d/2}u_z\,dy=-\frac{d^3}{12\mu}p_z.
$$

Integrating across the cusp gives

$$
Q=-\frac{p_z}{12\mu a^3}\int_0^wx^6dx=-\frac{w^7}{84\mu a^3}p_z.
$$

The local meniscus edge correction occupies a transverse width small compared with $w$ and does not change this leading flux. Since $p_z=4\gamma a w^{-3}w_z$, the axial [volume flux](../../../../../volumetric-flow-rate.md) is $Q=-\gamma w^4w_z/(21\mu a^2)$. Area conservation $\mathcal A_t+Q_z=0$ now gives

$$
\boxed{(w^3)_t=\frac\gamma{7\mu a}(w^4w_z)_z.}
$$

Writing $u=w^3$ also puts this in [porous medium equation](../../../../../porous-medium-equation.md) form $u_t=\gamma(u^{5/3})_{zz}/(35\mu a)$, explaining the finite-support spreading profile.

Set $K=\gamma/(7\mu a)$. Fixed volume means $\int w^3dz=3aV$. If $w\propto t^{-\beta}$ and axial extent is proportional to $t^\alpha$, this conservation gives $\alpha=3\beta$. The evolution equation gives $3\beta+1=5\beta+2\alpha$, hence **$\beta=1/8$, $\alpha=3/8$**.

For the symmetric source-type [similarity solution](../../../../../similarity-solution.md), write $w=t^{-1/8}f(\eta)$, $\eta=z/t^{3/8}$. The differential equation becomes

$$
-\frac38(f^3+\eta(f^3)')=K(f^4f')'.
$$

Integrate from the centre using zero flux and symmetry. This gives $Kf^4f'=-3\eta f^3/8$, so on the positive support $ff'=-3\eta/(8K)$. With $f(\eta_N)=0$,

$$
f^2=\frac3{8K}(\eta_N^2-\eta^2).
$$

Therefore the [fixed-volume capillary spreading in a cylindrical cusp](../../../../../fixed-volume-capillary-spreading-in-a-cylindrical-cusp.md) profile is

$$
\boxed{w(z,t)=\left[\frac{21\mu a}{8\gamma t}(z_N(t)^2-z^2)\right]_+^{1/2}.}
$$

Let $B=21\mu a/(8\gamma t)$. Its volume is

$$
V=\frac1{3a}\int_{-z_N}^{z_N}w^3dz=\frac{B^{3/2}z_N^4}{3a}\int_{-1}^1(1-s^2)^{3/2}ds.
$$

With $s=\sin\theta$, the last integral is $\int_{-\pi/2}^{\pi/2}\cos^4\theta\,d\theta=3\pi/8$, equal to the supplied sine integral by symmetry. Consequently $V=\pi B^{3/2}z_N^4/(8a)$, yielding

$$
\boxed{z_N(t)=\left(\frac{8Va}\pi\right)^{1/4}\left(\frac{8\gamma t}{21\mu a}\right)^{3/8}.}
$$

The other tip is at $-z_N$. The maximum width decays as $t^{-1/8}$. This is the leading slender outer solution: the ideal point injection and the steep microscopic nose require local descriptions outside its uniform lubrication range.

Finally, for vertical cylinders let $\rho$ denote the liquid density, and take the bath [pressure](../../../../../pressure.md) at $z=0$ as the air-[pressure](../../../../../pressure.md) reference. At rest the liquid [pressure](../../../../../pressure.md) is $p(z)=-\rho gz$. Equating hydrostatic suction with the wetting-meniscus [capillary pressure](../../../../../capillary-pressure.md) gives the [hydrostatic rise in a cylindrical cusp](../../../../../hydrostatic-rise-in-a-cylindrical-cusp.md):

$$
\rho gz=\frac{2\gamma a}{w^2},\qquad\boxed{w(z)\sim\left(\frac{2\gamma a}{\rho gz}\right)^{1/2}\quad(z\text{ large}).}
$$

The cusp can therefore support an indefinitely high, increasingly narrow ideal wetting tail rather than a fixed terminal rise height. Large $z$ makes $w\ll a$ and strengthens the transverse cusp approximation, until microscopic physics limits the continuum description.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
