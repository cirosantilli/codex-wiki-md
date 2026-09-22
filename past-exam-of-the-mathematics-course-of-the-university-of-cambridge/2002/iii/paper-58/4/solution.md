<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Near a spatially extended [Hopf bifurcation](../../../../../hopf-bifurcation.md), a critical oscillatory [normal mode](../../../../../normal-mode.md) has a slowly varying complex amplitude. For a selected travelling-wave branch, a [method of multiple scales](../../../../../method-of-multiple-scales.md) expansion takes the form

$$
u(x,t)=\varepsilon\{A(X,T)v_0e^{i(k_0x-\omega_0t)}+\text{complex conjugate}\}+O(\varepsilon^2),\qquad
X=\varepsilon(x-v_gt),\quad T=\varepsilon^2t.
$$

Here the distance from onset is of order $\varepsilon^2$, $v_0$ is the critical [eigenvector](../../../../../eigenvector.md), and $v_g$ is the [group velocity](../../../../../group-velocity.md). The comoving coordinate removes the first spatial derivative of the envelope. Projection at the first resonant order gives $A_T=\rho A+D_0A_{XX}-G_0|A|^2A$. Spatial translation and the temporal phase of the Hopf oscillation give a constant-phase [symmetry](../../../../../symmetry-physics.md) $A\mapsto e^{i\theta}A$, which permits the cubic term $|A|^2A$ but forbids a generic $A^2$ term. The coefficients are complex because the envelope has both growth and frequency detuning. For a supercritical branch with positive real diffusion, real rescalings and a uniform phase rotation give the [complex Ginzburg–Landau equation](../../../../../complex-ginzburg-landau-equation.md)

$$
\boxed{A_T=A+(1+ib)A_{XX}-(1+ic)|A|^2A,\qquad b,c\in\mathbb R.}
$$

A subcritical Hopf branch requires higher saturation terms instead. If spatial reflection makes opposite travelling waves critical together, two coupled [amplitude equations](../../../../../amplitude-equation.md) are required initially; the scalar equation applies to a selected single-wave branch when its competing amplitude is stable.

Distant boundaries can still determine which travelling pattern is observed. They can select its phase and [wavenumber](../../../../../wavenumber.md), reflect a travelling disturbance, inject a competing wave, or let a growing wave packet leave the domain. In particular, amplification in a comoving frame can be [convective wave-packet instability](../../../../../convective-wave-packet-instability.md) rather than [absolute wave-packet instability](../../../../../absolute-wave-packet-instability.md) at a fixed laboratory point. A finite-domain outcome then need not reflect intrinsic bulk modulation dynamics. [Periodic boundary conditions](../../../../../periodic-boundary-conditions.md) are the appropriate idealization when studying bulk instabilities without end selection or reflected-wave forcing: they eliminate physical end layers and make the allowed envelope [Fourier modes](../../../../../fourier-mode.md) discrete. They do not assert that real distant boundaries are always negligible. Choose a periodic length compatible with the carrier, fix the phase winding, and compare perturbations within that same periodic problem. On an open physical domain the group velocity and actual boundary conditions must be restored.

The optimum carrier [wavenumber](../../../../../wavenumber.md) corresponds to the spatially uniform envelope $A_f=e^{-icT}$, often called a flat state. Its phase is arbitrary. Write $A=e^{-icT}(1+r)e^{i\phi}$ with real small amplitude and phase disturbances. To first order,

$$
r_T=-2r+r_{XX}-b\phi_{XX},\qquad
\phi_T=-2cr+\phi_{XX}+br_{XX}.
$$

A [Fourier mode](../../../../../fourier-mode.md) $e^{\lambda T+ikX}$ therefore has matrix and [dispersion relation](../../../../../dispersion-relation.md)

$$
M(k)=\begin{pmatrix}-2-k^2&bk^2\\-2c-bk^2&-k^2\end{pmatrix},\qquad
\lambda^2+(2+2k^2)\lambda+2(1+bc)k^2+(1+b^2)k^4=0.
$$

The trace is negative. The amplitude mode at $k=0$ has [eigenvalue](../../../../../eigenvalue.md) $-2$, while the phase mode is neutral because constant phase shifts preserve the solution. Put $D=1+bc$. For every nonzero real $k$, the determinant is positive if $D\ge0$, whereas $D<0$ makes it negative for $0<k^2<-2D/(1+b^2)$. Thus

$$
\boxed{1+bc>0:\ \text{flat state stable modulo phase};\qquad
1+bc<0:\ \text{long-wave modulational instability}.}
$$

This is the [Benjamin-Feir stability condition](../../../../../benjamin-feir-stability-condition.md). At $D=0$, nonzero modes still decay, but the leading long-wave decay is fourth order rather than diffusive. On a periodic envelope interval of length $L$, the smallest nonzero [wavenumber](../../../../../wavenumber.md) is $2\pi/L$, so strict stability of all allowed nonzero modes requires

$$
2D+(1+b^2)(2\pi/L)^2>0.
$$

A sufficiently short periodic domain can therefore exclude the unstable band even when the infinite-domain [Benjamin-Feir stability condition](../../../../../benjamin-feir-stability-condition.md) fails.

The amplitude is damped while the phase is slow. For a slowly varying phase, the leading slaved amplitude is $r=-\tfrac12\{b\phi_{XX}+(\phi_X)^2\}+\cdots$. Substitution in the phase equation gives the diffusion term $D\phi_{XX}$ and the nonlinear frequency shift $(c-b)(\phi_X)^2$. The latter also follows directly from a constant phase gradient: an envelope with gradient $q$ has amplitude squared $1-q^2$ and frequency $c+(b-c)q^2$. Constant phase [symmetry](../../../../../symmetry-physics.md) rules out undifferentiated $\phi$; translation invariance gives constant coefficients. The leading comoving Ginzburg-Landau equation also has spatial parity, so odd linear derivatives are absent at this order. Its neutral phase [eigenvalue](../../../../../eigenvalue.md) expands as

$$
\lambda_{\rm phase}(k)=-Dk^2-Ek^4+O(k^6),\qquad
E=\frac{b^2(1+c^2)}2.
$$

This coefficient follows by inserting a power series for $\lambda$ in the quadratic [dispersion relation](../../../../../dispersion-relation.md). Close to $D=0$, it becomes $E=(1+b^2)/2>0$ at leading order. The [long-wave phase reduction of the complex Ginzburg-Landau equation](../../../../../long-wave-phase-reduction-of-the-complex-ginzburg-landau-equation.md) is consequently

$$
\phi_T=D\phi_{XX}-E\phi_{XXXX}+g(\phi_X)^2+\cdots,\qquad g=c-b.
$$

The fourth derivative regularizes negative phase diffusion. Terms omitted here have higher order in the long-wave expansion. First-order advection has been removed by the group-velocity frame; higher odd derivatives in a more general travelling-wave problem are beyond this leading amplitude approximation.

Take $D=-d$ with $d>0$ small. At the instability boundary $c=-1/b$, so $g=-(1+b^2)/b$ is nonzero. Set $\xi=\sqrt{d/E}\,X$, $\tau=d^2T/E$, and $\phi=(d/g)\Phi$. At leading order the phase dynamics become the potential [Kuramoto-Sivashinsky equation](../../../../../kuramoto-sivashinsky-equation.md),

$$
\Phi_\tau=-\Phi_{\xi\xi}-\Phi_{\xi\xi\xi\xi}+(\Phi_\xi)^2.
$$

With $u=-2\Phi_\xi$ this is

$$
\boxed{u_\tau+uu_\xi+u_{\xi\xi}+u_{\xi\xi\xi\xi}=0.}
$$

The variable $u$ is a phase-gradient disturbance, not the original physical field. Periodicity of the phase fixes $\int_0^P u\,d\xi=0$ for the zero-winding branch; the [Kuramoto-Sivashinsky equation](../../../../../kuramoto-sivashinsky-equation.md) conserves this mean. The scaled period is $P=L\sqrt{d/E}$.

At fixed period $P$, the flat phase has growth rates $\lambda_n=k_n^2-k_n^4$, $k_n=2\pi n/P$. Its first loss of stability occurs at $P=2\pi$. To find what replaces it, put $k=2\pi/P$ and consider $P$ just above $2\pi$. After choosing an origin by translation, expand a small steady modulation as $u=a\sin(k\xi)+b_2\sin(2k\xi)+\cdots$. Projection of $-uu_\xi$ onto the first two harmonics yields

$$
\dot a=\lambda_1a+\frac{k}{2}ab_2+\cdots,\qquad
\dot b_2=\lambda_2b_2-\frac{k}{2}a^2+\cdots,
\qquad \lambda_j=(jk)^2-(jk)^4.
$$

Since $\lambda_2=-12$ at onset, this harmonic is slaved to $b_2=ka^2/(2\lambda_2)+\cdots$. The fundamental amplitude obeys

$$
\dot a=\lambda_1a+\frac{k^2}{4\lambda_2}a^3+\cdots
=\lambda_1a-\frac{a^3}{48}+\cdots\quad(k\simeq1).
$$

The [primary periodic bifurcation of the Kuramoto-Sivashinsky equation](../../../../../primary-periodic-bifurcation-of-the-kuramoto-sivashinsky-equation.md) is therefore supercritical. For $0<P-2\pi\ll1$,

$$
\boxed{a^2=-\frac{4\lambda_1\lambda_2}{k^2}+O(\lambda_1^2),\qquad
b_2=\frac{ka^2}{2\lambda_2}+O(a^4).}
$$

The radial [eigenvalue](../../../../../eigenvalue.md) of this nonzero branch is $-2\lambda_1+O(\lambda_1^2)<0$; all higher harmonics remain damped and the modulation's spatial phase is neutral. Thus the small finite-amplitude modulation is stable in the sense of [orbital stability](../../../../../orbital-stability.md), at fixed mean and fixed period, despite the flat state's instability. The two signs of $a$ represent translations of the same modulation. In the potential formulation the spatial mean of $\Phi$ advances at $\langle(\Phi_\xi)^2\rangle$: the original wave acquires a nonlinear frequency correction rather than requiring a time-independent absolute phase.

For larger $P$, further linear modes become active and the small-amplitude argument no longer determines stability. A periodic modulation $\bar u$ must then be tested with the operator $v_\tau=-v_{\xi\xi}-v_{\xi\xi\xi\xi}-\partial_\xi(\bar u v)$ on mean-zero periodic disturbances. Its translation mode is always neutral, and secondary oscillatory or more complicated modulation can occur. Moreover, stability against perturbations of the same period does not prove stability against disturbances of a larger period; those require a separate sideband or [Floquet theory](../../../../../floquet-theory.md) calculation. The controlled conclusion near the first threshold is the existence of a stable small modulation family, not universal stability of all periodic Kuramoto-Sivashinsky solutions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
