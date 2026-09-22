# Paper 1

↑ **Parent:** [2022](../2022.md)

[Original paper, released PDF pages 150–154](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e/response/2127325/attach/3/FOI%202022%20639%20Sullivan%20materials.pdf?cookie_passthrough=1#page=150)

**Table of contents**

- [Section A](#section-a)
  - [1](#section-a/1)
    - [Solution](#section-a/1/solution)
  - [2](#section-a/2)
    - [Solution](#section-a/2/solution)
  - [3](#section-a/3)
    - [Solution](#section-a/3/solution)
  - [4](#section-a/4)
    - [Solution](#section-a/4/solution)
  - [5](#section-a/5)
    - [Solution](#section-a/5/solution)
- [Section B](#section-b)
  - [B6](#section-b/b6)
    - [a](#section-b/b6/a)
      - [Solution](#section-b/b6/a/solution)
    - [b](#section-b/b6/b)
      - [Solution](#section-b/b6/b/solution)
    - [c](#section-b/b6/c)
      - [Solution](#section-b/b6/c/solution)
    - [d](#section-b/b6/d)
      - [Solution](#section-b/b6/d/solution)
    - [e](#section-b/b6/e)
      - [Solution](#section-b/b6/e/solution)
  - [B7](#section-b/b7)
    - [a](#section-b/b7/a)
      - [Solution](#section-b/b7/a/solution)
    - [b](#section-b/b7/b)
      - [Solution](#section-b/b7/b/solution)
    - [c](#section-b/b7/c)
      - [Solution](#section-b/b7/c/solution)
    - [d](#section-b/b7/d)
      - [Solution](#section-b/b7/d/solution)
- [Section C](#section-c)
  - [C8](#section-c/c8)
    - [a](#section-c/c8/a)
      - [Solution](#section-c/c8/a/solution)
    - [b](#section-c/c8/b)
      - [Solution](#section-c/c8/b/solution)
    - [c](#section-c/c8/c)
      - [Solution](#section-c/c8/c/solution)
    - [d](#section-c/c8/d)
      - [Solution](#section-c/c8/d/solution)
- [Section D](#section-d)
  - [D9](#section-d/d9)
    - [Solution](#section-d/d9/solution)

## Section A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-a/1">1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/1/solution">Solution</h4>

↑ **Parent:** [1](#section-a/1)

Let the infinite outer walls be at $x=0,D$, the finite steps at $x=a,b$, and the three [potential energy](../../energy.md#potential-energy) values be $V_L,V_B,V_R$. The original drawing specifies the ordering

$$
V_L<E_0<E_1<V_R<E_2<V_B.
$$

The [energy eigenstates](../../energy-eigenvalue.md#energy-eigenstate) can be chosen real. The [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) are $\psi(0)=\psi(D)=0$; [wavefunction matching at a finite potential step](../../mathematical-physics.md#wavefunction-matching-at-a-finite-potential-step) requires both $\psi$ and $\psi'$ to be continuous at $a,b$. In particular, neither finite step acts as an additional hard wall.

The [time-independent Schrödinger equation](../../mathematical-physics.md#time-independent-schrodinger-equation) gives

$$
\psi''=\frac{2m}{\hbar^2}(V-E)\psi.
$$

Thus a [wavefunction](../../wave-function.md) is sinusoidal in a [classically allowed region](../../mathematical-physics.md#classically-allowed-region), with [wavenumber](../../wave-equation.md#wavenumber) $k=\sqrt{2m(E-V)}/\hbar$, and a [linear combination](../../vector-space.md#linear-combination) of [exponential functions](../../calculus.md#exponential-function) in a [classically forbidden region](../../mathematical-physics.md#classically-forbidden-region), with inverse decay length $q=\sqrt{2m(V-E)}/\hbar$. Its [curvature](../../differential-geometry.md#curvature) changes sign relative to $\psi$ at a step crossing $E$; its [slope](../../euclidean-geometry.md#slope) does not jump.

By the [Sturm oscillation theorem](../../sturm-liouville-theory.md#sturm-oscillation-theorem), the three [energy eigenstates](../../energy-eigenvalue.md#energy-eigenstate) have exactly **zero, one, and two interior nodes**, respectively. Choose their [global phases](../../quantum-system.md#global-phase) so that their slopes at the left wall are positive:

- $E_0$: a positive lobe in the left-hand [potential well](../../energy.md#potential-well), followed by a nonoscillatory tail through the barrier and right-hand region. The tail reaches zero at the right wall. There are no interior [nodes](../../dynamical-systems.md#node-dynamical-systems).
- $E_1$: two lobes of opposite sign in the left-hand [potential well](../../energy.md#potential-well), with one interior [node](../../dynamical-systems.md#node-dynamical-systems), followed by a nonoscillatory tail of the sign of the second lobe. Both the middle and right regions are [classically forbidden regions](../../mathematical-physics.md#classically-forbidden-region).
- $E_2$: sinusoidal behavior in both outer regions, joined through the nonoscillatory barrier. There are two interior [nodes](../../dynamical-systems.md#node-dynamical-systems) in total. The right-hand [wavelength](../../wave-equation.md#wavelength) is longer than the left-hand [wavelength](../../wave-equation.md#wavelength), because $E_2-V_R<E_2-V_L$.

For $E_0,E_1$, the right-hand piece is proportional to $\sinh[q_R(D-x)]$, rather than a pure decaying exponential: this enforces the finite-distance hard wall exactly. The barrier pieces likewise contain both exponential solutions. Their small tails are an instance of [quantum tunnelling](../../quantum-mechanics.md#quantum-tunnelling).

<a id="section-a/1/image-illustrative-lowest-three-wavefunctions-for-the-potential-ordering-in-a1"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1-a1-wavefunctions.png)

**[Figure 1](#section-a/1/image-illustrative-lowest-three-wavefunctions-for-the-potential-ordering-in-a1). Illustrative lowest three wavefunctions for the potential ordering in A1**.

This is an original illustrative calculation, with vertical lines marking only the region boundaries. It uses $D=1$, $a=0.4$, $b=0.6$, $V_L=0$, $V_R=0.62$, $V_B=0.82$, and $\hbar^2/(2mD^2)=0.002$ in arbitrary [energy](../../energy.md) units. Its lowest [energy eigenvalues](../../energy-eigenvalue.md) are approximately $0.098,0.384,0.696$, so it has exactly the required ordering. Here both [nodes](../../dynamical-systems.md#node-dynamical-systems) of the third [wavefunction](../../wave-function.md) happen to lie towards the left; its dominant lobe is on the right. These precise positions and relative amplitudes are illustrative: the original drawing supplies no numerical lengths, barrier heights, or [mass](../../classical-mechanics.md#mass), so it does not determine a unique quantitative [wavefunction](../../wave-function.md). The required sketch features are the matching, [curvature](../../differential-geometry.md#curvature), hard-wall zeros, and ordered [node](../../dynamical-systems.md#node-dynamical-systems) counts.

<h3 id="section-a/2">2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/2/solution">Solution</h4>

↑ **Parent:** [2](#section-a/2)

The [protons](../../physics.md#proton) at the [Large Hadron Collider](../../particle-accelerator.md#large-hadron-collider) are ultrarelativistic: their [energy](../../energy.md) is much greater than their [rest energy](../../special-relativity.md#rest-energy), about $0.938\,\mathrm{GeV}$. The [relativistic energy-momentum relation](../../special-relativity.md#energy-momentum-relation) therefore gives $pc\simeq E$. Using the [de Broglie wavelength](../../wave-function.md#de-broglie-wavelength),

$$
\lambda=\frac hp\simeq\frac{hc}{E}
=\frac{1.240\times10^{-6}\,\mathrm{eV\,m}}{6.5\times10^{12}\,\mathrm{eV}}
=1.91\times10^{-19}\,\mathrm m.
$$

Thus the conventional [de Broglie wavelength](../../wave-function.md#de-broglie-wavelength) estimate is **a distance of order $10^{-19}\,\mathrm m$**.

There is a conventional factor of $2\pi$ in interpreting this estimate. [Spatial resolution from momentum transfer](../../quantum-scattering.md#spatial-resolution-from-momentum-transfer) is often expressed as $\ell\sim\hbar c/Q$, where $Q$ is the transferred [momentum](../../momentum.md) multiplied by the [speed of light](../../special-relativity.md#speed-of-light). Taking $Q$ of order the beam [energy](../../energy.md) gives

$$
\ell\sim\frac{197.3\,\mathrm{MeV\,fm}}{6.5\times10^6\,\mathrm{MeV}}
=3.0\times10^{-20}\,\mathrm m.
$$

Both conventions describe the same characteristic scale up to $2\pi$. The beam [energy](../../energy.md) alone does not give an exact experimental [spatial resolution](../../optics.md#spatial-resolution): a particular collision probes a scale set by its actual [momentum transfer](../../quantum-scattering.md#momentum-transfer).

<h3 id="section-a/3">3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/3/solution">Solution</h4>

↑ **Parent:** [3](#section-a/3)

The [Born rule](../../wave-function.md#born-rule) uses the squared [modulus](../../complex-analysis.md#modulus) of the [wavefunction](../../wave-function.md), not its real part. Write $\psi=A[\sin x+i(1-\cos x)]$. Then

$$
|\psi|^2=|A|^2\bigl[\sin^2x+(1-\cos x)^2\bigr]
=2|A|^2(1-\cos x).
$$

[Wavefunction normalization](../../wave-function.md#wavefunction-normalization) requires

$$
1=2|A|^2\int_0^{2\pi}(1-\cos x)\,dx=4\pi|A|^2,
\qquad |A|^2=\frac1{4\pi}.
$$

Integrating the [probability density](../../wave-function.md#probability-density) over the required interval gives the dimensionless [probability](../../probability-theory.md#probability)

$$
\boxed{P=\frac1{2\pi}\int_0^{\pi/2}(1-\cos x)\,dx
=\frac{\pi/2-1}{2\pi}
=\frac14-\frac1{2\pi}\simeq0.09085.}
$$

Thus approximately **$9.08\%$** of [position measurements](../../quantum-measurement.md#position-measurement) fall in this interval.

<h3 id="section-a/4">4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/4/solution">Solution</h4>

↑ **Parent:** [4](#section-a/4)

Let $M$ denote an incident [muon](../../standard-model.md#muon) and $S$ a detector signal. The selected sample is conditioned on $S$. The [law of total probability](../../probability-space.md#law-of-total-probability) gives

$$
P(S)=P(S\mid M)P(M)+P(S\mid M^c)P(M^c)
=(0.90)(0.95)+(0.20)(0.05)=0.865.
$$

By [Bayes' theorem](../../probability-theory.md#bayes-theorem), the contamination, namely the [conditional probability](../../probability-theory.md#conditional-probability) that a selected particle is not a [muon](../../standard-model.md#muon), is

$$
\boxed{P(M^c\mid S)=\frac{(0.20)(0.05)}{0.865}
=0.01156\simeq1.16\%.}
$$

For example, per $10\,000$ incident particles the expected selected counts are $8550$ true [muons](../../standard-model.md#muon) and $100$ other particles. The denominator is the $8650$ selected particles; the rejected [muons](../../standard-model.md#muon) are outside this sample.

<h3 id="section-a/5">5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/5/solution">Solution</h4>

↑ **Parent:** [5](#section-a/5)

For the $110\,\mathrm{Hz}$ fundamental alone, the [Nyquist–Shannon sampling theorem](../../fourier-analysis.md#nyquist-shannon-sampling-theorem) places the limiting [sampling rate](../../wave-equation.md#sampling-rate) at twice that [frequency](../../wave.md#frequency):

$$
\boxed{f_s\gtrsim2(110\,\mathrm{Hz})=220\,\mathrm{samples\,s^{-1}}.}
$$

Use a rate strictly above this boundary for a sinusoid of unknown [phase](../../wave.md#phase-waves): exactly two samples per cycle can, for a particular [phase](../../wave.md#phase-waves), all fall at zero. If higher [Fourier harmonics](../../fourier-series.md#fourier-harmonic) are retained, the [sampling rate](../../wave-equation.md#sampling-rate) must instead exceed twice the highest retained [frequency](../../wave.md#frequency), or those components must be removed to prevent [aliasing](../../fourier-analysis.md#aliasing).

For a straightforward [discrete Fourier transform](../../discrete-fourier-transform.md) estimate, [Fourier frequency resolution](../../discrete-fourier-transform.md#fourier-frequency-resolution) obeys $\Delta f\sim1/T_{\mathrm{obs}}$. Resolving $0.07\,\mathrm{Hz}$ therefore suggests

$$
\boxed{T_{\mathrm{obs}}\gtrsim\frac1{0.07\,\mathrm{Hz}}=14.3\,\mathrm s.}
$$

At the limiting [sampling rate](../../wave-equation.md#sampling-rate) this is about $f_sT_{\mathrm{obs}}\simeq3143$ samples. These are the usual sampling and spectral-resolution estimates. The $14.3\,\mathrm s$ value is not a universal lower bound on single-tone [frequency estimation](../../statistical-inference.md#frequency-estimation): fitting a sinusoidal model with sufficiently low noise can estimate its [frequency](../../wave.md#frequency) more precisely than the spacing of [discrete Fourier transform](../../discrete-fourier-transform.md) bins. The question gives no noise level or estimator, so a sharper universal minimum time cannot be deduced.

## Section B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/a">a</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b6/a)

Use the [canonical commutation relations](../../quantum-mechanics.md#canonical-commutation-relation) $[\hat x,\hat p_x]=[\hat y,\hat p_y]=i\hbar$, with cross-coordinate [commutators](../../lie-algebra.md#commutator) zero. For either coordinate,

$$
[\hat a,\hat a^\dagger]=2\alpha\beta\hbar,
\qquad
\hat a^\dagger\hat a=\alpha^2\hat x^2+\beta^2\hat p_x^2-\alpha\beta\hbar.
$$

Thus $2\alpha\beta\hbar=1$. To obtain the required [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian), the ratio of its [position operator](../../quantum-mechanics.md#position-operator) and [momentum operator](../../quantum-mechanics.md#momentum-operator) coefficients must be preserved:

$$
\frac{\alpha^2}{\beta^2}=m^2\omega^2,
\qquad \alpha=m\omega\beta,
$$

where the positive root follows from the requested signs. Consequently

$$
\boxed{\alpha_x=\alpha_y=\sqrt{\frac{m\omega}{2\hbar}},
\qquad \beta_x=\beta_y=\frac1{\sqrt{2m\hbar\omega}}.}
$$

The [annihilation operators](../../quantum-harmonic-oscillator.md#annihilation-operator) are dimensionless; $\alpha$ has units of inverse length and $\beta$ has units of inverse [momentum](../../momentum.md). Operators belonging to different coordinates commute automatically. Writing the [number operators](../../quantum-harmonic-oscillator.md#number-operator) as $\hat N_j=\hat a_j^\dagger\hat a_j$, substitution gives

$$
\boxed{\hat H=\hbar\omega(\hat N_x+\hat N_y+1).}
$$

The constant is the sum of the two [zero-point energies](../../quantum-harmonic-oscillator.md#zero-point-energy) of this [two-dimensional isotropic harmonic oscillator](../../quantum-mechanics.md#two-dimensional-isotropic-harmonic-oscillator).

<h4 id="section-b/b6/b">b</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b6/b)

For either [number operator](../../quantum-harmonic-oscillator.md#number-operator) $\hat N=\hat a^\dagger\hat a$, positivity follows from

$$
\langle u|\hat N|u\rangle=\|\hat a|u\rangle\|^2\ge0.
$$

Hence an [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\nu$ cannot be negative. The [commutators](../../lie-algebra.md#commutator)

$$
[\hat N,\hat a]=-\hat a,\qquad [\hat N,\hat a^\dagger]=\hat a^\dagger
$$

show that $\hat a|\nu\rangle$, if nonzero, is an [eigenstate](../../energy-eigenvalue.md#eigenstate) with [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\nu-1$. For a normalized [eigenstate](../../energy-eigenvalue.md#eigenstate), $\|\hat a|\nu\rangle\|^2=\nu$.

If $\nu$ were not an integer, successive nonzero lowerings would eventually reach an [eigenstate](../../energy-eigenvalue.md#eigenstate) with $0<\nu'<1$. Its next lowering would have nonzero [norm](../../normed-vector-space.md#norm) but a negative [eigenvalue](../../linear-operator-theory.md#eigenvalue), contradicting positivity. The ladder must therefore terminate at $\nu=0$, with $\hat a|0\rangle=0$. Conversely, successive applications of the [creation operator](../../quantum-harmonic-oscillator.md#creation-operator) never vanish, because

$$
\|\hat a^\dagger|n\rangle\|^2=\langle n|(\hat N+1)|n\rangle=n+1>0.
$$

The normalizable bottom state exists explicitly: solving $\hat a\psi_0=0$ gives $\psi_0(x)\propto\exp[-m\omega x^2/(2\hbar)]$. Thus the [number operator](../../quantum-harmonic-oscillator.md#number-operator) has exactly the non-negative integer [eigenvalues](../../linear-operator-theory.md#eigenvalue).

Since the two coordinate [number operators](../../quantum-harmonic-oscillator.md#number-operator) commute, use the product [eigenstates](../../energy-eigenvalue.md#eigenstate) $|n_x,n_y\rangle$. Their [energy eigenvalues](../../energy-eigenvalue.md) are

$$
\boxed{E_{n_x,n_y}=\hbar\omega(n_x+n_y+1),\qquad n_x,n_y=0,1,2,\ldots.}
$$

At fixed $N=n_x+n_y$, the allowed pairs are $(0,N),(1,N-1),\ldots,(N,0)$. Thus the [energy level](../../quantum-mechanics.md#energy-level) $E_N=(N+1)\hbar\omega$ has [quantum degeneracy](../../quantum-mechanics.md#degenerate-energy-levels) $N+1$, and the [ground-state energy](../../quantum-mechanics.md#ground-state-energy) is $\hbar\omega$.

<h4 id="section-b/b6/c">c</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b6/c)

The [number operator](../../quantum-harmonic-oscillator.md#number-operator) [commutators](../../lie-algebra.md#commutator) established above imply that $\hat a_x^\dagger|n\rangle$ is proportional to $|n+1\rangle$ and $\hat a_x|n\rangle$ to $|n-1\rangle$. Their [norms](../../normed-vector-space.md#norm) determine the magnitudes of the proportionality constants:

$$
\|\hat a_x^\dagger|n\rangle\|^2
=\langle n|\hat a_x\hat a_x^\dagger|n\rangle=n+1,
\qquad
\|\hat a_x|n\rangle\|^2
=\langle n|\hat a_x^\dagger\hat a_x|n\rangle=n.
$$

Choose the [phase](../../wave.md#phase-waves) of the normalized ground [eigenstate](../../energy-eigenvalue.md#eigenstate) once, then define recursively

$$
|n+1\rangle=\frac{\hat a_x^\dagger|n\rangle}{\sqrt{n+1}},
\qquad
|n\rangle=\frac{(\hat a_x^\dagger)^n}{\sqrt{n!}}|0\rangle.
$$

This removes the otherwise arbitrary relative [phases](../../wave.md#phase-waves) of the [eigenstates](../../energy-eigenvalue.md#eigenstate). The [Hermitian adjoint](../../hilbert-space.md#adjoint-operator) relation then fixes the lowering coefficient with the same positive sign, giving

$$
\boxed{\hat a_x^\dagger|n\rangle=\sqrt{n+1}|n+1\rangle,
\qquad \hat a_x|n\rangle=\sqrt n|n-1\rangle.}
$$

At $n=0$, the second expression means the [zero vector](../../vector-space.md#zero-vector), $\hat a_x|0\rangle=0$; it does not introduce a physical state $|-1\rangle$.

<h4 id="section-b/b6/d">d</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b6/d)

Set $\hat B=\hat a_x^\dagger\hat a_y-\hat a_y^\dagger\hat a_x$. Taking the [Hermitian adjoint](../../hilbert-space.md#adjoint-operator) reverses the order of products, so $\hat B^\dagger=-\hat B$. [Complex conjugation](../../complex-analysis.md#complex-conjugation) also reverses the sign of $-i$, and therefore

$$
\hat Q^\dagger=i\hbar\hat B^\dagger=-i\hbar\hat B=\hat Q.
$$

Thus $\hat Q$ is a [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) on the usual [oscillator](../../wave.md#oscillator) states.

Using the coefficients in part (a), products containing two [position operators](../../quantum-mechanics.md#position-operator) or two [momentum operators](../../quantum-mechanics.md#momentum-operator) cancel in the difference. Cross-coordinate operators commute, leaving

$$
\hat B=2i\alpha\beta(\hat x\hat p_y-\hat y\hat p_x)
=\frac i\hbar(\hat x\hat p_y-\hat y\hat p_x).
$$

Hence

$$
\boxed{\hat Q=\hat x\hat p_y-\hat y\hat p_x=\hat L_z.}
$$

It is the component of [orbital angular momentum](../../quantum-mechanics.md#orbital-angular-momentum) perpendicular to the plane, with units $\mathrm{kg\,m^2\,s^{-1}}$ (equivalently $\mathrm{J\,s}$). The [rotational symmetry](../../linear-algebra.md#rotational-symmetry) of the [two-dimensional isotropic harmonic oscillator](../../quantum-mechanics.md#two-dimensional-isotropic-harmonic-oscillator) makes this a conserved [observable](../../quantum-system.md#observable); directly, each term in $\hat B$ preserves $N_x+N_y$, so $[\hat H,\hat Q]=0$.

<h4 id="section-b/b6/e">e</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/e/solution">Solution</h5>

↑ **Parent:** [E](#section-b/b6/e)

The specified [energy](../../energy.md) requires $n_x+n_y=2$, so the relevant [energy eigenspace](../../energy-eigenvalue.md#energy-eigenspace) has the [orthonormal basis](../../inner-product.md#orthonormal-basis)

$$
|2,0\rangle,\quad |1,1\rangle,\quad |0,2\rangle.
$$

Applying the [creation and annihilation operators](../../quantum-harmonic-oscillator.md#creation-and-annihilation-operators) gives

$$
\begin{aligned}
\hat Q|2,0\rangle&=i\sqrt2\hbar|1,1\rangle,\\
\hat Q|1,1\rangle&=-i\sqrt2\hbar|2,0\rangle+i\sqrt2\hbar|0,2\rangle,\\
\hat Q|0,2\rangle&=-i\sqrt2\hbar|1,1\rangle.
\end{aligned}
$$

Thus its [matrix](../../vector-space.md#matrix) in this ordered [basis](../../vector-space.md#basis) is

$$
Q=\hbar\begin{pmatrix}
0&-i\sqrt2&0\\
i\sqrt2&0&-i\sqrt2\\
0&i\sqrt2&0
\end{pmatrix}.
$$

Writing $q=\hbar\lambda$, the [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) gives $\lambda(\lambda^2-4)=0$. The possible [angular momentum](../../momentum.md#angular-momentum) [eigenvalues](../../linear-operator-theory.md#eigenvalue) are therefore

$$
\boxed{q=-2\hbar,\quad0,\quad+2\hbar.}
$$

For completeness, normalized simultaneous [energy](../../energy.md) and [angular momentum](../../momentum.md#angular-momentum) [eigenstates](../../energy-eigenvalue.md#eigenstate) are

$$
\begin{aligned}
|q=+2\hbar\rangle&=\tfrac12\bigl(|2,0\rangle+i\sqrt2|1,1\rangle-|0,2\rangle\bigr),\\
|q=0\rangle&=\tfrac1{\sqrt2}\bigl(|2,0\rangle+|0,2\rangle\bigr),\\
|q=-2\hbar\rangle&=\tfrac12\bigl(|2,0\rangle-i\sqrt2|1,1\rangle-|0,2\rangle\bigr).
\end{aligned}
$$

Each value occurs once in this [energy eigenspace](../../energy-eigenvalue.md#energy-eigenspace). Equivalently, [circular ladder operators of a two-dimensional oscillator](../../quantum-mechanics.md#circular-ladder-operators-of-a-two-dimensional-oscillator) give $\hat H=\hbar\omega(\hat N_++\hat N_-+1)$ and $\hat L_z=\hbar(\hat N_+-\hat N_-)$. With $N_++N_-=2$, the difference can only be $2,0,-2$.

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/a">a</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b7/a)

For a [particle in a ring](../../quantum-mechanics.md#particle-in-a-ring), the arc-length coordinate is $s=R\phi$. The tangential [kinetic energy](../../energy.md#kinetic-energy) is

$$
H=\frac{p_s^2}{2m}=\frac{L_z^2}{2mR^2}.
$$

The constraint removes radial motion; the constant [potential energy](../../energy.md#potential-energy) along the ring can be chosen as zero. The tangential [momentum operator](../../quantum-mechanics.md#momentum-operator) is $\hat p_s=-i\hbar\partial_s$, or equivalently the [angular momentum operator](../../angular-momentum-operator.md) is $\hat L_z=-i\hbar\partial_\phi$. Thus

$$
\boxed{\hat H=-\frac{\hbar^2}{2mR^2}\frac{\partial^2}{\partial\phi^2}.}
$$

Its physical domain has periodic [boundary conditions](../../differential-equation.md#boundary-condition), $\psi(\phi+2\pi)=\psi(\phi)$ and $\psi'(\phi+2\pi)=\psi'(\phi)$. These make the [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) [self-adjoint](../../linear-operator-theory.md#self-adjoint-operator) and reflect that $\phi$ and $\phi+2\pi$ describe the same point. No magnetic flux or additional angle-dependent [potential energy](../../energy.md#potential-energy) is present.

<h4 id="section-b/b7/b">b</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b7/b)

Solving the [time-independent Schrödinger equation](../../mathematical-physics.md#time-independent-schrodinger-equation) with $\psi\propto e^{ik\phi}$ gives $E=\hbar^2k^2/(2mR^2)$. The periodic [boundary condition](../../differential-equation.md#boundary-condition) requires $e^{2\pi ik}=1$, hence $k=n\in\mathbb Z$. With the angular integration measure $d\phi$, [wavefunction normalization](../../wave-function.md#wavefunction-normalization) gives

$$
\int_0^{2\pi}|A|^2\,d\phi=1,
$$

so a convenient [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis) is

$$
\boxed{u_n(\phi)=\frac{e^{in\phi}}{\sqrt{2\pi}},
\qquad E_n=\frac{\hbar^2n^2}{2mR^2},\qquad n\in\mathbb Z.}
$$

The $n=0$ [ground state](../../quantum-mechanics.md#ground-state) is nondegenerate. For each $|n|>0$, $u_n$ and $u_{-n}$ span a two-dimensional [energy eigenspace](../../energy-eigenvalue.md#energy-eigenspace); real [sine](../../geometry-and-topology.md#sine) and [cosine](../../geometry-and-topology.md#cosine) combinations are an equally valid [basis](../../vector-space.md#basis). These opposite-circulation [eigenstates](../../energy-eigenvalue.md#eigenstate) have [angular momentum](../../momentum.md#angular-momentum) $n\hbar$ and $-n\hbar$.

If instead the [wavefunction](../../wave-function.md) is normalized with respect to physical arc length $ds=R\,d\phi$, its expression is $e^{in\phi}/\sqrt{2\pi R}$. The two conventions describe the same [probability](../../probability-theory.md#probability), since $|u_n|^2d\phi=|u_n/\sqrt R|^2ds$. The remaining parts use $d\phi$.

<h4 id="section-b/b7/c">c</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b7/c)

Put $\epsilon=\hbar^2/(2mR^2)$. The two-particle product [energy eigenstates](../../energy-eigenvalue.md#energy-eigenstate) are

$$
u_{n_1}(\phi_1)u_{n_2}(\phi_2),\qquad E=\epsilon(n_1^2+n_2^2).
$$

Because the particles are distinguishable, $(n_1,n_2)$ and $(n_2,n_1)$ are distinct when $n_1\ne n_2$. Also, the signs of nonzero integers distinguish opposite [angular momenta](../../momentum.md#angular-momentum). The [quantum degeneracy](../../quantum-mechanics.md#degenerate-energy-levels) is therefore the number of ordered integer pairs at each sum of squares.

The first distinct [energy levels](../../quantum-mechanics.md#energy-level) are $0,\epsilon,2\epsilon,4\epsilon,5\epsilon,\ldots$. This ordering matters: $4\epsilon$ is the third excited level, while $5\epsilon$ is the fourth excited level.

- At $E=0$, only $(0,0)$ occurs: **$g_0=1$**.
- At the first excited level, $E=\epsilon$, the pairs are $(\pm1,0)$ and $(0,\pm1)$: **$g_1=4$**.
- At the fourth excited level, $E=5\epsilon$, the pairs are $(\pm1,\pm2)$ and $(\pm2,\pm1)$, with independent signs: **$g_4=8$**.
- At $E=25\epsilon$, the pairs are $(\pm5,0),(0,\pm5)$, contributing four, and $(\pm3,\pm4),(\pm4,\pm3)$, contributing eight: **$g_{25}=12$**.

These counts concern [energy eigenspaces](../../energy-eigenvalue.md#energy-eigenspace); arbitrary [quantum superpositions](../../quantum-system.md#quantum-superposition) within each one do not create additional independent states.

<h4 id="section-b/b7/d">d</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b7/d)

Identical [spin one-half](../../angular-momentum-operator.md#spin-one-half) particles are [fermions](../../tensor-product-of-quantum-systems.md#fermion). By [fermionic exchange symmetry](../../tensor-product-of-quantum-systems.md#fermi-dirac-statistics), the complete spatial-and-spin [wavefunction](../../wave-function.md) must change sign when the two particle labels are exchanged. Define the normalized antisymmetric [spin-one-half singlet state](../../angular-momentum-operator.md#spin-one-half-singlet-state)

$$
\chi_S=\frac{|\uparrow\rangle_1|\downarrow\rangle_2-|\downarrow\rangle_1|\uparrow\rangle_2}{\sqrt2},
$$

and the three symmetric [spin-one-half triplet states](../../angular-momentum-operator.md#spin-one-half-triplet-state)

$$
\chi_+=|\uparrow\rangle_1|\uparrow\rangle_2,\qquad
\chi_0=\frac{|\uparrow\rangle_1|\downarrow\rangle_2+|\downarrow\rangle_1|\uparrow\rangle_2}{\sqrt2},\qquad
\chi_-=|\downarrow\rangle_1|\downarrow\rangle_2.
$$

The [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) is independent of [spin](../../angular-momentum-operator.md#spin), so these spin functions carry no additional [energy](../../energy.md).

Both particles can occupy $u_0$ if their [spin](../../angular-momentum-operator.md#spin) factor is antisymmetric. The unique [ground state](../../quantum-mechanics.md#ground-state) [wavefunction](../../wave-function.md) is

$$
\boxed{\Psi_g(\phi_1,\phi_2)=u_0(\phi_1)u_0(\phi_2)\chi_S
=\frac1{2\pi}\chi_S,\qquad E_g=0,\qquad g_g=1.}
$$

Two equal-spin particles could not share this orbital, by the [Pauli exclusion principle](../../tensor-product-of-quantum-systems.md#pauli-exclusion-principle).

At the first excited [energy](../../energy.md), $E=\epsilon=\hbar^2/(2mR^2)$, one orbital is $u_0$ and the other is $u_s$ with $s=+1$ or $-1$. Define symmetric and antisymmetric normalized spatial functions

$$
\Phi_s^{\pm}(\phi_1,\phi_2)
=\frac{u_0(\phi_1)u_s(\phi_2)\pm u_s(\phi_1)u_0(\phi_2)}{\sqrt2}
=\frac{e^{is\phi_2}\pm e^{is\phi_1}}{2\pi\sqrt2}.
$$

For each $s$, all allowed [wavefunctions](../../wave-function.md) are spanned by

$$
\boxed{\Phi_s^+\chi_S,\qquad
\Phi_s^-\chi_+,\quad\Phi_s^-\chi_0,\quad\Phi_s^-\chi_-,\qquad s=\pm1.}
$$

There are $2(1+3)$ [orthonormal](../../inner-product.md#orthonormal-set) states, hence **first-excited-state degeneracy $g=8$**. In each product, exactly one factor is antisymmetric, ensuring the required total [fermionic exchange symmetry](../../tensor-product-of-quantum-systems.md#fermi-dirac-statistics).

## Section C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-c/c8">C8</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c8/a">a</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c8/a)

The original apparatus has two small masses at distance $L/2$ from the suspension axis. Neglecting the rod's [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia), their total [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia) is $I=2m(L/2)^2=mL^2/2$, consistent with the supplied [torsion pendulum](../../classical-mechanics.md#torsion-pendulum) period. Treat $m$ and $L$ as exact because no uncertainties are specified. Rearranging the period relation gives

$$
\kappa=\frac{2\pi^2mL^2}{T^2}
=\frac{2\pi^2(0.038\,\mathrm{kg})(0.100\,\mathrm m)^2}{(498.2\,\mathrm s)^2}
=3.02208\times10^{-8}\,\mathrm{N\,m\,rad^{-1}}.
$$

The [torsion constant](../../classical-mechanics.md#torsion-constant) is a restoring [torque](../../momentum.md#torque) per unit [angle](../../geometry-and-topology.md#angle). In dimensional calculations the radian is dimensionless.

Using first-order [propagation of uncertainty](../../wave-equation.md#propagation-of-uncertainty), with the quoted period uncertainty interpreted as a [standard uncertainty](../../physics.md#standard-uncertainty),

$$
\sigma_\kappa=\left|\frac{d\kappa}{dT}\right|\sigma_T
=\frac{2\kappa}{T}\sigma_T,
\qquad \frac{\sigma_\kappa}{\kappa}=\frac{2(6.0)}{498.2}=0.02409.
$$

Consequently

$$
\boxed{\kappa=(3.022\pm0.073)\times10^{-8}\,\mathrm{N\,m\,rad^{-1}}.}
$$

<h4 id="section-c/c8/b">b</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c8/b)

Rearrange the given [torsion balance](../../classical-mechanics.md#torsion-balance) equilibrium relation as

$$
\theta=\frac{GmML}{\kappa}\frac1{r^2}.
$$

A useful choice, preserving equal measurement uncertainties on the vertical axis, is

$$
\boxed{y=\theta,\qquad x=r^{-2},\qquad c=\frac{GmML}{\kappa}.}
$$

With [angle](../../geometry-and-topology.md#angle) measured in radians, $y$ is dimensionless and $x$ has units $\mathrm{m^{-2}}$, so $c$ has units $\mathrm{m^2}$, as required. The four $x$ values, in the order of the original table, are

$$
(3906.25,\ 3086.41975,\ 2066.11570,\ 976.56250)\,\mathrm{m^{-2}}.
$$

The corresponding $y$ values are $(0.066,0.055,0.044,0.025)$, each with [standard uncertainty](../../physics.md#standard-uncertainty) $\sigma_y=0.002$. The uncertainty of $x$ is negligible by assumption, making [linear regression through the origin](../../normal-linear-model.md#linear-regression-through-the-origin) appropriate for the proposed model.

<h4 id="section-c/c8/c">c</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c8/c)

All four [angle](../../geometry-and-topology.md#angle) measurements have the same [standard uncertainty](../../physics.md#standard-uncertainty), so [ordinary least squares](../../normal-linear-model.md#ordinary-least-squares) minimizes

$$
S(c)=\sum_{i=1}^4(y_i-cx_i)^2.
$$

[Differentiation](../../calculus.md#differentiation) gives

$$
\frac{dS}{dc}=-2\sum_i x_i(y_i-cx_i)=0,
\qquad \frac{d^2S}{dc^2}=2\sum_i x_i^2>0.
$$

Thus the unique minimum is

$$
\boxed{\hat c=\frac{\sum_i x_iy_i}{\sum_i x_i^2}
=\frac{\overline{xy}}{\overline{xx}}.}
$$

The overbars denote [sample means](../../variance.md#sample-mean) over the four observations. Numerically,

$$
\sum_i x_iy_i=542.888740\,\mathrm{m^{-2}},\qquad
\sum_i x_i^2=3.00072844\times10^7\,\mathrm{m^{-4}},
$$

so

$$
\boxed{\hat c=1.80919\times10^{-5}\,\mathrm{m^2},\qquad
\hat G=\frac{\kappa\hat c}{mML}=9.59\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.}
$$

The fixed $x_i$ have negligible uncertainty. Assuming [independent](../../random-variable.md#independent-random-variables) errors in the four $y_i$, [propagation of uncertainty](../../wave-equation.md#propagation-of-uncertainty) in quadrature gives

$$
\sigma_{\hat c}^2=\sum_i\left(\frac{\partial\hat c}{\partial y_i}\right)^2\sigma_y^2
=\frac{\sigma_y^2\sum_i x_i^2}{(\sum_i x_i^2)^2}
=\frac{\sigma_y^2}{\sum_i x_i^2}.
$$

Hence

$$
\boxed{\sigma_{\hat c}=3.65\times10^{-7}\,\mathrm{m^2},\qquad
\hat c=(1.809\pm0.037)\times10^{-5}\,\mathrm{m^2}.}
$$

If the period measurement is [independent](../../random-variable.md#independent-random-variables) of the [angle](../../geometry-and-topology.md#angle) measurements, including its calibration uncertainty gives

$$
\frac{\sigma_G}{\hat G}=\sqrt{\left(\frac{\sigma_{\hat c}}{\hat c}\right)^2+
\left(\frac{\sigma_\kappa}{\kappa}\right)^2}=0.0314,
\qquad \hat G=(9.59\pm0.30)\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.
$$

This last uncertainty includes the stated random measurement errors only. Whether the model describes the data must be checked before treating it as a reliable measurement of the [gravitational constant](../../newton-s-law-of-universal-gravitation.md#gravitational-constant).

<h4 id="section-c/c8/d">d</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/d/solution">Solution</h5>

↑ **Parent:** [D](#section-c/c8/d)

Assume independent [normally distributed](../../probability-distribution.md#normal-distribution) [angle](../../geometry-and-topology.md#angle) errors with known [standard deviation](../../variance.md#standard-deviation) $\sigma_y=0.002$. The relevant [chi-squared test](../../statistical-inference.md#chi-squared-test) uses the sum of squared standardized residuals,

$$
\chi^2=\sum_i\frac{(y_i-y_{\mathrm{fit},i})^2}{\sigma_y^2}.
$$

For the model through the origin, the predictions and residuals, expressed in milliradians, are

$$
\begin{array}{c|rrrr}
r\ (\mathrm{mm})&16&18&22&32\\\hline
\hat c x\ (\mathrm{mrad})&70.6715&55.8392&37.3800&17.6679\\
y-\hat c x\ (\mathrm{mrad})&-4.6715&-0.8392&6.6200&7.3321
\end{array}
$$

Consequently $\chi_0^2=30.0280$. There are $4-1=3$ [statistical degrees of freedom](../../statistical-inference.md#statistical-degrees-of-freedom). The upper-tail [P-value](../../statistical-hypothesis-test.md#p-value) is approximately $1.36\times10^{-6}$; equivalently the value greatly exceeds the $5\%$ critical value $7.815$. The zero-intercept model is strongly rejected under the stated errors.

For the alternative [linear regression](../../linear-regression.md), minimize $\sum_i(y_i-c'x_i-d)^2$. Setting both partial [derivatives](../../calculus.md#derivative) to zero gives the [normal equations](../../normal-linear-model.md#normal-equation), whose solution is

$$
\hat c'=\frac{\sum_i(x_i-\bar x)(y_i-\bar y)}{S_{xx}},
\qquad \hat d=\bar y-\hat c'\bar x,
\qquad S_{xx}=\sum_i(x_i-\bar x)^2.
$$

For these data $\bar x=2508.83699\,\mathrm{m^{-2}}$, $\bar y=0.0475$, and $S_{xx}=4.830232\times10^6\,\mathrm{m^{-4}}$. This yields

$$
\boxed{\hat c'=1.37074\times10^{-5}\,\mathrm{m^2},\qquad
\hat d=0.0131105=13.1105\,\mathrm{mrad}.}
$$

The new predictions are $(66.6548,55.4171,41.4315,26.4966)\,\mathrm{mrad}$, with residuals $(-0.6548,-0.4171,2.5685,-1.4966)\,\mathrm{mrad}$. Therefore

$$
\boxed{\chi_1^2=2.35998,\qquad \nu=4-2=2,\qquad p=0.307.}
$$

The affine model is compatible with the data. Allowing for its additional fitted parameter, the decrease $\Delta\chi^2=27.668$ has a [chi-squared distribution](../../probability-distribution.md#chi-squared-distribution) with one [statistical degree of freedom](../../statistical-inference.md#statistical-degrees-of-freedom) under the nested zero-intercept hypothesis, corresponding to $p\simeq1.44\times10^{-7}$. Thus **the model with a fitted intercept provides the better description**, rather than merely lowering the residual by adding a parameter.

With the measurement variance treated as known, the coefficient uncertainties are

$$
\sigma_{c'}=\frac{\sigma_y}{\sqrt{S_{xx}}}=9.10\times10^{-7}\,\mathrm{m^2},
\qquad
\sigma_d=\sigma_y\sqrt{\frac14+\frac{\bar x^2}{S_{xx}}}=0.0024925.
$$

Hence **$d=(13.11\pm2.49)\,\mathrm{mrad}$**, about $5.26$ [standard deviations](../../variance.md#standard-deviation) above zero. A positive constant [systematic error](../../physics.md#systematic-error) in the angular zero, or an additional nearly constant [torque](../../momentum.md#torque), could account for it. Its presence is evidence against the ideal zero-intercept model; four points alone do not identify the physical cause uniquely. A calibration error in $\kappa$ only rescales the inferred [gravitational constant](../../newton-s-law-of-universal-gravitation.md#gravitational-constant) and cannot remove this residual pattern.

Using the fitted slope after allowing for this offset would give $G'=\kappa\hat c'/(mML)=(7.27\pm0.51)\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, with the period and slope errors combined in quadrature. This is conditional on the constant-offset model.

## Section D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-d/d9">D9</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d9/solution">Solution</h4>

↑ **Parent:** [D9](#section-d/d9)

Time dependence in [quantum mechanics](../../quantum-mechanics.md) describes how a prepared [quantum state](../../quantum-system.md#quantum-state) changes and thereby changes the [probabilities](../../probability-theory.md#probability) of later measurements. For an isolated system, the [Schrödinger picture](../../quantum-system.md#schrodinger-picture) assigns this evolution to a state vector $|\psi(t)\rangle$, governed by the [Time-dependent Schrödinger equation](../../mathematical-physics.md#time-dependent-schrodinger-equation)

$$
i\hbar\frac{d}{dt}|\psi(t)\rangle=\hat H(t)|\psi(t)\rangle.
$$

The [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) is a [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator); it has units of [energy](../../energy.md), while $\hbar$ has units of [action](../../lagrangian-mechanics.md#action), so $\hat H/\hbar$ has units of inverse time. For a particle with [potential energy](../../energy.md#potential-energy) $V(\mathbf r,t)$, this becomes

$$
i\hbar\partial_t\psi(\mathbf r,t)
=\left[-\frac{\hbar^2}{2m}\nabla^2+V(\mathbf r,t)\right]\psi(\mathbf r,t).
$$

Given a suitable initial [wavefunction](../../wave-function.md) and the physical [boundary conditions](../../differential-equation.md#boundary-condition), this first-order equation determines its subsequent propagation. Its [linearity](../../vector-space.md#linearity) means that the evolution of a [quantum superposition](../../quantum-system.md#quantum-superposition) is the corresponding [quantum superposition](../../quantum-system.md#quantum-superposition) of evolved states.

For a real [potential energy](../../energy.md#potential-energy), this equation and its [complex conjugate](../../complex-analysis.md#complex-conjugate) imply the local [continuity equation](../../mathematical-physics.md#continuity-equation)

$$
\partial_t\rho+\nabla\cdot\mathbf j=0,
\qquad \rho=|\psi|^2,
\qquad \mathbf j=\frac{\hbar}{m}\operatorname{Im}(\psi^*\nabla\psi).
$$

Here $\rho$ is the [probability density](../../wave-function.md#probability-density) and $\mathbf j$ the [probability current](../../wave-function.md#probability-current). Vanishing net boundary flux preserves [wavefunction normalization](../../wave-function.md#wavefunction-normalization), as required by the [Born rule](../../wave-function.md#born-rule).

The [time-evolution operator](../../quantum-system.md#time-evolution-operator) packages the solution for every initial state:

$$
|\psi(t)\rangle=U(t,t_0)|\psi(t_0)\rangle,
\qquad i\hbar\partial_tU(t,t_0)=\hat H(t)U(t,t_0),
\qquad U(t_0,t_0)=I.
$$

Because $\hat H^\dagger=\hat H$, differentiation gives

$$
\frac d{dt}(U^\dagger U)
=\frac i\hbar U^\dagger\hat H U-\frac i\hbar U^\dagger\hat H U=0.
$$

Therefore $U^\dagger U=I$: this is [unitary time evolution](../../quantum-system.md#unitary-time-evolution), preserving [inner products](../../inner-product.md) and all state [norms](../../normed-vector-space.md#norm). It is reversible, with $U(t,t_0)^{-1}=U(t_0,t)=U(t,t_0)^\dagger$, and obeys the composition law $U(t_2,t_0)=U(t_2,t_1)U(t_1,t_0)$.

For a time-independent [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian), the solution is the [operator exponential](../../linear-operator-theory.md#operator-exponential)

$$
\boxed{U(t,t_0)=\exp[-i\hat H(t-t_0)/\hbar].}
$$

If the [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) varies with time, the analogous simple exponential of its integral is valid when $[\hat H(t),\hat H(t')]=0$ for all relevant times. Otherwise [time ordering](../../perturbative-quantum-field-theory.md#time-ordering) is essential:

$$
U(t,t_0)=\mathcal T\exp\left[-\frac i\hbar\int_{t_0}^t\hat H(t')\,dt'\right].
$$

The meaning is explicit in the first terms of the ordered series,

$$
U=I-\frac i\hbar\int_{t_0}^t\hat H(t_1)\,dt_1
-\frac1{\hbar^2}\int_{t_0}^t dt_1\int_{t_0}^{t_1}dt_2\,\hat H(t_1)\hat H(t_2)+\cdots:
$$

the later-time operator stands on the left. In the position representation, the same propagation is expressed by the [quantum-mechanical propagator](../../quantum-system.md#quantum-mechanical-propagator)

$$
K(\mathbf r,t;\mathbf r',t_0)=\langle\mathbf r|U(t,t_0)|\mathbf r'\rangle,
\qquad
\psi(\mathbf r,t)=\int K(\mathbf r,t;\mathbf r',t_0)\psi(\mathbf r',t_0)\,d^3r'.
$$

Its initial value is the [Dirac delta function](../../distribution-theory.md#dirac-delta-function) $\delta^3(\mathbf r-\mathbf r')$.

A time-independent [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) has [energy eigenstates](../../energy-eigenvalue.md#energy-eigenstate) satisfying $\hat H|n\rangle=E_n|n\rangle$. A single such initial state evolves as

$$
|\psi_n(t)\rangle=e^{-iE_n(t-t_0)/\hbar}|n\rangle.
$$

It is a [stationary state](../../quantum-system.md#stationary-state): its [global phase](../../quantum-system.md#global-phase) changes, but its [probability density](../../wave-function.md#probability-density) and the distributions of time-independent [observables](../../quantum-system.md#observable) do not. Its [energy](../../energy.md) is sharp. Any [quantum superposition](../../quantum-system.md#quantum-superposition) entirely within one degenerate [energy eigenspace](../../energy-eigenvalue.md#energy-eigenspace) also acquires one common [global phase](../../quantum-system.md#global-phase) and is stationary. Stationarity does not require zero [probability current](../../wave-function.md#probability-current); for instance, $u_n(\phi)=e^{in\phi}/\sqrt{2\pi}$ on the ring has a constant density and persistent circulation when $n\ne0$.

An arbitrary normalized state can instead contain different [energy eigenvalues](../../energy-eigenvalue.md):

$$
|\psi(t)\rangle=\sum_n c_ne^{-iE_n(t-t_0)/\hbar}|n\rangle,
\qquad \sum_n|c_n|^2=1.
$$

A [continuous spectrum](../../linear-operator-theory.md#continuous-spectrum) requires corresponding integrals. For the discrete case, an [energy measurement](../../wave-function.md#energy-measurement) gives $E_n$ with fixed [probability](../../probability-theory.md#probability) $|c_n|^2$ (summed over degeneracies), but relative [quantum phases](../../quantum-system.md#quantum-phase) change with time. Consequently

$$
|\psi(\mathbf r,t)|^2=\sum_{m,n}c_m^*c_n\phi_m^*(\mathbf r)\phi_n(\mathbf r)
 e^{i(E_m-E_n)(t-t_0)/\hbar}.
$$

The [interference](../../physical-optics.md#interference-wave-propagation) terms can oscillate at [angular frequencies](../../lagrangian-mechanics.md#angular-frequency) $(E_m-E_n)/\hbar$. For two populated [energy levels](../../quantum-mechanics.md#energy-level), this supplies a characteristic period $2\pi\hbar/|E_m-E_n|$ when the [interference](../../physical-optics.md#interference-wave-propagation) term is nonzero. Thus fixed energy populations do not imply a stationary spatial distribution.

For a normalized state and an [observable](../../quantum-system.md#observable) $\hat A(t)$, its [expectation value](../../quantum-system.md#expectation-value) is

$$
\langle A\rangle_t=\langle\psi(t)|\hat A(t)|\psi(t)\rangle.
$$

This is the statistical [mean](../../expected-value.md) over repeated preparations and measurements. In an [eigenbasis](../../linear-operator-theory.md#eigenbasis) of [energy eigenstates](../../energy-eigenvalue.md#energy-eigenstate) for a time-independent [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) and a time-independent $\hat A$,

$$
\langle A\rangle_t=\sum_{m,n}c_m^*c_n A_{mn}e^{i(E_m-E_n)(t-t_0)/\hbar}.
$$

Only [matrix elements](../../vector-space.md#matrix-element) connecting different [energies](../../energy.md) can generate these oscillations. If $[\hat A,\hat H]=0$, its [expectation value](../../quantum-system.md#expectation-value) is constant for every initial state, provided it has no explicit time dependence.

Differentiating the [expectation value](../../quantum-system.md#expectation-value) and substituting the [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation) for both the bra and ket proves the general [Ehrenfest theorem](../../quantum-mechanics.md#ehrenfest-theorem):

$$
\begin{aligned}
\frac d{dt}\langle A\rangle
&=\langle\dot\psi|\hat A|\psi\rangle+
\left\langle\frac{\partial\hat A}{\partial t}\right\rangle+
\langle\psi|\hat A|\dot\psi\rangle\\
&=\frac i\hbar\langle\hat H\hat A-\hat A\hat H\rangle+
\left\langle\frac{\partial\hat A}{\partial t}\right\rangle.
\end{aligned}
$$

Equivalently,

$$
\boxed{\frac d{dt}\langle A\rangle
=\frac1{i\hbar}\langle[\hat A,\hat H]\rangle+
\left\langle\frac{\partial\hat A}{\partial t}\right\rangle.}
$$

These manipulations require the state to lie in the relevant [operator domains](../../vector-space.md#operator-domain). Taking $\hat A=\hat H$ gives $d\langle H\rangle/dt=\langle\partial_t\hat H\rangle$, so [energy](../../energy.md) is conserved under a time-independent [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian).

For $\hat H=\hat p^2/(2m)+V(\hat x)$, the [canonical commutation relation](../../quantum-mechanics.md#canonical-commutation-relation) gives

$$
[\hat x,\hat H]=\frac{i\hbar}{m}\hat p,
\qquad [\hat p,\hat H]=-i\hbar V'(\hat x).
$$

Hence the particularly useful position-and-momentum form of [Ehrenfest theorem](../../quantum-mechanics.md#ehrenfest-theorem) is

$$
\boxed{\frac d{dt}\langle x\rangle=\frac{\langle p\rangle}{m},
\qquad \frac d{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

It resembles [Newton's second law](../../force.md#newton-s-second-law), but the mean [force](../../force.md) generally differs from the [force](../../force.md) at the mean position. If a narrow [wave packet](../../dispersion-relation.md#wave-packet) samples a region where the [force](../../force.md) varies little, $\langle V'(x)\rangle\simeq V'(\langle x\rangle)$ gives approximate classical motion. For a quadratic [potential energy](../../energy.md#potential-energy) this replacement is exact. In particular the [quantum harmonic oscillator](../../quantum-harmonic-oscillator.md) obeys

$$
\frac{d^2}{dt^2}\langle x\rangle=-\omega^2\langle x\rangle,
\qquad
\langle x\rangle_t=\langle x\rangle_{t_0}\cos\omega\tau+
\frac{\langle p\rangle_{t_0}}{m\omega}\sin\omega\tau,
\qquad \tau=t-t_0.
$$

The centroid follows the classical [harmonic oscillator](../../classical-mechanics.md#simple-harmonic-motion), although this does not specify the full evolving [wavefunction](../../wave-function.md) or its width.

The [Heisenberg picture](../../quantum-system.md#heisenberg-picture) expresses the same physics by assigning evolution to [observables](../../quantum-system.md#observable) instead:

$$
\hat A_H(t)=U^\dagger(t,t_0)\hat A_S(t)U(t,t_0),
\qquad |\psi_H\rangle=|\psi(t_0)\rangle.
$$

The [expectation value](../../quantum-system.md#expectation-value) is unchanged, and differentiation yields $d\hat A_H/dt=(i/\hbar)[\hat H_H,\hat A_H]+U^\dagger(\partial_t\hat A_S)U$. Thus state propagation, evolving [expectation values](../../quantum-system.md#expectation-value), and the classical correspondence in [Ehrenfest theorem](../../quantum-mechanics.md#ehrenfest-theorem) are mutually consistent descriptions of the same [unitary time evolution](../../quantum-system.md#unitary-time-evolution).

## ↑ Ancestors (11)

1. [2022](../2022.md)
2. [Past exam of the physics A course of the University of Cambridge](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge.md)
3. [Physics A course of the University of Cambridge](../../university-of-cambridge.md#physics-a-course-of-the-university-of-cambridge)
4. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
