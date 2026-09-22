<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

To keep the paper's coupling convention explicit, write $g=\sqrt\beta$ and use physical coordinates $X=x/m$, $T=t/m$. Assume $\beta>0$ and weak coupling $g\ll1$. The canonical [real scalar field](../../../../../real-scalar-field.md) is $\varphi=\phi/g$, and the physical potential is

$$
U(\varphi)=\frac{m^2}{g^2}(1-\cos g\varphi).
$$

The symbol $g$ is the coupling usually appearing in canonical [Sine-Gordon theory](../../../../../sine-gordon-theory.md); the paper's $\beta$ is its square. The vacua have $g\varphi=2\pi n$. A static [Sine-Gordon kink](../../../../../sine-gordon-kink.md) has $g\varphi_K=4\arctan e^{m(X-X_0)}$ and satisfies $\tfrac12\varphi_K'^2=U(\varphi_K)$. Since $1-\cos(g\varphi_K)=2\operatorname{sech}^2[m(X-X_0)]$, its classical [mass](../../../../../mass.md) is

$$
M_{\rm cl}=\int dX\left[\tfrac12\varphi_K'^2+U(\varphi_K)\right]=\frac{4m^2}{g^2}\int dX\operatorname{sech}^2[m(X-X_0)]=\boxed{\frac{8m}{\beta}.}
$$

The [topological sector](../../../../../topological-sector.md) is important: this energy is measured relative to a vacuum, and the [kink](../../../../../scalar-field-kink.md) joins distinct vacua at the two spatial ends. Expanding around a spatially constant vacuum cannot construct this state by any finite-order perturbation in $g$.

For the general [one-loop soliton mass correction](../../../../../one-loop-soliton-mass-correction.md), start with a canonical [scalar field](../../../../../scalar-field.md) potential $U$ and a stable static [soliton](../../../../../soliton.md) $\varphi_K$. Write $\varphi=\varphi_K+\eta$. The term linear in $\eta$ vanishes by the classical [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md). The [quadratic fluctuation Hamiltonian](../../../../../quadratic-fluctuation-hamiltonian.md) is

$$
H_2=\frac12\int dX\left[\pi_\eta^2+\eta\mathcal H_K\eta\right],\qquad\mathcal H_K=-\partial_X^2+U''(\varphi_K(X)).
$$

Choose a common large box and a common finite-mode [regularization in quantum field theory](../../../../../regularization-in-quantum-field-theory.md). Expand the nonzero [normal modes](../../../../../normal-mode.md) as $\eta=\sum_n q_n f_n$, with $\mathcal H_Kf_n=\omega_n^2 f_n$ and normalized [eigenfunctions](../../../../../eigenfunction.md). Each pair $(q_n,p_n)$ is a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) contributing ground-state energy $\hbar\omega_n/2$. In the vacuum, replace $\mathcal H_K$ by $\mathcal H_0=-\partial_X^2+U''(\varphi_{\rm vac})$. Subtract the two ground-state energies and add the local [counterterms](../../../../../counterterm.md) evaluated on the [soliton](../../../../../soliton.md) relative to the vacuum. This derives the general formula

$$
\boxed{\Delta M^{(1)}=\lim_{\mathrm{reg}\to\infty}\left[\frac\hbar2\left(\sum_n'\omega_n^{K}-\sum_n\omega_n^{0}\right)+\Delta M_{\rm ct}\right].}
$$

The prime excludes exact [zero modes in field theory](../../../../../zero-mode-in-field-theory.md) from oscillator quantization; their zero frequencies contribute no [zero-point energy](../../../../../zero-point-energy.md), but their role in mode counting must not be forgotten. The two sums mean a paired finite regulator, not separate subtractions of divergent answers. Equivalently the nonzero-mode term is the regulated difference of the square-root traces of the two fluctuation operators. Discrete [bound states](../../../../../bound-state.md) and continuum modes both contribute. This is a [vacuum-subtracted soliton mass](../../../../../vacuum-subtracted-soliton-mass.md) and the first term in the [semiclassical soliton mass](../../../../../semiclassical-soliton-mass.md) expansion.

Translation gives a [zero mode in field theory](../../../../../zero-mode-in-field-theory.md) because differentiating the static equation yields $\mathcal H_K\varphi_K'=0$. A Gaussian oscillator or an unprimed [functional determinant](../../../../../functional-determinant.md) is inappropriate along this flat direction. Replace its amplitude by the position [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md) $X_0(T)$ and require the residual fluctuation to obey $\int\eta\varphi_K'\,dX=0$, preventing double counting. The associated change-of-variables Jacobian supplies the zero-mode normalization. At low speed the [collective-coordinate effective Lagrangian for a soliton](../../../../../collective-coordinate-effective-lagrangian-for-a-soliton.md) is $-M_{\rm cl}+\tfrac12M_{\rm cl}\dot X_0^2+\cdots$; quantizing the position gives the [soliton](../../../../../soliton.md) momentum and its translational states, not an extra oscillator rest energy. More generally, every physical continuous modulus needs a [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md); gauge directions require [gauge fixing](../../../../../gauge-fixing.md) rather than additional physical states.

The [Sine-Gordon kink fluctuation operator](../../../../../sine-gordon-kink-fluctuation-operator.md) is particularly simple:

$$
\mathcal H_K=-\partial_X^2+m^2\left[1-2\operatorname{sech}^2m(X-X_0)\right]=D^\dagger D,\qquad D=\partial_X+m\tanh m(X-X_0),
$$

while $DD^\dagger=-\partial_X^2+m^2=\mathcal H_0$. This [supersymmetric factorization of the one-soliton potential](../../../../../supersymmetric-factorization-of-the-one-soliton-potential.md) shows stability and generates all nonzero [eigenfunctions](../../../../../eigenfunction.md) from vacuum plane waves. The sole normalizable [bound state](../../../../../bound-state.md) is the [translational zero mode of a sine-Gordon kink](../../../../../translational-zero-mode-of-a-sine-gordon-kink.md), proportional to $\operatorname{sech}m(X-X_0)$; there is no positive-frequency internal bound oscillator. The continuum has $\omega(k)=\sqrt{k^2+m^2}$ and no reflection. Applying $D^\dagger$ to $e^{ikX}$ gives a [transmission amplitude](../../../../../transmission-amplitude.md)

$$
T(k)=\frac{k+im}{k-im}=e^{i\delta(k)},\qquad\delta(k)=2\arctan\frac{m}{k}\quad(k>0).
$$

This [scattering phase shift](../../../../../scattering-phase-shift.md) changes the density of continuum modes. The high-frequency vacuum subtraction cancels the extensive vacuum contribution but still leaves a logarithmic [ultraviolet divergence](../../../../../ultraviolet-divergence.md).

The finite part also requires consistent [mode-number regularization of soliton masses](../../../../../mode-number-regularization-of-soliton-masses.md). The [periodic-box phase-shift quantization](../../../../../periodic-box-phase-shift-quantization.md) condition is $k_nL+\delta(k_n)=2\pi n$. Match $2N+1$ modes: the [kink](../../../../../scalar-field-kink.md) has its translation mode plus the two continuum modes at each $n=1,\ldots,N$, while the vacuum has the $k=0$ oscillator of frequency $m$ and the corresponding continuum pairs. With $\hbar=1$ and $\Lambda=2\pi N/L$, expanding $k_n-k_n^{(0)}=-\delta(k_n^{(0)})/L+o(L^{-1})$ gives

$$
\Delta M_{\rm bare}=-\frac m2-\frac1{2\pi}\int_0^\Lambda\delta(k)\frac{k}{\sqrt{k^2+m^2}}\,dk.
$$

Integration by parts uses $\delta(0)=\pi$ and yields

$$
\Delta M_{\rm bare}=\frac1{2\pi}\int_0^\Lambda\omega(k)\delta'(k)\,dk-\frac{\omega(\Lambda)\delta(\Lambda)}{2\pi}=-\frac m\pi\operatorname{arsinh}\frac\Lambda m-\frac{\omega(\Lambda)\delta(\Lambda)}{2\pi}.
$$

The [cutoff surface term for a Sine-Gordon kink](../../../../../cutoff-surface-term-for-a-sine-gordon-kink.md) tends to $-m/\pi$. It cannot be dropped merely because $\delta(\Lambda)\to0$: $\omega(\Lambda)$ grows at the same time.

A [renormalization condition](../../../../../renormalization-condition.md) must specify which mass and coupling are held fixed. For vacuum [normal ordering](../../../../../normal-ordering.md), or cancellation of the vacuum [tadpole diagram](../../../../../tadpole-diagram.md) with the elementary mass fixed at $m$, the quartic interaction gives the [mass counterterm](../../../../../mass-counterterm.md)

$$
\delta m^2=\frac{m^2g^2}{4}\int_{-\Lambda}^{\Lambda}\frac{dk}{2\pi\sqrt{k^2+m^2}}.
$$

Evaluating this [Sine-Gordon vacuum tadpole counterterm](../../../../../sine-gordon-vacuum-tadpole-counterterm.md) on the [kink](../../../../../scalar-field-kink.md) gives

$$
\Delta M_{\rm ct}=\frac{\delta m^2}{g^2}\int(1-\cos g\varphi_K)\,dX=\frac{4\delta m^2}{mg^2}=\frac m\pi\operatorname{arsinh}\frac\Lambda m.
$$

The logarithmic [ultraviolet divergence](../../../../../ultraviolet-divergence.md) cancels, leaving **the renormalized one-loop [Sine-Gordon kink](../../../../../sine-gordon-kink.md) mass in the stated vacuum scheme:**

$$
\boxed{\Delta M^{(1)}=-\frac m\pi,\qquad M=\frac{8m}{\beta}-\frac m\pi+O(m\beta).}
$$

This example illustrates why a [zero mode in field theory](../../../../../zero-mode-in-field-theory.md) must be treated as a [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md), why vacuum subtraction alone need not remove [ultraviolet divergences](../../../../../ultraviolet-divergence.md), and why the finite relation between the two regulators matters. Different finite [counterterms](../../../../../counterterm.md) amount to different definitions of the renormalized parameters; an unregulated frequency difference without a [renormalization condition](../../../../../renormalization-condition.md) is not a physical mass prediction.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
