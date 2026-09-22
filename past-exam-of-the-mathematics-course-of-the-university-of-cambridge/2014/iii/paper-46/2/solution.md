<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $x^\pm=(x^0\pm x^{D-1})/\sqrt2$, transverse coordinates $x^i$, $i=1,\ldots,d=D-2$, and the [Minkowski metric](../../../../../minkowski-metric.md)

$$
ds^2=-2dx^+dx^-+dx^i dx^i,\qquad
p^2=-2p_+p_-+p_i p_i.
$$

The [relativistic particle phase-space action](../../../../../relativistic-particle-phase-space-action.md) becomes

$$
I=\int dt\left[\dot x^+p_++\dot x^-p_-+\dot x^i p_i
-\frac e2(-2p_+p_-+p_i^2+\mu^2)\right].
$$

In the [light cone gauge](../../../../../light-cone-gauge.md) $x^+=t$, solve the [mass-shell condition](../../../../../string-mass-shell-condition.md) for $p_+$, assuming $p_-\ne0$. The reduced [phase-space action](../../../../../phase-space-action.md) is $\int dt(\dot x^-p_-+\dot x^ip_i-H)$, with

$$
\boxed{H=-p_+=-\frac{p_i^2+\mu^2}{2p_-}
=\frac{p_i^2+\mu^2}{2p^+},\qquad p^+=-p_->0.}
$$

The last equality selects the future-directed [momentum](../../../../../momentum.md) sector and makes positivity transparent. With $\hbar=1$ and $p_a=-i\partial_a$, the [Schrödinger equation](../../../../../schrodinger-equation.md) is

$$
i\partial_+\Psi=-\frac{-\Delta_\perp+\mu^2}{2(-i\partial_-)}\Psi.
$$

The inverse acts only on [Fourier modes](../../../../../fourier-mode.md) with nonzero $p_-$. Multiplication by $2p_-$ gives $2\partial_-\partial_+\Psi=(\Delta_\perp-\mu^2)\Psi$. Therefore

$$
\boxed{(\square_D-\mu^2)\Psi=0,\qquad
\square_D=-2\partial_+\partial_-+\Delta_\perp.}
$$

The [light-cone Hamiltonian](../../../../../light-cone-hamiltonian.md) thus gives the same [Klein-Gordon equation](../../../../../klein-gordon-equation.md) as covariant quantization.

For the [massive two-form field](../../../../../massive-two-form-field.md), take $\mu\ne0$. Apply $\partial^n$ to its field equation. Antisymmetry of $F_{mnp}$ makes $\partial^n\partial^m F_{mnp}=0$, so

$$
\partial^n A_{np}=0.
$$

Expanding $F=dA$, the other divergence terms vanish by this condition, leaving **$(\square_D-\mu^2)A_{np}=0$**. The [light-cone decomposition of a massive two-form](../../../../../light-cone-decomposition-of-a-massive-two-form.md) makes its dependent components explicit. The divergence equation is

$$
-\partial_- A_{+n}-\partial_+A_{-n}+\partial_iA_{in}=0.
$$

Taking $n=-$ and $n=i$, respectively, gives

$$
\boxed{A_{+-}=-\partial_-^{-1}\partial_iA_{-i},\qquad
A_{+i}=-\partial_-^{-1}\partial_+A_{-i}
+\partial_-^{-1}\partial_jA_{ji}.}
$$

The $n=+$ equation follows from these expressions: the two terms containing $\partial_+\partial_iA_{-i}$ cancel and $\partial_i\partial_jA_{ji}=0$. Consequently **$A_{-i}$ and $A_{ij}$ are independent**, each satisfying the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) with mass $\mu$. The number of independent [particle polarizations](../../../../../particle-polarization.md) is

$$
\boxed{d+\binom d2=\binom{D-1}{2}.}
$$

This is the [exterior square](../../../../../exterior-square.md) of the [vector representation](../../../../../vector-representation.md) of the massive [little group](../../../../../little-group.md) $SO(D-1)$. In the analogous [Proca equation](../../../../../proca-equation.md), $\partial^m A_m=0$ determines $A_+$ from $A_-$ and $A_i$, leaving $D-1$ components. A massive field has no gauge freedom that would justify setting these longitudinal components to zero. If $\mu=0$, instead use the [two-form gauge field](../../../../../two-form-gauge-field.md) symmetry $A\mapsto A+d\Lambda$: the [light-cone gauge for a two-form](../../../../../light-cone-gauge-for-a-two-form.md) removes $A_{-m}$, leaving $\binom{D-2}{2}$ transverse [particle polarizations](../../../../../particle-polarization.md). The massive and massless counts are different.

In the [closed-string mode expansion](../../../../../closed-string-mode-expansion.md), $x^m,p_m$ are center-of-mass [canonical variables](../../../../../canonical-variables.md), while $\alpha_k^i,\widetilde\alpha_k^i$ are independent left- and right-moving transverse [string oscillators](../../../../../string-oscillator.md). Their complex conjugates are $\alpha_{-k}^i,\widetilde\alpha_{-k}^i$. The two zero-mode [Lagrange multipliers](../../../../../lagrange-multiplier.md) impose the remaining [mass-shell condition](../../../../../string-mass-shell-condition.md) and [closed-string level matching](../../../../../closed-string-level-matching.md). The [string level operators](../../../../../string-level-operator.md) are

$$
N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k,\qquad
\widetilde N=\sum_{k>0}\widetilde\alpha_{-k}\cdot\widetilde\alpha_k.
$$

Their quantum definitions use [normal ordering](../../../../../normal-ordering.md). The symplectic terms in the [phase-space action](../../../../../phase-space-action.md) give

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_m^i,\alpha_n^j]=m\delta^{ij}\delta_{m+n,0},\qquad
[\widetilde\alpha_m^i,\widetilde\alpha_n^j]=m\delta^{ij}\delta_{m+n,0},
$$

with all brackets between distinct sectors zero. The nonzero-index [string oscillators](../../../../../string-oscillator.md) obey $\alpha_n^{i\dagger}=\alpha_{-n}^i$ and similarly for the right-moving sector. Define the momentum-labelled [oscillator vacuum](../../../../../oscillator-vacuum.md) by

$$
\alpha_k^i|0;p\rangle=\widetilde\alpha_k^i|0;p\rangle=0\quad(k>0),\qquad
p_m|0;p\rangle=p_m^{\mathrm{label}}|0;p\rangle.
$$

For $k>0$, $a_k^i=\alpha_k^i/\sqrt{k}$ has $[a_k^i,a_l^{j\dagger}]=\delta_{kl}\delta^{ij}$. Hence

$$
N=\sum_{k,i}k\,a_k^{i\dagger}a_k^i,\qquad
[N,\alpha_{-k}^i]=k\alpha_{-k}^i.
$$

Starting with $N|0;p\rangle=0$, a finite product with $r_{ki}$ [creation operators](../../../../../creation-operator.md) of mode $k$ has [eigenvalue](../../../../../eigenvalue.md) $\sum_{k,i}kr_{ki}$. The [Fock space](../../../../../fock-space.md) is generated by these products; **both level operators have nonnegative integer [eigenvalues](../../../../../eigenvalue.md)**. This establishes the [integer string oscillator level](../../../../../integer-string-oscillator-level.md) property. Subtracting their physical zero-mode constraints enforces $N=\widetilde N$.

There is a distinction between the displayed classical zero modes and their quantum constraints. With the [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md) $a$, these are

$$
\frac{p^2}{8\pi T}+N-a=0,\qquad
\frac{p^2}{8\pi T}+\widetilde N-a=0.
$$

At the [massless first closed-string level](../../../../../massless-first-closed-string-level.md), the states are

$$
\alpha_{-1}^i\widetilde\alpha_{-1}^j|0;p\rangle.
$$

Their transverse [polarization tensor](../../../../../polarization-tensor.md) splits into a symmetric trace-free part, an antisymmetric part, and its trace. These are the [graviton](../../../../../graviton.md), [Kalb–Ramond field](../../../../../kalb-ramond-field.md), and [dilaton](../../../../../dilaton.md), with respective [particle polarization](../../../../../particle-polarization.md) counts $d(d+1)/2-1$, $d(d-1)/2$, and one. They have the transverse [little group](../../../../../little-group.md) representations of massless particles. In a Lorentz-consistent [bosonic string theory](../../../../../bosonic-string-theory.md), the first chiral level is a massless vector, not a massive vector with one missing physical polarization; the closed-string products are therefore massless. This fixes $a=1$. Equivalently, regularized transverse zero-point energy gives $a=(D-2)/24$, and Lorentz consistency fixes the [critical dimension of the bosonic string](../../../../../critical-dimension-of-string-theory.md) $D=26$.

It follows that the [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md) is

$$
\boxed{M_N^2=-p^2=8\pi T(N-1)=\frac4{\alpha'}(N-1),\qquad
\alpha'=\frac1{2\pi T},\quad N=\widetilde N.}
$$

The ground state has $M_0^2=-8\pi T$ and is a [tachyon](../../../../../tachyon.md); level one is massless; for $N\geq2$ the mass is $M_N=\sqrt{8\pi T(N-1)}$. The masslessness claim uses the consistent quantum theory, rather than an unshifted reading of the classical $L_0$.

**A [massive two-form at closed-string level two](../../../../../massive-two-form-at-closed-string-level-two.md) is present.** To see it without confusing it with the level-one massless [Kalb–Ramond field](../../../../../kalb-ramond-field.md), the level-two states in one chiral sector are

$$
\alpha_{-2}^i|0\rangle,\qquad
\alpha_{-1}^i\alpha_{-1}^j|0\rangle.
$$

They have $d+d(d+1)/2=(D-1)D/2-1$ components and assemble into the [symmetric traceless square](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md) $S^2_0V$ of the massive [little group](../../../../../little-group.md) vector space $V=\mathbb R^{D-1}$. The full closed-string level is $S^2_0V\otimes S^2_0V$. For two symmetric trace-free matrices $S,\widetilde S$, the map

$$
(S,\widetilde S)\longmapsto [S,\widetilde S]_{ab}
=S_{ac}\widetilde S_{cb}-\widetilde S_{ac}S_{cb}
$$

is an equivariant map onto antisymmetric matrices. To verify surjectivity, take $S$ diagonal with distinct entries in positions $a,b$ and $\widetilde S$ with only its symmetric $ab$ entry nonzero. Their commutator gives the $ab$ antisymmetric basis element. Finite-dimensional representations of the compact [little group](../../../../../little-group.md) are completely reducible, so this quotient representation is also a [subrepresentation](../../../../../subrepresentation.md). It has exactly $\binom{D-1}{2}$ [particle polarizations](../../../../../particle-polarization.md) and is described by the massive field equation with **$\mu^2=8\pi T$**. At $D=26$ this gives 300 [particle polarizations](../../../../../particle-polarization.md), consisting in [light-cone coordinates](../../../../../light-cone-coordinates.md) of 24 components $A_{-i}$ and 276 components $A_{ij}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
