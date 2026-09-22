<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $a=\kappa m^2$, with $\kappa>0$ and $m\ne0$. The relevant [homogenization of a periodic advection-diffusion equation](../../../../../homogenization-of-a-periodic-advection-diffusion-equation.md) limit is a long horizontal wavelength observed on its [diffusive time scale](../../../../../diffusive-time-scale.md). Introduce $X=\varepsilon x$ and $\tau=\varepsilon^2t$, retaining the fast variables $y,t$. Since the [velocity field](../../../../../velocity-field.md) is independent of $x$, no fast horizontal cell variable is needed. Write the [multiple-scale expansion](../../../../../method-of-multiple-scales.md)

$$
\chi=C(X,\tau)+\varepsilon\chi_1(X,y,\tau,t)+\varepsilon^2\chi_2(X,y,\tau,t)+\cdots,
\qquad L=\partial_t-\kappa\partial_y^2.
$$

The cell functions are periodic in $y$ and in the period of $U$. The [kernel](../../../../../kernel-of-a-linear-map.md) of $L$ on this periodic cell consists of constants: multiplying $Lh=0$ by $h$ and integrating over the cell gives $\kappa\langle|h_y|^2\rangle=0$, after which $h_t=0$. Thus the leading concentration really is independent of the fast variables. At first order,

$$
L\chi_1=-U(t)\sin(my)C_X,
\qquad \chi_1=-g(t)\sin(my)C_X,
\qquad g'+ag=U.
$$

There is a unique periodic $g$: differences of two solutions are proportional to $e^{-at}$, and the periodicity condition fixes the integration constant. Equivalently,

$$
g(t)=\int_{-\infty}^t e^{-a(t-s)}U(s)\,ds.
$$

At second order the [advection-diffusion equation](../../../../../advection-diffusion-equation.md) gives

$$
L\chi_2=-C_\tau-U\sin(my)\partial_X\chi_1+\kappa C_{XX}
=-C_\tau+\bigl[\kappa+Ug\sin^2(my)\bigr]C_{XX}.
$$

Integration over the fast cell annihilates the left side. Since the spatial average of $\sin^2(my)$ is $1/2$, its [solvability condition](../../../../../solvability-condition.md) is

$$
C_\tau=\kappa_e C_{XX},\qquad
\boxed{\kappa_e=\kappa+\frac12\langle Ug\rangle
=\kappa+\frac{a}{2}\langle g^2\rangle.}
$$

For the second equality, multiply $g'+ag=U$ by $g$ and average over a period: $\langle gg'\rangle=0$. In particular the enhancement of [diffusivity](../../../../../diffusion-coefficient.md) is nonnegative. Once this [solvability condition](../../../../../solvability-condition.md) holds, the remaining zero-mean forcing admits a periodic cell solution: its nonconstant spatial [Fourier modes](../../../../../fourier-mode.md) are damped by $\kappa n^2m^2$, while its spatially constant mode has a periodic antiderivative because its temporal average is zero. This also explains the relaxation of initial transverse inhomogeneity. The first corrector has zero spatial mean, so $\bar\chi=C+O(\varepsilon^2)$.

This derivation describes the large-scale, long-time limit, after times comparable to the period and to $a^{-1}$. It does not give an exact closed equation for the spatial average of arbitrary finite-time data: that average contains a correlation between the [velocity field](../../../../../velocity-field.md) and concentration. In physical coordinates the leading long-wavelength concentration therefore obeys **$\bar\chi_t=\kappa_e\bar\chi_{xx}$ asymptotically**. The cell expansion, its bounded periodic correctors, and the decay of transverse cell transients justify this [effective diffusivity of a periodic sinusoidal shear](../../../../../effective-diffusivity-of-a-periodic-sinusoidal-shear.md).

For constant $U_0$, the periodic cell solution is $g=U_0/a$. Consequently

$$
\boxed{\kappa_e=\kappa+\frac{U_0^2}{2\kappa m^2}.}
$$

This is [Taylor dispersion](../../../../../taylor-dispersion.md): [molecular diffusion](../../../../../molecular-diffusion.md) moves particles between different horizontal velocities and turns their accumulated horizontal displacement into large-scale [diffusion](../../../../../diffusion.md).

For the impulsive flow, $g$ jumps by $U_1$ at each kick and decays exponentially between kicks. If $G$ denotes its value just after a kick, periodicity requires $G=e^{-aT}G+U_1$. Thus, within one period,

$$
G=\frac{U_1}{1-e^{-aT}},\qquad g(t)=G e^{-at}\quad(0<t<T),
\qquad \langle g^2\rangle=\frac{G^2(1-e^{-2aT})}{2aT}.
$$

Using the mean-square expression, which has no ambiguous product of a [Dirac delta](../../../../../dirac-delta-function.md) with a discontinuous function, gives

$$
\boxed{\kappa_e=\kappa+\frac{U_1^2}{4T}
\frac{1-e^{-2aT}}{(1-e^{-aT})^2}
=\kappa+\frac{U_1^2}{4T}\coth\!\left(\frac{aT}{2}\right).}
$$

The impulsive model can also be obtained by shrinking smooth pulses of fixed integrated strength. The [passive scalar](../../../../../passive-scalar.md) undergoes the exact horizontal shear map $x\mapsto x+U_1\sin(my)$ at a kick, while the transverse coordinate is unchanged. The cell solution above is the corresponding limit of the smooth cell solutions. Using a one-sided value in $Ug$ instead would miss the contribution from the jump of $g^2$.

For $aT\gg1$,

$$
\kappa_e=\kappa+\frac{U_1^2}{4T}\bigl[1+2e^{-aT}+O(e^{-2aT})\bigr].
$$

Transverse [Brownian motion](../../../../../brownian-motion-split.md) substantially decorrelates the shear phase between successive kicks. A uniformly distributed phase has horizontal displacement variance $U_1^2/2$ per kick, producing an extra [diffusivity](../../../../../diffusion-coefficient.md) $\operatorname{Var}(\Delta x)/(2T)=U_1^2/(4T)$.

For $aT\ll1$,

$$
\boxed{\kappa_e=\kappa+\frac{U_1^2}{2aT^2}+\frac{U_1^2a}{24}+O(U_1^2a^3T^2).}
$$

Many kicks occur before transverse [diffusion](../../../../../diffusion.md) changes a particle's shear phase. Their leading effect is therefore the steady shear with mean velocity amplitude $U_1/T$, whose [Taylor dispersion](../../../../../taylor-dispersion.md) coefficient is precisely $U_1^2/(2\kappa m^2T^2)$. The divergence as $\kappa\to0$ describes a very long decorrelation time; it does not imply infinite finite-time spreading. At $\kappa=0$ the phase never changes and, for a uniform phase, $n$ kicks give variance $n^2U_1^2/2$. The spreading is then [ballistic transport](../../../../../ballistic-transport.md), rather than [diffusion](../../../../../diffusion.md). **The long-time diffusive limit must precede the zero-diffusivity limit**, with $t\gg a^{-1}$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
