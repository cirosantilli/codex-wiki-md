# Paper 2

↑ **Parent:** [2011](../2011.md)

Original paper: [FOI release, physical PDF pages 21–27, printed pages 1–7](https://www.whatdotheyknow.com/request/physics_past_papers_23/response/3514893/attach/4/FOI%202026%20628%20Smith%20materials.pdf?cookie_passthrough=1). The solutions include every optional question and note topic.

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
    - [Solution](#section-b/b6/solution)
  - [B7](#section-b/b7)
    - [Solution](#section-b/b7/solution)
  - [B8](#section-b/b8)
    - [Solution](#section-b/b8/solution)
    - [a](#section-b/b8/a)
      - [Solution](#section-b/b8/a/solution)
    - [b](#section-b/b8/b)
      - [Solution](#section-b/b8/b/solution)
  - [B9](#section-b/b9)
    - [Solution](#section-b/b9/solution)
- [Section C](#section-c)
  - [C10](#section-c/c10)
    - [Solution](#section-c/c10/solution)
  - [C11](#section-c/c11)
    - [a](#section-c/c11/a)
      - [Solution](#section-c/c11/a/solution)
    - [b](#section-c/c11/b)
      - [Solution](#section-c/c11/b/solution)
    - [c](#section-c/c11/c)
      - [Solution](#section-c/c11/c/solution)
- [Section D](#section-d)
  - [D12](#section-d/d12)
    - [a](#section-d/d12/a)
      - [Solution](#section-d/d12/a/solution)
    - [b](#section-d/d12/b)
      - [Solution](#section-d/d12/b/solution)
    - [c](#section-d/d12/c)
      - [Solution](#section-d/d12/c/solution)
  - [D13](#section-d/d13)
    - [Solution](#section-d/d13/solution)
    - [a](#section-d/d13/a)
      - [Solution](#section-d/d13/a/solution)
    - [b](#section-d/d13/b)
      - [Solution](#section-d/d13/b/solution)

## Section A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-a/1">1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/1/solution">Solution</h4>

↑ **Parent:** [1](#section-a/1)

For a [normalizable](../../wave-function.md#normalizable-wavefunction) state take $a>0$. [inverse construction of a quantum potential](../../mathematical-physics.md#inverse-construction-of-a-quantum-potential) gives $V=E+\hbar^2\Psi''/(2m\Psi)$. [differentiation](../../calculus.md#differentiation) yields $\Psi''/\Psi=16a^2x^6-12ax^2$, so the chosen [potential energy](../../energy.md#potential-energy) zero fixes $E=0$. Thus

$$
\boxed{V(x)=\frac{8\hbar^2a^2}{m}x^6-\frac{6\hbar^2a}{m}x^2,\qquad E=0.}
$$

This [energy](../../energy.md) lies above the negative minima of the [potential energy](../../energy.md#potential-energy); its zero value does not mean zero [kinetic energy](../../energy.md#kinetic-energy). The [nodeless eigenfunction](../../linear-operator-theory.md#nodeless-eigenfunction) is the [ground state](../../quantum-mechanics.md#ground-state).

<h3 id="section-a/2">2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/2/solution">Solution</h4>

↑ **Parent:** [2](#section-a/2)

The [Sturm oscillation theorem](../../sturm-liouville-theory.md#sturm-oscillation-theorem) gives **three [nodes of a wavefunction](../../wave-function.md#node-of-a-wavefunction)** for the fourth [bound state](../../quantum-system.md#bound-state). [reflection symmetry](../../physics.md#reflection-symmetry) and [nondegeneracy of one-dimensional bound states](../../mathematical-physics.md#nondegeneracy-of-one-dimensional-bound-states) make it **odd**: one [node of a wavefunction](../../wave-function.md#node-of-a-wavefunction) is at the centre, and the other two lie at opposite positions. In each flat allowed region the [wavefunction](../../wave-function.md) is a [sinusoid](../../geometry-and-topology.md#sinusoid), with $k=\sqrt{2m(E-V)}/\hbar$; its [wavelength](../../wave-equation.md#wavelength) is shortest in the central, deepest region. Outside the well it decays exponentially, with opposite signs on the two sides. Both $\Psi$ and $\Psi'$ remain continuous at every finite step, as required by [wavefunction matching at a finite potential step](../../mathematical-physics.md#wavefunction-matching-at-a-finite-potential-step); only the curvature jumps. In particular, the [wavefunction](../../wave-function.md) need not vanish at a step.

<a id="section-a/2/image-fourth-bound-state"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2-stepped-state.png)

**[Figure 1](#section-a/2/image-fourth-bound-state). Fourth bound state**.

This original [wavefunction matching at a finite potential step](../../mathematical-physics.md#wavefunction-matching-at-a-finite-potential-step) illustration uses freely chosen well dimensions and [energies](../../energy.md). It shows the required [parity](../../quantum-mechanics.md#parity), node count, [wavelength](../../wave-equation.md#wavelength) ordering and decaying tails; the source drawing supplies no numerical scale from which to fix exact node positions.

<h3 id="section-a/3">3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/3/solution">Solution</h4>

↑ **Parent:** [3](#section-a/3)

The [canonical commutation relation](../../quantum-mechanics.md#canonical-commutation-relation) is $[p_x,x]=-i\hbar I$. Applying the [commutator product rule](../../lie-algebra.md#commutator-product-rule) on a common [operator domain](../../vector-space.md#operator-domain),

$$
[p_x^2,x]=p_x[p_x,x]+[p_x,x]p_x
=\boxed{-2i\hbar p_x}.
$$

Equivalently, applying both sides to a twice differentiable [test function](../../distribution-theory.md#test-function) gives $-\hbar^2[(xf)''-xf'']=-2\hbar^2f'$, the same result.

<h3 id="section-a/4">4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/4/solution">Solution</h4>

↑ **Parent:** [4](#section-a/4)

The central estimate is $z=3.2743$. [propagation of uncertainty](../../wave-equation.md#propagation-of-uncertainty) must include the occurrence of $x$ in both numerator and denominator. With angular [derivatives](../../calculus.md#derivative) measured per [radian](../../geometry-and-topology.md#radian),

$$
z_x=\frac{\sec^2(x+y)}{\tan x}-\frac{\tan(x+y)}{\sin^2x}=-3.5382,\qquad
z_y=\frac{\sec^2(x+y)}{\tan x}=6.6497.
$$

Interpreting the two quoted errors as independent [standard deviations](../../variance.md#standard-deviation), convert them to [radians](../../geometry-and-topology.md#radian) before calculating

$$
\sigma_z^2=z_x^2(4\pi/180)^2+z_y^2(3\pi/180)^2,
\qquad \boxed{z\simeq3.27\pm0.43}.
$$

If the quoted errors are instead absolute bounds, the first-order worst-case estimate is $|\delta z|\lesssim |z_x|\delta x+|z_y|\delta y=0.60$. Correlated errors add $2z_xz_y\operatorname{Cov}(x,y)$ to the [variance](../../variance.md). Treating $x+y$ and $x$ as independent would lose their shared [measurement uncertainty](../../physics.md#measurement-uncertainty).

<h3 id="section-a/5">5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/5/solution">Solution</h4>

↑ **Parent:** [5](#section-a/5)

In the [high-resolution quantization approximation](../../electrical-engineering.md#high-resolution-quantization-approximation), a smooth input distribution varies little across one conversion interval, so [rounding](../../numerical-analysis.md#rounding) to the nearest level gives an approximately [uniform quantization error](../../electrical-engineering.md#uniform-quantization-error) $\epsilon\in[-\Delta V/2,\Delta V/2]$. Therefore

$$
\langle\epsilon\rangle=0,\qquad
\langle\epsilon^2\rangle=\frac1{\Delta V}\int_{-\Delta V/2}^{\Delta V/2}\epsilon^2\,d\epsilon
=\frac{\Delta V^2}{12},\qquad
\boxed{\epsilon_{\rm rms}=\frac{\Delta V}{\sqrt{12}}}.
$$

The input must stay within the [analogue-to-digital converter](../../electrical-engineering.md#analog-to-digital-converter)'s range. A large [standard deviation](../../variance.md#standard-deviation) alone does not guarantee [uniform quantization error](../../electrical-engineering.md#uniform-quantization-error): an input concentrated exactly on widely separated conversion levels has zero error. Truncation without a half-step correction also has a different mean and [root mean square](../../analysis.md#root-mean-square).

## Section B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/solution">Solution</h4>

↑ **Parent:** [B6](#section-b/b6)

For each mode in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system), $[a_i,a_j^\dagger]=\delta_{ij}$ and $a_i^\dagger a_i=H_i/(\hbar\omega)-1/2$. Consequently the [two-dimensional isotropic harmonic oscillator](../../quantum-mechanics.md#two-dimensional-isotropic-harmonic-oscillator) has

$$
\boxed{H=\hbar\omega(N_x+N_y+1)},\qquad N_i=a_i^\dagger a_i,\qquad E_{kl}=\hbar\omega(k+l+1).
$$

The normalized actions of the [creation and annihilation operators](../../quantum-harmonic-oscillator.md#creation-and-annihilation-operators) are

$$
a_x|k,l\rangle=\sqrt{k}\,|k-1,l\rangle,\qquad
a_y^\dagger|k,l\rangle=\sqrt{l+1}\,|k,l+1\rangle,\qquad
a_x|0,l\rangle=0.
$$

Invert their definitions as $x=\sqrt{\hbar/(2m\omega)}(a_x+a_x^\dagger)$ and $p_x=i\sqrt{m\hbar\omega/2}(a_x^\dagger-a_x)$, and similarly for $y$. [linear operators](../../vector-space.md#linear-operator) belonging to different coordinates commute, so substitution into $L_z=xp_y-yp_x$ gives

$$
L_z=\frac{i\hbar}{2}\big[(a_x+a_x^\dagger)(a_y^\dagger-a_y)-(a_y+a_y^\dagger)(a_x^\dagger-a_x)\big]
=\boxed{-i\hbar(a_x^\dagger a_y-a_y^\dagger a_x)}.
$$

Each term transfers one excitation between the two modes: $[N_x+N_y,a_x^\dagger a_y]=(1-1)a_x^\dagger a_y=0$, and likewise for its adjoint. Thus $[H,L_z]=0$ and, with no explicit time dependence, $dL_z/dt=(i/\hbar)[H,L_z]=0$. This is [conservation of angular momentum](../../momentum.md#conservation-of-angular-momentum) under [planar rotations](../../linear-algebra.md#planar-rotation).

Finally $L_z|1,0\rangle=i\hbar|0,1\rangle$ and $L_z|0,1\rangle=-i\hbar|1,0\rangle$. Hence

$$
\boxed{L_z\big(|1,0\rangle+i|0,1\rangle\big)
=\hbar\big(|1,0\rangle+i|0,1\rangle\big)}.
$$

The [angular momentum](../../momentum.md#angular-momentum) is $+\hbar$; division by $\sqrt2$ performs [wavefunction normalization](../../wave-function.md#wavefunction-normalization) on this state without changing its [eigenvalue](../../linear-operator-theory.md#eigenvalue). It is one excitation of the positive circular mode.

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/solution">Solution</h4>

↑ **Parent:** [B7](#section-b/b7)

A pure [stationary state](../../quantum-system.md#stationary-state) of a time-independent [Hamiltonian operator](../../quantum-system.md#hamiltonian-quantum-mechanics) is $\Psi(\mathbf r,t)=\psi(\mathbf r)e^{-iEt/\hbar}$. Its [probability density](../../wave-function.md#probability-density) and all expectations of time-independent [observables](../../quantum-system.md#observable) are constant. This does not require zero [probability current](../../wave-function.md#probability-current).

For real scalar [potential energy](../../energy.md#potential-energy) and no [vector potential](../../multivariable-calculus.md#vector-potential), substitute $i\hbar\dot\Psi=-(\hbar^2/2m)\nabla^2\Psi+V\Psi$ and its [complex conjugate](../../complex-analysis.md#complex-conjugate) into $\dot\rho=\Psi^*\dot\Psi+\dot\Psi^*\Psi$. The potential terms cancel:

$$
\dot\rho=\frac{i\hbar}{2m}\big(\Psi^*\nabla^2\Psi-\Psi\nabla^2\Psi^*\big)
=-\nabla\cdot\left[\frac{\hbar}{2im}(\Psi^*\nabla\Psi-\Psi\nabla\Psi^*)\right].
$$

Thus the [probability current](../../wave-function.md#probability-current) is $\mathbf j=(\hbar/m)\operatorname{Im}(\Psi^*\nabla\Psi)$. In a [stationary state](../../quantum-system.md#stationary-state) $\nabla\cdot\mathbf j=0$: flow may circulate without changing the [density](../../fluid-mechanics.md#density).

Here only the azimuthal [phase](../../wave.md#phase-waves) contributes an imaginary logarithmic [derivative](../../calculus.md#derivative). Since $\nabla\phi=\hat{\boldsymbol\phi}/(r\sin\theta)$,

$$
\boxed{\mathbf j=\frac{\hbar|\Psi|^2}{mr\sin\theta}\hat{\boldsymbol\phi}
=\frac{\hbar A^2}{m}r e^{-r/a_0}\sin\theta\,\hat{\boldsymbol\phi}}.
$$

There is no radial or polar flow; the azimuthal current is independent of $\phi$, so its [divergence](../../multivariable-calculus.md#divergence) vanishes. The apparent coordinate singularity at $\sin\theta=0$ cancels in the final expression.

The z-component of [orbital angular momentum](../../quantum-mechanics.md#orbital-angular-momentum) follows from the moment of the [mass](../../classical-mechanics.md#mass) current:

$$
\langle L_z\rangle
=\int mr\sin\theta\,j_\phi\,dV
=\hbar A^2
\left(\int_0^\infty r^4e^{-r/a_0}dr\right)
\left(\int_0^\pi\sin^3\theta\,d\theta\right)
\left(\int_0^{2\pi}d\phi\right)
=\boxed{\hbar}.
$$

Indeed $A^2(24a_0^5)(4/3)(2\pi)=1$. This agrees with $L_z=-i\hbar\partial_\phi$ acting on the [wavefunction](../../wave-function.md).

<h3 id="section-b/b8">B8</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b8/solution">Solution</h4>

↑ **Parent:** [B8](#section-b/b8)

Write $\gamma=ge/(2m)$, retaining the printed [magnetic moment](../../electromagnetism.md#magnetic-dipole-moment) convention. The displayed two-dimensional [matrices](../../vector-space.md#matrix) are [Pauli matrices](../../algebra.md#pauli-matrices), and the [spin](../../angular-momentum-operator.md#spin) [Hamiltonian operator](../../quantum-system.md#hamiltonian-quantum-mechanics) is

$$
\boxed{H=-\frac{\gamma\hbar}{2}
\begin{pmatrix}B_z&B_x-iB_y\\B_x+iB_y&-B_z\end{pmatrix}}.
$$

For an x-directed field let $\omega=\gamma B_x/2$. The [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation) gives $i\dot c_+=-\omega c_-$ and $i\dot c_-=-\omega c_+$. With $c_+(0)=1,c_-(0)=0$, these equations yield

$$
\boxed{|\Psi(t)\rangle=\cos(\omega t)|+z\rangle+i\sin(\omega t)|-z\rangle,\qquad
\omega=\frac{geB_x}{4m}}.
$$

Equivalently, $U(t)=e^{i\omega t\sigma_x}=I\cos\omega t+i\sigma_x\sin\omega t$. If $e$ denotes a positive [elementary charge](../../electric-charge.md#elementary-charge) magnitude, a free [electron](../../physics.md#electron) is conventionally assigned a minus sign in its [magnetic moment](../../electromagnetism.md#magnetic-dipole-moment); that alternative reverses the rotation sense. The expressions here consistently use the moment specified in the paper.

<h4 id="section-b/b8/a">a</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b8/a)

Put $c=\cos\omega t$, $s=\sin\omega t$. The real part of the off-diagonal coherence vanishes:

$$
\langle S_x\rangle=\frac{\hbar}{2}(c\,is-is\,c)=\boxed{0}.
$$

This also follows from $[H,S_x]=0$ and its zero initial expectation. Individual measurements still give $\pm\hbar/2$, each with [probability](../../probability-theory.md#probability) $1/2$.

<h4 id="section-b/b8/b">b</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b8/b)

The populations give

$$
\boxed{\langle S_z\rangle=\frac{\hbar}{2}(c^2-s^2)=\frac{\hbar}{2}\cos(\Omega t),\qquad
\Omega=2\omega=\frac{geB_x}{2m}}.
$$

Together with $\langle S_y\rangle=(\hbar/2)\sin(\Omega t)$, this describes [Larmor precession](../../angular-momentum-operator.md#larmor-precession) of a [spin](../../angular-momentum-operator.md#spin) initially perpendicular to the field. The positive angular [frequency](../../wave.md#frequency) is $|\Omega|$; the sign specifies the rotation sense through $d\langle\mathbf S\rangle/dt=\gamma\langle\mathbf S\rangle\times\mathbf B$. The factor of two between the [spinor](../../algebra-over-a-field.md#spinor) amplitudes and the measured [spin](../../angular-momentum-operator.md#spin) is essential. The model with [quantum coherence](../../density-matrix.md#quantum-coherence-in-a-specified-basis) predicts no decay; [spin relaxation](../../angular-momentum-operator.md#spin-relaxation) or [dephasing](../../quantum-information-theory.md#dephasing-channel) in a real solid can damp the oscillation.

<h3 id="section-b/b9">B9</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b9/solution">Solution</h4>

↑ **Parent:** [B9](#section-b/b9)

Put $\kappa=e^2/(4\pi\epsilon_0)$. Substitution of $\psi=R(r)\Phi(\phi)$ into the [time-independent Schrödinger equation](../../mathematical-physics.md#time-independent-schrodinger-equation), followed by division by $R\Phi$ and multiplication by $r^2$, separates the angular dependence:

$$
\frac{r^2R''+rR'}R+\frac{2\mu}{\hbar^2}(Er^2+\kappa r)
=-\frac{\Phi''}{\Phi}=m^2.
$$

Thus $\Phi=e^{im\phi}/\sqrt{2\pi}$ and

$$
rR''+R'+\left[\frac{2\mu}{\hbar^2}(Er+\kappa)-\frac{m^2}{r}\right]R=0.
$$

The [single-valued wavefunction](../../wave-function.md#single-valued-wavefunction) condition, $\Phi(\phi+2\pi)=\Phi(\phi)$, requires **$m\in\mathbb Z$**. The regular [boundary condition](../../differential-equation.md#boundary-condition) at the origin selects $R\sim r^{|m|}$. Accordingly use $s=|m|$ in the radial ansatz; the printed $x^m$ notation describes the $m\geq0$ representatives.

For the [two-dimensional Coulomb bound state](../../quantum-system.md#two-dimensional-coulomb-bound-state), substitution of $R=x^s e^{-x/2}G$ with the stipulated radial and [energy](../../energy.md) scales gives

$$
xG''+(2s+1-x)G'+(N-s-\tfrac12)G=0.
$$

The coefficient of $x^n$ in the [power series](../../sequence-and-series.md#power-series) is

$$
(n+1)(n+2s+1)a_{n+1}
+(N-s-\tfrac12-n)a_n=0,
\qquad
\boxed{a_{n+1}=\frac{n+s+\tfrac12-N}{(n+1)(n+2s+1)}a_n}.
$$

The regular solution otherwise has an exponentially growing contribution at large $x$, incompatible with being [normalizable](../../wave-function.md#normalizable-wavefunction). Termination at degree $n_r\geq0$ therefore requires

$$
\boxed{N=n_r+|m|+\tfrac12,\quad
E_{n_rm}=-\frac{\mu\kappa^2}{2\hbar^2(n_r+|m|+\tfrac12)^2}}.
$$

The resulting $G$ is proportional to a [Generalized Laguerre polynomial](../../linear-operator-theory.md#generalized-laguerre-polynomial).

Define $R_{\rm y}=\mu\kappa^2/(2\hbar^2)$, the hydrogenic Rydberg [energy](../../energy.md) for the stipulated [mass](../../classical-mechanics.md#mass). The first three distinct two-dimensional [energies](../../energy.md) are **$-4R_{\rm y},-4R_{\rm y}/9,-4R_{\rm y}/25$**, whereas in three dimensions they are **$-R_{\rm y},-R_{\rm y}/4,-R_{\rm y}/9$**. Both series approach zero from below, but the planar [ground state](../../quantum-mechanics.md#ground-state) is four times more tightly bound. Without [spin](../../angular-momentum-operator.md#spin) the respective [quantum degeneracies](../../quantum-mechanics.md#degenerate-energy-levels) are $1,3,5$ and $1,4,9$; if individual degenerate states are counted, the second and third planar states already share the first excited [energy](../../energy.md). This comparison retains the supplied $1/r$ interaction; it does not replace it by the logarithmic [electrostatic potential](../../electric-field.md#electric-potential) of a genuinely two-dimensional electromagnetic theory.

## Section C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-c/c10">C10</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c10/solution">Solution</h4>

↑ **Parent:** [C10](#section-c/c10)

[identical particles](../../tensor-product-of-quantum-systems.md#indistinguishable-particles) have the same intrinsic properties. Exchanging their bookkeeping labels cannot distinguish a physical preparation or change a measurable prediction. This is stronger than merely failing to track classical trajectories. For ordinary [bosons](../../tensor-product-of-quantum-systems.md#boson) and [fermions](../../tensor-product-of-quantum-systems.md#fermion), the many-particle [wavefunction](../../wave-function.md) has respectively [bosonic exchange symmetry](../../tensor-product-of-quantum-systems.md#bosonic-exchange-symmetry) or [fermionic exchange symmetry](../../tensor-product-of-quantum-systems.md#fermi-dirac-statistics) under every [particle exchange operator](../../tensor-product-of-quantum-systems.md#particle-exchange-operator), acting on spatial and [spin](../../angular-momentum-operator.md#spin) coordinates together. The [Spin-statistics theorem](../../tensor-product-of-quantum-systems.md#spin-statistics-theorem) connects integer [spin](../../angular-momentum-operator.md#spin) to [bosons](../../tensor-product-of-quantum-systems.md#boson) and half-integer [spin](../../angular-momentum-operator.md#spin) to [fermions](../../tensor-product-of-quantum-systems.md#fermion); this connection uses relativistic quantum-field assumptions, rather than following from the nonrelativistic [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation) alone.

For [one-particle states](../../quantum-field-theory.md#one-particle-state) $u,v$ satisfying [orthonormality](../../inner-product.md#orthonormal-set), the two alternatives form a [quantum superposition](../../quantum-system.md#quantum-superposition):

$$
\Psi_\pm(1,2)=\frac{u(1)v(2)\pm v(1)u(2)}{\sqrt2}.
$$

Its [probability density](../../wave-function.md#probability-density) contains an exchange interference term, absent from an incoherent mixture of labelled alternatives. The antisymmetric expression vanishes when both [one-particle states](../../quantum-field-theory.md#one-particle-state) are identical: **one complete [one-particle state](../../quantum-field-theory.md#one-particle-state) can contain at most one [fermion](../../tensor-product-of-quantum-systems.md#fermion)**. This [Pauli exclusion principle](../../tensor-product-of-quantum-systems.md#pauli-exclusion-principle) explains [electron shell](../../chemistry.md#electron-shell) filling, the electronic [Fermi sea](../../quantum-ideal-gas-statistics.md#fermi-sea) and [degeneracy pressure](../../quantum-ideal-gas-statistics.md#degeneracy-pressure). Opposite [spins](../../angular-momentum-operator.md#spin) are different [one-particle states](../../quantum-field-theory.md#one-particle-state), so two [electrons](../../physics.md#electron) may share an [atomic orbital](../../chemistry.md#atomic-orbital). Spatially separated [wave packets](../../dispersion-relation.md#wave-packet) with negligible overlap can often be treated as distinguishable for local measurements; the underlying exchange symmetry remains.

In [thermal equilibrium](../../thermal-equilibrium.md), occupation of a level of [energy](../../energy.md) $\epsilon$ obeys

$$
\bar n_{\rm B}=\frac1{e^{(\epsilon-\mu)/(k_BT)}-1},\qquad
\bar n_{\rm F}=\frac1{e^{(\epsilon-\mu)/(k_BT)}+1}.
$$

[bosons](../../tensor-product-of-quantum-systems.md#boson) can accumulate macroscopically in one state, giving [Bose-Einstein condensation](../../quantum-ideal-gas-statistics.md#bose-einstein-condensation); [fermions](../../tensor-product-of-quantum-systems.md#fermion) instead fill successive states up to the [Fermi energy](../../quantum-ideal-gas-statistics.md#fermi-energy) at zero [temperature](../../temperature.md). When occupation is dilute, both expressions reduce to the [Maxwell-Boltzmann distribution](../../quantum-ideal-gas-statistics.md#maxwell-boltzmann-distribution). The identical-particle classical [partition function](../../canonical-ensemble.md#canonical-partition-function) contains $1/N!$, avoiding spurious [entropy](../../entropy.md) from permutations and the [Gibbs paradox](../../canonical-ensemble.md#gibbs-paradox). Exchange effects become conspicuous when the [thermal de Broglie wavelength](../../canonical-ensemble.md#thermal-de-broglie-wavelength) is comparable to the interparticle spacing.

An operational test is the [Hong-Ou-Mandel effect](../../quantum-system.md#hong-ou-mandel-effect). Down-converted [photon](../../quantum-mechanics.md#photon) pairs enter separate ports of a balanced [beam splitter](../../optical-instrument.md#beam-splitter); indistinguishable alternatives for one [photon](../../quantum-mechanics.md#photon) per output cancel. Scanning the relative arrival delay restores coincidences away from overlap. Matching [polarization](../../wave.md#polarization-waves), spectral filtering and spatial alignment controls distinguishability; measuring delayed accidental coincidences controls background. The observed dip tests two-photon interference, and its finite depth must not automatically be interpreted as a failure of bosonic symmetry. The original apparatus varied beam-splitter position and subtracted a separately measured accidental background.[pp. 2044–2046, Fig. 1, Eq. (2), coincidence-background procedure and Fig. 2](../../physics-bibliography.md#measurement-of-subpicosecond-time-intervals-between-two-photons-by-interference-by-c-k-hong-and-others)

<h3 id="section-c/c11">C11</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c11/a">a</h4>

↑ **Parent:** [C11](#section-c/c11)

<h5 id="section-c/c11/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c11/a)

For [observables](../../quantum-system.md#observable) $A,B$, nonzero $[A,B]$ obstructs a complete common [eigenbasis](../../linear-operator-theory.md#eigenbasis). In a finite-dimensional system, commuting [Hermitian operators](../../hilbert-space.md#hermitian-operator) can be simultaneously diagonalized; [quantum degeneracy](../../quantum-mechanics.md#degenerate-energy-levels) may require choosing an appropriate basis inside the degenerate [eigenspace](../../linear-operator-theory.md#eigenspace). Noncommuting [observables](../../quantum-system.md#observable) can still share particular [eigenvectors](../../linear-operator-theory.md#eigenvector), so incompatibility is not a claim that every individual state must have nonzero spreads in both quantities.

The [Robertson uncertainty relation](../../quantum-theory.md#robertson-uncertainty-principle) follows by applying [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality) to $(A-\langle A\rangle)|\psi\rangle$ and $(B-\langle B\rangle)|\psi\rangle$:

$$
\boxed{\Delta A\,\Delta B\geq\frac12|\langle[A,B]\rangle|}.
$$

In particular $[x,p_x]=i\hbar$ gives $\Delta x\,\Delta p_x\geq\hbar/2$. These are preparation spreads, not necessarily [measurement errors](../../probability-and-statistics.md#measurement-error). A zero [commutator](../../lie-algebra.md#commutator) expectation can make this bound zero even when the [linear operators](../../vector-space.md#linear-operator) do not commute.

Measurement order can matter: preparing $|+z\rangle$, measuring $S_x$, then measuring $S_z$ gives both z outcomes with [probability](../../probability-theory.md#probability) $1/2$ when the intermediate result is ignored. A direct z measurement would give $+\hbar/2$ certainly. Finally the [Heisenberg equation of motion](../../quantum-system.md#heisenberg-equation-of-motion) $dA/dt=(i/\hbar)[H,A]+\partial A/\partial t$ relates commutation to conservation: an [observable](../../quantum-system.md#observable) with no explicit time dependence and $[H,A]=0$ is conserved. For [unbounded self-adjoint operators](../../linear-operator-theory.md#unbounded-self-adjoint-operator) these statements require the appropriate common domains; a formal commutator calculation alone need not justify simultaneous spectral measurements.

<h4 id="section-c/c11/b">b</h4>

↑ **Parent:** [C11](#section-c/c11)

<h5 id="section-c/c11/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c11/b)

In a [classically forbidden region](../../mathematical-physics.md#classically-forbidden-region), the [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation) has evanescent solutions rather than forcing the [wavefunction](../../wave-function.md) to vanish. Matching at both sides of a finite barrier permits nonzero transmission. For a broad barrier the [WKB approximation](../../analysis.md#wkb-approximation) gives

$$
T\simeq C\exp\left[-2\int_{x_1}^{x_2}\frac{\sqrt{2m(V(x)-E)}}{\hbar}\,dx\right],
$$

where $C$ is a matching prefactor. **Transmission is exponentially sensitive to barrier width and height.** A single decaying [exponential function](../../calculus.md#exponential-function) carries no [probability current](../../wave-function.md#probability-current); the matched scattering solution includes the combination needed for transmitted current. [energy](../../energy.md) is conserved throughout.

In [alpha decay](../../physics.md#alpha-decay), a quasibound alpha particle penetrates the nuclear [Coulomb barrier](../../physics.md#coulomb-barrier). Multiplying the penetration [probability](../../probability-theory.md#probability) by an assault [frequency](../../wave.md#frequency) estimates the decay rate; the strong dependence on alpha [energy](../../energy.md) explains the wide range of lifetimes. In a [scanning tunnelling microscope](../../quantum-mechanics.md#scanning-tunneling-microscope), a [voltage](../../random-walk.md#voltage) drives [electron](../../physics.md#electron) [quantum tunnelling](../../quantum-mechanics.md#quantum-tunnelling) between a conducting tip and sample. Approximately $I\propto V e^{-2\kappa d}$, so constant-current feedback resolves changes in gap width, with electronic [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) also affecting the image. Piezoelectric motion, vibration isolation and stable [voltage](../../random-walk.md#voltage) are necessary; a bright feature is not automatically a taller atom. Atomic-scale imaging was demonstrated with a vacuum-tunnelling microscope in the original surface study.[Abstract and pp. 57–61: atomic-scale steps and surface reconstruction](../../physics-bibliography.md#surface-studies-by-scanning-tunneling-microscopy-by-gerd-binnig-and-others) In a [Josephson junction](../../superconductivity.md#josephson-junction), [Cooper pair](../../fermi-liquid.md#cooper-pair) [quantum tunnelling](../../quantum-mechanics.md#quantum-tunnelling) through a weak link gives $I=I_c\sin\varphi$, allowing supercurrent without an applied [voltage](../../random-walk.md#voltage) and phase-sensitive interference. These are distinct applications of barrier penetration and coupling with [quantum coherence](../../density-matrix.md#quantum-coherence-in-a-specified-basis), not particles borrowing [energy](../../energy.md) to climb over a barrier.

<h4 id="section-c/c11/c">c</h4>

↑ **Parent:** [C11](#section-c/c11)

<h5 id="section-c/c11/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c11/c)

Addition of two spin-one-half angular momenta gives total [spin](../../angular-momentum-operator.md#spin) $S=0$ or $S=1$. The normalized [singlet state](../../angular-momentum-operator.md#singlet-state) and [triplet states](../../angular-momentum-operator.md#spin-one-half-triplet-state) are

$$
|0,0\rangle=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2},
\qquad
|1,1\rangle=|\uparrow\uparrow\rangle,\quad
|1,0\rangle=\frac{|\uparrow\downarrow\rangle+|\downarrow\uparrow\rangle}{\sqrt2},
\quad |1,-1\rangle=|\downarrow\downarrow\rangle.
$$

They have $S^2$ [eigenvalues](../../linear-operator-theory.md#eigenvalue) $0$ and $2\hbar^2$, and $S_z=M\hbar$. The [singlet state](../../angular-momentum-operator.md#singlet-state) is antisymmetric under a [particle exchange operator](../../tensor-product-of-quantum-systems.md#particle-exchange-operator), whereas all three triplets have symmetric spin-exchange parity. For two identical [electrons](../../physics.md#electron) the full state must be antisymmetric: a [singlet state](../../angular-momentum-operator.md#singlet-state) pairs with a spatial state with symmetric exchange parity, a [triplet state](../../angular-momentum-operator.md#spin-one-half-triplet-state) with an antisymmetric spatial state. Thus **two [electrons](../../physics.md#electron) in the same [atomic orbital](../../chemistry.md#atomic-orbital) must form a [singlet state](../../angular-momentum-operator.md#singlet-state)**.

The identity $\mathbf S_1\cdot\mathbf S_2=(S^2-S_1^2-S_2^2)/2$ gives $-3\hbar^2/4$ in the [singlet state](../../angular-momentum-operator.md#singlet-state) and $+\hbar^2/4$ in the [triplet state](../../angular-momentum-operator.md#spin-one-half-triplet-state). Hence an [exchange interaction](../../electromagnetism.md#exchange-interaction) distinguishes their [energies](../../energy.md), with ordering determined by its coupling sign. The [singlet state](../../angular-momentum-operator.md#singlet-state) has perfect opposite-spin correlations along any common measurement axis and is [entangled](../../bell-state.md#entangled-state). The $M=0$ [triplet state](../../angular-momentum-operator.md#spin-one-half-triplet-state) is also [entangled](../../bell-state.md#entangled-state), while the $M=\pm1$ [triplet states](../../angular-momentum-operator.md#spin-one-half-triplet-state) are [product states](../../bell-state.md#product-state) along the chosen axis.

## Section D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-d/d12">D12</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d12/a">a</h4>

↑ **Parent:** [D12](#section-d/d12)

<h5 id="section-d/d12/a/solution">Solution</h5>

↑ **Parent:** [A](#section-d/d12/a)

[Bayes' theorem](../../probability-theory.md#bayes-theorem) updates a parameter distribution using measured data:

$$
\boxed{p(\theta\mid D)=\frac{p(D\mid\theta)p(\theta)}{\int p(D\mid\theta')p(\theta')\,d\theta'}}.
$$

The [likelihood](../../maximum-likelihood-estimation.md#likelihood-function) describes the measurement process, the [prior distribution](../../bayesian-statistics.md#prior-probability) encodes information before the present data, and the denominator normalizes the [posterior distribution](../../bayesian-statistics.md#bayesian-posterior). Include instrumental [noise](../../electrical-engineering.md#noise-signal-processing) and known selection effects in the [likelihood](../../maximum-likelihood-estimation.md#likelihood-function). [nuisance parameters](../../statistical-model.md#nuisance-parameter), such as an uncertain background, should be jointly inferred and marginalized, rather than silently fixed.

For $n$ independent readings with a [Gaussian distribution](../../probability-distribution.md#normal-distribution) with known common [variance](../../variance.md) $\sigma^2$ and [prior distribution](../../bayesian-statistics.md#prior-probability) $\theta\sim N(\mu_0,\tau_0^2)$, completing the square gives

$$
\tau_n^{-2}=\tau_0^{-2}+n\sigma^{-2},\qquad
\mu_n=\tau_n^2\big(\mu_0\tau_0^{-2}+n\bar x\,\sigma^{-2}\big).
$$

The [posterior distribution](../../bayesian-statistics.md#bayesian-posterior) is $N(\mu_n,\tau_n^2)$: [prior distribution](../../bayesian-statistics.md#prior-probability) and data contribute in proportion to precision. A broad [prior distribution](../../bayesian-statistics.md#prior-probability) recovers the usual estimate $\bar x$ with [standard deviation](../../variance.md#standard-deviation) $\sigma/\sqrt n$. Report a [posterior distribution](../../bayesian-statistics.md#bayesian-posterior) estimate and [credible interval](../../bayesian-statistics.md#credible-interval), specify the [prior distribution](../../bayesian-statistics.md#prior-probability), and examine sensitivity when the data are weak. A [credible interval](../../bayesian-statistics.md#credible-interval) is a [posterior distribution](../../bayesian-statistics.md#bayesian-posterior) [probability](../../probability-theory.md#probability) statement about the parameter conditional on the model; it is not defined by the repeated-sampling coverage of a [confidence interval](../../statistical-inference.md#confidence-interval).

<h4 id="section-d/d12/b">b</h4>

↑ **Parent:** [D12](#section-d/d12)

<h5 id="section-d/d12/b/solution">Solution</h5>

↑ **Parent:** [B](#section-d/d12/b)

Uniform samples at $t_n=n/f_s$ cannot distinguish [frequencies](../../wave.md#frequency) separated by integer multiples of $f_s$:

$$
e^{2\pi i(f+kf_s)t_n}=e^{2\pi ift_n},\qquad k\in\mathbb Z.
$$

For a real [cosine](../../geometry-and-topology.md#cosine), opposite [frequencies](../../wave.md#frequency) also coincide. Thus an unknown high-frequency component can appear in the sampled record at its folded [frequency](../../wave.md#frequency) $f_{\rm alias}\in[0,f_s/2]$. For example, **2 Hz and 8 Hz [cosines](../../geometry-and-topology.md#cosine) give identical samples at 10 samples per second**. This ambiguity is [aliasing](../../fourier-analysis.md#aliasing), rather than [uniform quantization error](../../electrical-engineering.md#uniform-quantization-error).

<a id="section-d/d12/b/image-two-signals-identical-samples"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2-aliasing.png)

**[Figure 2](#section-d/d12/b/image-two-signals-identical-samples). Two signals, identical samples**.

The [Nyquist–Shannon sampling theorem](../../fourier-analysis.md#nyquist-shannon-sampling-theorem) permits reconstruction of an ideally [bandlimited function](../../fourier-transform.md#bandlimited-function) of [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) $B$ when $f_s>2B$. Use an analogue [anti-aliasing filter](../../fourier-analysis.md#anti-aliasing-filter) before conversion and allow a transition band between the desired passband and the [frequencies](../../wave.md#frequency) that fold into it. Sampling faster relaxes the filter requirement. Digital filtering after undersampling cannot separate already identical sample sequences. Finite observation time, [clock jitter](../../electrical-engineering.md#clock-jitter), [noise](../../electrical-engineering.md#noise-signal-processing) and imperfect filter rejection impose further practical limits.

<h4 id="section-d/d12/c">c</h4>

↑ **Parent:** [D12](#section-d/d12)

<h5 id="section-d/d12/c/solution">Solution</h5>

↑ **Parent:** [C](#section-d/d12/c)

Identify the physical coupling that causes a [systematic error](../../physics.md#systematic-error) and change the apparatus so that it can be measured or cancelled. [measurement calibration](../../physics.md#measurement-calibration) against known reference standards at several points reveals zero and gain errors; blanks and background runs measure additive contributions. Carry uncertainties of the standards and fitted corrections into the final result.

Reversal provides a particularly transparent test. If $D_+=S+b$ and $D_-=-S+b$, the combination $(D_+-D_-)/2$ isolates $S$ while $(D_++D_-)/2$ measures the [measurement zero offset](../../physics.md#measurement-zero-offset). Interleave and repeat the reversals so drift can be detected. The cancellation assumes a stable [measurement zero offset](../../physics.md#measurement-zero-offset) and a genuinely odd signal; a common gain error remains. [null measurements](../../electrical-engineering.md#null-measurement) and bridge comparisons can reduce dependence on detector gain. Swapping sensors or leads exposes asymmetry; checking alignment, shielding, grounding and [temperature](../../temperature.md) control tests specific unwanted couplings. Varying signal amplitude or measurement [frequency](../../wave.md#frequency) can reveal heating, nonlinear response or pickup.

Use independent measurement principles where possible, and test the predicted response to each deliberate change. **Repeated readings alone do not remove a fixed [systematic error](../../physics.md#systematic-error).** Correct identified significant effects and retain uncertainty for imperfectly known corrections; complete elimination cannot generally be demonstrated. Type A and Type B classify how uncertainty is evaluated, rather than simply meaning [random measurement errors](../../probability-and-statistics.md#random-measurement-error) and [systematic errors](../../physics.md#systematic-error).[§§2–5, especially §5.2; Appendix D.1.1.6–D.1.1.8](../../physics-bibliography.md#guidelines-for-evaluating-and-expressing-the-uncertainty-of-nist-measurement-results-by-barry-n-taylor-and-chris-e-kuyatt)

<h3 id="section-d/d13">D13</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d13/solution">Solution</h4>

↑ **Parent:** [D13](#section-d/d13)

An [ideal operational amplifier](../../electrical-circuit.md#ideal-operational-amplifier) draws no current at either input. With stable [operational-amplifier negative feedback](../../electrical-circuit.md#operational-amplifier-negative-feedback) in its unsaturated linear range, infinite [open-loop gain](../../electrical-circuit.md#open-loop-gain) also gives a [virtual short](../../electrical-circuit.md#virtual-short), $V_+=V_-$. The amplifier adjusts its output to enforce that equality; it is not a conducting connection between the inputs. Here $V_+=0$, so the ideal summing node is a [virtual ground](../../electrical-circuit.md#virtual-ground). [Kirchhoff's current law](../../random-walk.md#kirchhoff-node-law) gives $V_{\rm in}/R_1=-V_{\rm out}/R_2$, hence **the ideal gain is $-R_2/R_1$**.

For the [finite-input-resistance inverting amplifier](../../electrical-circuit.md#finite-input-resistance-inverting-amplifier) let the inverting-node [voltage](../../random-walk.md#voltage) be $v$, and continue to neglect [output impedance](../../electrical-circuit.md#output-impedance). The controlled output and node-current balance are

$$
V_{\rm out}=-Av,\qquad
\frac{v-V_{\rm in}}{R_1}+\frac{v-V_{\rm out}}{R_2}+\frac{v}{R_{\rm in}}=0.
$$

Eliminating $v$ gives

$$
\boxed{\frac{V_{\rm out}}{V_{\rm in}}
=-\frac{R_2/R_1}{1+\dfrac1A\left(1+\dfrac{R_2}{R_1}+\dfrac{R_2}{R_{\rm in}}\right)}}.
$$

Dividing the denominator by $R_2$ gives the requested resistance-sum form. The ideal result follows whenever $|A|\gg 1+R_2/R_1+R_2/R_{\rm in}$; taking $R_{\rm in}\to\infty$ alone is insufficient if $A$ is small. At finite [frequency](../../wave.md#frequency) $A$ and the gain are [phasor](../../wave.md#phasor) ratios, subject to feedback stability.

With equal [resistors](../../electric-charge.md#resistor) and sufficiently large loop gain, **$V_{\rm out}\simeq -V_{\rm in}$**. This gives a controlled sign reversal or 180-degree [phase](../../wave.md#phase-waves) inversion, useful for subtraction and opposite-phase signal paths, with amplitude set by a [resistor](../../electric-charge.md#resistor) ratio rather than uncertain [open-loop gain](../../electrical-circuit.md#open-loop-gain). The source still sees approximately $R_1$, so this is not a high-input-impedance [voltage](../../random-walk.md#voltage) follower. For the ideal-input, single-pole model, the [noise gain of an operational amplifier](../../electrical-circuit.md#noise-gain-of-an-operational-amplifier) is two and the closed-loop [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) is approximately half the [gain-bandwidth product](../../electrical-circuit.md#gain-bandwidth-product). Output swing, [slew rate](../../electrical-circuit.md#slew-rate) and load constraints must also permit linear operation.

<h4 id="section-d/d13/a">a</h4>

↑ **Parent:** [D13](#section-d/d13)

<h5 id="section-d/d13/a/solution">Solution</h5>

↑ **Parent:** [A](#section-d/d13/a)

A representative bipolar-input 741 amplifier has **$R_{\rm in}$ of order $10^6\,\Omega$**; the LM741 specification gives a typical $2\,\mathrm{M\Omega}$ at $25^\circ\mathrm C$. This is an illustrative device specification, not an identification of an unspecified practical-class part. Other input architectures can have much larger [electrical resistance](../../electric-charge.md#electrical-resistance), and finite input [capacitance](../../electromagnetism.md#capacitance) makes the [input impedance](../../electrical-circuit.md#input-impedance) [frequency](../../wave.md#frequency) dependent.[SNOSC25D, §6.5, p. 5, input-resistance row and its test conditions](../../physics-bibliography.md#lm741-operational-amplifier-by-texas-instruments)

<h4 id="section-d/d13/b">b</h4>

↑ **Parent:** [D13](#section-d/d13)

<h5 id="section-d/d13/b/solution">Solution</h5>

↑ **Parent:** [B](#section-d/d13/b)

The [open-loop gain](../../electrical-circuit.md#open-loop-gain) is large and roughly constant at low [frequency](../../wave.md#frequency), then falls as internal [poles](../../isolated-singularity.md#pole) become important. A dominant-pole approximation is

$$
\boxed{A(f)\simeq\frac{A_0}{1+if/f_p}}.
$$

Above $f_p$, but before higher [poles](../../isolated-singularity.md#pole) dominate, $|A|\propto f^{-1}$, a slope of $-20\,\mathrm{dB}$ per decade, with increasing [phase](../../wave.md#phase-waves) lag. The approximate unity-gain [frequency](../../wave.md#frequency) is $f_T=A_0f_p$. A 741-class amplifier has typical low-frequency gain about $2\times10^5$; this is the [open-loop gain](../../electrical-circuit.md#open-loop-gain), distinct from the feedback-set signal gain. The finite-gain formula at the parent level explains why the closed-loop response eventually rolls off.[§6.5, p. 5, large-signal voltage-gain row](../../physics-bibliography.md#lm741-operational-amplifier-by-texas-instruments)

## ↑ Ancestors (11)

1. [2011](../2011.md)
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
