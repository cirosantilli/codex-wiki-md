# Paper 46

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_46.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_46.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the mostly-plus [Minkowski metric](../../../special-relativity.md#minkowski-metric), and write $\approx$ for equality on the [constraint surface](../../../classical-mechanics.md#constraint-surface). Assume that the [mechanical constraints](../../../classical-mechanics.md#constraint-mechanics) are locally independent. They are [first-class constraints](../../../classical-mechanics.md#first-class-constraint) when

$$
\{\varphi_i,\varphi_j\}=C_{ij}{}^k(q,p)\varphi_k.
$$

Thus their [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) vanish on the [constraint surface](../../../classical-mechanics.md#constraint-surface), and their [Hamiltonian](../../../classical-mechanics.md#hamiltonian) flows preserve that surface. The [structure functions of a constraint algebra](../../../classical-mechanics.md#structure-functions-of-a-constraint-algebra) $C_{ij}{}^k$ may depend on the [phase space](../../../classical-mechanics.md#phase-space) point. **The finite real span of the constraints is a [Lie algebra](../../../lie-algebra.md) if it closes with constant structure coefficients**, in a suitable choice of generators. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) then gives the usual conditions on the [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra). With general structure functions the finite real span need not close, even though the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) of all smooth functions is itself a [Lie bracket](../../../lie-algebra.md#lie-bracket).

To see the [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) directly, let $G=\epsilon^i(t)\varphi_i$ generate a [canonical gauge transformation](../../../classical-mechanics.md#canonical-gauge-transformation):

$$
\delta q^I=\{q^I,G\},\qquad
\delta p_I=\{p_I,G\},\qquad
\boxed{\delta\lambda^k=\dot\epsilon^k-\lambda^i\epsilon^jC_{ij}{}^k.}
$$

The variation of the [phase-space action](../../../classical-mechanics.md#phase-space-action) integrand is

$$
\delta(p_I\dot q^I-\lambda^i\varphi_i)
=\frac{d}{dt}(p_I\delta q^I-G)
+\left(\dot\epsilon^k-\delta\lambda^k-\lambda^i\epsilon^jC_{ij}{}^k\right)\varphi_k.
$$

The second term cancels without using the [equations of motion](../../../classical-mechanics.md#equation-of-motion). Taking $\epsilon^i$ to vanish at the temporal boundaries leaves the [action](../../../classical-mechanics.md#action) invariant. Arbitrary functions $\epsilon^i(t)$ therefore relate different descriptions of the same physical motion. This reasoning also works with structure functions; constant structure coefficients are only needed for the finite-dimensional [Lie algebra](../../../lie-algebra.md) claim.

For a [closed string](../../../string-theory.md#closed-string), choose $0\leq\sigma<2\pi$ and periodic fields. A convenient [Nambu-Goto phase-space action](../../../string-theory.md#nambu-goto-phase-space-action) is

$$
I=\int dt\,d\sigma\left[P_m\dot X^m-\frac e2(P^2+T^2X'^2)-vP\cdot X'\right].
$$

Here $e$ and $v$ are [Lagrange multipliers](../../../mathematical-optimization.md#lagrange-multiplier). The [Nambu–Goto phase-space constraints](../../../string-theory.md#nambu-goto-phase-space-constraints) are $\mathcal H_0=(P^2+T^2X'^2)/2\approx0$ and $\mathcal H_1=P\cdot X'\approx0$, with canonical [Poisson brackets](../../../classical-mechanics.md#poisson-bracket)

$$
\{X^m(\sigma),P_n(\sigma')\}=\delta^m_n\delta_{2\pi}(\sigma-\sigma').
$$

Let $J_\pm^m=P^m\pm TX'^m$. Differentiating the periodic [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) gives

$$
\{P^m(\sigma),X'^n(\sigma')\}
=\eta^{mn}\partial_\sigma\delta_{2\pi}(\sigma-\sigma'),
\qquad
\{X'^m(\sigma),P^n(\sigma')\}
=\eta^{mn}\partial_\sigma\delta_{2\pi}(\sigma-\sigma').
$$

The opposite signs in $J_+$ and $J_-$ cancel these terms, so **$\{J_+^m(\sigma),J_-^n(\sigma')\}=0$**. Replace the original [constraints](../../../classical-mechanics.md#constraint-mechanics) by the equivalent chiral densities

$$
\mathcal H_\pm=\frac{J_\pm^2}{4T},\qquad
\mathcal H_0=T(\mathcal H_++\mathcal H_-),\qquad
\mathcal H_1=\mathcal H_+-\mathcal H_-.
$$

Their mixed [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) vanish. Choose opposite Fourier orientations for the two sectors:

$$
L_n=\int_0^{2\pi}d\sigma\,e^{in\sigma}\mathcal H_+(\sigma),\qquad
\widetilde L_n=\int_0^{2\pi}d\sigma\,e^{-in\sigma}\mathcal H_-(\sigma).
$$

The [chiral constraint algebra of a closed string](../../../string-theory.md#chiral-constraint-algebra-of-a-closed-string) is

$$
\boxed{\{L_m,L_n\}=-i(m-n)L_{m+n},\quad
\{\widetilde L_m,\widetilde L_n\}=-i(m-n)\widetilde L_{m+n},\quad
\{L_m,\widetilde L_n\}=0.}
$$

Each is the [Witt algebra](../../../lie-algebra.md#witt-algebra): the [vector fields](../../../calculus.md#vector-field) $\ell_n=ie^{in\sigma}\partial_\sigma$ on a circle satisfy $[\ell_m,\ell_n]=(m-n)\ell_{m+n}$. Fourier expansion identifies each real algebra, with $L_n^*=L_{-n}$, with the [Lie algebra](../../../lie-algebra.md) of [vector fields](../../../calculus.md#vector-field) on the circle. The two commuting copies give **$\mathrm{Diff}_1\oplus\mathrm{Diff}_1$**, not a quantum central extension.

For an [open string](../../../string-theory.md#open-string), allowed [boundary conditions](../../../differential-equation.md#boundary-condition) must remove the endpoint term in the variation of the [action](../../../classical-mechanics.md#action), consistently with the allowed endpoint variations. The spatial boundary term is

$$
\delta I\big|_{\partial\sigma}=-\int dt\,
\left[(eT^2X'_m+vP_m)\delta X^m\right]_{\sigma=a}^{\sigma=b}.
$$

It expresses the [open-string endpoint momentum flux](../../../string-theory.md#open-string-endpoint-momentum-flux). In the [temporal gauge for a string](../../../string-theory.md#temporal-gauge-for-a-string) $X^0=t$, take a boundary-adapted parametrization with $v=0$ at the ends. Fixing $X^i(t,a)=0$ gives $\delta X^i(t,a)=0$, a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition). At the other end allow arbitrary spatial variations; for nonzero $e$ these require $X'^i(t,b)=0$, a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition). Also $X'^0=0$ in this [temporal gauge for a string](../../../string-theory.md#temporal-gauge-for-a-string), so $X'^m(t,b)=0$. The [constraint](../../../classical-mechanics.md#constraint-mechanics) at this [free-end string boundary condition](../../../string-theory.md#free-end-string-boundary-condition) reduces to $P^2=0$. Hamilton's equation $\dot X=eP+vX'$ consequently gives $\dot X^2=0$ there. Since $\dot X^0=1$, **the free endpoint has spatial speed one**. This is the [null motion of a free string endpoint](../../../string-theory.md#null-motion-of-a-free-string-endpoint).

A [straight rotating string with one fixed endpoint](../../../string-theory.md#straight-rotating-string-with-one-fixed-endpoint) supplies the required solution in at least two spatial dimensions. Set $e=1/T$, $v=0$, and

$$
\boxed{X^0=t,\qquad
\boldsymbol X(t,\sigma)=L\sin(\sigma/L)
\big(\cos(t/L),\sin(t/L),0,\ldots\big),\quad
0\leq\sigma\leq\frac{\pi L}{2}.}
$$

Take $P_m=T\dot X_m$. The [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) become $\ddot X=X''$, which holds because both second derivatives give $-\boldsymbol X/L^2$. The [Nambu–Goto phase-space constraints](../../../string-theory.md#nambu-goto-phase-space-constraints) are satisfied by

$$
\dot X\cdot X'=0,\qquad
\dot X^2+X'^2=-1+\sin^2(\sigma/L)+\cos^2(\sigma/L)=0.
$$

The endpoint at $\sigma=0$ stays at the origin, while $X'=0$ at $\sigma=\pi L/2$ and the endpoint moves around a circle of radius $L$ with [angular speed](../../../classical-mechanics.md#angular-speed) $1/L$. At each time the whole string lies on a straight radial segment. Its spatial [proper length](../../../special-relativity.md#proper-length) is

$$
\int_0^{\pi L/2}|\boldsymbol X'|\,d\sigma
=\int_0^{\pi L/2}\cos(\sigma/L)\,d\sigma=L.
$$

The [velocity](../../../classical-mechanics.md#velocity) is everywhere perpendicular to the segment, so this also equals the sum of local rest-frame lengths. The induced [worldsheet metric](../../../string-theory.md#worldsheet-metric) becomes degenerate at the null free endpoint, as expected for the limiting free-end solution.

## 2

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use $x^\pm=(x^0\pm x^{D-1})/\sqrt2$, transverse coordinates $x^i$, $i=1,\ldots,d=D-2$, and the [Minkowski metric](../../../special-relativity.md#minkowski-metric)

$$
ds^2=-2dx^+dx^-+dx^i dx^i,\qquad
p^2=-2p_+p_-+p_i p_i.
$$

The [relativistic particle phase-space action](../../../classical-mechanics.md#relativistic-particle-phase-space-action) becomes

$$
I=\int dt\left[\dot x^+p_++\dot x^-p_-+\dot x^i p_i
-\frac e2(-2p_+p_-+p_i^2+\mu^2)\right].
$$

In the [light cone gauge](../../../relativistic-quantum-field.md#light-cone-gauge) $x^+=t$, solve the [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) for $p_+$, assuming $p_-\ne0$. The reduced [phase-space action](../../../classical-mechanics.md#phase-space-action) is $\int dt(\dot x^-p_-+\dot x^ip_i-H)$, with

$$
\boxed{H=-p_+=-\frac{p_i^2+\mu^2}{2p_-}
=\frac{p_i^2+\mu^2}{2p^+},\qquad p^+=-p_->0.}
$$

The last equality selects the future-directed [momentum](../../../classical-mechanics.md#momentum) sector and makes positivity transparent. With $\hbar=1$ and $p_a=-i\partial_a$, the [Schrödinger equation](../../../physics.md#schrodinger-equation) is

$$
i\partial_+\Psi=-\frac{-\Delta_\perp+\mu^2}{2(-i\partial_-)}\Psi.
$$

The inverse acts only on [Fourier modes](../../../fourier-analysis.md#fourier-mode) with nonzero $p_-$. Multiplication by $2p_-$ gives $2\partial_-\partial_+\Psi=(\Delta_\perp-\mu^2)\Psi$. Therefore

$$
\boxed{(\square_D-\mu^2)\Psi=0,\qquad
\square_D=-2\partial_+\partial_-+\Delta_\perp.}
$$

The [light-cone Hamiltonian](../../../classical-mechanics.md#light-cone-hamiltonian) thus gives the same [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) as covariant quantization.

For the [massive two-form field](../../../quantum-field-theory.md#massive-two-form-field), take $\mu\ne0$. Apply $\partial^n$ to its field equation. Antisymmetry of $F_{mnp}$ makes $\partial^n\partial^m F_{mnp}=0$, so

$$
\partial^n A_{np}=0.
$$

Expanding $F=dA$, the other divergence terms vanish by this condition, leaving **$(\square_D-\mu^2)A_{np}=0$**. The [light-cone decomposition of a massive two-form](../../../quantum-field-theory.md#light-cone-decomposition-of-a-massive-two-form) makes its dependent components explicit. The divergence equation is

$$
-\partial_- A_{+n}-\partial_+A_{-n}+\partial_iA_{in}=0.
$$

Taking $n=-$ and $n=i$, respectively, gives

$$
\boxed{A_{+-}=-\partial_-^{-1}\partial_iA_{-i},\qquad
A_{+i}=-\partial_-^{-1}\partial_+A_{-i}
+\partial_-^{-1}\partial_jA_{ji}.}
$$

The $n=+$ equation follows from these expressions: the two terms containing $\partial_+\partial_iA_{-i}$ cancel and $\partial_i\partial_jA_{ji}=0$. Consequently **$A_{-i}$ and $A_{ij}$ are independent**, each satisfying the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) with mass $\mu$. The number of independent [particle polarizations](../../../special-relativity.md#particle-polarization) is

$$
\boxed{d+\binom d2=\binom{D-1}{2}.}
$$

This is the [exterior square](../../../linear-algebra.md#exterior-square) of the [vector representation](../../../representation-theory.md#vector-representation) of the massive [little group](../../../special-relativity.md#little-group) $SO(D-1)$. In the analogous [Proca equation](../../../electromagnetism.md#proca-equation), $\partial^m A_m=0$ determines $A_+$ from $A_-$ and $A_i$, leaving $D-1$ components. A massive field has no gauge freedom that would justify setting these longitudinal components to zero. If $\mu=0$, instead use the [two-form gauge field](../../../relativistic-quantum-field.md#two-form-gauge-field) symmetry $A\mapsto A+d\Lambda$: the [light-cone gauge for a two-form](../../../string-theory.md#light-cone-gauge-for-a-two-form) removes $A_{-m}$, leaving $\binom{D-2}{2}$ transverse [particle polarizations](../../../special-relativity.md#particle-polarization). The massive and massless counts are different.

In the [closed-string mode expansion](../../../string-theory.md#closed-string-mode-expansion), $x^m,p_m$ are center-of-mass [canonical variables](../../../classical-mechanics.md#canonical-variables), while $\alpha_k^i,\widetilde\alpha_k^i$ are independent left- and right-moving transverse [string oscillators](../../../string-theory.md#string-oscillator). Their complex conjugates are $\alpha_{-k}^i,\widetilde\alpha_{-k}^i$. The two zero-mode [Lagrange multipliers](../../../mathematical-optimization.md#lagrange-multiplier) impose the remaining [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) and [closed-string level matching](../../../string-theory.md#closed-string-level-matching). The [string level operators](../../../string-theory.md#string-level-operator) are

$$
N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k,\qquad
\widetilde N=\sum_{k>0}\widetilde\alpha_{-k}\cdot\widetilde\alpha_k.
$$

Their quantum definitions use [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering). The symplectic terms in the [phase-space action](../../../classical-mechanics.md#phase-space-action) give

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_m^i,\alpha_n^j]=m\delta^{ij}\delta_{m+n,0},\qquad
[\widetilde\alpha_m^i,\widetilde\alpha_n^j]=m\delta^{ij}\delta_{m+n,0},
$$

with all brackets between distinct sectors zero. The nonzero-index [string oscillators](../../../string-theory.md#string-oscillator) obey $\alpha_n^{i\dagger}=\alpha_{-n}^i$ and similarly for the right-moving sector. Define the momentum-labelled [oscillator vacuum](../../../string-theory.md#oscillator-vacuum) by

$$
\alpha_k^i|0;p\rangle=\widetilde\alpha_k^i|0;p\rangle=0\quad(k>0),\qquad
p_m|0;p\rangle=p_m^{\mathrm{label}}|0;p\rangle.
$$

For $k>0$, $a_k^i=\alpha_k^i/\sqrt{k}$ has $[a_k^i,a_l^{j\dagger}]=\delta_{kl}\delta^{ij}$. Hence

$$
N=\sum_{k,i}k\,a_k^{i\dagger}a_k^i,\qquad
[N,\alpha_{-k}^i]=k\alpha_{-k}^i.
$$

Starting with $N|0;p\rangle=0$, a finite product with $r_{ki}$ [creation operators](../../../quantum-mechanics.md#creation-operator) of mode $k$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\sum_{k,i}kr_{ki}$. The [Fock space](../../../quantum-field-theory.md#fock-space) is generated by these products; **both level operators have nonnegative integer [eigenvalues](../../../linear-operator-theory.md#eigenvalue)**. This establishes the [integer string oscillator level](../../../string-theory.md#integer-string-oscillator-level) property. Subtracting their physical zero-mode constraints enforces $N=\widetilde N$.

There is a distinction between the displayed classical zero modes and their quantum constraints. With the [normal-ordering constant of a string](../../../string-theory.md#normal-ordering-constant-of-a-string) $a$, these are

$$
\frac{p^2}{8\pi T}+N-a=0,\qquad
\frac{p^2}{8\pi T}+\widetilde N-a=0.
$$

At the [massless first closed-string level](../../../string-theory.md#massless-first-closed-string-level), the states are

$$
\alpha_{-1}^i\widetilde\alpha_{-1}^j|0;p\rangle.
$$

Their transverse [polarization tensor](../../../string-theory.md#polarization-tensor) splits into a symmetric trace-free part, an antisymmetric part, and its trace. These are the [graviton](../../../quantum-theory.md#graviton), [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), and [dilaton](../../../string-theory.md#dilaton), with respective [particle polarization](../../../special-relativity.md#particle-polarization) counts $d(d+1)/2-1$, $d(d-1)/2$, and one. They have the transverse [little group](../../../special-relativity.md#little-group) representations of massless particles. In a Lorentz-consistent [bosonic string theory](../../../string-theory.md#bosonic-string-theory), the first chiral level is a massless vector, not a massive vector with one missing physical polarization; the closed-string products are therefore massless. This fixes $a=1$. Equivalently, regularized transverse zero-point energy gives $a=(D-2)/24$, and Lorentz consistency fixes the [critical dimension of the bosonic string](../../../string-theory.md#critical-dimension-of-string-theory) $D=26$.

It follows that the [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum) is

$$
\boxed{M_N^2=-p^2=8\pi T(N-1)=\frac4{\alpha'}(N-1),\qquad
\alpha'=\frac1{2\pi T},\quad N=\widetilde N.}
$$

The ground state has $M_0^2=-8\pi T$ and is a [tachyon](../../../physics.md#tachyon); level one is massless; for $N\geq2$ the mass is $M_N=\sqrt{8\pi T(N-1)}$. The masslessness claim uses the consistent quantum theory, rather than an unshifted reading of the classical $L_0$.

**A [massive two-form at closed-string level two](../../../string-theory.md#massive-two-form-at-closed-string-level-two) is present.** To see it without confusing it with the level-one massless [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), the level-two states in one chiral sector are

$$
\alpha_{-2}^i|0\rangle,\qquad
\alpha_{-1}^i\alpha_{-1}^j|0\rangle.
$$

They have $d+d(d+1)/2=(D-1)D/2-1$ components and assemble into the [symmetric traceless square](../../../linear-algebra.md#symmetric-trace-free-square-of-the-defining-orthogonal-representation) $S^2_0V$ of the massive [little group](../../../special-relativity.md#little-group) vector space $V=\mathbb R^{D-1}$. The full closed-string level is $S^2_0V\otimes S^2_0V$. For two symmetric trace-free matrices $S,\widetilde S$, the map

$$
(S,\widetilde S)\longmapsto [S,\widetilde S]_{ab}
=S_{ac}\widetilde S_{cb}-\widetilde S_{ac}S_{cb}
$$

is an equivariant map onto antisymmetric matrices. To verify surjectivity, take $S$ diagonal with distinct entries in positions $a,b$ and $\widetilde S$ with only its symmetric $ab$ entry nonzero. Their commutator gives the $ab$ antisymmetric basis element. Finite-dimensional representations of the compact [little group](../../../special-relativity.md#little-group) are completely reducible, so this quotient representation is also a [subrepresentation](../../../representation-theory.md#subrepresentation). It has exactly $\binom{D-1}{2}$ [particle polarizations](../../../special-relativity.md#particle-polarization) and is described by the massive field equation with **$\mu^2=8\pi T$**. At $D=26$ this gives 300 [particle polarizations](../../../special-relativity.md#particle-polarization), consisting in [light-cone coordinates](../../../special-relativity.md#light-cone-coordinates) of 24 components $A_{-i}$ and 276 components $A_{ij}$.

## 3

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For the [relativistic particle phase-space action](../../../classical-mechanics.md#relativistic-particle-phase-space-action), the [first-class constraint](../../../classical-mechanics.md#first-class-constraint) $\varphi=(p^2+m^2)/2$ generates

$$
\boxed{\delta x^m=\epsilon(t)p^m,\qquad
\delta p_m=0,\qquad\delta e=\dot\epsilon(t).}
$$

Indeed the integrand varies by $\tfrac12\,d[\epsilon(p^2-m^2)]/dt$. The [canonical gauge transformation](../../../classical-mechanics.md#canonical-gauge-transformation) is an invariance when the gauge parameter vanishes at fixed temporal endpoints, or when all fields and the parameter are periodic. The boundary restriction matters for the [proper-time modulus](../../../classical-mechanics.md#proper-time-modulus).

Normalize the [worldline](../../../special-relativity.md#world-line) interval to $[0,1]$. Then

$$
s=\int_0^1 e(t)\,dt
$$

is invariant because $\delta s=\epsilon(1)-\epsilon(0)=0$. Every allowed $e$ in its orbit can be written $e(t)=s+\dot\epsilon(t)$: set $\epsilon(t)=\int_0^t[e(u)-s]du$. Thus **$s$ remains a gauge-invariant integration variable**, not another removable nonconstant mode. For a [worldline](../../../special-relativity.md#world-line) circle the constant gauge parameter is a residual zero mode. Without the endpoint restriction, the assertion that $s$ is invariant would not hold.

The [worldline gauge-orbit determinant](../../../classical-mechanics.md#worldline-gauge-orbit-determinant) is the Jacobian from gauge-orbit coordinates $\epsilon$ to the nonconstant part of $e$ is the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) of $\partial_t$. Equivalently, the gauge-fixing identity has the form

$$
1=\Delta_{\mathrm{FP}}[e]\int\mathcal D\epsilon\,
\delta\big(e^\epsilon-s\big),\qquad
\Delta_{\mathrm{FP}}=\det{}'\partial_t.
$$

The determinant is taken between the appropriate boundary-condition spaces, with the modulus removed; on a circle the prime also removes the constant parameter. [Gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) therefore leaves a factor $\det{}'\partial_t$ and a modulus measure, after division by any residual gauge volume. Even though this determinant is field independent in the present Abelian example, it is the required change-of-variables Jacobian. A [Grassmann integral](../../../quantum-mechanics.md#berezin-integral) over the [Faddeev-Popov ghosts](../../../relativistic-quantum-field.md#faddeev-popov-ghost) exponentiates it:

$$
\det{}'\partial_t\ \propto\ \int\mathcal Db\,\mathcal Dc\,e^{iI_{\mathrm{gh}}},\qquad
I_{\mathrm{gh}}=i\int_0^1dt\,b\dot c.
$$

The overall determinant phase depends on the integration convention and can be absorbed into normalization. Zero modes and the same endpoint restrictions must be treated separately rather than included in an invertible determinant.

For the free-ended [open string](../../../string-theory.md#open-string), take $0\leq\sigma\leq\pi$. A canonical cosine expansion at a fixed time is

$$
X^m(\sigma)=x^m+\frac{i}{\sqrt{\pi T}}\sum_{n\ne0}\frac{\alpha_n^m}{n}\cos(n\sigma),\qquad
P_m(\sigma)=\frac{p_m}{\pi}+\sqrt{\frac T\pi}\sum_{n\ne0}\alpha_{nm}\cos(n\sigma).
$$

It implements the [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) and has $\alpha_n^\dagger=\alpha_{-n}$. With $\alpha_0^m=p^m/\sqrt{\pi T}$, its [Nambu-Goto phase-space action](../../../string-theory.md#nambu-goto-phase-space-action), up to a total time derivative, is

$$
I=\int dt\left[p_m\dot x^m+\sum_{n>0}\frac{i}{n}\dot\alpha_n\cdot\alpha_{-n}
-\sum_{n\in\mathbb Z}\lambda_{-n}L_n^{\mathrm{cl}}\right],\qquad
L_n^{\mathrm{cl}}=\frac12\sum_{k\in\mathbb Z}\alpha_{n-k}\cdot\alpha_k.
$$

Reality requires $\lambda_{-n}=\lambda_n^*$. Numerical factors can be absorbed into these [Lagrange multipliers](../../../mathematical-optimization.md#lagrange-multiplier). In this [covariant quantization of the bosonic string](../../../string-theory.md#covariant-quantization-of-the-bosonic-string) the oscillators retain all $D$ spacetime components, in contrast to the transverse oscillators in the preceding solution. The [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) are

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_m^r,\alpha_n^s]=m\eta^{rs}\delta_{m+n,0}.
$$

The [oscillator vacuum](../../../string-theory.md#oscillator-vacuum) $|0;p\rangle$ is annihilated by $\alpha_n^m$ for $n>0$. Its [momentum](../../../classical-mechanics.md#momentum) label will sometimes be suppressed.

Define the matter [Virasoro algebra](../../../string-theory.md#virasoro-algebra) generators using [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering):

$$
L_n=\frac12\sum_k:\!\alpha_{n-k}\cdot\alpha_k\!:,qquad
\boxed{L_0=\alpha'p^2+\sum_{k>0}\alpha_{-k}\cdot\alpha_k,quad
\alpha'=\frac1{2\pi T}.}
$$

No additive intercept is included in this definition of $L_0$. For $n>0$ the indices of the two factors in each term add to $n$; they cannot both be negative. After [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) there is a positive-mode [annihilation operator](../../../quantum-mechanics.md#annihilation-operator) on the right, possibly accompanied by the zero mode. Hence **$L_n|0;p\rangle=0$ for every $n>0$**. In $L_0$, commuting positive modes past negative modes formally adds $\tfrac D2\sum_{k>0}k$. This divergent constant needs a prescription, and a finite shift is an ordering ambiguity. Our convention instead puts the physical [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) into the constraint $L_0-a$.

With this convention the matter [Virasoro algebra](../../../string-theory.md#virasoro-algebra) is

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}
+\frac D{12}(m^3-m)\delta_{m+n,0}.}
$$

A different additive constant in $L_0$ would change the linear-in-$m$ central term, so stating the convention is essential.

For the [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field), use

$$
\{b_m,c_n\}=\delta_{m+n,0},\qquad
\{b_m,b_n\}=\{c_m,c_n\}=0,
$$

and choose a [ghost oscillator vacuum](../../../string-theory.md#ghost-oscillator-vacuum) with

$$
b_n|0\rangle_{\mathrm{gh}}=c_n|0\rangle_{\mathrm{gh}}=0\quad(n>0),\qquad
b_0|0\rangle_{\mathrm{gh}}=0.
$$

Then $c_0|0\rangle_{\mathrm{gh}}\ne0$ since $\{b_0,c_0\}=1$. This choice specifies the ghost zero-mode doublet; it is not a claim that both zero modes annihilate one state. With the printed [ghost Virasoro zero-mode convention](../../../string-theory.md#ghost-virasoro-zero-mode-convention), $L_0^{\mathrm{gh}}|0\rangle_{\mathrm{gh}}=0$ and $L_m^{\mathrm{gh}}|0\rangle_{\mathrm{gh}}=0$ for $m>0$. The latter follows by putting positive ghost modes on the right; a possible contraction requires $m=0$ and is absent here.

Apply the supplied [BRST charge](../../../relativistic-quantum-field.md#brst-charge) to the matter state times this [ghost oscillator vacuum](../../../string-theory.md#ghost-oscillator-vacuum). Terms with a rightmost $c_m$, $m>0$, vanish, as do the positive-mode ghost generators. Thus

$$
Q_{\mathrm{BRST}}(|\Psi\rangle\otimes|0\rangle_{\mathrm{gh}})
=(L_0-1)|\Psi\rangle\otimes c_0|0\rangle_{\mathrm{gh}}
+\sum_{m>0}L_m|\Psi\rangle\otimes c_{-m}|0\rangle_{\mathrm{gh}}.
$$

These one-ghost states are independent, as can also be seen by applying $b_0,b_m$. Therefore the [BRST physical-state constraints of an open string](../../../string-theory.md#brst-physical-state-constraints-of-an-open-string) are

$$
\boxed{(L_0-1)|\Psi\rangle=0,\qquad L_m|\Psi\rangle=0\quad(m>0).}
$$

For the matter [oscillator vacuum](../../../string-theory.md#oscillator-vacuum), $L_0=\alpha'p^2$, so $p^2=1/\alpha'$ and **$M^2=-1/\alpha'=-2\pi T$**: the physical ground state is a [tachyon](../../../physics.md#tachyon). The [momentum](../../../classical-mechanics.md#momentum) must satisfy this equation; the zero-momentum [oscillator vacuum](../../../string-theory.md#oscillator-vacuum) by itself would not be [BRST-closed](../../../relativistic-quantum-field.md#brst-closed-operator).

Matter and ghost generators commute with one another. Add their two algebras and write $\mathcal L_m=L_m+L_m^{\mathrm{gh}}$. The given ghost constant must be retained:

$$
\boxed{[\mathcal L_m,\mathcal L_n]
=(m-n)(\mathcal L_{m+n}-\delta_{m+n,0})
+\frac{D-26}{12}(m^3-m)\delta_{m+n,0}.}
$$

Define the shifted generators $\widehat{\mathcal L}_m=\mathcal L_m-\delta_{m,0}$. Then

$$
[\widehat{\mathcal L}_m,\widehat{\mathcal L}_n]
=(m-n)\widehat{\mathcal L}_{m+n}
+\frac{D-26}{12}(m^3-m)\delta_{m+n,0}.
$$

[BRST nilpotence](../../../relativistic-quantum-field.md#brst-nilpotence) requires cancellation of the anomalous central term in this shifted [constraint algebra](../../../classical-mechanics.md#constraint-algebra), together with the intercept one already present in the charge. At $m=2,n=-2$ the remaining anomalous coefficient is $(D-26)/2$, so **$D=26$**. At this value the shifted total generators obey the [Witt algebra](../../../lie-algebra.md#witt-algebra). The unshifted $\mathcal L_m$ still have the displayed linear zero-mode shift; it must not be silently discarded.

## 4

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Take an oriented [closed string](../../../string-theory.md#closed-string) in flat, critical [bosonic string theory](../../../string-theory.md#bosonic-string-theory), with $\alpha'=1/(2\pi T)$ and a mostly-plus target [Minkowski metric](../../../special-relativity.md#minkowski-metric). After continuation of the [worldsheet](../../../string-theory.md#worldsheet) to Euclidean signature, the [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) sums over embeddings $X$ and [worldsheet metrics](../../../string-theory.md#worldsheet-metric), divided by [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformations](../../../string-theory.md#weyl-transformation). In a flat target its kinetic [action](../../../classical-mechanics.md#action) is

$$
S_E=\frac1{4\pi\alpha'}\int_\Sigma d^2z\,\sqrt g\,g^{ab}
\partial_aX^m\partial_bX_m.
$$

Target-time continuation or analytic continuation of external momenta defines the Lorentzian scattering amplitude; a naive real Euclidean Gaussian for timelike $X^0$ would not be convergent.

An external [tachyon](../../../physics.md#tachyon) is represented by the [tachyon vertex operator](../../../string-theory.md#tachyon-vertex-operator) $V_p(z,\bar z)=:\!e^{ip\cdot X}\!:$, with [conformal weights](../../../string-theory.md#conformal-weight) $h=\bar h=\alpha'p^2/4$. The physical integrated vertex has $(h,\bar h)=(1,1)$, so $p^2=4/\alpha'$. Schematically its tree amplitude is

$$
\mathcal A_N\ \propto\ \int\frac{\mathcal DX\,\mathcal Dg}
{\operatorname{Vol}(\mathrm{Diff}\times\mathrm{Weyl})}
\,e^{-S_E}\prod_{a=1}^N\int_\Sigma d^2z_a\,\sqrt g\,V_{p_a}(z_a,\bar z_a).
$$

The [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) from [conformal gauge](../../../string-theory.md#conformal-gauge) is represented by the [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field). At tree level the [worldsheet](../../../string-theory.md#worldsheet) is a [Riemann sphere](../../../complex-analysis.md#riemann-sphere), whose unpunctured [complex structure](../../../complex-geometry.md#complex-structure) has no moduli. Its residual conformal automorphisms are the [Möbius transformations](../../../group-theory.md#mobius-transformation), $PSL(2,\mathbb C)$. Fix three insertion points, accompanying their unintegrated vertices by the required $c\widetilde c$ ghost factors. The remaining $N-3$ complex insertion positions are integrated over the sphere; equivalently one integrates all positions and divides by the residual conformal group.

The embedding fields are free, with

$$
\langle X^m(z)X^n(w)\rangle
=-\frac{\alpha'}2\eta^{mn}\log|z-w|^2.
$$

Their zero-mode integral gives [momentum conservation](../../../classical-mechanics.md#momentum-conservation), and their nonzero-mode [Gaussian integral](../../../calculus.md#gaussian-integral) gives the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor)

$$
(2\pi)^D\delta^D\!\left(\sum_a p_a\right)
\prod_{a<b}|z_a-z_b|^{\alpha'p_a\cdot p_b}.
$$

This explains the [sphere tachyon position integral](../../../string-theory.md#sphere-tachyon-position-integral) without needing its evaluation. For four [tachyons](../../../physics.md#tachyon) the resulting [Virasoro–Shapiro amplitude](../../../string-theory.md#virasoro-shapiro-amplitude) displays the exchanged string spectrum directly.

Use all-incoming external momenta and introduce $u=-(p_1+p_4)^2/(8\pi T)$ alongside the two printed dimensionless [Mandelstam variables](../../../special-relativity.md#mandelstam-variables). Since $p_a^2=8\pi T$ and $\sum_a p_a=0$, one obtains $s+t+u=-4$. The physical center-of-mass energy squared in the $s$ channel is $s_{\mathrm{phys}}=8\pi T s=4s/\alpha'$. The $t$ channel measures the analogous crossed [momentum](../../../classical-mechanics.md#momentum) transfer, with sign determined by the mostly-plus convention. Rewriting the Gamma factors in a symmetric form gives

$$
A(s,t)=\prod_{x=s,t,u}\frac{\Gamma(-1-x)}{\Gamma(2+x)}.
$$

The [Gamma function](../../../complex-analysis.md#gamma-function) [poles](../../../isolated-singularity.md#pole) imply, at generic fixed values of the other invariant,

$$
\boxed{s=n-1\quad\hbox{or}\quad t=n-1,\qquad n=0,1,2,\ldots.}
$$

The denominator Gamma factors can remove [residues](../../../analysis.md#residue) at special intersecting channel kinematics; the statement concerns a generic single-channel limit. An $s$-channel [pole](../../../isolated-singularity.md#pole) occurs when the intermediate [momentum](../../../classical-mechanics.md#momentum) $p_1+p_2$ satisfies the [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) for a closed-string state:

$$
M_n^2=8\pi T(n-1).
$$

The [pole](../../../isolated-singularity.md#pole) at $s=-1$ exchanges the ground-state [tachyon](../../../physics.md#tachyon), the [pole](../../../isolated-singularity.md#pole) at $s=0$ exchanges massless states, and the positive integer [poles](../../../isolated-singularity.md#pole) exchange the infinite massive tower. The $t$-channel interpretation is the crossed version. Factorization means that each [residue](../../../analysis.md#residue) is a sum of products of couplings to intermediate physical states that couple to the chosen external particles. It need not expose every representation at that mass.

For example, the [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence) and [Gamma function residue at a nonpositive integer](../../../complex-analysis.md#gamma-function-residue-at-a-nonpositive-integer) give the dimensionless [Virasoro–Shapiro amplitude pole residue](../../../string-theory.md#virasoro-shapiro-amplitude-pole-residue)

$$
\operatorname*{Res}_{s=n-1}A(s,t)
=-\frac{[(t+2)_n]^2}{(n!)^2},\qquad
(t+2)_n=\prod_{j=0}^{n-1}(t+2+j).
$$

The [residue](../../../analysis.md#residue) polynomial has degree $2n$, consistent with maximum spin $2n$ in the exchanged level. The amplitude also has the corresponding $u$-channel [poles](../../../isolated-singularity.md#pole) by [crossing symmetry](../../../quantum-mechanics.md#crossing-symmetry).

The massless fields can be treated as target backgrounds rather than separate asymptotic insertions. Write the target metric as $G_{mn}=\eta_{mn}+h_{mn}$, introduce a [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) $B_{mn}$, and a [dilaton](../../../string-theory.md#dilaton) $\Phi$. In conventional Euclidean signs their [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model) [action](../../../classical-mechanics.md#action) is

$$
S_E[X;G,B,\Phi]=\frac1{4\pi\alpha'}\int d^2z\left[
\sqrt g\,g^{ab}G_{mn}(X)\partial_aX^m\partial_bX^n
+i\epsilon^{ab}B_{mn}(X)\partial_aX^m\partial_bX^n\right]
+\frac1{4\pi}\int d^2z\,\sqrt g\,\Phi(X)R^{(2)}.
$$

Here $\epsilon^{ab}$ is the antisymmetric tensor density. The three backgrounds correspond to the [graviton](../../../quantum-theory.md#graviton), antisymmetric tensor and scalar states at closed-string level one. Expanding the vacuum functional in $h,B,\Phi$, then Fourier expanding the backgrounds, produces exactly their integrated [string vertex operators](../../../string-theory.md#string-vertex-operator). Its [functional derivatives](../../../calculus-of-variations.md#functional-derivative) therefore generate the amplitudes with massless external strings. The connected vacuum functional organizes connected amplitudes; the spacetime effective [action](../../../classical-mechanics.md#action) organizes the corresponding vertices after treating massless propagation consistently.

At momenta small compared with $1/\sqrt{\alpha'}$, massive string propagators can be expanded in powers of momenta over their masses. The analytic part of the amplitudes consequently determines local higher-derivative interactions, ordered by powers of $\alpha'$. Massless exchange [poles](../../../isolated-singularity.md#pole) are retained through propagation of the massless fields, rather than expanded into local contact terms. Up to field redefinitions, the leading massless-sector [action](../../../classical-mechanics.md#action) in the [string-frame metric](../../../string-theory.md#string-frame-metric) is

$$
\boxed{S_{\mathrm{eff}}^{\mathrm{tree}}
=\frac1{2\kappa_0^2}\int d^Dx\,\sqrt{-G}\,e^{-2\Phi}
\left[R+4(\nabla\Phi)^2-\frac1{12}H_{mnp}H^{mnp}+O(\alpha')\right],\qquad H=dB.}
$$

The terms denoted $O(\alpha')$ contain additional derivatives, including curvature-squared terms in the bosonic theory. The expansion concerns the massless sector around the perturbative bosonic background; the [tachyon](../../../physics.md#tachyon) instability remains and is not cured by omitting its field from this displayed [action](../../../classical-mechanics.md#action). Thus this is a formal perturbative effective description, not a claim of a stable bosonic vacuum.

Finally split the [dilaton](../../../string-theory.md#dilaton) into a constant and its variation, $\Phi=\Phi_0+\phi$. By the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem), its [dilaton Euler-characteristic weighting](../../../string-theory.md#dilaton-euler-characteristic-weighting) on a connected closed oriented surface follows from

$$
S_{\Phi_0}=\frac{\Phi_0}{4\pi}\int_\Sigma\sqrt g\,R^{(2)}
=\Phi_0\chi(\Sigma)=\Phi_0(2-2g).
$$

Define the [string coupling](../../../string-theory.md#string-coupling) by **$g_s=e^{\Phi_0}$**. A genus-$g$ path integral is weighted by

$$
\boxed{e^{-S_{\Phi_0}}=g_s^{2g-2}.}
$$

The sphere carries $g_s^{-2}$, the torus carries $g_s^0$, and each extra handle adds $g_s^2$. At higher genus one integrates over complex-structure moduli as well as insertion points, with the associated antighost insertions supplying the correct moduli measure. With canonically normalized external vertices an $N$-point genus-$g$ amplitude scales as $g_s^{2g-2+N}$.

Summing connected [worldsheets](../../../string-theory.md#worldsheet) of every [genus of a surface](../../../topology.md#genus-of-a-surface) yields the [string-loop effective action expansion](../../../string-theory.md#string-loop-effective-action-expansion)

$$
\boxed{S_{\mathrm{eff}}=
\sum_{g=0}^{\infty}g_s^{2g-2}\,S_g[G,B,\phi;\alpha'].}
$$

Each coefficient has its own low-energy $\alpha'$ expansion. The two parameters have different roles: $\alpha'$ resolves finite string size through higher derivatives, while $g_s^2$ counts additional string loops.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
