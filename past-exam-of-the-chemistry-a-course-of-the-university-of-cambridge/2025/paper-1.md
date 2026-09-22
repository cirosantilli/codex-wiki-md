# Paper 1

↑ **Parent:** [2025](../2025.md)

[Original paper, released PDF pages 166–172](https://www.whatdotheyknow.com/request/request_for_nst_past_papers/response/3572306/attach/4/FOI%202026%20862%20Stack%20materials.pdf?cookie_passthrough=1#page=166)

**Table of contents**

- [A1](#a1)
  - [a](#a1/a)
    - [i](#a1/a/i)
      - [Solution](#a1/a/i/solution)
    - [ii](#a1/a/ii)
      - [1](#a1/a/ii/1)
        - [Solution](#a1/a/ii/1/solution)
      - [2](#a1/a/ii/2)
        - [Solution](#a1/a/ii/2/solution)
  - [b](#a1/b)
    - [i](#a1/b/i)
      - [Solution](#a1/b/i/solution)
    - [ii](#a1/b/ii)
      - [Solution](#a1/b/ii/solution)
    - [iii](#a1/b/iii)
      - [Solution](#a1/b/iii/solution)
- [A2](#a2)
  - [a](#a2/a)
    - [Solution](#a2/a/solution)
  - [b](#a2/b)
    - [Solution](#a2/b/solution)
  - [c](#a2/c)
    - [Solution](#a2/c/solution)
  - [d](#a2/d)
    - [Solution](#a2/d/solution)
  - [e](#a2/e)
    - [Solution](#a2/e/solution)
  - [f](#a2/f)
    - [Solution](#a2/f/solution)
  - [g](#a2/g)
    - [Solution](#a2/g/solution)
- [A3](#a3)
  - [a](#a3/a)
    - [i](#a3/a/i)
      - [Solution](#a3/a/i/solution)
    - [ii](#a3/a/ii)
      - [Solution](#a3/a/ii/solution)
    - [iii](#a3/a/iii)
      - [Solution](#a3/a/iii/solution)
    - [iv](#a3/a/iv)
      - [Solution](#a3/a/iv/solution)
  - [b](#a3/b)
    - [Solution](#a3/b/solution)
  - [c](#a3/c)
    - [i](#a3/c/i)
      - [Solution](#a3/c/i/solution)
    - [ii](#a3/c/ii)
      - [Solution](#a3/c/ii/solution)
  - [d](#a3/d)
    - [i](#a3/d/i)
      - [Solution](#a3/d/i/solution)
    - [ii](#a3/d/ii)
      - [Solution](#a3/d/ii/solution)
    - [iii](#a3/d/iii)
      - [Solution](#a3/d/iii/solution)
- [A4](#a4)
  - [a](#a4/a)
    - [Solution](#a4/a/solution)
  - [b](#a4/b)
    - [i](#a4/b/i)
      - [Solution](#a4/b/i/solution)
    - [ii](#a4/b/ii)
      - [Solution](#a4/b/ii/solution)
    - [iii](#a4/b/iii)
      - [Solution](#a4/b/iii/solution)
  - [c](#a4/c)
    - [i](#a4/c/i)
      - [Solution](#a4/c/i/solution)
    - [ii](#a4/c/ii)
      - [Solution](#a4/c/ii/solution)
  - [d](#a4/d)
    - [Solution](#a4/d/solution)
- [A5](#a5)
  - [a](#a5/a)
    - [Solution](#a5/a/solution)
  - [b](#a5/b)
    - [Solution](#a5/b/solution)
  - [c](#a5/c)
    - [Solution](#a5/c/solution)
  - [d](#a5/d)
    - [Solution](#a5/d/solution)

## A1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="a1/a">a</h3>

↑ **Parent:** [A1](#a1)

<h4 id="a1/a/i">i</h4>

↑ **Parent:** [A](#a1/a)

<h5 id="a1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#a1/a/i)

Take $\widehat V\psi=V(x)\psi$ with real $V$, and $\widehat T=-(\hbar^2/2m)d^2/dx^2$. The [operator domain](../../vector-space.md#operator-domain) matters: use sufficiently smooth [wavefunctions](../../wave-function.md) for which the following boundary terms vanish at both infinities. A real multiplication operator gives

$$
\langle f,\widehat Vg\rangle=\int f^*Vg\,dx=\int(Vf)^*g\,dx=\langle\widehat Vf,g\rangle.
$$

Two applications of [integration by parts](../../calculus.md#integration-by-parts) give

$$
\langle f,\widehat Tg\rangle-\langle\widehat Tf,g\rangle
=-\frac{\hbar^2}{2m}[f^*g'-f'^*g]_{-\infty}^{\infty}=0.
$$

Thus the [potential energy](../../energy.md#potential-energy) and [kinetic energy](../../energy.md#kinetic-energy) operators obey the stated [Hermitian operator](../../hilbert-space.md#hermitian-operator) identity on this common domain. For $D=d/dx$, one application of [integration by parts](../../calculus.md#integration-by-parts) instead gives

$$
\langle f,Dg\rangle=[f^*g]_{-\infty}^{\infty}-\langle Df,g\rangle=-\langle Df,g\rangle.
$$

The derivative is [anti-Hermitian](../../linear-operator-theory.md#skew-hermitian-matrix), rather than [Hermitian](../../hilbert-space.md#hermitian-operator); the minus sign cannot generally be removed. Multiplication by $-i\hbar$ makes the corresponding [momentum operator](../../quantum-mechanics.md#momentum-operator) Hermitian. These integrations establish the requested symmetry identities; full [self-adjointness](../../linear-operator-theory.md#self-adjoint-operator) of an unbounded operator additionally requires equality of its domain with its adjoint's domain.

<h4 id="a1/a/ii">ii</h4>

↑ **Parent:** [A](#a1/a)

<h5 id="a1/a/ii/1">1</h5>

↑ **Parent:** [Ii](#a1/a/ii)

<h6 id="a1/a/ii/1/solution">Solution</h6>

↑ **Parent:** [1](#a1/a/ii/1)

Let $\widehat Q\psi_n=q_n\psi_n$ with $\psi_n\ne0$. The [Hermitian operator](../../hilbert-space.md#hermitian-operator) identity and conjugate linearity of the first slot of the [inner product](../../inner-product.md) imply

$$
q_n\langle\psi_n,\psi_n\rangle
=\langle\psi_n,\widehat Q\psi_n\rangle
=\langle\widehat Q\psi_n,\psi_n\rangle
=q_n^*\langle\psi_n,\psi_n\rangle.
$$

The squared [norm](../../normed-vector-space.md#norm) is positive, so $q_n=q_n^*$: every such [eigenvalue](../../linear-operator-theory.md#eigenvalue) is real.

<h5 id="a1/a/ii/2">2</h5>

↑ **Parent:** [Ii](#a1/a/ii)

<h6 id="a1/a/ii/2/solution">Solution</h6>

↑ **Parent:** [2](#a1/a/ii/2)

For two [eigenfunctions](../../linear-operator-theory.md#eigenfunction), apply the same [Hermitian operator](../../hilbert-space.md#hermitian-operator) identity across the two states:

$$
q_n\langle\psi_m,\psi_n\rangle
=\langle\psi_m,\widehat Q\psi_n\rangle
=\langle\widehat Q\psi_m,\psi_n\rangle
=q_m\langle\psi_m,\psi_n\rangle.
$$

Hence $(q_n-q_m)\langle\psi_m,\psi_n\rangle=0$. Distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue) therefore imply [orthogonal](../../inner-product.md#orthogonal-vectors) [eigenfunctions](../../linear-operator-theory.md#eigenfunction). Within a degenerate eigenspace, [orthogonality](../../inner-product.md#orthogonal-vectors) is a possible basis choice, rather than a consequence for every pair of vectors.

<h3 id="a1/b">b</h3>

↑ **Parent:** [A1](#a1)

<h4 id="a1/b/i">i</h4>

↑ **Parent:** [B](#a1/b)

<h5 id="a1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#a1/b/i)

Multiply the [eigenfunction expansion](../../algebra.md#eigenfunction-expansion) by $\psi_m^*$ and integrate over the common domain. [Orthogonality](../../inner-product.md#orthogonal-vectors) and [wavefunction normalization](../../wave-function.md#wavefunction-normalization) give

$$
\int\psi_m^*(x)f(x)\,dx
=\sum_n c_n\int\psi_m^*(x)\psi_n(x)\,dx
=\sum_n c_n\delta_{mn}=c_m.
$$

Thus $\boxed{c_m=\langle\psi_m,f\rangle}$. For a normalized $f$, the [Born rule](../../wave-function.md#born-rule) identifies $|c_m|^2$ as the probability of this basis outcome.

<h4 id="a1/b/ii">ii</h4>

↑ **Parent:** [B](#a1/b)

<h5 id="a1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#a1/b/ii)

The decisive observation is that $x$ is itself an [eigenfunction](../../linear-operator-theory.md#eigenfunction):

$$
\widehat Qx=\frac d{dx}\left[(x^2-1)\frac{dx}{dx}\right]=2x.
$$

On the regular [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) domain, integration by parts has endpoint factor $x^2-1$, so the boundary form vanishes for regular functions at $x=\pm1$. The interval alone is not an endpoint condition; regularity is the usual condition selecting the [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial). Their [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $n(n+1)$, and the $n=1$ normalized function is

$$
\psi_1(x)=\sqrt{\frac32}\,x,\qquad \int_{-1}^{1}|\psi_1|^2dx=1.
$$

Therefore

$$
\boxed{x=\sqrt{\frac23}\,\psi_1(x),\qquad c_1=\sqrt{\frac23},\quad c_n=0\ (n\ne1).}
$$

Equivalently, the [Hermitian operator](../../hilbert-space.md#hermitian-operator) identity gives $(q_n-2)c_n=0$, and nondegeneracy leaves only one possible nonzero coefficient. The unnormalized function $x$ has squared [norm](../../normed-vector-space.md#norm) $2/3$, consistent with this coefficient.

<h4 id="a1/b/iii">iii</h4>

↑ **Parent:** [B](#a1/b)

<h5 id="a1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#a1/b/iii)

The [quantum variational principle](../../quantum-mechanics.md#quantum-variational-principle) states that the energy expectation of an admissible trial [wavefunction](../../wave-function.md) is at least the [ground state](../../quantum-mechanics.md#ground-state) energy:

$$
\boxed{\frac{\langle f,\widehat Hf\rangle}{\langle f,f\rangle}\ge E_0.}
$$

For the discrete, complete [orthonormal basis](../../inner-product.md#orthonormal-basis) assumed here, expand in [Hamiltonian operator](../../quantum-system.md#hamiltonian-quantum-mechanics) eigenfunctions, $f=\sum_n c_n\phi_n$, with $\widehat H\phi_n=E_n\phi_n$ and $E_n\ge E_0$. Then

$$
\frac{\langle f,\widehat Hf\rangle}{\langle f,f\rangle}-E_0
=\frac{\sum_n|c_n|^2(E_n-E_0)}{\sum_n|c_n|^2}\ge0.
$$

Every summand is nonnegative. Equality holds precisely when all occupied components lie in the ground eigenspace. Thus minimizing trial energies supplies upper bounds on $E_0$, with exact equality if the trial family contains a [ground state](../../quantum-mechanics.md#ground-state).

## A2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="a2/a">a</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/a/solution">Solution</h4>

↑ **Parent:** [A](#a2/a)

The [Pauli principle](../../tensor-product-of-quantum-systems.md#pauli-principle) requires the complete [wavefunction](../../wave-function.md) of identical [fermions](../../tensor-product-of-quantum-systems.md#fermion) to be antisymmetric under exchanging the full coordinates, including [spin](../../angular-momentum-operator.md#spin):

$$
\boxed{\Psi(x_2,x_1)=-\Psi(x_1,x_2),\qquad x_i=(\mathbf r_i,s_i).}
$$

It is the total spatial-and-spin state that changes sign; the spatial factor alone need not be antisymmetric.

<h3 id="a2/b">b</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/b/solution">Solution</h4>

↑ **Parent:** [B](#a2/b)

Let $a=\phi_{1s}$ and $b=\phi_{2s}$ be orthonormal [atomic orbitals](../../chemistry.md#atomic-orbital). The normalized spatial factors are

$$
\Phi_\pm(1,2)=\frac{a(1)b(2)\pm b(1)a(2)}{\sqrt2}.
$$

For the [singlet state](../../angular-momentum-operator.md#singlet-state), use the antisymmetric spin factor

$$
\chi_{00}=\frac{\alpha(1)\beta(2)-\beta(1)\alpha(2)}{\sqrt2},\qquad \Psi_S=\Phi_+\chi_{00}.
$$

For the three components of the [triplet state](../../angular-momentum-operator.md#spin-one-half-triplet-state), use

$$
\chi_{11}=\alpha(1)\alpha(2),\quad
\chi_{10}=\frac{\alpha(1)\beta(2)+\beta(1)\alpha(2)}{\sqrt2},\quad
\chi_{1,-1}=\beta(1)\beta(2),\qquad \Psi_{T,M}=\Phi_-\chi_{1M}.
$$

Each total [wavefunction](../../wave-function.md) obeys the [Pauli principle](../../tensor-product-of-quantum-systems.md#pauli-principle). At coincident spatial coordinates,

$$
\Phi_-(\mathbf r,\mathbf r)=\frac{a(\mathbf r)b(\mathbf r)-b(\mathbf r)a(\mathbf r)}{\sqrt2}=0.
$$

Consequently the triplet pair [probability density](../../wave-function.md#probability-density) vanishes at coincidence, even for its $M=0$ component. This zero is stronger than the trivial statement that any exact point has zero integrated probability in a continuum.

<h3 id="a2/c">c</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/c/solution">Solution</h4>

↑ **Parent:** [C](#a2/c)

In [atomic units](../../physics.md#atomic-units), define the [Coulomb integral](../../chemistry.md#coulomb-integral) and [exchange integral](../../chemistry.md#exchange-integral) by

$$
J=\iint\frac{|a(1)|^2|b(2)|^2}{r_{12}}\,d^3r_1d^3r_2,\qquad
K=\iint\frac{a^*(1)b(1)b^*(2)a(2)}{r_{12}}\,d^3r_1d^3r_2.
$$

Expanding the four products in the expectation of $r_{12}^{-1}$ yields

$$
\langle\Phi_\pm|r_{12}^{-1}|\Phi_\pm\rangle=\tfrac12(J+J\pm K\pm K)=J\pm K.
$$

The one-electron terms have the same value for these two states. Within this common-orbital approximation,

$$
E_S=\epsilon_{1s}+\epsilon_{2s}+J+K,\qquad
E_T=\epsilon_{1s}+\epsilon_{2s}+J-K,
$$

so $\boxed{E_S-E_T=2K}$. The [exchange integral](../../chemistry.md#exchange-integral) is nonnegative: it is the positive Coulomb quadratic form of the transition density $a^*b$, or equivalently has a nonnegative Fourier representation. The triplet is lower. Actual orbital relaxation and correlation make the common-orbital $2K$ an approximate physical splitting.

<h3 id="a2/d">d</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/d/solution">Solution</h4>

↑ **Parent:** [D](#a2/d)

Keeping the same two spin states but incorrectly imposing [boson](../../tensor-product-of-quantum-systems.md#boson) exchange symmetry would require a symmetric total [wavefunction](../../wave-function.md). The spin-antisymmetric [singlet state](../../angular-momentum-operator.md#singlet-state) would then accompany $\Phi_-$, while the spin-symmetric [triplet state](../../angular-momentum-operator.md#spin-one-half-triplet-state) would accompany $\Phi_+$. Thus

$$
E_S^{\rm hypothetical}=E_{\rm one}+J-K,\qquad
E_T^{\rm hypothetical}=E_{\rm one}+J+K,
$$

and $\boxed{E_T^{\rm hypothetical}-E_S^{\rm hypothetical}=2K}$. The ordering reverses: the triplet would be destabilized by $2K$ relative to the singlet. A genuinely spinless [boson](../../tensor-product-of-quantum-systems.md#boson) would have no singlet/triplet spin distinction; this comparison changes exchange symmetry while retaining the question's spin degrees of freedom.

<h3 id="a2/e">e</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/e/solution">Solution</h4>

↑ **Parent:** [E](#a2/e)

If two [fermions](../../tensor-product-of-quantum-systems.md#fermion) occupied the same complete [spin orbital](../../tensor-product-of-quantum-systems.md#spin-orbital) $u$, their antisymmetrized product would be

$$
\frac{u(1)u(2)-u(2)u(1)}{\sqrt2}=0.
$$

The zero vector cannot represent a normalized [quantum state](../../quantum-system.md#quantum-state). This is the [Pauli exclusion principle](../../tensor-product-of-quantum-systems.md#pauli-exclusion-principle): at most one identical [fermion](../../tensor-product-of-quantum-systems.md#fermion) occupies any complete one-particle state. Two [electrons](../../physics.md#electron) may occupy the same [spatial orbital](../../tensor-product-of-quantum-systems.md#spatial-orbital) with opposite spins, because $a\alpha$ and $a\beta$ are different [spin orbitals](../../tensor-product-of-quantum-systems.md#spin-orbital).

<h3 id="a2/f">f</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/f/solution">Solution</h4>

↑ **Parent:** [F](#a2/f)

The $3d$ and $4s$ [atomic orbitals](../../chemistry.md#atomic-orbital) of [chromium](../../chemical-substance.md#chromium) are close enough in energy that electron-electron terms can overturn the simple filling order. The configuration $[\mathrm{Ar}]\,3d^54s^1$ permits five singly occupied $3d$ orbitals and a parallel-spin $4s$ electron. Relative to $3d^44s^2$, it removes the $4s$ pair and permits more parallel-spin exchange interactions, lowering the Coulomb-and-exchange contribution enough to offset the orbital promotion cost.

As qualitative bookkeeping, six parallel [electron spins](../../angular-momentum-operator.md#electron-spin) give $\binom62=15$ same-spin pairs, compared with $\binom52=10$ in high-spin $3d^44s^2$. The individual [exchange integrals](../../chemistry.md#exchange-integral) are unequal, so this is an explanation of the tendency, rather than a quantitative atomic energy calculation. The observed [ground state](../../quantum-mechanics.md#ground-state) configuration is $\boxed{[\mathrm{Ar}]\,3d^54s^1}$.[Cr I ground level, 3d5(6S)4s, a7S, J=3, energy 0 cm−1](../../physics-bibliography.md#energy-levels-of-neutral-chromium-in-the-nist-handbook)

<h3 id="a2/g">g</h3>

↑ **Parent:** [A2](#a2)

<h4 id="a2/g/solution">Solution</h4>

↑ **Parent:** [G](#a2/g)

The closed argon core contributes $L=S=0$. In the half-filled $3d^5$ shell, [Hund's rules](../../chemistry.md#hund-s-rules) put one parallel-spin electron in each $m_\ell=-2,-1,0,1,2$ orbital. This gives $S_d=5/2$ and the orbital term $L_d=0$. Adding the parallel $4s$ electron, with $\ell=0$ and $s=1/2$, gives

$$
\boxed{S=3,\qquad L=0,\qquad J=3,\qquad {}^{2S+1}L_J={}^7S_3.}
$$

The [spin multiplicity](../../angular-momentum-operator.md#spin-multiplicity) is seven. The magnetic projection labels run $M_S,M_J=-3,-2,\ldots,3$, while $M_L=0$. The [term symbol](../../atomic-physics.md#term-symbol) agrees with the observed neutral-[chromium](../../chemical-substance.md#chromium) ground level.[Cr I, ground level a7S3](../../physics-bibliography.md#energy-levels-of-neutral-chromium-in-the-nist-handbook)

## A3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="a3/a">a</h3>

↑ **Parent:** [A3](#a3)

<h4 id="a3/a/i">i</h4>

↑ **Parent:** [A](#a3/a)

<h5 id="a3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#a3/a/i)

For one [normal mode](../../wave-equation.md#normal-mode), the fundamental is $v=0\to1$, with other modes initially in their ground levels. In the linear-dipole [harmonic approximation](../../lagrangian-mechanics.md#harmonic-approximation), the transition moment is nonzero for $\Delta v=\pm1$, so a [vibrational fundamental](../../molecule.md#vibrational-fundamental) is normally much stronger than its overtones, provided the mode has [vibrational infrared activity](../../molecule.md#vibrational-infrared-activity).

<h4 id="a3/a/ii">ii</h4>

↑ **Parent:** [A](#a3/a)

<h5 id="a3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#a3/a/ii)

The first [vibrational overtone](../../molecule.md#vibrational-overtone) is $v=0\to2$, with $\Delta v=2$. It lies near twice the fundamental wavenumber, generally slightly below it because of [anharmonicity](../../wave.md#anharmonicity). The linear-dipole harmonic model forbids it; anharmonic wavefunctions or higher terms in the dipole expansion give a weak intensity. Thus it is generally weaker than the corresponding fundamental.

<h4 id="a3/a/iii">iii</h4>

↑ **Parent:** [A](#a3/a)

<h5 id="a3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#a3/a/iii)

The second [vibrational overtone](../../molecule.md#vibrational-overtone) is $v=0\to3$, with $\Delta v=3$, near three times the fundamental wavenumber. It requires higher-order departures from the linear-dipole harmonic model and is ordinarily weaker again. These are qualitative intensity trends; resonances can redistribute intensity between nearby vibrational states.

<h4 id="a3/a/iv">iv</h4>

↑ **Parent:** [A](#a3/a)

<h5 id="a3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#a3/a/iv)

A [hot band](../../molecule.md#hot-band) starts from a thermally populated vibrationally excited state, for example $v=1\to2$. It can satisfy $\Delta v=1$ and need not have a small transition moment, but its lower-state population is reduced by the [Boltzmann distribution](../../thermodynamics.md#boltzmann-distribution):

$$
\frac{N_1}{N_0}\simeq\exp[-(E_1-E_0)/(k_BT)].
$$

It is therefore usually weak at low temperature and grows relative to the fundamental on heating. [Anharmonicity](../../wave.md#anharmonicity) shifts its frequency away from the $0\to1$ transition; in a polyatomic molecule, excitation in another mode can also produce a hot-band sequence.

<h3 id="a3/b">b</h3>

↑ **Parent:** [A3](#a3)

<h4 id="a3/b/solution">Solution</h4>

↑ **Parent:** [B](#a3/b)

A useful vibration-rotation expression, with energies measured from the potential minimum, is

$$
\boxed{\frac{E(v,J)}{hc}=\widetilde\nu_e(v+\tfrac12)-\widetilde\nu_ex_e(v+\tfrac12)^2+B_vJ(J+1),\qquad
B_v\simeq B_e-\alpha_e(v+\tfrac12).}
$$

Here $v=0,1,\ldots$ is the vibrational quantum number, $J=0,1,\ldots$ the rotational angular-momentum quantum number, $\widetilde\nu_e$ the harmonic [spectroscopic wavenumber](../../wave-equation.md#spectroscopic-wavenumber), $x_e$ a dimensionless anharmonic coefficient, and $B_v$ the vibrational-state-dependent [rotational constant](../../molecule.md#rotational-constant). $B_e$ is its equilibrium value and $\alpha_e$ describes vibration-rotation coupling. All wavenumber constants use the same inverse-length units; $h$ is the [Planck constant](../../quantum-mechanics.md#planck-constant) and $c$ the [speed of light](../../special-relativity.md#speed-of-light).

The elementary harmonic [rigid rotor](../../molecule.md#rigid-rotor) result follows by setting $x_e=\alpha_e=0$, with $\widetilde\nu_e=(2\pi c)^{-1}\sqrt{k/\mu}$ and $B_e=h/(8\pi^2cI)$, where $I=\mu r_e^2$. The molecule's electronic energy would add a common constant.

<h3 id="a3/c">c</h3>

↑ **Parent:** [A3](#a3)

<h4 id="a3/c/i">i</h4>

↑ **Parent:** [C](#a3/c)

<h5 id="a3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#a3/c/i)

A [diatomic molecule](../../molecule.md#diatomic-molecule) has $3N-5=1$ vibrational [normal mode](../../wave-equation.md#normal-mode): the bond stretch. For [hydrogen chloride](../../electronegativity.md#hydrogen-chloride), opposite longitudinal displacements change the [electric dipole moment](../../electrostatics.md#electric-dipole-moment), so the mode has [vibrational infrared activity](../../molecule.md#vibrational-infrared-activity). The following original sketches show one phase of this motion and the three water modes; arrow lengths are schematic, not mass-weighted amplitudes.

<a id="a3/c/i/image-original-sketches-of-the-hydrogen-chloride-stretch-and-the-three-molecular-vibrations-of-water"></a>
![](../../past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-1-vibrations.png)

**[Figure 1](#a3/c/i/image-original-sketches-of-the-hydrogen-chloride-stretch-and-the-three-molecular-vibrations-of-water). Original sketches of the hydrogen chloride stretch and the three molecular vibrations of water**.

<h4 id="a3/c/ii">ii</h4>

↑ **Parent:** [C](#a3/c)

<h5 id="a3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#a3/c/ii)

A nonlinear triatomic molecule has $3N-6=3$ vibrational [normal modes](../../wave-equation.md#normal-mode). For water they are the symmetric O–H stretch, the H–O–H bend, and the antisymmetric O–H stretch, shown above. In the symmetric stretch both O–H lengths increase together; in the antisymmetric stretch one increases while the other decreases; the bend predominantly changes the bond angle. All three change a component of the [electric dipole moment](../../electrostatics.md#electric-dipole-moment) and are infrared-active. Every arrow reverses half a period later; motion of oxygen maintains the molecular [centre of mass](../../classical-mechanics.md#center-of-mass).

<h3 id="a3/d">d</h3>

↑ **Parent:** [A3](#a3)

<h4 id="a3/d/i">i</h4>

↑ **Parent:** [D](#a3/d)

<h5 id="a3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#a3/d/i)

This is a [rovibrational spectrum](../../molecule.md#rovibrational-spectrum): the vibrational excitation is accompanied by quantized [molecular rotation](../../molecule.md#molecular-rotation). The high-wavenumber R branch has $\Delta J=+1$, and the low-wavenumber P branch has $\Delta J=-1$. In the simplest common-$B$ approximation,

$$
\widetilde\nu_R(J)=\widetilde\nu_0+2B(J+1),\qquad
\widetilde\nu_P(J)=\widetilde\nu_0-2BJ.
$$

Consecutive lines within either branch are therefore separated by roughly $2B$, while the gap between P(1) and R(0) is roughly $4B$. There is no Q branch: for this diatomic parallel $\Sigma\to\Sigma$ transition, the electric-dipole rotational selection rule allows $\Delta J=\pm1$, and the $\Delta J=0$ line strength vanishes.

The intensity envelope comes from rotational populations, approximately $(2J+1)e^{-hcBJ(J+1)/(k_BT)}$, together with the rotational line strengths. The paired peaks arise from the two chlorine [isotopologues](../../chemical-substance.md#isotopologue), $\mathrm H^{35}Cl$ and $\mathrm H^{37}Cl$: their different [reduced masses](../../classical-mechanics.md#reduced-mass) shift both rotational and vibrational spacings. The more abundant $^{35}\mathrm{Cl}$ gives the stronger member. The changing spacing away from the band centre reflects $B_1\ne B_0$ and, at higher $J$, centrifugal distortion; it is not evidence for additional vibrational fundamentals.

<h4 id="a3/d/ii">ii</h4>

↑ **Parent:** [D](#a3/d)

<h5 id="a3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#a3/d/ii)

Use the two-body [reduced mass](../../classical-mechanics.md#reduced-mass), rather than the chlorine mass or hydrogen mass alone:

$$
\mu=\frac{1.0078\times34.9688}{1.0078+34.9688}m_u
=1.62661\times10^{-27}\ \mathrm{kg}.
$$

The [bond force constant](../../molecule.md#bond-force-constant) gives

$$
\nu_{\rm harm}=\frac1{2\pi}\sqrt{\frac{481}{\mu}}=8.65467\times10^{13}\ \mathrm{s^{-1}},\qquad
\boxed{\widetilde\nu_{\rm harm}=\frac{\nu_{\rm harm}}{2.99792458\times10^{10}\ \mathrm{cm\,s^{-1}}}=2886.89\ \mathrm{cm^{-1}}.}
$$

The requested “frequency in cm−1” is a [spectroscopic wavenumber](../../wave-equation.md#spectroscopic-wavenumber); the ordinary frequency is the value in s−1 above. This calculation uses the question's force constant in the harmonic model, rather than replacing it with a tabulated spectroscopic constant.

<h4 id="a3/d/iii">iii</h4>

↑ **Parent:** [D](#a3/d)

<h5 id="a3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#a3/d/iii)

Read the stronger members of the inset doublets at about $2945$, $2926$ and $2906\ \mathrm{cm^{-1}}$. Their spacings are roughly $19$–$20\ \mathrm{cm^{-1}}$, so the common-$B$ estimate is

$$
\boxed{B\simeq\tfrac12\Delta\widetilde\nu\simeq10\ \mathrm{cm^{-1}}.}
$$

Using the harmonic wavenumber from the preceding calculation and labelling lines by the lower-state $J$,

$$
\boxed{\widetilde\nu_{P_1}\simeq2886.89-2(10)=2867\ \mathrm{cm^{-1}},\qquad
\widetilde\nu_{R_1}\simeq2886.89+4(10)=2927\ \mathrm{cm^{-1}}.}
$$

These are graph-based estimates. Finite reading precision and different upper/lower [rotational constants](../../molecule.md#rotational-constant) limit their accuracy to a few cm−1; extra decimal places would not be justified. The R1 result refers to $J=1\to2$, while R0 is the line nearest the high-wavenumber side of the band gap.

## A4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="a4/a">a</h3>

↑ **Parent:** [A4](#a4)

<h4 id="a4/a/solution">Solution</h4>

↑ **Parent:** [A](#a4/a)

Let $Q_k$ be a vibrational [normal mode coordinate](../../classical-mechanics.md#normal-coordinate) with symmetry $\Gamma_k$. The harmonic vibrational ground state is totally symmetric; the one-quantum state transforms as $Q_k$. Integration over a symmetry-invariant domain annihilates any integrand lacking the [totally symmetric representation](../../representation-theory.md#totally-symmetric-representation). Thus a fundamental requires

$$
\Gamma(v'=1_k)\otimes\Gamma(\mu_\alpha)\otimes\Gamma(v''=0)
\supset A_1
$$

for some Cartesian component $\alpha$. For the one-dimensional irreducible representations used here, this means $\Gamma_k=\Gamma(x)$, $\Gamma(y)$ or $\Gamma(z)$. Equivalently, expanding the [electric dipole moment](../../electrostatics.md#electric-dipole-moment) gives

$$
\mu_\alpha=\mu_{\alpha,0}+\left(\frac{\partial\mu_\alpha}{\partial Q_k}\right)_0Q_k+\cdots;
$$

the derivative can be nonzero only if $Q_k$ and $\mu_\alpha$ have compatible symmetry. This is the symmetry criterion for [vibrational infrared activity](../../molecule.md#vibrational-infrared-activity); it permits a transition without guaranteeing a large intensity.

<h3 id="a4/b">b</h3>

↑ **Parent:** [A4](#a4)

<h4 id="a4/b/i">i</h4>

↑ **Parent:** [B](#a4/b)

<h5 id="a4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#a4/b/i)

With $z$ along C=O and the molecule in the $xz$ plane, [formaldehyde](../../chemical-substance.md#formaldehyde) has $E$, $C_2(z)$, $\sigma_{xz}$ and $\sigma_{yz}$. It belongs to the [C2v point group](../../euclidean-geometry.md#c2v-point-group), $\boxed{C_{2v}}$. Keeping this axis convention is essential when assigning the labels $B_1$ and $B_2$.

<h4 id="a4/b/ii">ii</h4>

↑ **Parent:** [B](#a4/b)

<h5 id="a4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#a4/b/ii)

For operations ordered as $(E,C_2(z),\sigma_{xz},\sigma_{yz})$, the characters of the twelve Cartesian displacements are

$$
\chi_{3N}=(12,-2,4,2).
$$

Only atoms left fixed contribute: all four for $E$ and $\sigma_{xz}$, but only C and O for $C_2$ and $\sigma_{yz}$. Multiplying their counts by the Cartesian traces $3,-1,1,1$ gives these numbers. Subtract

$$
\chi_{\rm trans}=(3,-1,1,1),\qquad \chi_{\rm rot}=(3,-1,-1,-1)
$$

to obtain $\chi_{\rm vib}=(6,0,4,2)$. The [character table](../../representation-theory.md#character-table) reduction gives

$$
\boxed{\Gamma_{\rm vib}=3A_1+2B_1+B_2.}
$$

The dimensions sum to $6=3N-6$, as required. The $B_2$ mode is the out-of-plane wag with this axis convention.

<h4 id="a4/b/iii">iii</h4>

↑ **Parent:** [B](#a4/b)

<h5 id="a4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#a4/b/iii)

In this [C2v point group](../../euclidean-geometry.md#c2v-point-group) convention, $z\sim A_1$, $x\sim B_1$, and $y\sim B_2$. Therefore all six [normal modes](../../wave-equation.md#normal-mode) have symmetry-allowed infrared fundamentals: $\boxed{6\text{ IR features}}$, absent accidental coincidences or vanishing intensities.

For [Raman spectroscopy](../../optics.md#raman-spectroscopy), examine the [polarizability tensor](../../electrostatics.md#polarizability-tensor): $x^2,y^2,z^2\sim A_1$, $xz\sim B_1$, and $yz\sim B_2$; $xy\sim A_2$ is also Raman-allowed but no $A_2$ vibration occurs here. All six vibrations are therefore Raman-active too, giving $\boxed{6\text{ Raman features and }6\text{ IR/Raman coincidences}}$. The centrosymmetric mutual-exclusion rule does not apply to $C_{2v}$ [formaldehyde](../../chemical-substance.md#formaldehyde).

<h3 id="a4/c">c</h3>

↑ **Parent:** [A4](#a4)

<h4 id="a4/c/i">i</h4>

↑ **Parent:** [C](#a4/c)

<h5 id="a4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#a4/c/i)

The C=O length is invariant under every operation, so its stretch is $A_1$. If $s_L,s_R$ are the two C–H bond-length changes, their sum and difference give

$$
Q_{\rm CO}\sim A_1,\qquad Q_{\rm CH,s}=\frac{s_L+s_R}{\sqrt2}\sim A_1,\qquad
Q_{\rm CH,a}=\frac{s_L-s_R}{\sqrt2}\sim B_1.
$$

Hence $\boxed{\Gamma_{\rm stretch}=2A_1+B_1}$. These are stretching symmetry coordinates; the two $A_1$ motions can mix in actual [normal modes](../../wave-equation.md#normal-mode), and mass-weighted atomic motions need not have the schematic arrow lengths below.

<a id="a4/c/i/image-original-formaldehyde-stretching-symmetry-sketches-in-the-paper-s-xz-plane"></a>
![](../../past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-1-formaldehyde-stretches.png)

**[Figure 2](#a4/c/i/image-original-formaldehyde-stretching-symmetry-sketches-in-the-paper-s-xz-plane). Original formaldehyde stretching symmetry sketches in the paper's $xz$ plane**.

<h4 id="a4/c/ii">ii</h4>

↑ **Parent:** [C](#a4/c)

<h5 id="a4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#a4/c/ii)

There are three stretching fundamentals, although four stretching-region features are listed. The low feature at $1746\ \mathrm{cm^{-1}}$ is predominantly C=O stretch ($A_1$). The two features at $2783$ and $2843\ \mathrm{cm^{-1}}$ are the symmetric and antisymmetric C–H stretches; their order is not determined by this mode count alone.

The $3482\ \mathrm{cm^{-1}}$ feature is consistent with the first C=O [vibrational overtone](../../molecule.md#vibrational-overtone), close to $2(1746)=3492\ \mathrm{cm^{-1}}$ and shifted downward by [anharmonicity](../../wave.md#anharmonicity). Its symmetry is $A_1\otimes A_1=A_1$, so symmetry permits the weak anharmonic transition. It is not a fourth stretching fundamental. The combination-band evidence in the next part distinguishes the two C–H assignments.

<h3 id="a4/d">d</h3>

↑ **Parent:** [A4](#a4)

<h4 id="a4/d/solution">Solution</h4>

↑ **Parent:** [D](#a4/d)

The out-of-plane displacements in the wag transform as $y$, hence as $B_2$. A one-quantum combination of two distinct [normal modes](../../wave-equation.md#normal-mode) transforms as the product of their irreducible representations. The observed feature satisfies

$$
3950-1167=2783\ \mathrm{cm^{-1}}.
$$

A combination of the wag with an $A_1$ stretch has symmetry $B_2\otimes A_1=B_2$ and can absorb through $\mu_y$. In contrast, $B_2\otimes B_1=A_2$ has no electric-dipole component in $C_{2v}$ and is forbidden in the stated symmetry model. The missing feature near $4010=1167+2843\ \mathrm{cm^{-1}}$ therefore identifies the $2843$ stretch as $B_1$.

The completed assignments are

$$
\boxed{1746:\ \mathrm{C{=}O}\ (A_1),\quad2783:\ \mathrm{CH\ symmetric}\ (A_1),\quad2843:\ \mathrm{CH\ antisymmetric}\ (B_1),\quad3482:\ 2\nu_{\rm CO}\ (A_1).}
$$

The allowed combination obtains intensity through anharmonic/dipole-coupling terms; a purely separable harmonic model with a strictly linear dipole has no combination bands. The argument uses both the observed combination and the selection rule: absence of a feature by itself would not generally prove a forbidden symmetry.[Gas-phase fundamentals: CH2 symmetric stretch 2783, antisymmetric stretch 2843, CO stretch 1746, wag 1167 cm−1, with the same symmetry convention](../../chemistry-bibliography.md#formaldehyde-vibrational-data-in-the-nist-chemistry-webbook)

## A5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="a5/a">a</h3>

↑ **Parent:** [A5](#a5)

<h4 id="a5/a/solution">Solution</h4>

↑ **Parent:** [A](#a5/a)

The planar [para-quinone](../../chemical-substance.md#1-4-benzoquinone) framework has three mutually perpendicular twofold axes, inversion through its centre, and the associated mirror planes. With $x$ horizontal, $y$ along the two C=O bonds and $z$ perpendicular to the molecule, it belongs to the [D2h point group](../../euclidean-geometry.md#d2h-point-group), $\boxed{D_{2h}}$.

<h3 id="a5/b">b</h3>

↑ **Parent:** [A5](#a5)

<h4 id="a5/b/solution">Solution</h4>

↑ **Parent:** [B](#a5/b)

Write $p_i$ for the orthonormal $2p_z$ [atomic orbital](../../chemistry.md#atomic-orbital) on numbered site $i$, with every positive lobe pointing along $+z$. A normalized set of [symmetry-adapted linear combinations](../../chemistry.md#symmetry-adapted-linear-combination) is

$$
\begin{array}{c|c|l}
\text{symmetry}&\text{name}&\text{symmetry orbital}\\\hline
B_{1u}&O_+&(p_1+p_8)/\sqrt2\\
B_{1u}&C_+&(p_2+p_7)/\sqrt2\\
B_{1u}&R_+&(p_3+p_4+p_5+p_6)/2\\
B_{3g}&O_-&(p_1-p_8)/\sqrt2\\
B_{3g}&C_-&(p_2-p_7)/\sqrt2\\
B_{3g}&R_-&(p_3+p_4-p_5-p_6)/2\\
B_{2g}&X&(p_3-p_4+p_5-p_6)/2\\
A_u&Y&(p_3-p_4-p_5+p_6)/2
\end{array}
$$

Each has unit squared coefficient sum, and every distinct pair has zero [inner product](../../inner-product.md). The orbital representation therefore reduces to $\boxed{3B_{1u}+3B_{3g}+B_{2g}+A_u}$. For example, the fully symmetric site sum still has $B_{1u}$ orbital symmetry because a $p_z$ orbital itself changes sign under operations that reverse $z$. Ignoring that sign would assign the wrong representations.

<a id="a5/b/image-original-phase-maps-of-the-eight-normalized-para-quinone-symmetry-orbitals"></a>
![](../../past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-1-quinone-symmetry-orbitals.png)

**[Figure 3](#a5/b/image-original-phase-maps-of-the-eight-normalized-para-quinone-symmetry-orbitals). Original phase maps of the eight normalized para-quinone symmetry orbitals**. Filled circles label the phases of the $+z$ lobes; the opposite lobe has the opposite phase. White circles mean zero coefficient. Areas scale with coefficient magnitude. Site numbers follow the source paper.

<h3 id="a5/c">c</h3>

↑ **Parent:** [A5](#a5)

<h4 id="a5/c/solution">Solution</h4>

↑ **Parent:** [C](#a5/c)

Set $E=\alpha+\lambda\beta$, with the usual bonding convention $\beta<0$. In the [Hückel method](../../chemistry.md#huckel-method), the dimensionless matrix $M=(H-\alpha I)/\beta$ has diagonal entries one on oxygen sites 1 and 8, zero on carbon, and unit entries between bonded neighbours. In the bases $(O_+,C_+,R_+)$ and $(O_-,C_-,R_-)$ above, its blocks are

$$
M_{B_{1u}}=\begin{pmatrix}1&1&0\\1&0&\sqrt2\\0&\sqrt2&1\end{pmatrix},\qquad
M_{B_{3g}}=\begin{pmatrix}1&1&0\\1&0&\sqrt2\\0&\sqrt2&-1\end{pmatrix}.
$$

The one-dimensional $B_{2g}$ and $A_u$ blocks have $\lambda=1$ and $-1$, respectively. The [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) of the $B_{1u}$ block factors as

$$
\det(\lambda I-M_{B_{1u}})=(\lambda-1)(\lambda^2-\lambda-3),
$$

so its three [molecular orbital](../../chemistry.md#molecular-orbital) energies are

$$
\boxed{E_{B_{1u}}=\alpha+\beta,\qquad\alpha+\frac{1+\sqrt{13}}2\beta,\qquad\alpha+\frac{1-\sqrt{13}}2\beta.}
$$

For the $B_{3g}$ block the [matrix trace](../../linear-algebra.md#matrix-trace) is zero. Thus its three $\lambda$ values sum to zero, and the pair supplied in the paper gives the remaining one as $-(1.86-2.12)\simeq0.26$. Directly, its secular equation is $\lambda^3-4\lambda+1=0$, whose roots are approximately $1.860806$, $0.254102$ and $-2.114908$. The supplied pair is approximate, so $0.26$ from its trace and $0.2541$ from the exact block should not be mistaken for an additional physical splitting.

All eight energies, ordered from low to high for $\beta<0$, are

$$
\begin{array}{c|c|c}
\lambda&\text{symmetry}&\text{neutral occupancy}\\\hline
2.302776&B_{1u}&2\\
1.860806&B_{3g}&2\\
1&B_{1u}&2\\
1&B_{2g}&2\\
0.254102&B_{3g}&0\\
-1&A_u&0\\
-1.302776&B_{1u}&0\\
-2.114908&B_{3g}&0
\end{array}
$$

The eight $\pi$ electrons fill the four lowest [molecular orbitals](../../chemistry.md#molecular-orbital). The equality at $\lambda=1$ is an accidental degeneracy of this parameterized model, not a multidimensional representation of $D_{2h}$.

<a id="a5/c/image-original-huckel-method-energy-level-diagram-for-neutral-para-quinone-with-eight-pi-electrons-and-its-unoccupied-b-3g-level"></a>
![](../../past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-1-quinone-energy-levels.png)

**[Figure 4](#a5/c/image-original-huckel-method-energy-level-diagram-for-neutral-para-quinone-with-eight-pi-electrons-and-its-unoccupied-b-3g-level). Original Hückel method energy-level diagram for neutral para-quinone, with eight $\pi$ electrons and its unoccupied $B_{3g}$ level**.

<h3 id="a5/d">d</h3>

↑ **Parent:** [A5](#a5)

<h4 id="a5/d/solution">Solution</h4>

↑ **Parent:** [D](#a5/d)

The extra electron occupies the [lowest unoccupied molecular orbital](../../chemistry.md#lowest-unoccupied-molecular-orbital) of the neutral molecule, the $B_{3g}$ orbital at the middle root $\lambda_L=0.25410169\ldots$ of $\lambda^3-4\lambda+1=0$. Write

$$
\psi_L=aO_-+bC_-+cR_-.
$$

The first and third rows of the $B_{3g}$ block give

$$
b=(\lambda_L-1)a,\qquad c=\frac{\sqrt2(\lambda_L-1)}{1+\lambda_L}a,\qquad
 a=\left[1+(\lambda_L-1)^2+\frac{2(\lambda_L-1)^2}{(1+\lambda_L)^2}\right]^{-1/2}.
$$

Choosing the overall phase so that site 1 is positive gives $(a,b,c)\simeq(0.664623,-0.495741,-0.559033)$. In the original site order,

$$
\boxed{\psi_L\simeq0.469959p_1-0.350542p_2-0.279516p_3-0.279516p_4
+0.279516p_5+0.279516p_6+0.350542p_7-0.469959p_8.}
$$

The squared coefficients sum to one. Within this fixed-orbital [Hückel orbital charge density](../../chemistry.md#huckel-orbital-charge-density) approximation, the added electron contributes site populations

$$
\Delta n_{1,8}\simeq0.220862\ \text{each},\qquad
\Delta n_{2,7}\simeq0.122880\ \text{each},\qquad
\Delta n_{3,4,5,6}\simeq0.078129\ \text{each}.
$$

Thus the oxygen sites $\boxed{1\text{ and }8}$ receive the largest added negative charge, each receiving an increment of approximately $-0.221e$. Including the four doubly occupied neutral orbitals gives an anion $\pi$ population of about $1.621$ on each oxygen, $0.870$ on sites 2 and 7, and $1.005$ on each remaining carbon. Thus oxygen also has the largest total $\pi$ population in this model. A coefficient's sign is an orbital phase, not the sign of its electric charge. Predicting an actual charge density would additionally require orbital relaxation and a population-analysis convention; the stated result is the requested orbital model.

## ↑ Ancestors (10)

1. [2025](../2025.md)
2. [Past exam of the chemistry A course of the University of Cambridge](../../past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge.md)
3. [Chemistry A course of the University of Cambridge](../../university-of-cambridge.md#chemistry-a-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
