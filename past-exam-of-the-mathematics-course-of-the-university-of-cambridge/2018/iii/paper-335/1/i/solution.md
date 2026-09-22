<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [time-harmonic wave](../../../../../../time-harmonic-wave.md) convention $\psi e^{-i\omega t}$ and write $\mathbf z=(y,z)$, $E(0,\mathbf z)=E_0(\mathbf z)$, with a deterministic incident [wave envelope](../../../../../../envelope-waves.md). The printed speed ratio is inconsistent with $k=k_0n$: the [refractive index](../../../../../../refractive-index.md) used below is $n=c_0/c$. Substituting $\psi=e^{ik_0x}E$ in the [Helmholtz equation](../../../../../../helmholtz-equation.md) gives

$$
2ik_0\partial_xE+\partial_x^2E+\Delta_\perp E+k_0^2(n^2-1)E=0.
$$

The [paraxial approximation](../../../../../../paraxial-approximation.md) discards $\partial_x^2E$. The usual weak-fluctuation model also linearizes $n^2-1=2\mu W+O(\mu^2W^2)$, giving

$$
\partial_xE=(D+S_x)E,\qquad D=\frac{i}{2k_0}\Delta_\perp,\qquad S_x=ik_0\mu W(x,\mathbf z).
$$

Dropping the quadratic contrast is an additional weak-fluctuation assumption, not a consequence of small propagation angles. Although the linearized random potential generates attenuation of order $\mu^2$, it does not retain every effect of that order in the literal finite-correlation index: the discarded quadratic contrast can also produce a mean [wave phase](../../../../../../phase-waves.md) shift. This linearization must precede a [Gaussian white noise](../../../../../../gaussian-white-noise.md) limit: the square of ideal [white noise](../../../../../../white-noise.md) has no ordinary pointwise meaning.

The [split-step Fourier method](../../../../../../split-step-fourier-method.md) alternates [free-space diffraction](../../../../../../free-space-diffraction.md), $U_h=e^{hD}$, with a [random phase screen](../../../../../../random-phase-screen.md),

$$
E(x+h,\mathbf z)\simeq U_h\left[e^{i\phi_h(\mathbf z)}E(x,\mathbf z)\right],\qquad
\phi_h(\mathbf z)=k_0\mu\int_x^{x+h}W(s,\mathbf z)\,ds.
$$

For jointly [Gaussian random fields](../../../../../../gaussian-random-field.md), [Gaussian phase averaging](../../../../../../gaussian-phase-averaging.md) gives $\mathbb E e^{i\phi_h}=e^{-\operatorname{Var}(\phi_h)/2}$. More generally, a product of $p$ fields and $q$ conjugate fields picks up $\exp(i\sum_a\epsilon_a\phi_h(\mathbf z_a))$, with signs $\epsilon_a=+1$ or $-1$. Its screen average is determined entirely by the [wave phase](../../../../../../phase-waves.md) [covariance matrix](../../../../../../covariance-matrix.md). The deterministic [diffraction](../../../../../../diffraction.md) step acts on each coordinate, with opposite signs on factors formed by [complex conjugation](../../../../../../complex-conjugation.md). This is the basis of the field-moment equations.

There is an important closure qualification. A [stationary Gaussian random field](../../../../../../stationary-gaussian-random-field.md) need not have independent longitudinal increments. For finite-correlation fluctuations, the unlinearized [parabolic wave equation](../../../../../../parabolic-wave-equation.md) instead gives

$$
\partial_xm=Dm+ik_0\mu\,\mathbb E[WE]+\frac{ik_0\mu^2}{2}\mathbb E[W^2E].
$$

In the weak-fluctuation model, the exact first-moment equation is

$$
\partial_xm=Dm+ik_0\mu\,\mathbb E[WE],\qquad m=\mathbb E E.
$$

The last term cannot in general be replaced by a constant times $m$. An exact generic solution of the linearized model is

$$
m(x)=\mathbb E\left[\mathcal T\exp\left(\int_0^x(D+ik_0\mu W(s,\cdot))\,ds\right)\right]E_0,
$$

where $\mathcal T$ denotes [time ordering](../../../../../../time-ordering.md) of the propagation operators. For the unlinearized model, add $ik_0\mu^2W^2/2$ inside the propagation generator. The [covariance function](../../../../../../covariance-function.md) of the medium is needed to evaluate this expression; One-point [Gaussian distributions](../../../../../../normal-distribution.md) alone would not even determine the joint [wave phase](../../../../../../phase-waves.md) statistics.

For example, omit [diffraction](../../../../../../diffraction.md) and take a longitudinal [autocovariance function](../../../../../../autocovariance.md) $R(s)=\mathbb E[W(s,\mathbf z)W(0,\mathbf z)]$. Direct [Gaussian phase averaging](../../../../../../gaussian-phase-averaging.md) gives

$$
m(x,\mathbf z)=E_0(\mathbf z)\exp\left[-k_0^2\mu^2\int_0^x(x-s)R(s)\,ds\right],\qquad
\partial_xm=-k_0^2\mu^2\left(\int_0^xR(s)\,ds\right)m.
$$

Even here, unit-[variance](../../../../../../variance-split.md) [stationary Gaussian random fields](../../../../../../stationary-gaussian-random-field.md) with different $R$ give different answers. In the general problem the [diffraction](../../../../../../diffraction.md) and multiplication operators do not commute, so this scalar attenuation cannot simply be multiplied by $U_x$ without an additional approximation.

The standard closed answer uses the [Markov approximation for a random medium](../../../../../../markov-approximation-for-a-random-medium.md), made explicit in part ii. Let the longitudinally integrated [covariance kernel](../../../../../../covariance-kernel.md) be

$$
B(\mathbf r)=\int_{\mathbb R}\mathbb E[W(s,\mathbf z+\mathbf r)W(0,\mathbf z)]\,ds.
$$

Replace the medium by longitudinal [Gaussian white noise](../../../../../../gaussian-white-noise.md) with this strength. A screen of thickness $h$ then has $\mathbb E[\phi_h(\mathbf z_a)\phi_h(\mathbf z_b)]=k_0^2\mu^2hB(\mathbf z_a-\mathbf z_b)$ and is independent of the incoming field. For the moment $M=\mathbb E\prod_a E_a^{(\epsilon_a)}$, expanding both steps to order $h$ gives

$$
\partial_xM=\frac{i}{2k_0}\sum_a\epsilon_a\Delta_{\mathbf z_a}M
-\frac{k_0^2\mu^2}{2}\sum_{a,b}\epsilon_a\epsilon_bB(\mathbf z_a-\mathbf z_b)M.
$$

In particular, the [coherent attenuation in a white-noise random medium](../../../../../../coherent-attenuation-in-a-white-noise-random-medium.md) and its [Fresnel propagator](../../../../../../fresnel-propagator.md) solution are

$$
\partial_xm=\frac{i}{2k_0}\Delta_\perp m-\gamma m,\qquad\gamma=\frac{k_0^2\mu^2B(0)}2.
$$



$$
\boxed{m(x)=e^{-\gamma x}U_xE_0.}
$$

Equivalently, write $W\,dx=d\beta_x$, where $\beta_x(\mathbf z)$ is [Brownian motion](../../../../../../brownian-motion-split.md) in $x$ with transverse [covariance kernel](../../../../../../covariance-kernel.md) $\mathbb E[d\beta_x(\mathbf z)d\beta_x(\mathbf z')]=B(\mathbf z-\mathbf z')dx$. The [Stratonovich integral](../../../../../../stratonovich-integral.md) formulation is $dE=DE\,dx+ik_0\mu E\circ d\beta_x$. Its [Itô integral](../../../../../../ito-integral.md) form is

$$
dE=(DE-\gamma E)\,dx+ik_0\mu E\,d\beta_x.
$$

The mean of the [Itô integral](../../../../../../ito-integral.md) vanishes, independently confirming the attenuation drift. For $x>0$ in two transverse dimensions,

$$
(U_xE_0)(\mathbf z)=\frac{k_0}{2\pi i x}\int_{\mathbb R^2}\exp\left(\frac{ik_0|\mathbf z-\mathbf z'|^2}{2x}\right)E_0(\mathbf z')\,d\mathbf z'.
$$

Thus a unit [plane wave](../../../../../../plane-wave.md) has $m=e^{-\gamma x}$. For a general incident [wave envelope](../../../../../../envelope-waves.md), the [Fresnel propagator](../../../../../../fresnel-propagator.md) supplies its spreading. The attenuation is redistribution between the [coherent and diffuse wave fields](../../../../../../coherent-and-diffuse-wave-fields.md), rather than [wave absorption](../../../../../../wave-absorption.md): for a field and its conjugate at the same point, the screen contribution in the second-moment equation cancels.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
