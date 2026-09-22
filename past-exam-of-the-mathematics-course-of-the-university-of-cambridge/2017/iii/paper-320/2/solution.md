<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume a time-independent spherical [relative potential](../../../../../relative-potential.md) $\psi(r)$, with [acceleration](../../../../../acceleration.md) $\nabla\psi$. The [relative energy](../../../../../relative-energy.md) and specific [angular momentum](../../../../../angular-momentum.md) are

$$
E=\psi-\frac12v^2,\qquad\boldsymbol\ell=\mathbf r\times\mathbf v,\qquad L=|\boldsymbol\ell|.
$$

Along an [orbit](../../../../../orbit-dynamical-system.md), $\dot E=\nabla\psi\cdot\mathbf v-\mathbf v\cdot\nabla\psi=0$ and $\dot{\boldsymbol\ell}=\mathbf r\times\nabla\psi=0$, since a spherical [gradient](../../../../../gradient.md) is radial. Thus both $E$ and $L$ are [integrals of motion](../../../../../integral-of-motion.md). Choose the escape level $\psi=0$ and take the bound [galactic distribution function](../../../../../galactic-distribution-function.md) to vanish for $E\leq0$.

For an isotropic $f(E)$, integrate over a [spherical coordinate system](../../../../../spherical-coordinate-system.md) in [velocity](../../../../../velocity.md) space:

$$
\rho(\psi)=4\pi\int_0^{\sqrt{2\psi}}v^2f(\psi-v^2/2)\,dv=4\pi\sqrt2\int_0^\psi f(E)\sqrt{\psi-E}\,dE.
$$

Differentiating gives $\rho'(\psi)=2\pi\sqrt2\int_0^\psi f(E)/\sqrt{\psi-E}\,dE$. Convolve once more with the reciprocal-square-root kernel. Reversing the order of [integration](../../../../../integral.md), under the usual integrability assumptions, uses

$$
\int_E^{E_0}\frac{d\psi}{\sqrt{\psi-E}\sqrt{E_0-\psi}}=\pi.
$$

Therefore $\int_0^{E_0}\rho'(\psi)/\sqrt{E_0-\psi}\,d\psi=2\sqrt2\pi^2\int_0^{E_0}f(E)\,dE$. Differentiating proves [Eddington inversion](../../../../../eddington-inversion.md):

$$
\boxed{f(E)=\frac1{\sqrt8\,\pi^2}\frac d{dE}\int_0^E\frac{\rho'(\psi)}{\sqrt{E-\psi}}\,d\psi.}
$$

Here $\pi^2$ is outside the square root, as in the original PDF; the TeX transcription wrongly places it inside. The assumptions include a locally integrable bound distribution and sufficient density regularity, with no extra unbound or boundary population. An inverted expression must additionally be nonnegative to be physical. Since the [velocity](../../../../../velocity.md) measure and $f$ are invariant under all [velocity](../../../../../velocity.md) rotations, $\langle v_r^2\rangle=\langle v_\theta^2\rangle=\langle v_\phi^2\rangle=\langle v^2\rangle/3$ whenever these moments exist; mixed moments vanish.

For the [half-anisotropic distribution function](../../../../../half-anisotropic-distribution-function.md), write the polar [velocity](../../../../../velocity.md) angle from the radial direction as $\eta$. Then $L=rv\sin\eta$, and

$$
f\,d^3v=\frac1r f_E(\psi-v^2/2)v\,dv\,d\eta\,d\varphi.
$$

The apparent $1/L$ singularity is integrable because it cancels the factor $v\sin\eta$ in the [velocity](../../../../../velocity.md) measure. Integrating $\eta\in[0,\pi]$ and $\varphi\in[0,2\pi]$ gives

$$
r\rho=2\pi^2\int_0^\psi f_E(E)\,dE,\qquad\boxed{f_E(E)=\left.\frac1{2\pi^2}\frac{d(r\rho)}{d\psi}\right|_{\psi=E}.}
$$

The density relation requires $r\rho\to0$ at the escape boundary and $f_E\geq0$ for a physical distribution. Consider a monotonically decreasing $\psi$. The largest allowed radius at fixed binding [energy](../../../../../energy.md) is the radial-orbit limit $r_E$ with $\psi(r_E)=E$; a nonzero-$L$ [orbit](../../../../../orbit-dynamical-system.md) normally has a smaller apocenter because of its centrifugal term. Changing from $\psi$ to $r$ gives

$$
\boxed{f(E,L)=\frac{g(r_E)}{2\pi^2L},\qquad g(r)=\frac{\rho(r)+r\rho'(r)}{\psi'(r)}.}
$$

The numerator in the original PDF instead uses $\rho+d\rho/d\psi$. That is a genuine printed error: the [chain rule](../../../../../chain-rule.md) for $d(r\rho)/d\psi$ requires $\rho+r\,d\rho/dr$. It is not legitimate to prove the printed expression as written. A concrete counterexample is the unit-parameter [Hernquist model](../../../../../hernquist-model.md) at $r=1$: $\psi'= -1/4$, $\rho'=-(5/2)\rho$ and $d\rho/d\psi=10\rho$. The printed quotient is $-44\rho$, whereas the correct $g$ is $6\rho>0$. The former would give a negative distribution.

The angular weight after cancellation is uniform in $\eta$, so the averages of $\cos^2\eta$ and $\sin^2\eta$ are both $1/2$. The azimuthal angle splits the tangential term equally. Hence $\langle v_r^2\rangle=\langle v_\theta^2+v_\phi^2\rangle$ and each individual tangential moment is half the radial one. The [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) is consequently

$$
\boxed{\beta=\frac12.}
$$

This is a radially biased [constant-anisotropy distribution function](../../../../../constant-anisotropy-distribution-function.md), not an isotropic one or purely radial motion. It does not by itself prove dynamical stability; it preferentially weights small [angular momentum](../../../../../angular-momentum.md) while remaining integrable.

For the [Hernquist model](../../../../../hernquist-model.md), use the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) with the relative-potential sign, $\nabla^2\psi=-4\pi G\rho$. Since $\psi'=-GM/(r+a)^2$,

$$
\boxed{\rho(r)=-\frac1{4\pi Gr^2}\frac d{dr}(r^2\psi')=\frac{Ma}{2\pi r(r+a)^3}.}
$$

Its enclosed [mass](../../../../../mass.md) is $Mr^2/(r+a)^2$, which tends to $M$. Expressing the augmented density in the [relative potential](../../../../../relative-potential.md) gives $r\rho=a\psi^3/(2\pi G^3M^2)$. The preceding [derivative](../../../../../derivative.md) therefore gives

$$
\boxed{f(E,L)=\frac{3aE^2}{4\pi^3G^3M^2L},\qquad0<E<GM/a,}
$$

with zero bound-model population outside the allowed [energy](../../../../../energy.md) domain. It is nonnegative and reproduces the density by direct [integration](../../../../../integral.md). The [Hernquist model](../../../../../hernquist-model.md) has a central density cusp, so the formulas for the local $1/L$ distribution are interpreted at $r>0$. As a further check, the radial [second moment](../../../../../second-moment.md) obtained from the same [integral](../../../../../integral.md) is $\psi/4$ and each tangential [second moment](../../../../../second-moment.md) is $\psi/8$, consistent with $\beta=1/2$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 320](../../paper-320-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
