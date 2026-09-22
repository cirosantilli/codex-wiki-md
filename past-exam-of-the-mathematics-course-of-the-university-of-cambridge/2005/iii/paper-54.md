# Paper 54

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper54.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper54.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use target signature $(-,+,\ldots,+)$ and a closed-string spatial coordinate $0\le\sigma\le2\pi$. Write $Y$ for the compact coordinate and $X^A$ for the noncompact coordinates. In [conformal gauge](../../../string-theory.md#conformal-gauge), the [wave equation](../../../wave-equation.md) factorizes, so every coordinate is a sum of a function of $\tau+\sigma$ and a function of $\tau-\sigma$. The closed-string boundary conditions are

$$
X^A(\tau,\sigma+2\pi)=X^A(\tau,\sigma),\qquad Y(\tau,\sigma+2\pi)=Y(\tau,\sigma)+2\pi wR,\quad w\in\mathbb Z.
$$

Thus the [derivatives](../../../calculus.md#derivative) of each chiral part are periodic and have [integer](../../../number-theory.md#integer) [Fourier modes](../../../fourier-analysis.md#fourier-mode); only their [worldsheet zero modes](../../../string-theory.md#worldsheet-zero-mode) can produce the winding displacement. Integrating these [Fourier series](../../../fourier-series.md) gives the [closed-string mode expansion](../../../string-theory.md#closed-string-mode-expansion)

$$
X^A=x^A+\alpha'p^A\tau+i\sqrt{\frac{\alpha'}2}\sum_{m\ne0}\frac{\alpha_m^Ae^{-im(\tau-\sigma)}+\widetilde\alpha_m^Ae^{-im(\tau+\sigma)}}m,
$$



$$
Y=y+\alpha'\frac nR\tau+wR\sigma+i\sqrt{\frac{\alpha'}2}\sum_{m\ne0}\frac{\alpha_m^Ye^{-im(\tau-\sigma)}+\widetilde\alpha_m^Ye^{-im(\tau+\sigma)}}m.
$$

The oscillator reality conditions are $\alpha_m^\dagger=\alpha_{-m}$ and similarly for the tilded modes. The coefficient of $\tau$ follows by integrating the [canonical momentum](../../../classical-mechanics.md#canonical-momentum) density $\dot Y/(2\pi\alpha')$. Single-valued wavefunctions of the center coordinate $y\sim y+2\pi R$ have [momentum](../../../classical-mechanics.md#momentum) $n/R$, with $n\in\mathbb Z$. Equivalently, the compact chiral [worldsheet zero modes](../../../string-theory.md#worldsheet-zero-mode) are $\alpha'p_L(\tau+\sigma)/2$ and $\alpha'p_R(\tau-\sigma)/2$, where

$$
\boxed{p_L=\frac nR+\frac{wR}{\alpha'},\qquad p_R=\frac nR-\frac{wR}{\alpha'}.}
$$

Here tildes denote the left-moving sector. This convention will also fix the sign in [compact-circle closed-string level matching](../../../string-theory.md#compact-circle-closed-string-level-matching).

Choose a noncompact light-cone pair and impose [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory) $X^+=x^++\alpha'p^+\tau$, with $p^+\ne0$. The [Virasoro constraints](../../../string-theory.md#virasoro-constraint) $(\partial_\pm X)^2=0$ then solve for $\partial_\pm X^-$ in terms of the transverse coordinates. For example, with $\partial_\pm=\partial_\tau\pm\partial_\sigma$, one has $\partial_\pm X^-=(\partial_\pm X^i)^2/(2\alpha'p^+)$. Thus there are two independent transverse oscillator [Fock spaces](../../../quantum-field-theory.md#fock-space), including $Y$ among the transverse coordinates. Quantization gives $[\alpha_m^i,\alpha_k^j]=m\delta^{ij}\delta_{m+k,0}$, and the same relation for the tilded oscillators, with the two sectors commuting. Lorentz consistency gives the [critical dimension of the bosonic string](../../../string-theory.md#critical-dimension-of-string-theory) $D=26$ and [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) one in each sector. Accordingly

$$
N=\sum_{m>0}\alpha_{-m}^i\alpha_m^i,\qquad \widetilde N=\sum_{m>0}\widetilde\alpha_{-m}^i\widetilde\alpha_m^i
$$

count 24 transverse oscillator species. The two zero-mode constraints give the lower-dimensional [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum)

$$
M^2=p_R^2+\frac4{\alpha'}(N-1)=p_L^2+\frac4{\alpha'}(\widetilde N-1).
$$

Taking their difference and average yields

$$
\boxed{\widetilde N-N+nw=0,\qquad M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}+\frac2{\alpha'}(N+\widetilde N-2).}
$$

Every choice of transverse [string oscillators](../../../string-theory.md#string-oscillator) and [integer](../../../number-theory.md#integer) charges satisfying this [closed-string level matching](../../../string-theory.md#closed-string-level-matching) is a [physical string state](../../../string-theory.md#physical-string-state) in light-cone gauge. The eliminated longitudinal oscillators do not supply additional polarizations.

To classify all massless states, positivity of the two compact terms implies $N+\widetilde N\le2$. When the sum is two, masslessness forces $n=w=0$, and [closed-string level matching](../../../string-theory.md#closed-string-level-matching) then forces $N=\widetilde N=1$. The states $\alpha_{-1}^i\widetilde\alpha_{-1}^j|0\rangle$ have $24^2=576$ polarizations. In 25 noncompact dimensions, their decomposition gives a [graviton](../../../quantum-theory.md#graviton), a [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), a [dilaton](../../../string-theory.md#dilaton), two Abelian gauge vectors from the metric and two-form with one compact index, and the radius [scalar field](../../../quantum-field-theory.md#scalar-field). Their physical polarization counts are

$$
275+253+2\cdot23+1+1=576.
$$

The first two numbers are the symmetric [traceless second-rank tensor](../../../linear-algebra.md#traceless-second-rank-tensor) and [antisymmetric second-rank tensor](../../../linear-algebra.md#antisymmetric-second-rank-tensor) of the massless [little group](../../../special-relativity.md#little-group) $SO(23)$.

When $N+\widetilde N=1$, [closed-string level matching](../../../string-theory.md#closed-string-level-matching) requires $|nw|=1$. The compact contribution obeys

$$
\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}\ge\frac{2|nw|}{\alpha'}=\frac2{\alpha'},
$$

and equality occurs precisely at $R=\sqrt{\alpha'}$. The charges $n=w=\pm1$ have $(N,\widetilde N)=(1,0)$; the charges $n=-w=\pm1$ have $(N,\widetilde N)=(0,1)$. Each charge has 24 polarizations supplied by its single excited sector. At a general radius these have

$$
M^2=\left(\frac R{\alpha'}-\frac1R\right)^2.
$$

Finally, $N=\widetilde N=0$ requires $nw=0$. The [exceptional massless ground states of a bosonic circle](../../../string-theory.md#exceptional-massless-ground-states-of-a-bosonic-circle) occur at

$$
R=\frac{|n|\sqrt{\alpha'}}2\quad(w=0,n\ne0),\qquad R=\frac{2\sqrt{\alpha'}}{|w|}\quad(n=0,w\ne0).
$$

Each charge is a [scalar field](../../../quantum-field-theory.md#scalar-field). These special radii must be included if “general radius” is to mean a complete classification, rather than only a generic radius. **At a generic radius the massless spectrum is the neutral 576-state spectrum above; at exceptional radii one adds exactly the states just listed.** The neutral [ground state](../../../quantum-mechanics.md#ground-state) remains tachyonic.

The map

$$
R'=\frac{\alpha'}R,\qquad (n',w')=(w,n)
$$

sends $p_L$ to $p_L$ and $p_R$ to $-p_R$. Reversing all right-moving compact [string oscillators](../../../string-theory.md#string-oscillator), $\alpha_m^Y\mapsto-\alpha_m^Y$, preserves their [commutators](../../../lie-algebra.md#commutator) and oscillator number; the left-moving oscillators are unchanged. Both the mass formula and [compact-circle closed-string level matching](../../../string-theory.md#compact-circle-closed-string-level-matching) are therefore unchanged, with a one-to-one map of the complete oscillator basis. **This proves [T-duality](../../../string-theory.md#t-duality) of the full spectrum, including winding, massive and tachyonic states.**

At the [self-dual circle](../../../string-theory.md#self-dual-circle-compactification) the four single-oscillator charge families give $4\cdot24=96$ new massless states. Each family decomposes into a 25-dimensional gauge vector with 23 polarizations and one [scalar field](../../../quantum-field-theory.md#scalar-field). There are also four massless [ground states](../../../quantum-mechanics.md#ground-state), with charges $(\pm2,0)$ and $(0,\pm2)$. Thus the [massless spectrum at the bosonic self-dual circle](../../../string-theory.md#massless-spectrum-at-the-bosonic-self-dual-circle) has

$$
\boxed{576+96+4=676\ \text{polarizations}:\quad4\ \text{extra vectors and}\ 8\ \text{extra scalars}.}
$$

The gauge interpretation follows directly from the chiral compact-boson operators. With $\langle Y_L(z)Y_L(0)\rangle=-\alpha'\log z/2$, the exponential $e^{ikY_L}$ has [conformal weight](../../../string-theory.md#conformal-weight) $\alpha'k^2/4$. At the self-dual radius,

$$
J_L^3=\frac{i}{\sqrt{\alpha'}}\partial Y_L,\qquad J_L^\pm=:e^{\pm2iY_L/\sqrt{\alpha'}}:
$$

have weight one and satisfy $J^3(z)J^3(0)\sim1/(2z^2)$, $J^3(z)J^\pm(0)\sim\pm J^\pm(0)/z$, and $J^+(z)J^-(0)\sim z^{-2}+2J^3(0)/z$. These are the level-one $SU(2)$ current relations; the right sector supplies another copy. Multiplying these currents by a noncompact oscillator produces six gauge vectors in total. The nine scalar [string vertex operators](../../../string-theory.md#string-vertex-operator) $J_L^aJ_R^b$ form the $(3,3)$ representation, accounting for the radius [scalar field](../../../quantum-field-theory.md#scalar-field) and eight new [scalar fields](../../../quantum-field-theory.md#scalar-field). The remaining neutral fields are the [graviton](../../../quantum-theory.md#graviton), two-form and [dilaton](../../../string-theory.md#dilaton).

A [radius deformation as a Higgs mechanism](../../../string-theory.md#radius-deformation-as-a-higgs-mechanism) is the [expectation value](../../../quantum-mechanics.md#expectation-value) of the Cartan–Cartan scalar [string vertex operator](../../../string-theory.md#string-vertex-operator) $J_L^3J_R^3\propto\partial Y_L\bar\partial Y_R$. Its stabilizer is $U(1)_L\times U(1)_R$, so

$$
\boxed{SU(2)_L\times SU(2)_R\longrightarrow U(1)_L\times U(1)_R,\qquad m_W=\left|\frac R{\alpha'}-\frac1R\right|.}
$$

The four compact single-oscillator [scalar field](../../../quantum-field-theory.md#scalar-field) polarizations become [longitudinal polarizations](../../../wave-equation.md#longitudinal-polarization) of the four [massive vectors](../../../special-relativity.md#massive-vector-particle), exactly as in the [Higgs mechanism](../../../standard-model.md#higgs-mechanism). The other four extra [scalar fields](../../../quantum-field-theory.md#scalar-field) have masses $4/R^2-4/\alpha'$ or $4R^2/\alpha'^2-4/\alpha'$ and need not remain massless; one pair becomes tachyonic on either side of the self-dual point. Together with the original bosonic [tachyon](../../../physics.md#tachyon), this means that the gauge-symmetry interpretation is formal and does not assert a stable bosonic-string vacuum.

## 2

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take $0\le\sigma\le\pi$ and split the coordinates into $a=0,\ldots,p$ along the branes and $I=p+1,\ldots,25$ transverse to them. In [conformal gauge](../../../string-theory.md#conformal-gauge) the [wave equation](../../../wave-equation.md) permits a separated mode $e^{-i\omega\tau}f(\sigma)$ with $f''+\omega^2f=0$. For [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) at both ends, $f'(0)=f'(\pi)=0$ selects $\cos m\sigma$ and [integer](../../../number-theory.md#integer) $m$. The zero-frequency solution is independent of $\sigma$, with a constant position and a term linear in time. Therefore the [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) is

$$
X^a=x^a+2\alpha'k^a\tau+i\sqrt{2\alpha'}\sum_{m\ne0}\frac{\alpha_m^a}{m}e^{-im\tau}\cos m\sigma.
$$

The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) density integrated over this interval is $k^a$.

For [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), subtract the static interpolation between fixed endpoint positions $y_0^I$ and $y_\pi^I$. The remaining field vanishes at both ends, selecting $\sin m\sigma$ with [integer](../../../number-theory.md#integer) $m$ and excluding a [momentum](../../../classical-mechanics.md#momentum) [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode). The expansion is

$$
\boxed{X^I=y_0^I+\frac{y_\pi^I-y_0^I}{\pi}\sigma+\sqrt{2\alpha'}\sum_{m\ne0}\frac{\alpha_m^I}{m}e^{-im\tau}\sin m\sigma.}
$$

Here $\alpha_m^{I\dagger}=\alpha_{-m}^I$. There is no factor $i$ in the [sine series](../../../fourier-series.md#fourier-sine-series) with this reality convention: changing $m$ to $-m$ reverses both the sine and the denominator. These are the [integer-mode expansion with parallel D-brane endpoints](../../../string-theory.md#integer-mode-expansion-with-parallel-d-brane-endpoints); they are not the half-integer modes of a coordinate with a Neumann condition at one endpoint and a Dirichlet condition at the other.

The endpoints can move on $(p+1)$-dimensional [worldvolumes](../../../string-theory.md#worldvolume) but are fixed in the transverse directions. Thus these are [open strings](../../../string-theory.md#open-string) attached to [D-branes](../../../string-theory.md#d-brane), or stretched between parallel [D-branes](../../../string-theory.md#d-brane) at $y_0$ and $y_\pi$. The tangential [momenta](../../../classical-mechanics.md#momentum) describe propagation on the brane; the transverse positions describe its embedding. Let $L=|y_\pi-y_0|$. The linear spatial [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode) contributes $L^2/(4\pi^2\alpha')$ to $L_0$. Quantization with [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) one gives

$$
\boxed{M^2=\frac{L^2}{4\pi^2\alpha'^2}+\frac{N-1}{\alpha'}.}
$$

The first term is also the square of the classical stretched-string energy $TL$, since the [string tension](../../../string-theory.md#string-tension) is $T=1/(2\pi\alpha')$.

For two coincident [D3-branes](../../../string-theory.md#d3-brane), label the ends of an oriented [open string](../../../string-theory.md#open-string) by $i,j\in\{1,2\}$. The four endpoint combinations give [Chan-Paton factors](../../../string-theory.md#chan-paton-factor) $\lambda_{ij}$, which form the full algebra of $2\times2$ [matrices](../../../vector-space.md#matrix). Under a change of brane basis these transform as $\lambda\mapsto U\lambda U^{-1}$, the [adjoint action](../../../lie-theory.md#adjoint-representation-of-a-lie-group) of $U(2)$. At $L=0$, the first oscillator level is massless. Its tangential polarization supplies a four-dimensional vector $A_a$, while the 22 [transverse polarizations](../../../wave-equation.md#transverse-polarization) supply real adjoint [scalar fields](../../../quantum-field-theory.md#scalar-field) $\Phi^I$. This is the [bosonic D3-brane low-energy field content](../../../string-theory.md#bosonic-d3-brane-low-energy-field-content).

The endpoint [matrices](../../../vector-space.md#matrix) multiply in their boundary order in disk amplitudes. The difference between the two orders in the three-vector interaction gives the [matrix commutator](../../../lie-algebra.md#commutator); the kinematic factor is the one-derivative [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) cubic vertex. Factorization and the vector [gauge redundancy](../../../relativistic-quantum-field.md#gauge-redundancy) then supply the quartic interaction with the same [commutator](../../../lie-algebra.md#commutator). Equivalently, the leading low-energy action is the [dimensional reduction](../../../physics.md#dimensional-reduction) of 26-dimensional [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory), with

$$
F_{ab}=\partial_aA_b-\partial_bA_a-i[A_a,A_b],\qquad D_a\Phi^I=\partial_a\Phi^I-i[A_a,\Phi^I],
$$



$$
S_{\mathrm{low}}=\frac1{g_{\mathrm{YM}}^2}\int d^4x\,\operatorname{Tr}\left(-\frac14F_{ab}F^{ab}-\frac12D_a\Phi^I D^a\Phi^I+\frac14[\Phi^I,\Phi^J][\Phi^I,\Phi^J]\right)+\cdots.
$$

For Hermitian [scalar fields](../../../quantum-field-theory.md#scalar-field) the last displayed term corresponds to a nonnegative potential, because their [commutators](../../../lie-algebra.md#commutator) are anti-Hermitian. Higher-derivative terms are suppressed at energies well below $1/\sqrt{\alpha'}$. **Ignoring the [tachyon](../../../physics.md#tachyon), the gauge sector is four-dimensional $U(2)$ [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory), accompanied by 22 adjoint [scalar fields](../../../quantum-field-theory.md#scalar-field).** It is not pure [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory), nor the supersymmetric six-scalar [D3-brane](../../../string-theory.md#d3-brane) theory of a ten-dimensional superstring.

Separate the two branes and use the [D-brane scalar-position normalization](../../../string-theory.md#d-brane-scalar-position-normalization)

$$
\langle\Phi^I\rangle=\frac1{2\pi\alpha'}\begin{pmatrix}y_1^I&0\\0&y_2^I\end{pmatrix}.
$$

A [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) preserves this [expectation value](../../../quantum-mechanics.md#expectation-value) only when it is diagonal if $y_1\ne y_2$. Thus the unbroken [group](../../../group.md) is $U(1)\times U(1)$. The [scalar field](../../../quantum-field-theory.md#scalar-field) [kinetic term](../../../quantum-field-theory.md#kinetic-term) supplies a mass for the off-diagonal vectors, since

$$
[A_a,\langle\Phi^I\rangle]_{12}=\frac{y_2^I-y_1^I}{2\pi\alpha'}(A_a)_{12}.
$$

Summing over $I$ gives $m_{12}^2=L^2/(4\pi^2\alpha'^2)$, exactly the mass of the stretched $N=1$ string. The two diagonal gauge vectors remain massless. This identifies brane separation with an adjoint [Higgs mechanism](../../../standard-model.md#higgs-mechanism), rather than an explicit deletion of the off-diagonal strings.

For the [ground state](../../../quantum-mechanics.md#ground-state) of an [open string](../../../string-theory.md#open-string) joining the two different branes, $N=0$, so the [bosonic stretched-string tachyon threshold](../../../string-theory.md#bosonic-stretched-string-tachyon-threshold) is

$$
\boxed{M_0^2<0\quad\Longleftrightarrow\quad L<2\pi\sqrt{\alpha'}.}
$$

At equality it is massless, and above it the stretched [ground state](../../../quantum-mechanics.md#ground-state) has positive mass squared. The same-brane ground strings still have $M_0^2=-1/\alpha'$; this calculation removes only the stretched-string instability, not the original instability of the bosonic branes.

## 3

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Polyakov action](../../../string-theory.md#polyakov-action) has independent [worldsheet metric](../../../string-theory.md#worldsheet-metric) $\gamma_{ab}$ and embedding fields $X^\mu$. Varying the metric before imposing a gauge gives

$$
T_{ab}=\frac1{\alpha'}\left(\partial_aX\cdot\partial_bX-\frac12\gamma_{ab}\gamma^{cd}\partial_cX\cdot\partial_dX\right)=0.
$$

[Worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformations](../../../string-theory.md#weyl-transformation) allow [conformal gauge](../../../string-theory.md#conformal-gauge) $\gamma_{ab}=e^{2\omega}\eta_{ab}$ locally. The Weyl factor then cancels out of the classical action, leaving

$$
S_X=\frac1{4\pi\alpha'}\int d\tau\,d\sigma\,(\dot X^2-X'^2),\qquad (\partial_\tau^2-\partial_\sigma^2)X^\mu=0.
$$

These are free two-dimensional [scalar fields](../../../quantum-field-theory.md#scalar-field), but the surviving metric equations require

$$
\boxed{(\dot X+X')^2=(\dot X-X')^2=0.}
$$

Equivalently, $\dot X^2+X'^2=0$ and $\dot X\cdot X'=0$. [Gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) does not license dropping these [Virasoro constraints](../../../string-theory.md#virasoro-constraint).

For an ordinary [open string](../../../string-theory.md#open-string), the boundary conditions relate the two chiral sectors. With $\alpha_0^\mu=\sqrt{2\alpha'}k^\mu$, their independent Fourier generators are

$$
L_m=\frac12\sum_{r\in\mathbb Z}\alpha_{m-r}\cdot\alpha_r.
$$

The classical oscillator [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) $\{\alpha_m^\mu,\alpha_n^\nu\}=-im\eta^{\mu\nu}\delta_{m+n,0}$ give the [classical Virasoro constraint algebra](../../../string-theory.md#classical-virasoro-constraint-algebra)

$$
\{L_m,L_n\}=-i(m-n)L_{m+n}.
$$

Thus they are [first-class constraints](../../../classical-mechanics.md#first-class-constraint). In the [quantum theory](../../../quantum-theory.md) one applies [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) to the product and uses $[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0}$. The oscillator [commutator](../../../lie-algebra.md#commutator) gives

$$
[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu,\qquad [L_m,L_n]=(m-n)L_{m+n}+\frac D{12}(m^3-m)\delta_{m+n,0}.
$$

For example, for $m>0$ the extra vacuum term is $(D/2)\sum_{r=1}^{m-1}r(m-r)=D(m^3-m)/12$. This exhibits the [Virasoro central extension](../../../string-theory.md#virasoro-central-extension) rather than concealing it in a classical constraint equation. The matter [central charge](../../../string-theory.md#central-charge) is $D$; the [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field) have charge $-26$. Quantum consistency sets $D=26$ and the [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) to one.

In [old covariant string quantization](../../../string-theory.md#old-covariant-string-quantization) the [physical-state Virasoro conditions for an open string](../../../string-theory.md#physical-state-virasoro-conditions-for-an-open-string) are

$$
L_m|\Psi\rangle=0\quad(m>0),\qquad (L_0-1)|\Psi\rangle=0,\qquad L_0=\alpha'k^2+N.
$$

[Physical string states](../../../string-theory.md#physical-string-state) are then identified modulo physical [null string states](../../../string-theory.md#null-string-state). One does not impose both positive and negative generators as annihilation conditions: their central extension would obstruct that prescription. The resulting [null-state quotient of a string](../../../string-theory.md#null-state-quotient-of-a-string) agrees with the transverse light-cone spectrum at nonzero [momentum](../../../classical-mechanics.md#momentum).

At $N=0$, the [oscillator vacuum](../../../string-theory.md#oscillator-vacuum) $|k\rangle$ is a single [spacetime](../../../special-relativity.md#spacetime) [scalar field](../../../quantum-field-theory.md#scalar-field) with $\alpha'M^2=-1$: the bosonic [tachyon](../../../physics.md#tachyon). At $N=1$, write $|\Psi\rangle=\epsilon_\mu\alpha_{-1}^\mu|k\rangle$. The zero-mode equation gives $k^2=0$, and $L_1$ gives $k\cdot\epsilon=0$. The null descendant $L_{-1}|k\rangle=\sqrt{2\alpha'}k\cdot\alpha_{-1}|k\rangle$ identifies $\epsilon\sim\epsilon+\lambda k$. **This leaves 24 physical polarizations of a massless gauge vector.**

At $N=2$, use the [level-two open-string polarization decomposition](../../../string-theory.md#level-two-open-string-polarization-decomposition)

$$
|\Psi\rangle=\left(\frac12h_{\mu\nu}\alpha_{-1}^\mu\alpha_{-1}^\nu+b_\mu\alpha_{-2}^\mu\right)|k\rangle,\qquad h_{\mu\nu}=h_{\nu\mu}.
$$

The mass is $M^2=1/\alpha'$. The oscillator [commutators](../../../lie-algebra.md#commutator) give all the nontrivial positive-mode conditions:

$$
\sqrt{2\alpha'}\,k^\mu h_{\mu\nu}+2b_\nu=0,\qquad \frac12h^\mu{}_{\mu}+2\sqrt{2\alpha'}\,k\cdot b=0.
$$

Higher positive modes annihilate this level. To see the quotient explicitly, the 25 transverse-parameter null states $L_{-1}(\xi\cdot\alpha_{-1}|k\rangle)$, with $k\cdot\xi=0$, shift

$$
\Delta h_{\mu\nu}=\sqrt{2\alpha'}(k_\mu\xi_\nu+k_\nu\xi_\mu),\qquad \Delta b_\mu=\xi_\mu.
$$

The additional [level-two scalar Virasoro null state](../../../string-theory.md#level-two-scalar-virasoro-null-state) $(L_{-2}+\tfrac32L_{-1}^2)|k\rangle$ shifts

$$
\Delta h_{\mu\nu}=\eta_{\mu\nu}+6\alpha'k_\mu k_\nu,\qquad \Delta b_\mu=\frac52\sqrt{2\alpha'}\,k_\mu.
$$

Substitution into the two physical equations verifies the null-state conditions; the second residual is $(D-26)/2$. Because $k$ is timelike, these null shifts span all components of $b$, so choose a representative with $b=0$. The physical conditions then say $k^\mu h_{\mu\nu}=0$ and $h^\mu{}_{\mu}=0$. In the [rest frame](../../../physics.md#rest-frame) this is a [traceless second-rank tensor](../../../linear-algebra.md#traceless-second-rank-tensor) in 25 spatial dimensions, with $25\cdot26/2-1=324$ polarizations. The light-cone basis independently gives $24$ states $\alpha_{-2}^i|k\rangle$ and $24\cdot25/2=300$ symmetric states $\alpha_{-1}^i\alpha_{-1}^j|k\rangle$. Hence

$$
\boxed{\alpha'M^2=-1,0,1:\qquad1\ \text{scalar},\quad24\ \text{vector polarizations},\quad324\ \text{massive spin-two polarizations}.}
$$

For the fermionic extension, an explicit convention prevents ambiguity in the signs. Keep [worldsheet](../../../string-theory.md#worldsheet) signature $(-,+)$ and use

$$
\rho^0=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\qquad \rho^1=\begin{pmatrix}0&i\\i&0\end{pmatrix},\qquad \{\rho^a,\rho^b\}=-2\eta^{ab}.
$$

Take $\psi=(\psi_1,\psi_2)^T$ and the constant parameter $\epsilon=(\epsilon_1,\epsilon_2)^T$ to be real Grassmann-odd Majorana components, with $\bar\psi=\psi^T\rho^0$. Put $\partial_\pm=\partial_\tau\pm\partial_\sigma$. Apart from the common factor $1/(4\pi\alpha')$, the combined Lagrangian is

$$
\mathcal L=\partial_+X\cdot\partial_-X+i\psi_1\cdot\partial_+\psi_1+i\psi_2\cdot\partial_-\psi_2.
$$

The rigid transformations can be written

$$
\delta X=\bar\epsilon\psi,\qquad \delta\psi=-i\rho^a\partial_aX\,\epsilon,
$$

or, in components,

$$
\delta X=i(\epsilon_2\psi_1-\epsilon_1\psi_2),\qquad \delta\psi_1=-\epsilon_2\partial_-X,\qquad \delta\psi_2=\epsilon_1\partial_+X.
$$

For the $\epsilon_2$ part, the bosonic variation is $i\epsilon_2(\partial_+\psi_1\cdot\partial_-X+\partial_+X\cdot\partial_-\psi_1)$, while the fermionic variation is $-i\epsilon_2\partial_-X\cdot\partial_+\psi_1+i\epsilon_2\psi_1\cdot\partial_+\partial_-X$. Anticommuting the constant parameter past the [fermion](../../../quantum-mechanics.md#fermion) is essential in the second term. The first terms cancel. The other chiral component works in the same way, giving the [chiral proof of rigid worldsheet supersymmetry](../../../string-theory.md#chiral-proof-of-rigid-worldsheet-supersymmetry)

$$
\boxed{\delta\mathcal L=i\epsilon_2\partial_-(\psi_1\cdot\partial_+X)-i\epsilon_1\partial_+(\psi_2\cdot\partial_-X).}
$$

Thus the action is invariant off shell up to a [boundary term](../../../calculus.md#boundary-term). The transformation is a genuine [supersymmetry](../../../supersymmetry.md): on $X$ its [commutator](../../../lie-algebra.md#commutator) for parameters $\epsilon,\zeta$ is the translation

$$
[\delta_\epsilon,\delta_\zeta]X=2i(\epsilon_2\zeta_2\partial_-+\epsilon_1\zeta_1\partial_+)X.
$$

On $\psi$ the same translation follows using $\partial_+\psi_1=0$ and $\partial_-\psi_2=0$; the remaining cross terms are proportional to these [Dirac equations](../../../relativistic-quantum-field.md#dirac-equation). This is [on-shell closure of rigid worldsheet supersymmetry](../../../string-theory.md#on-shell-closure-of-rigid-worldsheet-supersymmetry). On a [surface with boundary](../../../topology.md#surface-with-boundary), compatible endpoint conditions must make the boundary flux vanish. On a compact [worldsheet](../../../string-theory.md#worldsheet), a constant parameter must preserve the [spin structure](../../../riemannian-geometry.md#spin-structure); the local identity alone does not make a constant transformation compatible with every antiperiodic sector.

The [fermions](../../../quantum-mechanics.md#fermion) contribute to the [worldsheet stress-energy tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) and produce a fermionic [superconformal current](../../../string-theory.md#superconformal-current). In holomorphic normalization with $\psi^\mu(z)\psi^\nu(w)\sim\eta^{\mu\nu}/(z-w)$,

$$
T=-\frac1{\alpha'}:\partial X\cdot\partial X:-\frac12:\psi\cdot\partial\psi:,qquad G=i\sqrt{\frac2{\alpha'}}:\psi\cdot\partial X:.
$$

The free-field contractions give $G(z)G(w)\sim(2c/3)/(z-w)^3+2T(w)/(z-w)$ and [conformal weight](../../../string-theory.md#conformal-weight) $3/2$ for $G$, where $c=D+D/2=3D/2$. Consequently the modes obey the [N=1 super-Virasoro algebra](../../../string-theory.md#n-1-super-virasoro-algebra)

$$
\begin{aligned}
[L_m,L_n]&=(m-n)L_{m+n}+\frac c{12}(m^3-m)\delta_{m+n,0},\\
[L_m,G_r]&=\left(\frac m2-r\right)G_{m+r},\\
\{G_r,G_s\}&=2L_{r+s}+\frac c3\left(r^2-\frac14\right)\delta_{r+s,0}.
\end{aligned}
$$

Dropping the central terms gives the classical graded [constraint algebra](../../../classical-mechanics.md#constraint-algebra). [Integer](../../../number-theory.md#integer) $r$ gives the [Ramond sector](../../../string-theory.md#ramond-sector); half-integer $r$ gives the [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector). In the displayed conformal-plane convention $G_0^2=L_0-c/24$ in the [Ramond sector](../../../string-theory.md#ramond-sector). Shifting to the Ramond vacuum-normal-ordered [zero mode](../../../linear-operator-theory.md#zero-mode) gives the usual [Ramond supercurrent zero-mode square](../../../string-theory.md#ramond-supercurrent-zero-mode-square) $G_0^2=L_0^{(R)}$.

Rigid symmetry of matter already supplies these currents, but promoting their vanishing to new gauge constraints requires coupling to [worldsheet](../../../string-theory.md#worldsheet) [supergravity](../../../supersymmetry.md#supergravity) and varying its [worldsheet gravitino](../../../string-theory.md#worldsheet-gravitino). In [superconformal gauge](../../../string-theory.md#superconformal-gauge) one retains $T=G=0$. The fermionic current constraints and their physical-state conditions extend the bosonic Virasoro conditions. The ghost charges are $-26+11=-15$, so cancellation with $3D/2$ gives the [critical dimension of the RNS superstring](../../../string-theory.md#critical-dimension-of-the-rns-superstring) $D=10$; the NS and Ramond intercepts are respectively $1/2$ and zero. This distinguishes the global [supersymmetry](../../../supersymmetry.md) established above from its locally gauged string completion.

## 4

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the critical ten-dimensional [RNS string](../../../string-theory.md#spinning-string) and [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory), leaving eight transverse [bosons](../../../quantum-mechanics.md#boson) and eight transverse [fermions](../../../quantum-mechanics.md#fermion). The bosonic oscillators $\alpha_{-m}^i$ have [integer](../../../number-theory.md#integer) $m>0$. In the [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector) the fermionic oscillators $b_{-r}^i$ have positive half-integer $r$, while in the [Ramond sector](../../../string-theory.md#ramond-sector) the fermionic oscillators $d_{-m}^i$ have [integer](../../../number-theory.md#integer) $m$, including [zero modes](../../../linear-operator-theory.md#zero-mode). Their [anticommutators](../../../vector-space.md#anticommutator) are $\{b_r^i,b_s^j\}=\delta^{ij}\delta_{r+s,0}$ and $\{d_m^i,d_n^j\}=\delta^{ij}\delta_{m+n,0}$. The level and mass formulas are

$$
\begin{aligned}
N_{\mathrm{NS}}&=\sum_{m>0}\alpha_{-m}^i\alpha_m^i+\sum_{r>0}r\,b_{-r}^ib_r^i,&\alpha'M^2&=N_{\mathrm{NS}}-\frac12,\\
N_R&=\sum_{m>0}(\alpha_{-m}^i\alpha_m^i+m\,d_{-m}^id_m^i),&\alpha'M^2&=N_R.
\end{aligned}
$$

Before projection the NS [ground state](../../../quantum-mechanics.md#ground-state) is a [tachyon](../../../physics.md#tachyon) of mass squared $-1/(2\alpha')$. Its oscillator tower describes [spacetime](../../../special-relativity.md#spacetime) [bosons](../../../quantum-mechanics.md#boson). The [Ramond zero-mode Clifford algebra](../../../string-theory.md#ramond-zero-mode-clifford-algebra) $\{\sqrt2d_0^i,\sqrt2d_0^j\}=2\delta^{ij}$ makes the Ramond vacuum a 16-dimensional spinor of $SO(8)$, split into the two chiral eight-dimensional spinors. The Ramond tower describes [spacetime](../../../special-relativity.md#spacetime) [fermions](../../../quantum-mechanics.md#fermion); there is no Ramond [tachyon](../../../physics.md#tachyon).

Choose the supersymmetric [GSO projection](../../../string-theory.md#gso-projection). In the [NS sector](../../../string-theory.md#neveu-schwarz-sector) it keeps states with an [odd number](../../../number-theory.md#odd-number) of [fermionic creation operators](../../../relativistic-quantum-field.md#fermionic-creation-operator), eliminating the zero-oscillator [tachyon](../../../physics.md#tachyon). In the [Ramond sector](../../../string-theory.md#ramond-sector) it fixes the combined parity of the zero-mode [chirality](../../../relativistic-quantum-field.md#chirality-physics) and the nonzero-mode [fermion](../../../quantum-mechanics.md#fermion) number. Thus the Ramond vacuum retains one [chirality](../../../relativistic-quantum-field.md#chirality-physics); adding an [odd number](../../../number-theory.md#odd-number) of nonzero-mode [fermions](../../../quantum-mechanics.md#fermion) requires the opposite zero-mode [chirality](../../../relativistic-quantum-field.md#chirality-physics). The projected towers both have $\alpha'M^2=0,1,2,\ldots$. Here the counts refer to oscillator polarizations for a single endpoint multiplicity; any common Chan-Paton multiplicity multiplies both counts.

At the first retained mass level, $M^2=0$, the NS states are $b_{-1/2}^i|0;k\rangle$ for $i=1,\ldots,8$, furnishing the eight polarizations of the ten-dimensional gauge vector. The Ramond [ground state](../../../quantum-mechanics.md#ground-state) is one chiral spinor with eight physical polarizations. Hence

$$
\boxed{M^2=0:\qquad 8\ \text{bosons}=8\ \text{fermions}.}
$$

These form the massless [supersymmetric vector multiplet](../../../supersymmetry.md#supersymmetric-vector-multiplet).

At the next mass level, $\alpha'M^2=1$, the NS level is $3/2$. The odd-fermion condition leaves exactly

$$
 b_{-3/2}^i|0\rangle,\qquad \alpha_{-1}^ib_{-1/2}^j|0\rangle,\qquad b_{-1/2}^ib_{-1/2}^jb_{-1/2}^k|0\rangle\quad(i<j<k).
$$

Their counts are $8$, $8\cdot8=64$ and $\binom83=56$. Anticommutation requires distinct indices in the third family. There are no other partitions of $3/2$ with odd [fermion](../../../quantum-mechanics.md#fermion) number, so these are all 128 [bosons](../../../quantum-mechanics.md#boson). They assemble into the massive little-group $SO(9)$ representations of dimensions 44 and 84: a traceless symmetric two-tensor and a three-form.

At Ramond level one, the only possibilities are $\alpha_{-1}^i|s\rangle$ and $d_{-1}^i|s'\rangle$. The spinors $|s\rangle$ and $|s'\rangle$ each have eight components and have opposite zero-mode [chirality](../../../relativistic-quantum-field.md#chirality-physics) because the fermionic oscillator reverses the GSO parity. Consequently there are $64+64=128$ [fermions](../../../quantum-mechanics.md#fermion). They form a gamma-traceless vector-spinor of the massive [little group](../../../special-relativity.md#little-group): a vector-spinor has $9\cdot16$ components and its [gamma trace](../../../relativistic-quantum-field.md#gamma-trace-of-a-vector-spinor) removes 16. Therefore the [first massive level of the open RNS string](../../../string-theory.md#first-massive-level-of-the-open-rns-string) has

$$
\boxed{\alpha'M^2=1:\qquad8+64+56=128\ \text{bosons}=64+64=128\ \text{fermions}.}
$$

This is the open-string mass normalization; the same chiral oscillator count used in a [closed string](../../../string-theory.md#closed-string) would correspond to $\alpha'M^2=4$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Count oscillator polarizations at fixed center-of-mass [momentum](../../../classical-mechanics.md#momentum). In a critical [closed bosonic string](../../../string-theory.md#closed-string), each chiral sector has 24 transverse oscillator species. A species at frequency $m$ can be occupied $0,1,2,\ldots$ times, so its contribution is $(1-q^m)^{-1}$. The full chiral [generating function](../../../real-analysis.md#generating-function) is therefore

$$
F(q)=\sum_{N\ge0}d_Nq^N=\prod_{m\ge1}(1-q^m)^{-24}.
$$

The two sectors are independent, while [closed-string level matching](../../../string-theory.md#closed-string-level-matching) restricts their oscillator numbers to the same $N$. Thus the number of states at the closed-string mass level is $g_N=d_N^2$, not $d_{2N}$.

Put $q=e^{-\beta}$, with $\beta>0$. The [Dedekind eta function](../../../string-theory.md#dedekind-eta-function) obeys

$$
\eta\left(\frac{i\beta}{2\pi}\right)=e^{-\beta/24}\prod_{m\ge1}(1-e^{-\beta m}),\qquad \eta(-1/\tau)=\sqrt{-i\tau}\,\eta(\tau).
$$

The transformed argument $2\pi i/\beta$ has large [imaginary part](../../../complex-analysis.md#imaginary-part), so its product approaches one and $\eta(2\pi i/\beta)\sim e^{-\pi^2/(6\beta)}$. Hence

$$
F(e^{-\beta})\sim\left(\frac{\beta}{2\pi}\right)^{12}\exp\left(\frac{4\pi^2}{\beta}-\beta\right).
$$

This establishes the singular exponential as well as its power prefactor. The corrections to the transformed eta product are exponentially small in $1/\beta$.

The [Cauchy coefficient formula](../../../analysis.md#cauchy-coefficient-formula), followed by $q=e^{-\beta}$, gives a steepest-descent integral with leading form

$$
d_N\sim\frac1{2\pi i}\int d\beta\,\left(\frac\beta{2\pi}\right)^{12}\exp\left((N-1)\beta+\frac{4\pi^2}{\beta}\right).
$$

Let $n=N-1$. The saddle of $S(\beta)=n\beta+4\pi^2/\beta$ is

$$
\beta_* =\frac{2\pi}{\sqrt n},\qquad S(\beta_*)=4\pi\sqrt n,\qquad S''(\beta_*)=\frac{n^{3/2}}\pi.
$$

Along the vertical steepest-descent direction $\beta=\beta_*+it$, the quadratic part is $-S''(\beta_*)t^2/2$. Thus the [saddle-point approximation](../../../analysis.md#saddle-point-approximation) gives the Gaussian prefactor

$$
\frac{(\beta_*/2\pi)^{12}}{\sqrt{2\pi S''(\beta_*)}}=\frac1{\sqrt2}n^{-27/4}.
$$

The point $q=1$ supplies the largest exponential contribution. At another fixed [root of unity](../../../algebra.md#root-of-unity) of order $k>1$, the corresponding modular singularity gives a smaller exponential $e^{4\pi\sqrt n/k}$, so it does not change this leading asymptotic. Squaring the chiral result gives the [large-level degeneracy of a closed bosonic string](../../../string-theory.md#large-level-degeneracy-of-a-closed-bosonic-string)

$$
\boxed{d_N\sim\frac1{\sqrt2}(N-1)^{-27/4}e^{4\pi\sqrt{N-1}},\qquad g_N\sim\frac12(N-1)^{-27/2}e^{8\pi\sqrt{N-1}}.}
$$

Replacing $N-1$ by $N$ gives the equivalent usual leading asymptotic. The power $-27/2$ matters: the two-sector degeneracy is not just an unspecified exponential.

Since $M=2\sqrt{(N-1)/\alpha'}$, the exponential is $e^{\beta_H M}$ with

$$
\boxed{\beta_H=4\pi\sqrt{\alpha'},\qquad T_H=\frac1{4\pi\sqrt{\alpha'}}.}
$$

Here Boltzmann's constant is one. Coarse-graining the levels into a density per unit [rest mass](../../../special-relativity.md#invariant-mass) introduces the Jacobian $dN/dM=\alpha'M/2$. Consequently

$$
\rho(M)\sim C M^{-26}e^{\beta_HM},\qquad C=2^{25}\alpha'^{-25/2}.
$$

This is distinct from the degeneracy per level, whose power in $M$ is $-27$. The internal-state contribution to a [canonical partition function](../../../statistical-physics.md#canonical-partition-function) behaves at large mass as

$$
Z_{\mathrm{internal}}(\beta)\sim\int^\infty dM\,C M^{-26}e^{-(\beta-\beta_H)M}.
$$

It converges for $\beta>\beta_H$ and diverges for $\beta<\beta_H$. At $\beta=\beta_H$, this particular internal rest-mass integral converges because of the power $M^{-26}$; one should not discard the prefactor and claim divergence there without specifying the full thermodynamic ensemble. For example, including continuous [momenta](../../../classical-mechanics.md#momentum) in 25 spatial dimensions multiplies the high-mass integrand by a factor proportional to $M^{25/2}$, still leaving convergence of this ideal one-string integral at the endpoint, although sufficiently high [derivatives](../../../calculus.md#derivative) are singular. Multi-string effects, volume and interactions affect the detailed limiting thermodynamics.

The leading microcanonical entropy grows as $S(E)\sim\beta_HE$, with logarithmic corrections, so increasingly large energies are stored in increasingly excited, long strings rather than in an arbitrarily hot ordinary gas. The [Hagedorn temperature](../../../string-theory.md#hagedorn-temperature) is the boundary of canonical convergence from above in [inverse temperature](../../../thermodynamics.md#inverse-temperature); extrapolating the free-string canonical description to $T>T_H$ fails. This counting does not settle the interacting phase above that scale. Also, the bosonic ground-state [tachyon](../../../physics.md#tachyon) is a separate vacuum instability; the high-level asymptotic is meaningful as a formal spectrum calculation without asserting a stable bosonic thermal vacuum.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The starting point is a physical massless closed-string state

$$
\epsilon_{\mu\nu}\alpha_{-1}^\mu\widetilde\alpha_{-1}^\nu|k\rangle,\qquad k^2=0.
$$

Its symmetric traceless part is a [spacetime](../../../special-relativity.md#spacetime) spin-two field, the [graviton](../../../quantum-theory.md#graviton); the antisymmetric part is the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), and the [scalar field](../../../quantum-field-theory.md#scalar-field) part gives the [dilaton](../../../string-theory.md#dilaton). The physical-state conditions impose [transverse polarizations](../../../wave-equation.md#transverse-polarization), and longitudinal null states identify

$$
\epsilon_{\mu\nu}\sim\epsilon_{\mu\nu}+k_\mu\xi_\nu+k_\nu\xi_\mu
$$

for the symmetric component. In position space this is the linearized diffeomorphism $\delta h_{\mu\nu}=\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$. Thus the massless spin-two state has the [gauge redundancy](../../../relativistic-quantum-field.md#gauge-redundancy) required of a gravitational field, rather than an arbitrary massive tensor interaction.

Closed-string amplitudes factorize on this [graviton](../../../quantum-theory.md#graviton) pole. Its leading soft coupling is universal and couples to the [energy-momentum tensor](../../../general-relativity.md#stress-energy-tensor) of the other string states. Decoupling [longitudinal polarizations](../../../wave-equation.md#longitudinal-polarization) enforces the gravitational [Ward identities](../../../perturbative-quantum-field-theory.md#ward-identity). The two-derivative cubic [graviton](../../../quantum-theory.md#graviton) vertex extracted from the low-momentum three-point amplitude is the cubic vertex of the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action); continuing these [Ward identities](../../../perturbative-quantum-field-theory.md#ward-identity) requires the nonlinear diffeomorphism-invariant completion. A complementary way to derive the same dynamics is to demand quantum consistency of propagation in a curved background.

Replace the flat target metric in the [worldsheet](../../../string-theory.md#worldsheet) action by $G_{\mu\nu}(X)$, and allow the two-form and [dilaton](../../../string-theory.md#dilaton) backgrounds. After Euclidean continuation, their couplings have the schematic normalization

$$
S_\sigma=\frac1{4\pi\alpha'}\int d^2\sigma\,\left(\sqrt h\,h^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu+i\varepsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu+\alpha'\sqrt h\,\Phi(X)R^{(2)}\right).
$$

These backgrounds are couplings of a [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model). Quantum [Weyl invariance](../../../string-theory.md#weyl-transformation) requires their Weyl anomaly coefficients to vanish. To first order in $\alpha'$, the metric equation is

$$
0=\beta^G_{\mu\nu}=\alpha'\left(R_{\mu\nu}+2\nabla_\mu\nabla_\nu\Phi-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}\right)+O(\alpha'^2),\qquad H=dB.
$$

The [dilaton](../../../string-theory.md#dilaton) and two-form equations accompany it. In a critical-dimensional background with $H=0$ and constant $\Phi$, the leading metric equation is $R_{\mu\nu}=0$, precisely the vacuum [Einstein field equations](../../../general-relativity.md#einstein-field-equations). Matter and other massless string fields supply the corresponding stress-energy when retained. This argument also explains why arbitrary curved target metrics are not consistent string backgrounds.

The equations arise from the leading [string-frame massless effective action](../../../string-theory.md#string-frame-massless-effective-action)

$$
S_{\mathrm{eff}}=\frac1{2\kappa^2}\int d^Dx\,\sqrt{-G}\,e^{-2\Phi}\left(R[G]+4(\nabla\Phi)^2-\frac1{12}H_{\mu\nu\rho}H^{\mu\nu\rho}+O(\alpha')\right).
$$

A constant-dilaton expansion of its curvature term directly gives the Einstein-Hilbert kinetic and self-interaction terms. For a varying [dilaton](../../../string-theory.md#dilaton), introduce the [Einstein-frame metric](../../../string-theory.md#einstein-frame-metric) $G^E_{\mu\nu}=e^{-4\Phi/(D-2)}G_{\mu\nu}$. The [Weyl rescaling](../../../string-theory.md#weyl-transformation) of the metric and the corresponding transformation of the [Ricci scalar](../../../general-relativity.md#ricci-scalar) and an [integration by parts](../../../calculus.md#integration-by-parts) give

$$
S_{\mathrm{eff}}=\frac1{2\kappa^2}\int d^Dx\,\sqrt{-G_E}\left(R[G_E]-\frac4{D-2}(\nabla_E\Phi)^2-\frac1{12}e^{-8\Phi/(D-2)}H_E^2+O(\alpha')\right).
$$

This displays ordinary Einstein gravity coupled to the [dilaton](../../../string-theory.md#dilaton) and two-form. Gravity need not be the only low-energy field: those fields, compactification moduli and [gauge fields](../../../relativistic-quantum-field.md#gauge-field) have to be retained or stabilized as appropriate. Four-dimensional gravity additionally requires compactification from the critical target dimension, with its Newton constant depending on the compactification volume.

The approximation is controlled when external energies obey $E\sqrt{\alpha'}\ll1$ and curvatures obey $\alpha'|R_{\mu\nu\rho\sigma}|\ll1$. Massive string modes then produce suppressed higher-derivative interactions, such as higher-curvature corrections. Small [string coupling](../../../string-theory.md#string-coupling) $g_s=e^{\Phi_0}$ also suppresses higher-genus quantum corrections; dimensionally $G_D$ scales as $g_s^2\alpha'^{(D-2)/2}$. Thus **Einstein gravity is the universal leading two-derivative dynamics of the massless closed-string spin-two field**, with additional massless matter, string-length corrections and quantum corrections systematically controlled.

For the bosonic theory this is the massless-sector effective description in 26 dimensions; the [tachyon](../../../physics.md#tachyon) means that it is not by itself a proof of a stable vacuum. Tachyon-free supersymmetric [string theories](../../../string-theory.md) have the same massless [graviton](../../../quantum-theory.md#graviton) mechanism in ten dimensions before compactification. Removing the [tachyon](../../../physics.md#tachyon) and obtaining a realistic four-dimensional model require extra physical input beyond the emergence of the Einstein action.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
