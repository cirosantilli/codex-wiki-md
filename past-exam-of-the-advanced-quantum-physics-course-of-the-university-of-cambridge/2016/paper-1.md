# Paper 1

↑ **Parent:** [2016](../2016.md)

Original paper: [Public original PDF, physical pages 390–393; question pages 391–393](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=390).

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The open shell contains one $f$ [electron](../../physics.md#electron), so $L=3$ and $S=1/2$. For a less-than-half-filled shell, [Hund's rules](../../chemistry.md#hund-s-rules) select the smaller total angular [momentum](../../momentum.md), $J=L-S=5/2$, giving the free-ion ground level $ {}^2F_{5/2}$. The [Landé g-factor](../../atomic-physics.md#lande-g-factor) is

$$
g_J=\frac32+\frac{(1/2)(3/2)-3(4)}{2(5/2)(7/2)}
=\boxed{\frac67}.
$$

In a [magnetic field](../../magnetic-field.md) weak compared with the spin-orbit splitting, the electronic Zeeman shifts are $\delta E_{m_J}=g_J\mu_BBm_J$, for $m_J=-5/2,-3/2,\ldots,5/2$. Thus **six equally spaced magnetic substates** appear. At $B=1\,\mathrm T$, the adjacent-level spacing is

$$
\boxed{\Delta E_{\rm adjacent}=\frac67\mu_B B
=7.95\times10^{-24}\,\mathrm J
=4.96\times10^{-5}\,\mathrm{eV}.}
$$

The complete lowest-to-highest multiplet spread is five spacings,

$$
\boxed{\Delta E_{\rm full}=5\Delta E_{\rm adjacent}
=3.97\times10^{-23}\,\mathrm J
=2.48\times10^{-4}\,\mathrm{eV}.}
$$

Giving both quantities removes the ambiguity in the word splitting. This is the free-ion, weak-field result; no crystal-field doublet or [hyperfine structure](../../quantum-mechanics.md#hyperfine-structure) is specified.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Hermiticity supplies the reverse [matrix elements](../../vector-space.md#matrix-element), also equal to the real number $t$. In an [orthonormal basis](../../inner-product.md#orthonormal-basis) for the degenerate [eigenspace](../../linear-operator-theory.md#eigenspace), the perturbation is

$$
H_1=t\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix}
=t(\mathbf J_3-I),
$$

where $\mathbf J_3$ is the [all-ones matrix](../../vector-space.md#all-ones-matrix). Its symmetric [vector](../../vector-space.md#vector) $(1,1,1)/\sqrt3$ has [eigenvalue](../../linear-operator-theory.md#eigenvalue) $2t$. Every [vector](../../vector-space.md#vector) whose components sum to zero has [eigenvalue](../../linear-operator-theory.md#eigenvalue) $-t$; that subspace has dimension two. For example, $(1,-1,0)/\sqrt2$ and $(1,1,-2)/\sqrt6$ form an [orthonormal basis](../../inner-product.md#orthonormal-basis) for it.

The first-order energies are therefore

$$
\boxed{E_0+2t\quad\text{once},\qquad E_0-t\quad\text{twice}.}
$$

The [trace](../../linear-algebra.md#matrix-trace) of the shifts is $2t-t-t=0$, agreeing with the zero diagonal. The ordering depends on the sign of $t$; the formula does not assume that the symmetric state is the lowest. Diagonalizing the perturbation inside the degenerate space is essential: the original diagonal entries alone would incorrectly predict no splitting.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

Using a spherical Bohr-radius volume for the atom, the calculations below give a cutoff electromagnetic [vacuum energy density](../../perturbative-quantum-field-theory.md#vacuum-energy-density) of about $6.2\times10^{15}\,\mathrm{J\,m^{-3}}$, compared with a [hydrogen](../../chemical-substance.md#hydrogen) binding-energy density of about $3.5\times10^{12}\,\mathrm{J\,m^{-3}}$. **The cutoff vacuum estimate is about $1.8\times10^3$ times larger.** Alternative reasonable definitions of atomic volume change this ratio by a factor of a few, not the main order-of-magnitude conclusion.

The cutoff result is a bare zero-point mode sum. It is not a classical radiation bath incident on the atom, nor a calculation of an observable absolute vacuum energy without a subtraction or [renormalization](../../perturbative-quantum-field-theory.md#renormalization) prescription.

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

In a large periodic quantization volume $\mathcal V$, one [wavevector](../../elasticity-physics.md#wavevector) state occupies $(2\pi)^3/\mathcal V$ in [wavevector](../../elasticity-physics.md#wavevector) space. There are two transverse [photon polarizations](../../quantum-mechanics.md#photon-polarization), and each oscillator contributes $\hbar ck/2$. A lower [wavelength](../../wave-equation.md#wavelength) cutoff $\lambda_{\min}$ corresponds to $k_{\max}=2\pi/\lambda_{\min}$, so the [energy density](../../statistical-physics.md#energy-density) is

$$
u_{\rm vac}
=2\int_{|\mathbf k|\leq k_{\max}}\frac{\mathrm d^3k}{(2\pi)^3}
\frac{\hbar ck}{2}
=\frac{\hbar c}{2\pi^2}\int_0^{k_{\max}}k^3\,\mathrm dk
=\frac{\hbar c\,k_{\max}^4}{8\pi^2}
=\frac{2\pi^2\hbar c}{\lambda_{\min}^4}.
$$

For $\lambda_{\min}=10^{-10}\,\mathrm m$,

$$
\boxed{u_{\rm vac}\simeq6.24\times10^{15}\,\mathrm{J\,m^{-3}}.}
$$

The factor two is [polarization](../../wave.md#polarization-waves), not an extra independent count of positive and negative frequencies. The continuum [wavevector](../../elasticity-physics.md#wavevector) integral already counts independent travelling-wave modes in the usual field quantization convention. The quartic cutoff dependence also shows why an assumed shortest [wavelength](../../wave-equation.md#wavelength) is crucial.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Take the [hydrogen](../../chemical-substance.md#hydrogen) ground-state binding-energy magnitude as $E_B\simeq13.6\,\mathrm{eV}=2.18\times10^{-18}\,\mathrm J$, and use $a_0\simeq5.29\times10^{-11}\,\mathrm m$ as its characteristic radius. A definite volume convention is

$$
V_H=\frac{4\pi a_0^3}{3}\simeq6.21\times10^{-31}\,\mathrm{m^3}.
$$

It gives

$$
\boxed{u_H=\frac{E_B}{V_H}\simeq3.51\times10^{12}\,\mathrm{J\,m^{-3}},
\qquad\frac{u_{\rm vac}}{u_H}\simeq1.78\times10^3.}
$$

A quantum atom has no sharp outer surface. If instead its characteristic volume is taken as $a_0^3$, the estimate is $1.47\times10^{13}\,\mathrm{J\,m^{-3}}$ and the ratio is about $4.2\times10^2$. Both conventions place the two densities roughly three orders of magnitude apart at order-of-magnitude accuracy. The comparison uses the magnitude of the [binding energy](../../energy.md#binding-energy), not its negative sign relative to [ionization](../../atomic-physics.md#ionization).

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**The [WKB approximation](../../analysis.md#wkb-approximation) describes a wave whose local [wavelength](../../wave-equation.md#wavelength) changes slowly compared with one [wavelength](../../wave-equation.md#wavelength).** For the one-dimensional stationary [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation), put $p(x)=\sqrt{2m[E-V(x)]}$. In a [classically allowed region](../../mathematical-physics.md#classically-allowed-region),

$$
\psi(x)\simeq\frac{C_+}{\sqrt{p(x)}}\exp\!\left[\frac{i}{\hbar}\int^x p(s)\,\mathrm ds\right]
+\frac{C_-}{\sqrt{p(x)}}\exp\!\left[-\frac{i}{\hbar}\int^x p(s)\,\mathrm ds\right].
$$

The [phase](../../wave.md#phase-waves) is the classical action divided by $\hbar$. The amplitude varies as $p^{-1/2}$ so that a single travelling component has constant [probability current](../../wave-function.md#probability-current). A useful local validity condition is $|\hbar p'/p^2|\ll1$.

For $V>E$, write $\kappa=\sqrt{2m(V-E)}/\hbar$. The wave instead has growing and decaying components proportional to $\kappa^{-1/2}\exp(\pm\int\kappa\,\mathrm dx)$. At a simple [turning point](../../energy.md#turning-point), $p$ vanishes and neither local WKB expression is valid. Linearizing the potential gives an Airy-function solution that connects the two sides and supplies the turning-point [phase](../../wave.md#phase-waves) shift. It is not legitimate to carry the divergent WKB amplitude straight through the [turning point](../../energy.md#turning-point).[§2.2, semiclassical expansion and linear-potential matching](../../physics-bibliography.md#topics-in-quantum-mechanics-by-david-tong)

**A useful application is tunnelling through a smooth opaque barrier.** With [turning points](../../energy.md#turning-point) $x_1,x_2$, the leading [transmission probability](../../quantum-scattering.md#transmission-probability) is

$$
\boxed{T\simeq\exp\!\left[-2\int_{x_1}^{x_2}\kappa(x)\,\mathrm dx\right].}
$$

The exponent is twice the forbidden-region action in units of $\hbar$, because transmission is a [probability](../../probability-theory.md#probability) rather than a wave amplitude. For an ideal rectangular barrier of height $V_0>E$ and width $d$, the same leading exponential is $\exp[-2d\sqrt{2m(V_0-E)}/\hbar]$; matching at the abrupt edges supplies an additional prefactor.

<a id="2/a/image-original-smooth-barrier-construction-and-leading-wkb-transmission-exponent-the-shaded-interval-is-classically-forbidden"></a>
![](../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1-wkb-tunnelling.png)

**[Figure 1](#2/a/image-original-smooth-barrier-construction-and-leading-wkb-transmission-exponent-the-shaded-interval-is-classically-forbidden). Original smooth-barrier construction and leading WKB transmission exponent; the shaded interval is classically forbidden**.

For a bound state between two smooth [turning points](../../energy.md#turning-point), the related WKB quantization rule is $\int_{x_1}^{x_2}p\,\mathrm dx=(n+1/2)\pi\hbar$. In a [harmonic potential](../../energy.md#harmonic-potential) the integral equals $\pi E/\omega$, recovering $E_n=(n+1/2)\hbar\omega$. This exact agreement of energies for the harmonic oscillator does not make WKB [wavefunctions](../../wave-function.md) uniformly exact near its [turning points](../../energy.md#turning-point).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**[Stimulated emission](../../laser.md#stimulated-emission) adds a [photon](../../quantum-mechanics.md#photon) to an already occupied radiation mode; [spontaneous emission](../../atomic-physics.md#spontaneous-emission) can occur when that mode initially contains no [photons](../../quantum-mechanics.md#photon).** In the [electric-dipole approximation](../../quantum-mechanics.md#electric-dipole-approximation) the atom-field interaction is $H_{\rm int}=-\mathbf d\cdot\mathbf E$. Quantizing the radiation field makes the emission [matrix element](../../vector-space.md#matrix-element) into a mode with occupation $n$ proportional to

$$
\langle n+1|a^\dagger|n\rangle=\sqrt{n+1}.
$$

This [photon occupation enhancement of emission](../../laser.md#photon-occupation-enhancement-of-emission) makes the emission rate into that mode proportional to $n+1$: the part proportional to $n$ is stimulated and the remaining part is spontaneous. Absorption is proportional to $|\langle n-1|a|n\rangle|^2=n$. The [photon](../../quantum-mechanics.md#photon) energy is the atomic energy difference, up to any specified recoil or line broadening.

The stimulated contribution preferentially populates the stimulating mode, including its propagation direction and [polarization](../../wave.md#polarization-waves); it provides [optical gain](../../laser.md#optical-gain). Spontaneous [photons](../../quantum-mechanics.md#photon) populate the available modes according to the transition's dipole [matrix elements](../../vector-space.md#matrix-element) and radiation environment. They are not universally isotropic. An excited bare atom with the field vacuum is not an [eigenstate](../../energy-eigenvalue.md#eigenstate) of the fully coupled [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian), which resolves the apparent paradox of a nominally stationary excited state radiating.[§4.3.2, why the electromagnetic field must be included to describe spontaneous decay](../../physics-bibliography.md#topics-in-quantum-mechanics-by-david-tong)

<a id="2/b/image-original-two-level-transition-diagrams-and-the-n-versus-n-plus-1-occupation-factors-for-photon-absorption-and-emission"></a>
![](../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1-emission.png)

**[Figure 2](#2/b/image-original-two-level-transition-diagrams-and-the-n-versus-n-plus-1-occupation-factors-for-photon-absorption-and-emission). Original two-level transition diagrams and the $n$ versus $n+1$ occupation factors for photon absorption and emission**.

For lower and upper levels 1 and 2, with radiation spectral [energy density](../../statistical-physics.md#energy-density) $u_\nu$ per unit ordinary frequency, the rates are

$$
R_{\rm abs}=N_1B_{12}u_\nu,\qquad
R_{\rm stim}=N_2B_{21}u_\nu,\qquad
R_{\rm sp}=N_2A_{21}.
$$

Thermal detailed balance with the [Planck spectrum](../../statistical-physics.md#blackbody-spectrum) gives

$$
\boxed{g_1B_{12}=g_2B_{21},\qquad
\frac{A_{21}}{B_{21}}=\frac{8\pi h\nu^3}{c^3}.}
$$

The statistical weights $g_i$ here are level degeneracies, not [Landé g-factors](../../atomic-physics.md#lande-g-factor). A definition of $B$ multiplying intensity or angular-frequency density would change the normalization factors.

For a specified free-space electric-dipole transition, summing radiation modes gives

$$
A_{21}=\frac{\omega_{21}^3|\mathbf d_{12}|^2}
{3\pi\epsilon_0\hbar c^3},
\qquad \omega_{21}=2\pi\nu.
$$

Appropriate sums over final magnetic substates and averages over initial substates are needed for an unresolved degenerate level. The radiative lifetime is $1/A_{21}$ only when this is the sole decay channel. In a [laser](../../laser.md), net stimulated gain requires $N_2/g_2>N_1/g_1$, as well as sufficient gain to overcome cavity loss; [population inversion](../../laser.md#population-inversion) alone does not specify the lasing threshold.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**[Fermi's golden rule](../../quantum-mechanics.md#fermi-s-golden-rule) converts a weak transition [matrix element](../../vector-space.md#matrix-element) and the available density of final states into a transition rate.** For a static perturbation $W$ and a continuum,

$$
\boxed{\Gamma_{i\to{\rm all}}=\frac{2\pi}{\hbar}
\int |\langle f|W|i\rangle|^2\delta(E_f-E_i)\,\mathrm dN_f.}
$$

When the [matrix element](../../vector-space.md#matrix-element) is nearly constant on the energy shell, this becomes $(2\pi/\hbar)|W_{fi}|^2\rho(E_i)$. The energy delta function is to be integrated, rather than interpreted as a finite rate to one exactly resonant discrete level. The observation time must resolve a smooth final-state continuum while remaining short enough that first-order depletion is small. A periodically driven perturbation instead gives the corresponding absorption and emission energy shells.

For elastic scattering from a weak localized potential $W(\mathbf r)$, use box-normalized free states $\langle\mathbf r|\mathbf k\rangle=\mathcal V^{-1/2}e^{i\mathbf k\cdot\mathbf r}$. Then

$$
W_{fi}=\frac1{\mathcal V}\widetilde W(\mathbf q),\qquad
\widetilde W(\mathbf q)=\int e^{-i\mathbf q\cdot\mathbf r}
W(\mathbf r)\,\mathrm d^3r,\qquad
\mathbf q=\mathbf k_f-\mathbf k_i.
$$

The number of final states is $\mathcal V k_f^2\,\mathrm dk_f\,\mathrm d\Omega/(2\pi)^3$. With $E_f=\hbar^2k_f^2/(2m)$, the density per energy and [solid angle](../../euclidean-geometry.md#solid-angle) is $\mathcal V m k_f/[(2\pi)^3\hbar^2]$. Dividing the resulting golden-rule rate by the incident single-particle flux $j_i=\hbar k_i/(m\mathcal V)$ gives

$$
\frac{\mathrm d\sigma}{\mathrm d\Omega}
=\frac{m^2}{4\pi^2\hbar^4}\frac{k_f}{k_i}
|\widetilde W(\mathbf q)|^2.
$$

This is the [golden-rule derivation of the Born cross-section](../../quantum-mechanics.md#golden-rule-derivation-of-the-born-cross-section). For the elastic problem $k_f=k_i$, so the first Born [scattering amplitude](../../quantum-scattering.md#scattering-amplitude) and cross-section are

$$
\boxed{f_B(\mathbf k_f,\mathbf k_i)
=-\frac{m}{2\pi\hbar^2}\widetilde W(\mathbf q),\qquad
\frac{\mathrm d\sigma}{\mathrm d\Omega}=|f_B|^2.}
$$

The box volume cancels, as a physical cross-section must. The minus sign is fixed by the outgoing-wave scattering convention; the golden-rule rate alone determines only the modulus.

For example, $W(r)=g e^{-\kappa r}/r$ has $\widetilde W=4\pi g/(q^2+\kappa^2)$, hence $f_B=-2mg/[\hbar^2(q^2+\kappa^2)]$, with $q=2k\sin(\theta/2)$. Replacing the exact scattering state by the incident [plane wave](../../wave-function.md#plane-wave) is the essential [Born approximation](../../quantum-theory.md#born-approximation). It can fail for strong scattering, low-energy resonances and situations requiring repeated scattering; a small perturbation and a suitable continuum are separate conditions.[§6.3, Born approximation and Yukawa-potential example](../../physics-bibliography.md#topics-in-quantum-mechanics-by-david-tong)

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

**[Spin](../../angular-momentum-operator.md#spin) and spatial exchange symmetry.** Write the normalized [spin](../../angular-momentum-operator.md#spin) singlet and [triplet states](../../angular-momentum-operator.md#spin-one-half-triplet-state) as

$$
\chi_{00}=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2},
\qquad
\chi_{11}=|\uparrow\uparrow\rangle,\quad
\chi_{10}=\frac{|\uparrow\downarrow\rangle+|\downarrow\uparrow\rangle}{\sqrt2},
\quad\chi_{1,-1}=|\downarrow\downarrow\rangle.
$$

The singlet is antisymmetric under exchange and has total [spin](../../angular-momentum-operator.md#spin) zero; the triplet is symmetric and has total [spin](../../angular-momentum-operator.md#spin) one. For orthogonal orbitals define

$$
C=\frac{|ab\rangle+|ba\rangle}{\sqrt2},\qquad
A=\frac{|ab\rangle-|ba\rangle}{\sqrt2}.
$$

Identical [spin one-half](../../angular-momentum-operator.md#spin-one-half) particles are [fermions](../../tensor-product-of-quantum-systems.md#fermion), so the complete state must be antisymmetric. Thus **$C\chi_{00}$ is allowed, and $A\chi_{1M}$ is allowed for each triplet component**. The spatially symmetric same-orbital states $|aa\rangle,|bb\rangle$ also require the singlet. A same-orbital triplet vanishes by the [Pauli exclusion principle](../../tensor-product-of-quantum-systems.md#pauli-exclusion-principle).

These products give a spin-adapted basis. More generally the physical state can be written

$$
|\Psi\rangle=(c_a|aa\rangle+c_b|bb\rangle+c_C C)\chi_{00}
+A\sum_{M=-1}^{1}d_M\chi_{1M}.
$$

A superposition of the singlet and triplet sectors need not factor into one spatial function times one [spin](../../angular-momentum-operator.md#spin) function. Factorization holds for a definite-spin sector, as used in the subsequent model. If the original normalized orbitals are not orthogonal, the corresponding $ab\pm ba$ normalization is $\sqrt{2(1\pm|\langle a|b\rangle|^2)}$; the remainder of this calculation uses the stipulated orthogonal orbitals.

**Integral [matrix elements](../../vector-space.md#matrix-element) and positivity.** Let $a(\mathbf r)$ and $b(\mathbf r)$ denote the localized [spatial orbitals](../../tensor-product-of-quantum-systems.md#spatial-orbital). With fixed [proton](../../physics.md#proton) positions, the one-electron electronic operator is

$$
h=-\frac{\hbar^2}{2m_e}\nabla^2
-\frac{e^2}{4\pi\epsilon_0}
\left(\frac1{|\mathbf r-\mathbf R_a|}+
\frac1{|\mathbf r-\mathbf R_b|}\right).
$$

The proton-proton repulsion is a separate common nuclear energy. The requested one-electron and direct two-electron elements are

$$
\langle a|h|a\rangle=\int a^*(\mathbf r)\,h\,a(\mathbf r)\,\mathrm d^3r,
$$



$$
J_{ab}=\langle ab|H_{1,2}|ab\rangle
=\frac{e^2}{4\pi\epsilon_0}
\iint\frac{|a(\mathbf r_1)|^2|b(\mathbf r_2)|^2}
{|\mathbf r_1-\mathbf r_2|}\,\mathrm d^3r_1\,\mathrm d^3r_2.
$$

Since $H_1=h\otimes I$,

$$
\boxed{\langle aa|H_1|ab\rangle
=\langle a|h|a\rangle\langle a|b\rangle=0.}
$$

Likewise,

$$
\boxed{U=\frac{e^2}{4\pi\epsilon_0}
\iint\frac{|a(\mathbf r_1)|^2|a(\mathbf r_2)|^2}
{|\mathbf r_1-\mathbf r_2|}\,\mathrm d^3r_1\,\mathrm d^3r_2>0.}
$$

The integrand is nonnegative and is positive on a set of nonzero measure. This is the repulsion cost of [double occupancy](../../statistical-physics.md#double-occupancy); the coincidence singularity is integrable for ordinary smooth localized orbitals.

**One [electron](../../physics.md#electron) on each center.** Suppress the normalized singlet [spin](../../angular-momentum-operator.md#spin) factor and use $|\psi\rangle=C$. For each of the spatial products $ab$ and $ba$, the one-body sum has expectation $2E_0$. The cross terms vanish because a one-body hop leaves an orthogonal spectator orbital. The interaction contribution is the direct integral plus the [exchange integral](../../chemistry.md#exchange-integral), both neglected in the model. Consequently

$$
\boxed{E_\psi=\langle C|H|C\rangle=2E_0.}
$$

This state has no same-center [double occupancy](../../statistical-physics.md#double-occupancy), but remains an exchange-symmetric spatial superposition rather than assigning a distinguishable [electron](../../physics.md#electron) permanently to each [proton](../../physics.md#proton).

**Two [electrons](../../physics.md#electron) in the bonding orbital.** The normalized one-electron bonding orbital is $g=(a+b)/\sqrt2$. The trial spatial state is $|\phi\rangle=|gg\rangle$, whose one-body expectation is

$$
2\langle g|h|g\rangle
=2\left[\frac{E_0+E_0+t+t}{2}\right]
=2E_0+2t.
$$

Expanding the product gives $|\phi\rangle=(|aa\rangle+|ab\rangle+|ba\rangle+|bb\rangle)/2$. The total [probability](../../probability-theory.md#probability) of [double occupancy](../../statistical-physics.md#double-occupancy) is therefore $1/2$. Keeping only [on-site Coulomb repulsion](../../statistical-physics.md#on-site-coulomb-repulsion) gives the intended interaction truncation,

$$
H_{1,2}\simeq U\bigl(|aa\rangle\langle aa|+|bb\rangle\langle bb|\bigr),
$$

and the interaction expectation is $U/2$. Hence

$$
\boxed{E_\phi=2E_0+2t+\frac U2.}
$$

This truncation must be stated. In particular, mixed Coulomb elements such as $X=\langle aa|H_{1,2}|ab\rangle$ do not vanish merely by orbital [orthogonality](../../inner-product.md#orthogonal-vectors) or inversion symmetry. The printed list does not explicitly name them. If they are retained and are equal and real by site symmetry, their contribution to $E_\phi$ is $2X$; the requested expression uses their neglect along with the other off-site interaction terms. No numerical value of $X$ is supplied or invented.

**Energy comparison and the bond.** Put $x=|t|/U$ with $U>0$ and $t=-|t|$. Then

$$
\boxed{\frac{E_\phi-E_\psi}{U}=\frac12-2x.}
$$

The straight line starts at $1/2$ and crosses zero at $x=1/4$. The purely bonding-orbital trial state is better for $x>1/4$, while the singly occupied covalent trial state is better for $x<1/4$.

<a id="3/image-original-two-site-singlet-calculation-trial-energy-comparison-continuous-optimized-energy-and-double-occupancy-crossover-in-the-stated-on-site-model"></a>
![](../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1-two-site-bond.png)

**[Figure 3](#3/image-original-two-site-singlet-calculation-trial-energy-comparison-continuous-optimized-energy-and-double-occupancy-crossover-in-the-stated-on-site-model). Original two-site singlet calculation: trial-energy comparison, continuous optimized energy and double-occupancy crossover in the stated on-site model**.

For localized orbitals of approximately fixed atomic size, the hopping magnitude $|t|$ decreases rapidly, typically exponentially times a polynomial, as the [proton](../../physics.md#proton) separation grows. The on-site integral $U$ remains of atomic Coulomb scale and tends to the isolated-orbital value; it does not decay as the intersite repulsion $1/R$. If the orbitals themselves are allowed to relax, $U$ also changes, so no universal monotonic law for $U(R)$ follows from the data.

At small $|t|/U$, [electron correlation](../../physics.md#electron-correlation) suppresses the ionic configurations $aa$ and $bb$, favoring a singlet with roughly one [electron](../../physics.md#electron) on each center. A single doubly occupied bonding orbital has an artificial finite ionic weight even as the centers separate. At large $|t|/U$, delocalization gains enough [kinetic energy](../../energy.md#kinetic-energy) that the bonding-orbital description becomes useful and charge fluctuations are substantial.

The crossing of two restricted trial energies is **not a sharp transition of the actual two-site [ground state](../../quantum-mechanics.md#ground-state)**. To see this without adding empirical data, include both $C$ and the symmetric ionic state $I_+=(|aa\rangle+|bb\rangle)/\sqrt2$. This [two-site Hubbard dimer](../../statistical-physics.md#two-site-hubbard-dimer) reduces to

$$
H-2E_0I=\begin{pmatrix}0&2t\\2t&U\end{pmatrix}_{C,I_+},
\qquad
\boxed{E_g=2E_0+\frac{U-\sqrt{U^2+16t^2}}2.}
$$

Its [ground state](../../quantum-mechanics.md#ground-state) is $\cos\theta\,C+\sin\theta\,I_+$, with $\tan2\theta=4|t|/U$ and $0\leq\theta\leq\pi/4$. The ionic [probability](../../probability-theory.md#probability) is

$$
P_{\rm double}=\frac12\left(1-\frac{U}{\sqrt{U^2+16t^2}}\right).
$$

It changes smoothly from zero to $1/2$. At large separation, the electronic lowering is $-4t^2/U$ to leading order and vanishes as hopping vanishes. An absolute molecular binding curve would additionally require $E_0(R)$, the nuclear repulsion and the neglected intersite terms; this simplified comparison alone does not determine an equilibrium [bond length](../../chemical-bond.md#bond-length).

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

**Uniform system and dispersion.** A [plane wave](../../wave-function.md#plane-wave) reduces the differential [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) to a two-by-two [matrix](../../vector-space.md#matrix) acting on its [spinor](../../algebra-over-a-field.md#spinor):

$$
H(\mathbf k)=
\begin{pmatrix}
V&\hbar c(k_x-ik_y)\\
\hbar c(k_x+ik_y)&-V
\end{pmatrix}
=\mathbf d(\mathbf k)\cdot\boldsymbol\sigma,
\qquad
\mathbf d=(\hbar ck_x,\hbar ck_y,V).
$$

The Pauli anticommutation relations imply $H(\mathbf k)^2=|\mathbf d|^2I$. Choosing a [spinor](../../algebra-over-a-field.md#spinor) in one of its [eigenspaces](../../linear-operator-theory.md#eigenspace) therefore gives

$$
\boxed{E_\pm(k)=\pm\sqrt{\hbar^2c^2k^2+V^2},\qquad k=|\mathbf k|.}
$$

An arbitrary constant [spinor](../../algebra-over-a-field.md#spinor) multiplying a [plane wave](../../wave-function.md#plane-wave) is not necessarily an [energy eigenstate](../../energy-eigenvalue.md#energy-eigenstate); it must be an eigenvector of this [matrix](../../vector-space.md#matrix). For example, for the upper branch and $\varepsilon=|\mathbf d|$, one can use

$$
u_+(\mathbf k)=
\frac1{\sqrt{2\varepsilon(\varepsilon+V)}}
\begin{pmatrix}\varepsilon+V\\\hbar c(k_x+ik_y)\end{pmatrix},
$$

away from the coordinate singularity $\varepsilon+V=0$, where another normalized eigenvector chart is used.

For the usual $c>0$ convention, the massless branches are $E_\pm=\pm\hbar ck$. For nonzero $V$, the two branches have a gap $2|V|$ and are quadratic near $k=0$:

$$
E_\pm\simeq\pm|V|\pm\frac{\hbar^2c^2k^2}{2|V|}.
$$

**Changing the sign of $V$ does not change these energies.** It reverses the out-of-plane [spin](../../angular-momentum-operator.md#spin) [polarization](../../wave.md#polarization-waves) of a given band at the origin. The plots for equal positive and negative mass magnitudes therefore have identical dispersion curves, despite their different [spinors](../../algebra-over-a-field.md#spinor).

<a id="4/image-original-calculated-massive-and-massless-two-dimensional-dirac-dispersions-equal-and-opposite-masses-share-energies-but-reverse-the-band-spin-at-zero-momentum"></a>
![](../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1-dirac-bands.png)

**[Figure 4](#4/image-original-calculated-massive-and-massless-two-dimensional-dirac-dispersions-equal-and-opposite-masses-share-energies-but-reverse-the-band-spin-at-zero-momentum). Original calculated massive and massless two-dimensional Dirac dispersions; equal and opposite masses share energies but reverse the band spin at zero momentum**.

**[Spin](../../angular-momentum-operator.md#spin) direction in the massless case.** For $k>0$ put $k_x+ik_y=ke^{i\varphi}$. The normalized eigenspinors can be chosen as

$$
u_s(\mathbf k)=\frac1{\sqrt2}
\begin{pmatrix}1\\s e^{i\varphi}\end{pmatrix},
\qquad E_s=s\hbar ck,\qquad s=\pm1.
$$

Direct multiplication gives $\langle\sigma_x\rangle=s\cos\varphi$, $\langle\sigma_y\rangle=s\sin\varphi$ and $\langle\sigma_z\rangle=0$. Since the [Pauli matrices](../../algebra.md#pauli-matrices) represent physical [spin](../../angular-momentum-operator.md#spin) in this question,

$$
\boxed{\langle\mathbf S\rangle_s
=s\frac{\hbar}{2}\frac{(k_x,k_y,0)}{k}.}
$$

The [spin](../../angular-momentum-operator.md#spin) is **parallel to [momentum](../../momentum.md) on the positive-energy branch and antiparallel on the negative-energy branch**. Thus the branch-independent statement is collinearity; the printed parallel claim needs the positive-branch qualification. At $k=0,V=0$, the [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) is zero and [spin](../../angular-momentum-operator.md#spin) is not fixed by a [wavevector](../../elasticity-physics.md#wavevector) direction.

**Mass-domain-wall [eigenstate](../../energy-eigenvalue.md#eigenstate).** Assume $c>0$ for the stated normalizable wall state and write

$$
F(y)=\exp\!\left[-\frac1{\hbar c}\int_0^y V(s)\,\mathrm ds\right],
\qquad u_-=\frac1{\sqrt2}\begin{pmatrix}1\\-1\end{pmatrix}.
$$

Then $F'=-VF/(\hbar c)$, $\sigma_xu_-=-u_-$, and $(i\sigma_y+\sigma_z)u_-=0$. Applying the full operator gives

$$
H\{e^{ik_xx}F(y)u_-\}
=e^{ik_xx}F(y)
\{\hbar ck_x\sigma_x+iV(y)\sigma_y+V(y)\sigma_z\}u_-
=-\hbar ck_x\,e^{ik_xx}F(y)u_-.
$$

The transverse derivative and mass terms cancel pointwise. Hence **the specified state is an [eigenstate](../../energy-eigenvalue.md#eigenstate) with $E=-\hbar ck_x$**.

For a step mass $V(y)=V_+>0$ above the interface and $V(y)=V_-<0$ below it,

$$
F(y)=\begin{cases}
e^{-y/\xi_+},&y>0,\\
e^{y/\xi_-},&y<0,
\end{cases}
\qquad
\boxed{\xi_+=\frac{\hbar c}{V_+},\qquad
\xi_-=\frac{\hbar c}{|V_-|}.}
$$

The [Localization length at a step Dirac mass wall](../../relativistic-quantum-field.md#localization-length-at-a-step-dirac-mass-wall) sets the two exponential tails. The amplitude is continuous, peaks at the interface and decays on both sides, with generally unequal decay lengths. The [probability density](../../wave-function.md#probability-density) decays with lengths $\xi_\pm/2$. A normalized transverse function is $f(y)=\sqrt{2/(\xi_++\xi_-)}F(y)$ when multiplying the unit [spinor](../../algebra-over-a-field.md#spinor) $u_-$. The longitudinal [plane wave](../../wave-function.md#plane-wave) can independently be box-normalized. A step in $V$ allows a step in $F'$; the first-order Dirac equation does not impose continuity of that derivative.

<a id="4/image-original-mass-wall-solution-asymmetric-exponential-confinement-the-chiral-energy-branch-and-rigid-longitudinal-translation-of-a-localized-packet"></a>
![](../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1-dirac-interface.png)

**[Figure 5](#4/image-original-mass-wall-solution-asymmetric-exponential-confinement-the-chiral-energy-branch-and-rigid-longitudinal-translation-of-a-localized-packet). Original mass-wall solution: asymmetric exponential confinement, the chiral energy branch and rigid longitudinal translation of a localized packet**.

**Propagation.** The interface dispersion is the straight line

$$
\boxed{E(k_x)=-\hbar ck_x,\qquad
v_x=\frac1{\hbar}\frac{\mathrm dE}{\mathrm dk_x}=-c.}
$$

Every component on this branch travels in the negative $x$ direction. A packet has the form

$$
\Psi(x,y,t)=f(y)u_-\int A(k_x)e^{ik_x(x+ct)}\,\mathrm dk_x
=f(y)u_-\,g(x+ct).
$$

This [dispersionless chiral interface wavepacket](../../relativistic-quantum-field.md#dispersionless-chiral-interface-wavepacket) therefore translates rigidly with speed $c$ in that direction, without dispersion in this exactly linear model. It remains confined in $y$; there is no free transverse [group velocity](../../dispersion-relation.md#group-velocity), because the bound-state family is not labelled by a transverse travelling-wave [momentum](../../momentum.md).

The [continuity equation](../../mathematical-physics.md#continuity-equation) gives the current components $j_x=c\Psi^\dagger\sigma_x\Psi=-c|\Psi|^2$ and $j_y=c\Psi^\dagger\sigma_y\Psi=0$. This explicitly confirms absence of [probability](../../probability-theory.md#probability) transport away from the interface. For the step-mass case the profile is normalizable because its tails have positive decay constants and $c>0$. A general sign-changing profile also requires $F\in L^2(\mathbb R)$; nonzero asymptotic masses suffice, whereas signs alone do not guarantee confinement if their integrated magnitudes grow too slowly. If $c<0$, the supplied exponential instead grows at infinity; a normalizable state requires the opposite [spinor](../../algebra-over-a-field.md#spinor) and envelope sign. Reversing the wall orientation also reverses the propagation chirality.

## ↑ Ancestors (11)

1. [2016](../2016.md)
2. [Past exam of the advanced quantum physics course of the University of Cambridge](../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge.md)
3. [Advanced Quantum Physics course of the University of Cambridge](../../university-of-cambridge.md#advanced-quantum-physics-course-of-the-university-of-cambridge)
4. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
