# Paper 47

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_47.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_47.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [Minkowski metric](../../../special-relativity.md#minkowski-metric) with signature $(+,-)$, so the [Sine-Gordon equation](../../../integrable-systems.md#sine-gordon-equation) is $\phi_{tt}-\phi_{xx}+\sin\phi=0$. The [light-cone coordinates](../../../special-relativity.md#light-cone-coordinates) here satisfy

$$
\partial_+=\partial_x+\partial_t,\qquad\partial_-=\partial_x-\partial_t,\qquad\partial_+\partial_-=\partial_x^2-\partial_t^2.
$$

In particular, there is no extra factor of four with this coordinate normalization. The [Bäcklund transformation](../../../integrable-systems.md#backlund-transformation) requires $a\ne0$, because one of its equations contains $a^{-1}$.

Put $F=(\psi+\phi)/2$ and $G=(\psi-\phi)/2$. In the parameter convention of this paper the [Sine-Gordon Bäcklund transformation](../../../scalar-field-theory.md#sine-gordon-backlund-transformation) gives $G_+=a\sin F$ and $F_-=a^{-1}\sin G$. Differentiating, for a twice differentiable transformed field, gives

$$
G_{+-}=\cos F\sin G,\qquad F_{+-}=\cos G\sin F.
$$

Since $\psi=F+G$, the addition formula yields $\psi_{+-}=\sin(F+G)=\sin\psi$. Therefore **the transformed field satisfies the same [Sine-Gordon equation](../../../integrable-systems.md#sine-gordon-equation):**

$$
\boxed{\psi_{tt}-\psi_{xx}+\sin\psi=0.}
$$

Subtracting the two differentiated equations also gives $\phi_{+-}=\sin\phi$, showing the compatibility with the seed equation. This proves the unheaded request before the numbered parts, without assuming a particular [soliton](../../../integrable-systems.md#soliton) form.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

With zero seed, both [Bäcklund transformation](../../../integrable-systems.md#backlund-transformation) equations concern $\phi_a/2$. On a nonconstant branch, separation of variables uses $d\log|\tan(\phi_a/4)|=d\phi_a/[2\sin(\phi_a/2)]$, giving

$$
\tan\frac{\phi_a}{4}=C\exp(a x_++a^{-1}x_-),\qquad a\ne0.
$$

For $C>0$, absorb its magnitude into an additive constant $c=\log C$ in the exponent. A convenient smooth representative is

$$
\boxed{\phi_a(x,t)=4\arctan\exp\left[\frac{a+a^{-1}}2x+\frac{a-a^{-1}}2t+c\right].}
$$

The constant-phase condition for this traveling profile determines its [velocity](../../../classical-mechanics.md#velocity):

$$
\boxed{v_a=\frac{1-a^2}{1+a^2},\qquad\gamma_a=\frac{|a+a^{-1}|}{2}=\frac1{\sqrt{1-v_a^2}}.}
$$

**The profile is a traveling [soliton](../../../integrable-systems.md#soliton) with [velocity](../../../classical-mechanics.md#velocity) $v_a=(1-a^2)/(1+a^2)$, strictly between $-1$ and $1$.** The [scalar-field vacua](../../../quantum-field-theory.md#scalar-field-vacuum) on the two sides differ by $2\pi$. With the [topological charge](../../../classical-field-theory-soliton.md#topological-charge) convention $Q=[\phi(+\infty)-\phi(-\infty)]/(2\pi)$, this branch has $Q=\operatorname{sgn}a$: it is a [Sine-Gordon kink](../../../scalar-field-theory.md#sine-gordon-kink) for $a>0$ and an [antikink](../../../classical-field-theory-soliton.md#antikink) for $a<0$. Its width is proportional to $\gamma_a^{-1}$, and its derivative decays exponentially away from its center, giving a [finite-energy field configuration](../../../classical-field-theory-soliton.md#finite-energy-field-configuration).

For completeness, the classical rest [mass](../../../classical-mechanics.md#mass) in this paper's coupling convention is $8m/\beta$, as derived in Question 2; a [Lorentz boost](../../../special-relativity.md#lorentz-boost) gives energy $8m\gamma_a/\beta$. This localized, topologically protected traveling field is the required [classical field-theory soliton](../../../classical-field-theory-soliton.md). A negative $C$ reverses the field and hence the [topological charge](../../../classical-field-theory-soliton.md#topological-charge); $C=0$ gives the vacuum rather than a [soliton](../../../integrable-systems.md#soliton). Vacuum shifts by $4\pi$ can be made without changing the displayed [Bäcklund transformation](../../../integrable-systems.md#backlund-transformation) equations.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Choose the positive-exponential branches from part (i) and set their additive constants to zero. First take $0<b<1$, and define

$$
v=\frac{1-b^2}{1+b^2}\in(0,1),\qquad\gamma=\frac{b+b^{-1}}2=\frac1{\sqrt{1-v^2}},\qquad a=-b^{-1}.
$$

Then $\tan(\phi_b/4)=e^{\gamma(x-vt)}$ and $\tan(\phi_a/4)=e^{-\gamma(x+vt)}$. The tangent subtraction formula gives

$$
\tan\frac{\phi_b-\phi_a}{4}=\frac{\sinh(\gamma x)}{\cosh(\gamma vt)},\qquad\frac{b+a}{b-a}=-v.
$$

Consequently the allowed [Sine-Gordon superposition formula](../../../scalar-field-theory.md#bianchi-permutability-for-sine-gordon-backlund-transformations) produces the smooth field

$$
\boxed{\phi_{a,b}(x,t)=-4\arctan\left[\frac{v\sinh(\gamma x)}{\cosh(\gamma vt)}\right].}
$$

This is the negative of the [Sine-Gordon two-kink solution](../../../scalar-field-theory.md#sine-gordon-two-kink-solution), and hence a two-[antikink](../../../classical-field-theory-soliton.md#antikink) configuration. The auxiliary seeds have opposite [topological charges](../../../classical-field-theory-soliton.md#topological-charge), but their charges cannot simply be added to infer the charge of the nonlinear two-step [Bäcklund transformation](../../../integrable-systems.md#backlund-transformation). Indeed, the displayed final field tends to $2\pi$ at the left spatial end and $-2\pi$ at the right, so its total [topological charge](../../../classical-field-theory-soliton.md#topological-charge) is $-2$.

Let $T=|t|$ become large. Near the right transition, $x=vT+O(1)$, the tangent argument has the asymptotic form

$$
\frac{v\sinh(\gamma x)}{\cosh(\gamma vt)}=v e^{\gamma(x-vT)}+o(1),
$$

so the local field is $-4\arctan e^{\gamma(x-vT)+\log v}$, a single [antikink](../../../classical-field-theory-soliton.md#antikink). Near the left transition, the local field is $4\arctan e^{-\gamma(x+vT)+\log v}+o(1)$, again a decreasing [antikink](../../../classical-field-theory-soliton.md#antikink). The resulting asymptotic center lines are

$$
\begin{array}{c|cc}
& t\to-\infty&t\to+\infty\\
x_L(t)&vt+\gamma^{-1}\log v&-vt+\gamma^{-1}\log v\\
x_R(t)&-vt-\gamma^{-1}\log v&vt-\gamma^{-1}\log v.
\end{array}
$$

Thus two incoming [antikinks](../../../classical-field-theory-soliton.md#antikink) with [topological charges](../../../classical-field-theory-soliton.md#topological-charge) $(-1,-1)$ and [velocities](../../../classical-mechanics.md#velocity) $(+v,-v)$ separate again with exactly the same [topological charges](../../../classical-field-theory-soliton.md#topological-charge) and [velocities](../../../classical-mechanics.md#velocity). There is no radiative tail in these asymptotic profiles. Labeling the outgoing objects by their preserved [rapidities](../../../special-relativity.md#rapidity) makes this elastic [soliton](../../../integrable-systems.md#soliton) scattering; labeling the left and right lumps instead describes reflection with exchanged [velocities](../../../classical-mechanics.md#velocity).

For the right-moving [soliton](../../../integrable-systems.md#soliton), its incoming intercept is $\gamma^{-1}\log v$ and its outgoing intercept is $-\gamma^{-1}\log v$. The spatial shifts are therefore $\Delta x_+=-2\gamma^{-1}\log v$ and $\Delta x_-=2\gamma^{-1}\log v$. Define the [soliton time delay](../../../classical-field-theory-soliton.md#soliton-time-delay) as the change in arrival time at a fixed distant spatial point relative to continuation of the incoming straight line, so $\Delta t=-\Delta x/v_{\mathrm{particle}}$. Both objects have **the same signed [soliton time delay](../../../classical-field-theory-soliton.md#soliton-time-delay), which is an advance:**

$$
\boxed{\Delta t=\frac{2\log v}{\gamma v}<0.}
$$

This is the [Sine-Gordon two-kink time advance](../../../scalar-field-theory.md#sine-gordon-two-kink-time-advance). In physical coordinates $T_{\rm phys}=t/m$, the time shift is $2\log v/(m\gamma v)$. The explicit intercepts fix the sign convention unambiguously.

The remaining real parameter choices are covered without changing the calculation. For any $b\ne0$ with $b^2\ne1$, put $v_b=(1-b^2)/(1+b^2)$, $u=|v_b|$, $\gamma=(|b|+|b|^{-1})/2$ and $\epsilon=\operatorname{sgn}(b v_b)$. The same choice of zero additive constants gives

$$
\phi_{a,b}=-4\epsilon\arctan\left[\frac{u\sinh(\gamma x)}{\cosh(\gamma ut)}\right].
$$

Each scattered object's [topological charge](../../../classical-field-theory-soliton.md#topological-charge) is $-\epsilon$, the [velocities](../../../classical-mechanics.md#velocity) are $\pm u$, and the signed [soliton time delay](../../../classical-field-theory-soliton.md#soliton-time-delay) is $2\log u/(\gamma u)$. If $b=\pm1$, the superposition coefficient vanishes and this representative is the vacuum; there is no pair of separated moving [solitons](../../../integrable-systems.md#soliton) and no scattering delay to assign. Thus the scattering conclusion requires the nondegenerate case $0<u<1$.

## 2

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

To keep the paper's coupling convention explicit, write $g=\sqrt\beta$ and use physical coordinates $X=x/m$, $T=t/m$. Assume $\beta>0$ and weak coupling $g\ll1$. The canonical [real scalar field](../../../scalar-field-theory.md#real-scalar-field) is $\varphi=\phi/g$, and the physical potential is

$$
U(\varphi)=\frac{m^2}{g^2}(1-\cos g\varphi).
$$

The symbol $g$ is the coupling usually appearing in canonical [Sine-Gordon theory](../../../scalar-field-theory.md#sine-gordon-theory); the paper's $\beta$ is its square. The vacua have $g\varphi=2\pi n$. A static [Sine-Gordon kink](../../../scalar-field-theory.md#sine-gordon-kink) has $g\varphi_K=4\arctan e^{m(X-X_0)}$ and satisfies $\tfrac12\varphi_K'^2=U(\varphi_K)$. Since $1-\cos(g\varphi_K)=2\operatorname{sech}^2[m(X-X_0)]$, its classical [mass](../../../classical-mechanics.md#mass) is

$$
M_{\rm cl}=\int dX\left[\tfrac12\varphi_K'^2+U(\varphi_K)\right]=\frac{4m^2}{g^2}\int dX\operatorname{sech}^2[m(X-X_0)]=\boxed{\frac{8m}{\beta}.}
$$

The [topological sector](../../../classical-field-theory-soliton.md#topological-sector) is important: this energy is measured relative to a vacuum, and the [kink](../../../classical-field-theory-soliton.md#scalar-field-kink) joins distinct vacua at the two spatial ends. Expanding around a spatially constant vacuum cannot construct this state by any finite-order perturbation in $g$.

For the general [one-loop soliton mass correction](../../../classical-field-theory-soliton.md#one-loop-soliton-mass-correction), start with a canonical [scalar field](../../../quantum-field-theory.md#scalar-field) potential $U$ and a stable static [soliton](../../../integrable-systems.md#soliton) $\varphi_K$. Write $\varphi=\varphi_K+\eta$. The term linear in $\eta$ vanishes by the classical [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation). The [quadratic fluctuation Hamiltonian](../../../perturbative-quantum-field-theory.md#quadratic-fluctuation-hamiltonian) is

$$
H_2=\frac12\int dX\left[\pi_\eta^2+\eta\mathcal H_K\eta\right],\qquad\mathcal H_K=-\partial_X^2+U''(\varphi_K(X)).
$$

Choose a common large box and a common finite-mode [regularization in quantum field theory](../../../perturbative-quantum-field-theory.md#regularization-in-quantum-field-theory). Expand the nonzero [normal modes](../../../wave-equation.md#normal-mode) as $\eta=\sum_n q_n f_n$, with $\mathcal H_Kf_n=\omega_n^2 f_n$ and normalized [eigenfunctions](../../../linear-operator-theory.md#eigenfunction). Each pair $(q_n,p_n)$ is a [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator) contributing ground-state energy $\hbar\omega_n/2$. In the vacuum, replace $\mathcal H_K$ by $\mathcal H_0=-\partial_X^2+U''(\varphi_{\rm vac})$. Subtract the two ground-state energies and add the local [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) evaluated on the [soliton](../../../integrable-systems.md#soliton) relative to the vacuum. This derives the general formula

$$
\boxed{\Delta M^{(1)}=\lim_{\mathrm{reg}\to\infty}\left[\frac\hbar2\left(\sum_n'\omega_n^{K}-\sum_n\omega_n^{0}\right)+\Delta M_{\rm ct}\right].}
$$

The prime excludes exact [zero modes in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory) from oscillator quantization; their zero frequencies contribute no [zero-point energy](../../../quantum-mechanics.md#zero-point-energy), but their role in mode counting must not be forgotten. The two sums mean a paired finite regulator, not separate subtractions of divergent answers. Equivalently the nonzero-mode term is the regulated difference of the square-root traces of the two fluctuation operators. Discrete [bound states](../../../quantum-mechanics.md#bound-state) and continuum modes both contribute. This is a [vacuum-subtracted soliton mass](../../../classical-field-theory-soliton.md#vacuum-subtracted-soliton-mass) and the first term in the [semiclassical soliton mass](../../../classical-field-theory-soliton.md#semiclassical-soliton-mass) expansion.

Translation gives a [zero mode in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory) because differentiating the static equation yields $\mathcal H_K\varphi_K'=0$. A Gaussian oscillator or an unprimed [functional determinant](../../../quantum-field-theory.md#functional-determinant) is inappropriate along this flat direction. Replace its amplitude by the position [collective coordinate](../../../classical-field-theory-soliton.md#collective-coordinate-of-a-soliton) $X_0(T)$ and require the residual fluctuation to obey $\int\eta\varphi_K'\,dX=0$, preventing double counting. The associated change-of-variables Jacobian supplies the zero-mode normalization. At low speed the [collective-coordinate effective Lagrangian for a soliton](../../../classical-field-theory-soliton.md#collective-coordinate-effective-lagrangian-for-a-soliton) is $-M_{\rm cl}+\tfrac12M_{\rm cl}\dot X_0^2+\cdots$; quantizing the position gives the [soliton](../../../integrable-systems.md#soliton) momentum and its translational states, not an extra oscillator rest energy. More generally, every physical continuous modulus needs a [collective coordinate](../../../classical-field-theory-soliton.md#collective-coordinate-of-a-soliton); gauge directions require [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) rather than additional physical states.

The [Sine-Gordon kink fluctuation operator](../../../scalar-field-theory.md#sine-gordon-kink-fluctuation-operator) is particularly simple:

$$
\mathcal H_K=-\partial_X^2+m^2\left[1-2\operatorname{sech}^2m(X-X_0)\right]=D^\dagger D,\qquad D=\partial_X+m\tanh m(X-X_0),
$$

while $DD^\dagger=-\partial_X^2+m^2=\mathcal H_0$. This [supersymmetric factorization of the one-soliton potential](../../../quantum-mechanics.md#supersymmetric-factorization-of-the-one-soliton-potential) shows stability and generates all nonzero [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) from vacuum plane waves. The sole normalizable [bound state](../../../quantum-mechanics.md#bound-state) is the [translational zero mode of a sine-Gordon kink](../../../scalar-field-theory.md#translational-zero-mode-of-a-sine-gordon-kink), proportional to $\operatorname{sech}m(X-X_0)$; there is no positive-frequency internal bound oscillator. The continuum has $\omega(k)=\sqrt{k^2+m^2}$ and no reflection. Applying $D^\dagger$ to $e^{ikX}$ gives a [transmission amplitude](../../../quantum-mechanics.md#transmission-amplitude)

$$
T(k)=\frac{k+im}{k-im}=e^{i\delta(k)},\qquad\delta(k)=2\arctan\frac{m}{k}\quad(k>0).
$$

This [scattering phase shift](../../../quantum-mechanics.md#scattering-phase-shift) changes the density of continuum modes. The high-frequency vacuum subtraction cancels the extensive vacuum contribution but still leaves a logarithmic [ultraviolet divergence](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence).

The finite part also requires consistent [mode-number regularization of soliton masses](../../../classical-field-theory-soliton.md#mode-number-regularization-of-soliton-masses). The [periodic-box phase-shift quantization](../../../quantum-mechanics.md#periodic-box-phase-shift-quantization) condition is $k_nL+\delta(k_n)=2\pi n$. Match $2N+1$ modes: the [kink](../../../classical-field-theory-soliton.md#scalar-field-kink) has its translation mode plus the two continuum modes at each $n=1,\ldots,N$, while the vacuum has the $k=0$ oscillator of frequency $m$ and the corresponding continuum pairs. With $\hbar=1$ and $\Lambda=2\pi N/L$, expanding $k_n-k_n^{(0)}=-\delta(k_n^{(0)})/L+o(L^{-1})$ gives

$$
\Delta M_{\rm bare}=-\frac m2-\frac1{2\pi}\int_0^\Lambda\delta(k)\frac{k}{\sqrt{k^2+m^2}}\,dk.
$$

Integration by parts uses $\delta(0)=\pi$ and yields

$$
\Delta M_{\rm bare}=\frac1{2\pi}\int_0^\Lambda\omega(k)\delta'(k)\,dk-\frac{\omega(\Lambda)\delta(\Lambda)}{2\pi}=-\frac m\pi\operatorname{arsinh}\frac\Lambda m-\frac{\omega(\Lambda)\delta(\Lambda)}{2\pi}.
$$

The [cutoff surface term for a Sine-Gordon kink](../../../classical-field-theory-soliton.md#cutoff-surface-term-for-a-sine-gordon-kink) tends to $-m/\pi$. It cannot be dropped merely because $\delta(\Lambda)\to0$: $\omega(\Lambda)$ grows at the same time.

A [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) must specify which mass and coupling are held fixed. For vacuum [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering), or cancellation of the vacuum [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram) with the elementary mass fixed at $m$, the quartic interaction gives the [mass counterterm](../../../perturbative-quantum-field-theory.md#mass-counterterm)

$$
\delta m^2=\frac{m^2g^2}{4}\int_{-\Lambda}^{\Lambda}\frac{dk}{2\pi\sqrt{k^2+m^2}}.
$$

Evaluating this [Sine-Gordon vacuum tadpole counterterm](../../../scalar-field-theory.md#sine-gordon-vacuum-tadpole-counterterm) on the [kink](../../../classical-field-theory-soliton.md#scalar-field-kink) gives

$$
\Delta M_{\rm ct}=\frac{\delta m^2}{g^2}\int(1-\cos g\varphi_K)\,dX=\frac{4\delta m^2}{mg^2}=\frac m\pi\operatorname{arsinh}\frac\Lambda m.
$$

The logarithmic [ultraviolet divergence](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence) cancels, leaving **the renormalized one-loop [Sine-Gordon kink](../../../scalar-field-theory.md#sine-gordon-kink) mass in the stated vacuum scheme:**

$$
\boxed{\Delta M^{(1)}=-\frac m\pi,\qquad M=\frac{8m}{\beta}-\frac m\pi+O(m\beta).}
$$

This example illustrates why a [zero mode in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory) must be treated as a [collective coordinate](../../../classical-field-theory-soliton.md#collective-coordinate-of-a-soliton), why vacuum subtraction alone need not remove [ultraviolet divergences](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence), and why the finite relation between the two regulators matters. Different finite [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) amount to different definitions of the renormalized parameters; an unregulated frequency difference without a [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) is not a physical mass prediction.

## 3

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In elastic diagonal [factorized scattering](../../../quantum-field-theory.md#factorized-scattering), the [Faddeev-Zamolodchikov algebra](../../../quantum-field-theory.md#faddeev-zamolodchikov-algebra) describes an exchange of two particle operators. Exchanging the pair twice must restore the original state. This is analytic [unitarity](../../../vector-space.md#unitary-operator):

$$
S_{AA}(\theta)S_{AA}(-\theta)=1,\qquad S_{A\bar A}(\theta)S_{\bar A A}(-\theta)=1.
$$

Keeping the reversed species in this identity avoids an unstated parity assumption. For the particular amplitudes derived below, crossing and analytic [unitarity](../../../vector-space.md#unitary-operator) also imply $S_{\bar A A}=S_{A\bar A}$. [Hermitian analyticity of a two-particle S-matrix](../../../quantum-mechanics.md#hermitian-analyticity-of-a-two-particle-s-matrix) states $S_{ab}(\theta)^*=S_{ba}(-\theta^*)$ and, together with analytic [unitarity](../../../vector-space.md#unitary-operator), gives $|S_{ab}(\theta)|=1$ for real [rapidity](../../../special-relativity.md#rapidity) differences. [Crossing symmetry](../../../quantum-mechanics.md#crossing-symmetry) analytically turns an incoming particle into an outgoing [antiparticle](../../../relativistic-quantum-field.md#antiparticle), relating the two channels by $S_{A\bar A}(\theta)=S_{AA}(i\pi-\theta)$, with the reverse relation obtained by crossing again. The shift $i\pi$ follows from the sign reversal of the two-momentum $p(\theta)=(m\cosh\theta,m\sinh\theta)$.

Put $u=\lambda/2$. The given amplitude is the [unit-modulus hyperbolic scattering block](../../../quantum-mechanics.md#unit-modulus-hyperbolic-scattering-block) $S_u(\theta)=\sinh[(\theta+iu)/2]/\sinh[(\theta-iu)/2]$. Its numerator and denominator interchange under $\theta\mapsto-\theta$, proving analytic [unitarity](../../../vector-space.md#unitary-operator). For real $u$ it also obeys [Hermitian analyticity of a two-particle S-matrix](../../../quantum-mechanics.md#hermitian-analyticity-of-a-two-particle-s-matrix). Applying [crossing symmetry](../../../quantum-mechanics.md#crossing-symmetry) gives

$$
\boxed{S_{A\bar A}(\theta)=\frac{\cosh[(\theta-iu)/2]}{\cosh[(\theta+iu)/2]}.}
$$

This crossed amplitude also has unit modulus on the real axis. Thus both requested channel constraints hold.

The bound-state conclusion needs a coupling range. In the fundamental attractive range $0<u<\pi$, equivalently $0<\lambda<2\pi$, the denominator has a simple [pole](../../../isolated-singularity.md#pole) at $\theta=iu$ inside the [physical rapidity strip](../../../quantum-mechanics.md#physical-rapidity-strip). Its [residue](../../../analysis.md#residue) is

$$
\operatorname*{Res}_{\theta=iu}S_{AA}(\theta)=2i\sin u,
$$

with positive imaginary coefficient. Under the usual one-particle interpretation of this direct-channel [bound-state pole](../../../quantum-mechanics.md#bound-state-pole-of-the-scattering-amplitude), it couples two charge-$+1$ particles to a new charge-$+2$ particle $B$. In the center-of-mass frame its constituents have analytically continued [rapidities](../../../special-relativity.md#rapidity) $\pm iu/2$, and their total two-momentum is $(2m\cos(u/2),0)$. Thus the [relativistic bound-state mass from a rapidity pole](../../../quantum-mechanics.md#relativistic-bound-state-mass-from-a-rapidity-pole) gives

$$
\boxed{Q_B=+2,\qquad m_B=2m\cos\frac u2=2m\cos\frac\lambda4.}
$$

It is positive and less than the two-particle threshold $2m$. Without the coupling qualification the requested deduction is false: at $\lambda=0$ the amplitude is identically one after removing the apparent $0/0$ at the origin. A free massive complex [scalar field](../../../quantum-field-theory.md#scalar-field) has this diagonal amplitude, charge-$\pm1$ particles and no isolated charge-$+2$ [bound state](../../../quantum-mechanics.md#bound-state). At $u=\pi$ the amplitude similarly becomes constant $-1$ and the apparent boundary pole cancels. Neither endpoint supplies the claimed particle.

For [bound-state fusion of factorized S-matrices](../../../quantum-field-theory.md#bound-state-fusion-of-factorized-s-matrices), represent $B$ as the residue of $A(\theta_B+iu/2)A(\theta_B-iu/2)$ at its bound-state separation. Move a third $A(\theta_A)$ through both constituents using the [Faddeev-Zamolodchikov algebra](../../../quantum-field-theory.md#faddeev-zamolodchikov-algebra), then take the same residue. The bound-state normalization occurs on both sides and cancels. Consequently [bootstrap fusion](../../../quantum-field-theory.md#bound-state-fusion-of-factorized-s-matrices) gives

$$
S_{BA}(\theta)=S_{AA}(\theta+iu/2)S_{AA}(\theta-iu/2)=\boxed{\frac{\sinh(\theta/2+3iu/4)\sinh(\theta/2+iu/4)}{\sinh(\theta/2-iu/4)\sinh(\theta/2-3iu/4)}},
$$

where $\theta=\theta_B-\theta_A$. This has analytic [unitarity](../../../vector-space.md#unitary-operator) as a product of two shifted blocks. Its [poles](../../../isolated-singularity.md#pole) occur at $\theta=iu/2$ and $\theta=3iu/2$, modulo $2\pi i$; numerator zeroes occur at the corresponding negative positions, subject to cancellations at special couplings.

The nearer [pole](../../../isolated-singularity.md#pole), $\theta=iu/2$, has [residue](../../../analysis.md#residue) $-2i\sin u$. It is a [crossed-channel pole in diagonal factorized scattering](../../../quantum-mechanics.md#crossed-channel-pole-in-diagonal-factorized-scattering), not a new direct-channel charge-$+3$ state. Indeed, the exchanged momentum has invariant

$$
t=m_B^2+m^2-2m_Bm\cos\frac u2=m^2,
$$

using $m_B=2m\cos(u/2)$. The exchanged particle is therefore the already present $A$, with the appropriate charge flow at the crossed vertex. Equivalently, [crossing symmetry](../../../quantum-mechanics.md#crossing-symmetry) puts a positive-residue direct pole of $S_{B\bar A}$ at $i(\pi-u/2)$, corresponding to $B+\bar A\longrightarrow A$. This distinction avoids assigning an extra mass by applying the direct-channel formula to every [pole](../../../isolated-singularity.md#pole).

The farther [pole](../../../isolated-singularity.md#pole), $\theta=3iu/2$, lies in the [physical rapidity strip](../../../quantum-mechanics.md#physical-rapidity-strip) only for $0<u<2\pi/3$, equivalently $0<\lambda<4\pi/3$. Its [residue](../../../analysis.md#residue) is

$$
2i\sin u\,\frac{\sin(3u/2)}{\sin(u/2)},
$$

which has positive imaginary coefficient in that range. It gives a charge-$+3$ [bound state](../../../quantum-mechanics.md#bound-state) $C$. The [relativistic bound-state mass from a rapidity pole](../../../quantum-mechanics.md#relativistic-bound-state-mass-from-a-rapidity-pole) now yields

$$
m_C^2=m_B^2+m^2+2m_Bm\cos\frac{3u}{2}=m^2(1+2\cos u)^2.
$$

The positive root in the admitted range is

$$
\boxed{Q_C=+3,\qquad m_C=m(1+2\cos u)=m\frac{\sin(3u/2)}{\sin(u/2)}=m(1+2\cos(\lambda/2)),\quad0<\lambda<\frac{4\pi}{3}.}
$$

This is the [three-particle bound state from equal-mass fusion](../../../quantum-field-theory.md#three-particle-bound-state-from-equal-mass-fusion); in its own rest frame the constituent [rapidities](../../../special-relativity.md#rapidity) are $iu,0,-iu$. At $u=2\pi/3$ the farther apparent pole cancels because its numerator also vanishes; for $2\pi/3<u<\pi$ it lies outside the [physical rapidity strip](../../../quantum-mechanics.md#physical-rapidity-strip) and does not require a new charge-$+3$ particle. Charge-conjugate partners carry charges $-2$ and $-3$ where the corresponding states exist. **Fusion distinguishes an existing crossed-channel particle from a genuinely new direct-channel [bound state](../../../quantum-mechanics.md#bound-state), and the latter requires the stated smaller coupling range.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
