# Paper 67

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper67.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper67.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with signature $(-,+,\ldots,+)$, and write the [string tension](../../../string-theory.md#string-tension) as $T=1/(2\pi\alpha')$. If $X^\mu(\tau,\sigma)$ is the [string embedding map](../../../string-theory.md#string-embedding-map), its [induced worldsheet metric](../../../string-theory.md#induced-worldsheet-metric) is $\gamma_{ab}=\partial_aX\cdot\partial_bX$. The [Nambu–Goto action](../../../string-theory.md#nambu-goto-action) is

$$
S=-T\int d\tau\,d\sigma\,\sqrt{-\det\gamma}.
$$

The [first variation](../../../calculus-of-variations.md#first-variation) uses $\delta\gamma_{ab}=2\partial_{(a}X_\mu\partial_{b)}\delta X^\mu$ and therefore gives

$$
\delta S=-T\int\sqrt{-\gamma}\,\gamma^{ab}\partial_aX_\mu\partial_b\delta X^\mu\,d\tau\,d\sigma.
$$

An [integration by parts](../../../calculus.md#integration-by-parts) yields the bulk [Nambu–Goto equations of motion](../../../string-theory.md#nambu-goto-equations-of-motion) and the endpoint term:

$$
\boxed{\partial_a\!\left(\sqrt{-\gamma}\,\gamma^{ab}\partial_bX^\mu\right)=0},
\qquad
\Pi^a_\mu=-T\sqrt{-\gamma}\,\gamma^{ab}\partial_bX_\mu,
\qquad
\left.\Pi^\sigma_\mu\delta X^\mu\right|_{\partial\Sigma}=0.
$$

For a [closed string](../../../string-theory.md#closed-string), periodicity cancels the endpoint term. For a freely moving [open string](../../../string-theory.md#open-string), arbitrary endpoint variations require zero momentum flux, which is the [free-end string boundary condition](../../../string-theory.md#free-end-string-boundary-condition).

Choose orthogonal conformal coordinates on the nondegenerate part of the [worldsheet](../../../string-theory.md#worldsheet), so that $\gamma_{\tau\sigma}=0$ and $\gamma_{\tau\tau}+\gamma_{\sigma\sigma}=0$. The [Nambu–Goto equations of motion](../../../string-theory.md#nambu-goto-equations-of-motion) then become a [wave equation](../../../wave-equation.md), with the accompanying [Virasoro constraints](../../../string-theory.md#virasoro-constraint):

$$
\ddot X-X''=0,\qquad \dot X\cdot X'=0,\qquad \dot X^2+X'^2=0.
$$

Here a dot and a prime mean $\partial_\tau$ and $\partial_\sigma$. The last two equations are essential: a solution of the [wave equation](../../../wave-equation.md) alone need not be a relativistic [fundamental string](../../../string-theory.md#fundamental-string) motion.

For a free-ended [open string](../../../string-theory.md#open-string), take $0\leq\sigma\leq\pi$ and $a>0$, and set

$$
X^0=a\tau,\qquad X^1=a\cos\sigma\cos\tau,\qquad X^2=a\cos\sigma\sin\tau,
$$

with the other coordinates constant. Every component satisfies the [wave equation](../../../wave-equation.md), and

$$
\dot X^2=-a^2\sin^2\sigma,\qquad X'^2=a^2\sin^2\sigma,\qquad \dot X\cdot X'=0.
$$

Moreover $X'=0$ at both endpoints, giving the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition). At fixed target time $t=a\tau$, the spatial image is the straight segment

$$
\boldsymbol X=r\bigl(\cos(t/a),\sin(t/a)\bigr),\qquad -a\leq r\leq a.
$$

Thus its [angular velocity](../../../classical-mechanics.md#angular-velocity) is $1/a$. The speed at coordinate $r$ is $|r|/a$, so the endpoints have the [null motion of a free string endpoint](../../../string-theory.md#null-motion-of-a-free-string-endpoint). The [induced worldsheet metric](../../../string-theory.md#induced-worldsheet-metric) degenerates there; the conserved densities below have finite limits, so the endpoint degeneracy causes no divergent charge.

In these coordinates $\Pi^{\tau\mu}=T\dot X^\mu$. The [target-space Noether charges of a string](../../../string-theory.md#target-space-noether-charges-of-a-string) give the [energy](../../../classical-mechanics.md#energy), [momentum](../../../classical-mechanics.md#momentum) and [angular momentum](../../../classical-mechanics.md#angular-momentum):

$$
E=\int_0^\pi T\dot X^0\,d\sigma=\pi Ta,\qquad
\boldsymbol P=T\int_0^\pi\dot{\boldsymbol X}\,d\sigma=0,
$$



$$
J_{12}=T\int_0^\pi\left(X^1\dot X^2-X^2\dot X^1\right)d\sigma
=Ta^2\int_0^\pi\cos^2\sigma\,d\sigma=\frac{\pi Ta^2}{2}.
$$

Since this is the [centre-of-momentum frame](../../../special-relativity.md#center-of-momentum-frame), the rest [mass](../../../classical-mechanics.md#mass) is $M=E$. Eliminating $a$ proves the [free-ended straight-string Regge relation](../../../string-theory.md#free-ended-straight-string-regge-relation):

$$
\boxed{J=\frac{M^2}{2\pi T}=\alpha'M^2\quad\text{(free-ended open string)}}.
$$

A spacetime [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) of the solution changes its frame, not this rest-frame relation.

There is also a folded [closed string](../../../string-theory.md#closed-string) version: use the same formula over $0\leq\sigma\leq2\pi$. The spatial segment is then covered twice, with folds at $\sigma=0,\pi$, and the [closed-string mode expansion](../../../string-theory.md#closed-string-mode-expansion) is periodic. Each charge is twice its [open string](../../../string-theory.md#open-string) value, so

$$
M=2\pi Ta,\qquad J=\pi Ta^2,\qquad
\boxed{J=\frac{M^2}{4\pi T}=\frac{\alpha'M^2}{2}\quad\text{(folded closed string)}}.
$$

The folds also have degenerate induced metric and are understood through the finite canonical densities or a limiting smooth motion. The two classical [Regge trajectories](../../../string-theory.md#regge-trajectory) have different slopes because the [closed string](../../../string-theory.md#closed-string) has two coincident branches. No quantum [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) enters this classical calculation.

## 2

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Nambu–Goto action](../../../string-theory.md#nambu-goto-action) is invariant under [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism). Its canonical [Nambu–Goto phase-space constraints](../../../string-theory.md#nambu-goto-phase-space-constraints) are

$$
\Pi\cdot X'=0,\qquad \Pi^2+T^2X'^2=0.
$$

In [conformal gauge](../../../string-theory.md#conformal-gauge), $\Pi=T\dot X$, so these become $(\dot X\pm X')^2=0$. Their smeared generators implement the residual [conformal transformations](../../../geometry-and-topology.md#conformal-map) rather than independent propagating degrees of freedom. Classically their Fourier modes form the [classical Virasoro constraint algebra](../../../string-theory.md#classical-virasoro-constraint-algebra). Quantization promotes them to the [Virasoro algebra](../../../string-theory.md#virasoro-algebra), and its constraints select the [physical string states](../../../string-theory.md#physical-string-state) from the indefinite covariant [Fock space](../../../quantum-field-theory.md#fock-space).

For clarity, start with a [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) at both ends of an [open string](../../../string-theory.md#open-string), $0\leq\sigma\leq\pi$. Its [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) is

$$
X^\mu=x^\mu+2\alpha'p^\mu\tau+i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^\mu}{n}e^{-in\tau}\cos n\sigma,
\qquad \alpha_0^\mu=\sqrt{2\alpha'}\,p^\mu.
$$

Canonical quantization gives the [string oscillator](../../../string-theory.md#string-oscillator) relations

$$
[\alpha_m^\mu,\alpha_n^\nu]=m\delta_{m+n,0}\eta^{\mu\nu},\qquad
(\alpha_n^\mu)^\dagger=\alpha_{-n}^\mu.
$$

With $\partial_\pm=(\partial_\tau\pm\partial_\sigma)/2$, the [worldsheet stress-energy tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) obeys

$$
\frac1{\alpha'}\partial_\pm X\cdot\partial_\pm X
=\sum_{m\in\mathbb Z}L_m e^{-im(\tau\pm\sigma)}.
$$

Substituting the [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) into this quadratic expression derives the [Virasoro generators](../../../string-theory.md#virasoro-generator):

$$
\boxed{L_m=\frac12\sum_{r\in\mathbb Z}:\alpha_{m-r}\cdot\alpha_r:},
\qquad
L_0=\alpha'p^2+N,\qquad N=\sum_{r>0}\alpha_{-r}\cdot\alpha_r.
$$

The colons mean [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering), placing the negative-mode creation operators to the left. The [string level operator](../../../string-theory.md#string-level-operator) $N$ increases by $r$ when an oscillator $\alpha_{-r}$ is added.

Using the [commutator](../../../lie-algebra.md#commutator) once gives

$$
[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu.
$$

Applying this to the quadratic expression for $L_n$ produces $(m-n)L_{m+n}$, together with the double-contraction [Virasoro central extension](../../../string-theory.md#virasoro-central-extension). To determine its coefficient, take $m>0$ and evaluate $[L_m,L_{-m}]$ on a zero-momentum [oscillator vacuum](../../../string-theory.md#oscillator-vacuum). Only the creation pairs with $1\leq r\leq m-1$ contribute, giving

$$
\frac D2\sum_{r=1}^{m-1}r(m-r)=\frac D{12}(m^3-m).
$$

Here $D$ is the target [spacetime dimension](../../../general-relativity.md#spacetime-dimension); the timelike free boson also contributes one to the [central charge](../../../string-theory.md#central-charge), since a double contraction contains two metric factors. Thus

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}+\frac D{12}(m^3-m)\delta_{m+n,0}},
\qquad L_m^\dagger=L_{-m}.
$$

This derives both the [Virasoro generators](../../../string-theory.md#virasoro-generator) and their quantum anomaly.

In [old covariant string quantization](../../../string-theory.md#old-covariant-string-quantization), the [physical-state Virasoro conditions for an open string](../../../string-theory.md#physical-state-virasoro-conditions-for-an-open-string) are

$$
L_{n>0}|\psi\rangle=0,\qquad (L_0-a)|\psi\rangle=0,
$$

where $a$ is the [normal-ordering constant of a string](../../../string-theory.md#normal-ordering-constant-of-a-string). Requiring all positive and negative modes to annihilate a state would contradict the nonzero [Virasoro central extension](../../../string-theory.md#virasoro-central-extension); the positive-mode prescription is the appropriate covariant subsidiary condition. The zero-mode equation gives the [open bosonic string mass spectrum](../../../string-theory.md#open-bosonic-string-mass-spectrum),

$$
\alpha'M^2=N-a.
$$

For a [closed string](../../../string-theory.md#closed-string), there are two commuting [Virasoro algebras](../../../string-theory.md#virasoro-algebra). With uncompactified zero modes, $L_0=\alpha'p^2/4+N_R$ and $\widetilde L_0=\alpha'p^2/4+N_L$. Imposing both positive-mode conditions and both zero-mode conditions gives the [closed-string level matching](../../../string-theory.md#closed-string-level-matching) $N_L=N_R$ and $M^2=4(N_L-a)/\alpha'$.

Covariance initially retains the timelike [string oscillators](../../../string-theory.md#string-oscillator). For example, $\alpha_{-1}^0|0;p\rangle$ has negative norm because $\eta^{00}=-1$. Its existence in the unconstrained space is not an inconsistency if it is absent from the physical quotient. The [no-ghost theorem for the critical bosonic string](../../../string-theory.md#no-ghost-theorem-for-the-critical-bosonic-string) states that, at $D=26$ and $a=1$, the [inner product](../../../linear-algebra.md#inner-product) on [physical string states](../../../string-theory.md#physical-string-state) at ordinary nonzero momentum is positive semidefinite. After quotienting physical [null string states](../../../string-theory.md#null-string-state), this physical space is represented by the 24 positive-norm transverse [string oscillators](../../../string-theory.md#string-oscillator).

A [spurious string state](../../../string-theory.md#spurious-string-state) has the form $\sum_{n>0}L_{-n}|\chi_n\rangle$. Its [inner product](../../../linear-algebra.md#inner-product) with every [physical string state](../../../string-theory.md#physical-string-state) vanishes, by $L_n|\psi\rangle=0$ and $L_n^\dagger=L_{-n}$. Whenever such a state is itself physical, it is a [null string state](../../../string-theory.md#null-string-state) and represents a gauge redundancy, not an extra polarization. Consequently **the physical quotient has no negative-norm propagating states**, and agrees with [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory). This is the significance of the theorem; a proof is not needed here. It does not eliminate the bosonic [tachyon](../../../physics.md#tachyon), whose negative mass squared is distinct from negative norm, nor does it remove the auxiliary [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field) used in [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing).

## 3

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Polyakov action](../../../string-theory.md#polyakov-action) introduces an independent [worldsheet metric](../../../string-theory.md#worldsheet-metric) $h_{ab}$:

$$
S_P=-\frac1{4\pi\alpha'}\int d^2\sigma\,\sqrt{-h}\,h^{ab}\partial_aX\cdot\partial_bX.
$$

Its redundancies are [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformations](../../../string-theory.md#weyl-transformation). A [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) over all metrics without dividing by this gauge volume would count physically equivalent configurations repeatedly. Fixing [conformal gauge](../../../string-theory.md#conformal-gauge) therefore needs the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant), not merely the substitution of a flat metric into the action.

After using the [Weyl transformation](../../../string-theory.md#weyl-transformation) to remove the trace of a metric variation, the infinitesimal [worldsheet diffeomorphism ghost operator](../../../string-theory.md#worldsheet-diffeomorphism-ghost-operator) is

$$
(P_1c)_{ab}=\nabla_ac_b+\nabla_bc_a-h_{ab}\nabla_dc^d.
$$

The [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) of this operator is represented by anticommuting fields: a vector [Faddeev-Popov ghost](../../../relativistic-quantum-field.md#faddeev-popov-ghost) $c^a$ and a symmetric traceless [Faddeev-Popov antighost field](../../../relativistic-quantum-field.md#faddeev-popov-antighost-field) $b^{ab}$. In Euclidean coordinates their [worldsheet ghost action](../../../string-theory.md#worldsheet-ghost-action) is, up to a consistent overall normalization,

$$
S_{\mathrm{gh}}=\frac1{2\pi}\int\sqrt h\,b^{ab}(P_1c)_{ab}\,d^2\sigma
=\frac1{2\pi}\int d^2z\,(b\bar\partial c+\bar b\partial\bar c).
$$

The two chiral copies of this [bc system](../../../string-theory.md#bc-system) have [conformal weights](../../../string-theory.md#conformal-weight) $(2,-1)$ and [anticommutators](../../../vector-space.md#anticommutator) $\{b_m,c_n\}=\delta_{m+n,0}$. They are auxiliary fields for the gauge determinant, not additional spacetime particles. Their use is different from the unwanted timelike [negative-norm string states](../../../string-theory.md#negative-norm-string-state) of covariant matter quantization.

The chiral [holomorphic stress-energy tensor](../../../string-theory.md#holomorphic-stress-energy-tensor) of the [bc system](../../../string-theory.md#bc-system) is

$$
T_{\mathrm{gh}}=-2:b\partial c:-:(\partial b)c:.
$$

Double contractions in its [operator product expansion](../../../string-theory.md#operator-product-expansion) give the [central charge of reparameterization ghosts](../../../string-theory.md#central-charge-of-reparameterization-ghosts) $c_{\mathrm{gh}}=-26$. Equivalently, a fermionic [bc system](../../../string-theory.md#bc-system) with antighost weight $\lambda$ has $c=1-3(2\lambda-1)^2$, and $\lambda=2$ gives $-26$. The free coordinate matter contributes $c_{\mathrm m}=D$. Thus the total [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) vanishes for the flat critical [bosonic string theory](../../../string-theory.md#bosonic-string-theory) precisely when

$$
\boxed{c_{\mathrm{tot}}=D-26=0}.
$$

This statement assumes no additional matter or compensating [Liouville field theory](../../../string-theory.md#liouville-field-theory).

[BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry) expresses the gauge symmetry after gauge fixing by replacing its infinitesimal parameter with the [Grassmann variable](../../../linear-algebra.md#grassmann-variable) $c$. In one chiral conformal patch, its graded action has the form

$$
sX^\mu=c\partial X^\mu,\qquad sc=c\partial c,\qquad sb=T_{\mathrm{tot}};
$$

there is an analogous barred copy for a [closed string](../../../string-theory.md#closed-string). The [Grassmann parity](../../../linear-algebra.md#grassmann-parity) makes $s^2X=0$: the term from $sc$ cancels the term from applying $s$ to $\partial X$, while the term with $c^2$ vanishes. The gauge-fixed chiral transformations are on shell when their conservation equations are used. At the quantum level, [BRST nilpotence](../../../relativistic-quantum-field.md#brst-nilpotence) also tests the anomaly.

For example, an [open string](../../../string-theory.md#open-string) [BRST charge](../../../relativistic-quantum-field.md#brst-charge) can be written using the matter [Virasoro generators](../../../string-theory.md#virasoro-generator) as

$$
Q_B=\sum_n c_{-n}L_n^{\mathrm m}
-\frac12\sum_{m,n}(m-n):c_{-m}c_{-n}b_{m+n}:
-a c_0.
$$

Use the [ghost oscillator vacuum](../../../string-theory.md#ghost-oscillator-vacuum) $b_{n\geq0}|0\rangle_{mathrm{gh}}=c_{n>0}|0\rangle_{mathrm{gh}}=0$ and the corresponding oscillator [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering). In this convention the last term is $-c_0$ in the critical theory. With a differently shifted ghost $L_0$, the displayed intercept must be shifted consistently; one must not count the same shift twice. Squaring $Q_B$ shows why both critical conditions are needed. Its anomalous terms, in this convention, have coefficients

$$
Q_B^2=\frac12\sum_{n\in\mathbb Z}\left[\frac{D-26}{12}(n^3-n)+2(a-1)n\right]c_{-n}c_n.
$$

The independent cubic and linear terms vanish at $D=26$, $a=1$. The equivalent chiral [BRST current](../../../string-theory.md#brst-current) is $j_B=c(T_{mathrm m}+T_{mathrm{gh}}/2)+(3/2)\partial^2c$, with its contour integral defining the charge.

The graded identity $\{Q_B,b_n\}=L_n^{\mathrm{tot}}$ recovers the gauge constraints. In particular, on $|\psi\rangle\otimes|0\rangle_{mathrm{gh}}$, [BRST-closed](../../../relativistic-quantum-field.md#brst-closed-operator) imposes $L_{n>0}^{\mathrm m}|\psi\rangle=0$ and $(L_0^{\mathrm m}-1)|\psi\rangle=0$. Physical states are classes in [BRST cohomology](../../../relativistic-quantum-field.md#brst-cohomology),

$$
\boxed{\mathcal H_{\mathrm{phys}}=\ker Q_B/\operatorname{im}Q_B},
\qquad |\psi\rangle\sim|\psi\rangle+Q_B|\chi\rangle,
$$

at the appropriate ghost number: one for the usual open-string vertex and two for the closed-string vertex, with the closed-string zero-mode and [closed-string level matching](../../../string-theory.md#closed-string-level-matching) conditions also imposed. Since $Q_B^2=0$, an exact shift preserves closure. [BRST Ward identities](../../../relativistic-quantum-field.md#brst-ward-identity) make exact insertions decouple from physical amplitudes and establish gauge independence. Together with the [no-ghost theorem for the critical bosonic string](../../../string-theory.md#no-ghost-theorem-for-the-critical-bosonic-string), this explains how the auxiliary ghosts enforce gauge invariance while the physical spectrum retains positive norm.

## 4

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $Y$ be the compact coordinate, identified modulo $2\pi R$. The [closed string](../../../string-theory.md#closed-string) may wrap the circle:

$$
Y(\tau,\sigma+2\pi)=Y(\tau,\sigma)+2\pi wR,\qquad w\in\mathbb Z.
$$

Single-valued momentum eigenfunctions $e^{ipY}$ require $p=n/R$, $n\in\mathbb Z$. These are the [momentum and winding modes](../../../string-theory.md#momentum-and-winding-modes). Write the chiral zero-mode momenta as

$$
p_L=\frac nR+\frac{wR}{\alpha'},\qquad
p_R=\frac nR-\frac{wR}{\alpha'}.
$$

The left-moving [string oscillators](../../../string-theory.md#string-oscillator) will be tilded: $N_L=\widetilde N$, $N_R=N$. This fixes the sign in [compact-circle closed-string level matching](../../../string-theory.md#compact-circle-closed-string-level-matching).

Define the lower-dimensional [mass](../../../classical-mechanics.md#mass) by $M^2=-p_{\mathrm{noncompact}}^2$. The two [closed-string physical-state Virasoro conditions](../../../string-theory.md#closed-string-physical-state-virasoro-conditions), with bosonic [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) one, are

$$
\frac{\alpha'}4(-M^2+p_L^2)+N_L-1=0,
\qquad
\frac{\alpha'}4(-M^2+p_R^2)+N_R-1=0.
$$

Their average and difference derive the complete free [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum) on the circle:

$$
\boxed{M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}
+\frac2{\alpha'}(N_L+N_R-2)},
\qquad
\boxed{N_L-N_R+nw=0}.
$$

The allowed states have nonnegative integer oscillator levels and obey the [Virasoro constraints](../../../string-theory.md#virasoro-constraint) within each chiral sector. Compactification has not removed oscillator polarizations; it has added quantized compact momentum and allowed winding while changing the lower-dimensional interpretation of those polarizations.

At large $R$, the [momentum and winding modes](../../../string-theory.md#momentum-and-winding-modes) with $w=0$ have closely spaced momentum energies $|n|/R$, whereas nonzero winding costs $|w|R/\alpha'$. At small $R$ their roles reverse. The precise equality is [T-duality](../../../string-theory.md#t-duality):

$$
\boxed{R'=\frac{\alpha'}R,\qquad n'=w,\qquad w'=n}.
$$

It leaves $p_L$ unchanged and reverses $p_R$, and leaves the [mass](../../../classical-mechanics.md#mass) formula and [closed-string level matching](../../../string-theory.md#closed-string-level-matching) unchanged. On the [string embedding map](../../../string-theory.md#string-embedding-map) it reverses the right-moving part of $Y$. Therefore the small-radius spectrum is the large-radius spectrum of the dual theory, rather than a spectrum in which all charged states simply become heavy.

At a generic radius, the neutral level $(N_L,N_R)=(1,1)$ contains the lower-dimensional [graviton](../../../quantum-theory.md#graviton), [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) and [dilaton](../../../string-theory.md#dilaton), two [gauge bosons](../../../relativistic-quantum-field.md#gauge-boson) from the mixed components of the metric and two-form, and the radius [modulus of a string compactification](../../../string-theory.md#modulus-of-a-string-compactification). The two vector charges are the Cartan charges of $U(1)_L\times U(1)_R$.

Consider instead the following charged states:

$$
(N_L,N_R)=(0,1),\quad (n,w)=(1,1),(-1,-1),
$$



$$
(N_L,N_R)=(1,0),\quad (n,w)=(1,-1),(-1,1).
$$

Every state satisfies [compact-circle closed-string level matching](../../../string-theory.md#compact-circle-closed-string-level-matching). The single noncompact [string oscillator](../../../string-theory.md#string-oscillator) supplies a vector polarization. At the massless point, the level-one [Virasoro constraint](../../../string-theory.md#virasoro-constraint) imposes transverse polarization and its physical [null string state](../../../string-theory.md#null-string-state) identifies polarizations differing by the noncompact momentum. Thus these are genuine lower-dimensional vector states. Their squared [mass](../../../classical-mechanics.md#mass) is

$$
M^2=\frac1{R^2}+\frac{R^2}{\alpha'^2}-\frac2{\alpha'}
=\left(\frac1R-\frac R{\alpha'}\right)^2.
$$

Thus **four additional charged massless spin-one particles appear at**

$$
\boxed{R=\sqrt{\alpha'}}.
$$

For $(N_L,N_R)=(0,1)$ the charges have $p_R=0$, $p_L=\pm2/\sqrt{\alpha'}$; for $(1,0)$ they have $p_L=0$, $p_R=\pm2/\sqrt{\alpha'}$. This identifies the two pairs of charged roots.

The enhanced [gauge group](../../../relativistic-quantum-field.md#gauge-group) can be derived rather than just inferred from counting. At the [self-dual circle](../../../string-theory.md#self-dual-circle-compactification), the chiral [compact boson](../../../string-theory.md#compact-boson) satisfies $Y_L(z)Y_L(u)\sim-(\alpha'/2)\log(z-u)$. The [self-dual circle current algebra](../../../string-theory.md#self-dual-circle-current-algebra) has currents

$$
J_L^3=\frac{i}{\sqrt{\alpha'}}\partial Y_L,\qquad
J_L^\pm=:\!\exp\left(\pm\frac{2iY_L}{\sqrt{\alpha'}}\right)\!:.
$$

The exponentials have [conformal weight](../../../string-theory.md#conformal-weight) $\alpha'p_L^2/4=1$. Free-boson contractions give the [operator product expansions](../../../string-theory.md#operator-product-expansion)

$$
J^3(z)J^3(u)\sim\frac1{2(z-u)^2},\qquad
J^3(z)J^\pm(u)\sim\frac{\pm J^\pm(u)}{z-u},
$$



$$
J^+(z)J^-(u)\sim\frac1{(z-u)^2}+\frac{2J^3(u)}{z-u}.
$$

They form the level-one [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra), and there is an independent right-moving copy. The [string vertex operators](../../../string-theory.md#string-vertex-operator) $J_L^a\bar\partial X^\mu$ and $\partial X^\mu J_R^a$ give the six massless vectors. Consequently

$$
\boxed{U(1)_L\times U(1)_R\longrightarrow SU(2)_L\times SU(2)_R}.
$$

Changing $R$ gives the four charged vectors the mass found above, consistent with the [radius deformation as a Higgs mechanism](../../../string-theory.md#radius-deformation-as-a-higgs-mechanism).

For completeness, the enhanced spectrum also has [scalar fields](../../../quantum-field-theory.md#scalar-field). Using a compact rather than noncompact oscillator in the four singly excited charged families gives four scalars. At $(N_L,N_R)=(0,0)$, [closed-string level matching](../../../string-theory.md#closed-string-level-matching) requires $nw=0$; the [mass](../../../classical-mechanics.md#mass) equation then gives the four charges $(\pm2,0),(0,\pm2)$. These [exceptional massless ground states of a bosonic circle](../../../string-theory.md#exceptional-massless-ground-states-of-a-bosonic-circle) give another four scalars. Together with the radius scalar they form nine scalars in the $(3,3)$ representation, in addition to the neutral [dilaton](../../../string-theory.md#dilaton). The ever-present neutral bosonic [tachyon](../../../physics.md#tachyon) still has $M^2=-4/\alpha'$. The enhancement establishes the additional massless vectors, not stability of the entire bosonic vacuum.

## 5

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [RNS string](../../../string-theory.md#spinning-string) adds [worldsheet Majorana fermions](../../../string-theory.md#worldsheet-majorana-fermion) $\psi^\mu$ to the coordinate fields $X^\mu$. The new fields are spinors on the [worldsheet](../../../string-theory.md#worldsheet) but vectors under the target [Lorentz group](../../../special-relativity.md#lorentz-group); this distinction matters when interpreting their oscillator states. In a flat target, a convenient Lorentzian convention for the free gauge-fixed action is

$$
S=-\frac1{4\pi\alpha'}\int d^2\sigma\,
\left(\partial_aX^\mu\partial^aX_\mu-i\bar\psi^\mu\rho^a\partial_a\psi_\mu\right),
$$

where $\rho^a$ are two-dimensional [gamma matrices](../../../algebra.md#gamma-matrices). The bosonic and fermionic kinetic terms are related by [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry). Before fixing local [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry), one introduces a [worldsheet gravitino](../../../string-theory.md#worldsheet-gravitino) along with the [worldsheet metric](../../../string-theory.md#worldsheet-metric). After [superconformal gauge](../../../string-theory.md#superconformal-gauge) fixing, the residual matter constraints are the [Virasoro constraints](../../../string-theory.md#virasoro-constraint) and the constraints generated by the [superconformal current](../../../string-theory.md#superconformal-current) $G\propto\psi\cdot\partial X$.

Each real [worldsheet Majorana fermion](../../../string-theory.md#worldsheet-majorana-fermion) contributes $1/2$ to the chiral [central charge](../../../string-theory.md#central-charge), while each coordinate contributes one. The reparameterization [bc system](../../../string-theory.md#bc-system) contributes $-26$, and fixing local [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry) also produces commuting [superconformal ghosts](../../../string-theory.md#superconformal-ghost) of weights $(3/2,-1/2)$, with [central charge](../../../string-theory.md#central-charge) $11$. Thus

$$
c_{\mathrm{tot}}=\frac32D-26+11=0
\quad\Longrightarrow\quad
\boxed{D=10}.
$$

In [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory) there are eight physical transverse coordinate fields and eight transverse [worldsheet Majorana fermions](../../../string-theory.md#worldsheet-majorana-fermion).

On the doubled spatial interval of an [open string](../../../string-theory.md#open-string), the two allowed fermionic periodicities are

$$
\psi(\sigma+2\pi)=+\psi(\sigma)\quad\text{(Ramond)},\qquad
\psi(\sigma+2\pi)=-\psi(\sigma)\quad\text{(Neveu--Schwarz)}.
$$

They arise from the relative signs of the left-right fermion gluing conditions at the two ends. Thus the [Ramond sector](../../../string-theory.md#ramond-sector) has integer-mode oscillators $d_n$, including $d_0$, and the [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector) has half-integer oscillators $b_r$, $r\in\mathbb Z+1/2$, without zero modes. In either sector,

$$
\{\psi_r^\mu,\psi_s^\nu\}=\eta^{\mu\nu}\delta_{r+s,0}.
$$

A [closed string](../../../string-theory.md#closed-string) has independent left- and right-moving periodicities, giving four sector choices rather than two.

The [Ramond zero-mode Clifford algebra](../../../string-theory.md#ramond-zero-mode-clifford-algebra) is

$$
\{d_0^\mu,d_0^\nu\}=\eta^{\mu\nu},\qquad
\Gamma^\mu=\sqrt2\,d_0^\mu,\qquad
\{\Gamma^\mu,\Gamma^\nu\}=2\eta^{\mu\nu}.
$$

Hence its [ground states](../../../quantum-mechanics.md#ground-state) carry a [Spinor representation of the Lorentz group](../../../relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group). The zero-mode supercurrent constraint reduces on a ground state to the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) $p_\mu\Gamma^\mu u=0$. In the [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector) the [oscillator vacuum](../../../string-theory.md#oscillator-vacuum) instead carries a scalar representation. Consequently the [open string](../../../string-theory.md#open-string) [NS sector](../../../string-theory.md#neveu-schwarz-sector) describes spacetime [bosons](../../../quantum-mechanics.md#boson), while the [R sector](../../../string-theory.md#ramond-sector) describes spacetime [fermions](../../../quantum-mechanics.md#fermion). Exciting a target-vector oscillator does not change this statistics assignment.

The [string intercepts](../../../string-theory.md#normal-ordering-constant-of-a-string) follow from the transverse [zero-point energy](../../../quantum-mechanics.md#zero-point-energy). Per boson the integer-mode contribution is $\frac12\zeta(-1)=-1/24$. Per fermion it is the negative of the corresponding half-sum. Since $\zeta(-1,1/2)=1/24$, the eight transverse pairs give

$$
E_0^{\mathrm{NS}}=8\left(-\frac1{24}-\frac1{48}\right)=-\frac12,
\qquad
E_0^{\mathrm R}=8\left(-\frac1{24}+\frac1{24}\right)=0.
$$

Thus $a_{\mathrm{NS}}=1/2$, $a_{\mathrm R}=0$, and the [open string](../../../string-theory.md#open-string) [mass](../../../classical-mechanics.md#mass) formula is $\alpha'M^2=N-a$. This distinguishes the lowest states explicitly:

- In the [NS sector](../../../string-theory.md#neveu-schwarz-sector), the level-zero scalar is a [tachyon](../../../physics.md#tachyon) with $M^2=-1/(2\alpha')$. At level $1/2$, $\epsilon_\mu b_{-1/2}^\mu|0;p\rangle$ is a massless vector. The supercurrent and [Virasoro constraints](../../../string-theory.md#virasoro-constraint) give $p\cdot\epsilon=0$ and the equivalence $\epsilon\sim\epsilon+\lambda p$. There are eight physical vector polarizations.
- In the [R sector](../../../string-theory.md#ramond-sector), the level-zero states are massless spacetime [spinors](../../../algebra.md#spinor) satisfying the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation). Before the [GSO projection](../../../string-theory.md#gso-projection), the two chiralities together give 16 on-shell polarizations; they split into the two eight-dimensional transverse spinor representations.

The supersymmetric [GSO projection](../../../string-theory.md#gso-projection) keeps odd oscillator fermion number in the [NS sector](../../../string-theory.md#neveu-schwarz-sector). Defining $F_{\mathrm{osc}}$ so that the NS vacuum has $F_{\mathrm{osc}}=0$, its projector is

$$
P_{\mathrm{NS}}=\frac12\left(1-(-1)^{F_{\mathrm{osc}}}\right).
$$

It removes the scalar [tachyon](../../../physics.md#tachyon) and keeps the massless vector. In the [R sector](../../../string-theory.md#ramond-sector), fermion parity contains the zero-mode chirality operator, so one may write

$$
P_{\mathrm R}=\frac12\left(1+\eta\Gamma_{11}(-1)^{F_{\mathrm{osc}}}\right),\qquad \eta=\pm1.
$$

Here $F_{\mathrm{osc}}$ counts nonzero-mode fermionic excitations. On the [ground states](../../../quantum-mechanics.md#ground-state), this keeps one [Majorana-Weyl spinor](../../../relativistic-quantum-field.md#majorana-weyl-spinor) chirality: 16 real covariant components, or eight on-shell polarizations after the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation). **The projected massless open-string states are an eight-polarization gauge vector and an eight-polarization gaugino.** The compatible projected tower exhibits spacetime [supersymmetry](../../../supersymmetry.md); unprojected [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry) by itself did not eliminate the tachyon or equalize these massless counts.

For a [closed string](../../../string-theory.md#closed-string), both chiral zero-mode constraints must hold:

$$
\boxed{M^2=\frac4{\alpha'}(N_L-a_L)=\frac4{\alpha'}(N_R-a_R)},\qquad
\boxed{N_L-a_L=N_R-a_R}.
$$

This shifted [closed-string level matching](../../../string-theory.md#closed-string-level-matching) is particularly important in the mixed sectors. The lowest states and their spacetime nature are as follows.

- The [NS-NS sector](../../../string-theory.md#neveu-schwarz-neveu-schwarz-sector) is bosonic. Before projection, $(N_L,N_R)=(0,0)$ is a scalar [tachyon](../../../physics.md#tachyon) with $M^2=-2/\alpha'$. The [GSO projection](../../../string-theory.md#gso-projection) on each side removes it. The surviving lowest level is $(1/2,1/2)$, with transverse states $b_{-1/2}^i\widetilde b_{-1/2}^j|0;p\rangle$. Decomposing their tensor product into symmetric traceless, antisymmetric and trace parts gives the [graviton](../../../quantum-theory.md#graviton), [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) and [dilaton](../../../string-theory.md#dilaton), with $35+28+1=64$ physical polarizations.
- The [RR sector](../../../string-theory.md#ramond-ramond-sector) is bosonic, since it combines two spacetime [spinors](../../../algebra.md#spinor). Its lowest states have $(N_L,N_R)=(0,0)$ and are massless. The two [Dirac equations](../../../relativistic-quantum-field.md#dirac-equation) on the bispinor polarizations identify them with on-shell differential-form field strengths. After projection they supply 64 bosonic polarizations. The actual form degrees depend on the two chosen [Ramond sector](../../../string-theory.md#ramond-sector) chiralities.
- The [NS-R sector](../../../string-theory.md#neveu-schwarz-ramond-sector) and [R-NS sector](../../../string-theory.md#ramond-neveu-schwarz-sector) are fermionic. Their respective lowest level-matched pairs are $(1/2,0)$ and $(0,1/2)$, not two oscillator vacua. A vector tensored with a chiral spinor decomposes into its gamma-traceless vector-spinor and gamma trace. These give a massless [gravitino](../../../supersymmetry.md#gravitino) and [dilatino](../../../supersymmetry.md#dilatino), with $56+8=64$ polarizations in each mixed sector. The vacuum pair would fail the shifted [closed-string level matching](../../../string-theory.md#closed-string-level-matching), so it cannot be counted as a mixed-sector tachyon.

For [type IIA superstring theory](../../../string-theory.md#type-iia-superstring-theory), the two [R sector](../../../string-theory.md#ramond-sector) ground-state chiralities are opposite. The [Ramond–Ramond potentials](../../../string-theory.md#ramond-ramond-potential) can be represented by $C_1,C_3$, with transverse counts $8+56=64$. The two mixed-sector [gravitinos](../../../supersymmetry.md#gravitino) have opposite chiralities, and the ten-dimensional theory is nonchiral. For [type IIB superstring theory](../../../string-theory.md#type-iib-superstring-theory), the two [R sector](../../../string-theory.md#ramond-sector) chiralities agree; the [Ramond–Ramond potentials](../../../string-theory.md#ramond-ramond-potential) are $C_0,C_2,C_4$, with self-dual five-form field strength, giving $1+28+35=64$. Its two [gravitinos](../../../supersymmetry.md#gravitino) have the same chirality. Thus **both projected type II theories have 128 massless bosonic and 128 massless fermionic polarizations and no tachyon**, while their chiralities and form spectra differ.

If unoriented [open strings](../../../string-theory.md#open-string) are included in the complete theory, the supersymmetric example is [type I string theory](../../../string-theory.md#type-i-string-theory). Worldsheet orientation reversal projects the closed [type IIB superstring theory](../../../string-theory.md#type-iib-superstring-theory) spectrum and identifies the two mixed sectors; the surviving closed fields include the [graviton](../../../quantum-theory.md#graviton), [dilaton](../../../string-theory.md#dilaton), a [Ramond–Ramond potential](../../../string-theory.md#ramond-ramond-potential) $C_2$, and one [gravitino](../../../supersymmetry.md#gravitino) and [dilatino](../../../supersymmetry.md#dilatino). The open states form vector and gaugino multiplets with [Chan-Paton factors](../../../string-theory.md#chan-paton-factor); tadpole and anomaly cancellation select $SO(32)$. This is an additional orientation projection, not part of the [GSO projection](../../../string-theory.md#gso-projection) itself. The [heterotic string](../../../string-theory.md#heterotic-string) instead pairs one supersymmetric chiral side with a bosonic chiral side carrying an internal gauge sector; it does not have a Ramond choice on both sides.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
