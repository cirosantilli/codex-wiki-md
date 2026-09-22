<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The three contributions to the [Frank elastic energy](../../../../../distortion-free-energy-density.md) penalize distinct slow distortions of the [nematic director](../../../../../nematic-director.md). [Nematic splay](../../../../../nematic-splay.md) measures local spreading or convergence and is governed by $K_1(\nabla\cdot\mathbf n)^2/2$. [Nematic twist](../../../../../nematic-twist.md) measures rotation around an axis perpendicular to the director, with cost $K_2(\mathbf n\cdot\nabla\times\mathbf n)^2/2$. [Nematic bend](../../../../../nematic-bend.md) measures curvature of director integral lines; for a unit vector, $(\mathbf n\cdot\nabla)\mathbf n=-\mathbf n\times(\nabla\times\mathbf n)$, giving cost $K_3|\mathbf n\times\nabla\times\mathbf n|^2/2$. These terms respect the head-tail symmetry of a [nematic liquid crystal](../../../../../nematic-liquid-crystal.md). Positive elastic constants oppose these distortions.

For the one-dimensional reduction assume lateral uniformity, so $\theta$ and $\phi$ depend only on $z$. A prime below means $d/dz$. Directly differentiating the [nematic director](../../../../../nematic-director.md) gives

$$
\nabla\cdot\mathbf n=\cos\theta\,\theta',\qquad \nabla\times\mathbf n=(-n_y',n_x',0),\qquad \mathbf n\cdot\nabla\times\mathbf n=-\cos^2\theta\,\phi'.
$$

The squared [curl](../../../../../curl.md) is $\sin^2\theta\,\theta'^2+\cos^2\theta\,\phi'^2$. Subtracting the squared twist invariant gives

$$
|\mathbf n\times\nabla\times\mathbf n|^2=\sin^2\theta\,\theta'^2+\sin^2\theta\cos^2\theta\,\phi'^2.
$$

Consequently the [one-dimensional twisted nematic energy](../../../../../one-dimensional-twisted-nematic-energy.md) has elastic coefficients

$$
\boxed{f(\theta)=K_1\cos^2\theta+K_3\sin^2\theta,\qquad g(\theta)=K_2\cos^4\theta+K_3\sin^2\theta\cos^2\theta.}
$$

A normal [electric field](../../../../../electric-field.md) has $\mathbf E\cdot\mathbf n=E_0\sin\theta$. There is a genuine factor-of-two inconsistency in the source: its initial functional places the electric term inside the overall factor $1/2$, whereas its subsequent density and threshold use the full electric term. For the requested density and threshold, use the usual orientational coupling $-\epsilon E_0^2\sin^2\theta/(8\pi)$. Here $\epsilon$ is the [dielectric anisotropy of a nematic](../../../../../dielectric-anisotropy-of-a-nematic.md), in the printed Gaussian-unit convention. If the first functional is instead read literally, this coupling is halved and the resulting threshold voltage is multiplied by $\sqrt2$.

Put $c=\epsilon E_0^2/(8\pi)$ and $\mathcal L=f\theta'^2/2+g\phi'^2/2-c\sin^2\theta$. Apply the [Euler-Lagrange equations for two fields](../../../../../euler-lagrange-equations-for-two-fields.md). Variation in $\phi$, which does not appear explicitly, gives

$$
\boxed{(g(\theta)\phi')'=0.}
$$

Variation in $\theta$ gives $(f\theta')'-f_\theta\theta'^2/2-g_\theta\phi'^2/2+2c\sin\theta\cos\theta=0$, or

$$
\boxed{f\theta''+\frac12f_\theta\theta'^2-\frac12g_\theta\phi'^2+\frac{\epsilon E_0^2}{4\pi}\sin\theta\cos\theta=0.}
$$

At $\theta=0$, $f=K_1$, $g=K_2$, and $f_\theta=g_\theta=0$. With zero field, $\theta'=0$ and $\phi'=\pi/(2L)$ satisfy both equations and the imposed azimuthal endpoints. Thus the quarter-turn planar texture is a stationary solution. Stationarity alone is not a claim of stability for arbitrary elastic constants.

To find the [Fréedericksz transition](../../../../../freedericksz-transition.md), impose the additional strong planar anchoring $\theta(0)=\theta(L)=0$. Write $\alpha=\pi/(2L)$. The small-angle expansions are

$$
f=K_1+(K_3-K_1)\theta^2+O(\theta^4),\qquad g=K_2+(K_3-2K_2)\theta^2+O(\theta^4).
$$

The conserved $g\phi'$ and fixed total twist imply $\phi'=\alpha+O(\theta^2)$ for a pure tilt perturbation. Linearizing the tilt [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) therefore gives

$$
K_1\theta''+\left[\frac{\epsilon E_0^2}{4\pi}-(K_3-2K_2)\alpha^2\right]\theta=0.
$$

Substitute $\theta=\theta_0\sin(\pi z/L)$. A nonzero neutral amplitude requires

$$
\frac{\epsilon E_c^2}{4\pi}=\frac{\pi^2}{L^2}\left[K_1+\frac{K_3-2K_2}{4}\right].
$$

Since $V_c=E_cL$, the [quarter-turn nematic instability threshold](../../../../../quarter-turn-nematic-instability-threshold.md) is

$$
\boxed{V_c=2\pi^{3/2}\sqrt{K_1+\frac14(K_3-2K_2)}\,\epsilon^{-1/2}.}
$$

This is the first zero-endpoint mode: higher sine modes replace $K_1$ by $n^2K_1$ and cost more elastic energy. The quadratic energy change is $\frac12\int[K_1\theta'^2+\{(K_3-2K_2)\alpha^2-\epsilon E_0^2/(4\pi)\}\theta^2]dz$, so the first mode has negative stiffness above this voltage. The result assumes $\epsilon>0$ and $K_1+(K_3-2K_2)/4>0$. If the latter is negative the planar state is already unstable at zero field; for negative [dielectric anisotropy of a nematic](../../../../../dielectric-anisotropy-of-a-nematic.md), a normal field opposes this tilt. The literal initial electric prefactor would give $V_{c,\mathrm{literal}}=\sqrt2V_c$.

For reflective operation of the [twisted nematic field effect](../../../../../twisted-nematic-field-effect.md), orient each [polarizer](../../../../../polarizer.md)'s transmission axis along the adjacent planar [nematic director](../../../../../nematic-director.md). Light entering through the top [polarizer](../../../../../polarizer.md) initially has $y$ [linear polarization](../../../../../linear-polarization.md). At low voltage, [adiabatic optical following in a twisted nematic](../../../../../adiabatic-optical-following-in-a-twisted-nematic.md) rotates it through a quarter turn to $x$ as it travels downward, so it passes the bottom [polarizer](../../../../../polarizer.md) and reaches the mirror. On returning, it follows the reverse twist back to $y$ and exits the top [polarizer](../../../../../polarizer.md): the pixel appears bright. At sufficiently high voltage, positive [dielectric anisotropy of a nematic](../../../../../dielectric-anisotropy-of-a-nematic.md) aligns most of the director with the normal field. The bulk no longer produces the quarter-turn optical rotation, so the crossed bottom [polarizer](../../../../../polarizer.md) blocks the incident light and the pixel appears dark. Elastic relaxation restores the bright twisted state after voltage is removed. The adiabatic requirement is more precisely $2\pi|\Delta n|/\lambda\gg|\phi'|$, involving [birefringence](../../../../../birefringence.md), not thickness alone. **Voltage switches director orientation and hence the reflected brightness; it does not require the liquid crystal to emit light.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
