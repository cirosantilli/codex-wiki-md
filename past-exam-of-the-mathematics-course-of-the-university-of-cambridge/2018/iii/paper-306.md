# Paper 306

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_306.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_306.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $\eta_{mn}=\operatorname{diag}(-1,1,\ldots,1)$ and units with [speed of light](../../../special-relativity.md#speed-of-light) one. The contractions are $P^2=\eta^{mn}P_mP_n$ and $(TX')^2=T^2\eta_{mn}(X^m)'(X^n)'$; $(X^m)'P_m$ and $\dot X^mP_m$ pair a [vector](../../../vector-space.md#vector) with a [covector](../../../linear-algebra.md#covector) without another metric. The [Lagrange multipliers](../../../mathematical-optimization.md#lagrange-multiplier) impose the two [first-class constraints](../../../classical-mechanics.md#first-class-constraint)

$$
\mathcal H=\tfrac12(P^2+T^2X'^2)=0,\qquad \mathcal D=X'\cdot P=0.
$$

They generate [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism), so the [phase space](../../../classical-mechanics.md#phase-space) contains both constrained directions and [gauge redundancy](../../../relativistic-quantum-field.md#gauge-redundancy). Two [first-class constraints](../../../classical-mechanics.md#first-class-constraint) remove two [canonical pairs](../../../classical-mechanics.md#canonical-pair), leaving $D-2$ physical [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) per point.

In [Monge gauge](../../../string-theory.md#monge-gauge), $X^0=t$ and $X^1=\sigma$. Write the transverse [canonical variables](../../../classical-mechanics.md#canonical-variables) as $\boldsymbol X=(X^2,\ldots,X^{D-1})$ and $\boldsymbol P=(P_2,\ldots,P_{D-1})$. Solving the [first-class constraints](../../../classical-mechanics.md#first-class-constraint) gives

$$
P_1=-\boldsymbol X'\cdot\boldsymbol P,\qquad
P_0=-\mathcal E,\qquad
\mathcal E=\sqrt{T^2(1+|\boldsymbol X'|^2)+|\boldsymbol P|^2+(\boldsymbol X'\cdot\boldsymbol P)^2}.
$$

The negative root selects positive [energy](../../../classical-mechanics.md#energy). Substitution into the [phase-space action](../../../classical-mechanics.md#phase-space-action) gives the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) reduction

$$
\boxed{I_{\mathrm{red}}=\int dt\int_0^\pi d\sigma\,
\bigl(\dot{\boldsymbol X}\cdot\boldsymbol P-\mathcal E\bigr).}
$$

For a static segment, $\boldsymbol P=0$, its [proper length](../../../special-relativity.md#proper-length) element is $d\ell=\sqrt{1+|\boldsymbol X'|^2}\,d\sigma$, and $\mathcal E\,d\sigma=T\,d\ell$. Thus **the [string tension](../../../string-theory.md#string-tension) is the [rest energy](../../../special-relativity.md#rest-energy) per unit [proper length](../../../special-relativity.md#proper-length)**. In particular a straight resting segment has $\mathcal E=T$. [Monge gauge](../../../string-theory.md#monge-gauge) is a local choice on a [string embedding map](../../../string-theory.md#string-embedding-map) for which $X^1$ is a valid coordinate; it need not cover folded strings or all endpoint configurations.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) equation is $\dot X=eP+uX'$. Eliminating $P$ from the [phase-space action](../../../classical-mechanics.md#phase-space-action) yields the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density)

$$
\mathcal L=\frac{(\dot X-uX')^2}{2e}-\frac{eT^2}{2}X'^2.
$$

This is the [Polyakov action](../../../string-theory.md#polyakov-action) after identifying its inverse [metric tensor](../../../general-relativity.md#metric-tensor) density as

$$
\sqrt{-\gamma}\,\gamma^{\mu\nu}
=\frac1{Te}\begin{pmatrix}-1&u\\u&T^2e^2-u^2\end{pmatrix},\qquad
\gamma=\det\gamma_{\mu\nu}.
$$

The [determinant](../../../linear-algebra.md#determinant) of this [matrix](../../../vector-space.md#matrix) is $-1$, as required in two dimensions. The [Weyl transformation](../../../string-theory.md#weyl-transformation) leaves the [matrix](../../../vector-space.md#matrix) unchanged, so $e,u$ encode the metric modulo its [conformal factor](../../../general-relativity.md#conformal-factor).

Define the [induced worldsheet metric](../../../string-theory.md#induced-worldsheet-metric) by $g_{\mu\nu}=\eta_{mn}\partial_\mu X^m\partial_\nu X^n$. Varying the independent inverse [metric tensor](../../../general-relativity.md#metric-tensor) in the [Polyakov action](../../../string-theory.md#polyakov-action) gives

$$
g_{\mu\nu}-\tfrac12\gamma_{\mu\nu}\gamma^{\rho\sigma}g_{\rho\sigma}=0.
$$

Consequently $g_{\mu\nu}=f\gamma_{\mu\nu}$, where $f=\tfrac12\gamma^{\rho\sigma}g_{\rho\sigma}$. For a nondegenerate Lorentzian [string worldsheet](../../../string-theory.md#worldsheet) with the usual compatible time orientation, take $f>0$, or $\gamma_{\mu\nu}=e^{2\omega}g_{\mu\nu}$. The undetermined function is precisely [Weyl invariance](../../../string-theory.md#weyl-transformation). Since $\sqrt{-\gamma}\,\gamma^{\mu\nu}g_{\mu\nu}=2\sqrt{-g}$, elimination of the independent [metric tensor](../../../general-relativity.md#metric-tensor) gives

$$
\boxed{I_{\mathrm{NG}}=-T\int dt\,d\sigma\,\sqrt{-\det g_{\mu\nu}}.}
$$

Thus the [Nambu–Goto action](../../../string-theory.md#nambu-goto-action) measures minus [string tension](../../../string-theory.md#string-tension) times Lorentzian [worldsheet area](../../../string-theory.md#worldsheet-area). The metric elimination holds in the nondegenerate interior; null endpoints are understood as boundary limits.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

In [conformal gauge](../../../string-theory.md#conformal-gauge), $\gamma_{\mu\nu}=e^{2\omega}\operatorname{diag}(-1,1)$. The [Weyl invariance](../../../string-theory.md#weyl-transformation) of the [Polyakov action](../../../string-theory.md#polyakov-action) removes $\omega$, leaving

$$
I_{\mathrm{conf}}=\frac T2\int_{t_i}^{t_f}dt\int_0^\ell d\sigma\,
(\dot X^2-X'^2).
$$

Its complete variation is

$$
\delta I_{\mathrm{conf}}=
T\int dt\,d\sigma\,(X''-\ddot X)\cdot\delta X
+T\left[\int_0^\ell d\sigma\,\dot X\cdot\delta X\right]_{t_i}^{t_f}
-T\int dt\,[X'\cdot\delta X]_0^\ell.
$$

Fix the [string embedding map](../../../string-theory.md#string-embedding-map) on the initial and final time slices. The interior [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) is the [wave equation](../../../wave-equation.md)

$$
\boxed{\ddot X^m-X^{m\prime\prime}=0.}
$$

At each spatial endpoint the remaining variation vanishes under either [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), $\delta X^m=0$, or [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition), $X^{m\prime}=0$, independently for each target-space component. Thus **a fixed endpoint or a free endpoint makes the boundary contribution vanish**. Fixing a spatial point throughout time imposes [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) on its spatial coordinates, while the time coordinate may retain [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition).

The independent [metric tensor](../../../general-relativity.md#metric-tensor) equation must also be retained after [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing). Its [Virasoro constraints](../../../string-theory.md#virasoro-constraint) are

$$
\dot X\cdot X'=0,\qquad \dot X^2+X'^2=0.
$$

Together with the [wave equation](../../../wave-equation.md), these ensure equivalence to the [Nambu–Goto action](../../../string-theory.md#nambu-goto-action); varying only the already fixed metric would lose these [Virasoro constraints](../../../string-theory.md#virasoro-constraint).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Let $q=\sigma/L$, with $L>0$, and let $Z=X^1+iX^2$. Direct differentiation gives $\ddot Z=Z''=-Z/L^2$, while the time coordinate also satisfies the [wave equation](../../../wave-equation.md). Using the [Minkowski metric](../../../special-relativity.md#minkowski-metric),

$$
\dot X\cdot X'=0,\qquad \dot X^2=-\cos^2q,\qquad X'^2=\cos^2q.
$$

Thus both [Virasoro constraints](../../../string-theory.md#virasoro-constraint) hold, and the [induced worldsheet metric](../../../string-theory.md#induced-worldsheet-metric) is $g_{\mu\nu}=\cos^2q\,\operatorname{diag}(-1,1)$. The configuration solves the [Nambu–Goto action](../../../string-theory.md#nambu-goto-action) equations in its interior.

Place the fixed end at $\sigma=0$. The first free endpoint has $Z'=e^{it/L}\cos q=0$ at $q=\pi/2$. For the usual single unfolded [rotating Nambu–Goto string](../../../string-theory.md#rotating-nambu-goto-string),

$$
\boxed{0\leq\sigma\leq\frac{\pi L}{2},\qquad
\ell_{\mathrm{proper}}=\int_0^{\pi L/2}|Z'|\,d\sigma=L.}
$$

This parameter interval need not equal the earlier interval $[0,\pi]$, since that interval was a coordinate convention. The [proper length](../../../special-relativity.md#proper-length) is measured on a constant-$X^0$ slice; the local motion is perpendicular to the string, so there is no longitudinal [Lorentz contraction](../../../special-relativity.md#length-contraction).

All points have the same phase $t/L$, hence the segment rotates rigidly with [angular velocity](../../../classical-mechanics.md#angular-velocity) $\Omega=1/L$. At radius $r=L\sin q$, its [speed](../../../classical-mechanics.md#speed) is $v=r/L$. Therefore **the free tip moves at the [speed of light](../../../special-relativity.md#speed-of-light)**. This is consistent with its [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition): $X'=0$ and the [Virasoro constraints](../../../string-theory.md#virasoro-constraint) imply $\dot X^2=0$ at the free tip. The null endpoint is a boundary limit, not a nondegenerate interior point.

In this [conformal gauge](../../../string-theory.md#conformal-gauge), $P_m=T\dot X_m$, so the [energy density](../../../statistical-physics.md#energy-density) per $\sigma$ is $-P_0=T$. Equivalently, the [energy density](../../../statistical-physics.md#energy-density) per [proper length](../../../special-relativity.md#proper-length) is $T/\sqrt{1-r^2/L^2}$. Thus

$$
E=T\int_0^{\pi L/2}d\sigma=\frac{\pi TL}{2},\qquad
E_{\mathrm{rest}}=TL,
$$

and the [rotational kinetic energy](../../../classical-mechanics.md#rotational-kinetic-energy) is

$$
\boxed{E_{\mathrm{rot}}=\left(\frac\pi2-1\right)TL
=\left(1-\frac2\pi\right)E.}
$$

The [angular momentum](../../../classical-mechanics.md#angular-momentum) about the fixed point is

$$
J=\int d\sigma\,(X^1P_2-X^2P_1)
=TL\int_0^{\pi L/2}\sin^2(\sigma/L)\,d\sigma
=\frac{\pi TL^2}{4}.
$$

Therefore the [Regge trajectory](../../../string-theory.md#regge-trajectory) is

$$
\boxed{E=\frac{\pi TL}{2},\qquad J=\frac{E^2}{\pi T},\qquad\beta=\frac1{\pi T}.}
$$

The endpoint conditions alone also admit folded extensions with parameter length $(n+\tfrac12)\pi L$, $n\geq0$. Their [proper length](../../../special-relativity.md#proper-length), [energy](../../../classical-mechanics.md#energy) and [angular momentum](../../../classical-mechanics.md#angular-momentum) are $(2n+1)$ times the values above, and $\beta=1/[(2n+1)\pi T]$. The displayed answer uses the implicit unfolded-segment convention.

## 2

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The real [canonical variables](../../../classical-mechanics.md#canonical-variables) $x^m,p_m$ describe the center-of-mass position and total [momentum](../../../classical-mechanics.md#momentum) of the [open string](../../../string-theory.md#open-string). The nonzero [string oscillators](../../../string-theory.md#string-oscillator) are complex [Fourier modes](../../../fourier-analysis.md#fourier-mode) with $\alpha_{-k}^m=(\alpha_k^m)^*$; the [Lagrange multipliers](../../../mathematical-optimization.md#lagrange-multiplier) obey $\lambda_{-j}=\lambda_j^*$. The [Virasoro constraints](../../../string-theory.md#virasoro-constraint) satisfy $L_{-j}=L_j^*$, so the multiplier term is real.

For each $k>0$, the oscillator kinetic term differs from the manifestly real expression

$$
\frac{i}{2k}\bigl(\dot\alpha_k\cdot\alpha_{-k}
-\alpha_k\cdot\dot\alpha_{-k}\bigr)
$$

by $\frac{i}{2k}\frac{d}{dt}(\alpha_k\cdot\alpha_{-k})$. Thus the written [action](../../../classical-mechanics.md#action) is real up to a boundary term, which does not change its [symplectic form](../../../symplectic-geometry.md#symplectic-form) or bulk dynamics. Adding the corresponding endpoint term makes reality exact.

The independent nonzero [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) are

$$
\boxed{\{x^m,p_n\}=\delta^m_n,\qquad
\{\alpha_j^m,\alpha_k^n\}=-ij\,\eta^{mn}\delta_{j+k,0},\quad j,k\neq0.}
$$

All brackets between these independent center-of-mass and oscillator variables vanish. The dependent zero mode is $\alpha_0^m=p^m/\sqrt{\pi T}$, so, if it is used, $\{x^m,\alpha_0^n\}=\eta^{mn}/\sqrt{\pi T}$.

The [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) of the [Virasoro constraints](../../../string-theory.md#virasoro-constraint) are

$$
L_j=\frac12\sum_{k\in\mathbb Z}\alpha_{j-k}\cdot\alpha_k,\qquad
L_0=\frac{p^2}{2\pi T}+\sum_{k=1}^{\infty}\alpha_{-k}\cdot\alpha_k.
$$

Their [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) are

$$
\boxed{\{L_j,L_k\}=-i(j-k)L_{j+k}.}
$$

They form the classical [Witt algebra](../../../lie-algebra.md#witt-algebra), with no [Virasoro central extension](../../../string-theory.md#virasoro-central-extension). In particular they are [first-class constraints](../../../classical-mechanics.md#first-class-constraint), closing on the constraint surface, and generate the remaining [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) rather than independent physical excitations.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

In the displayed version of [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory), the oscillators have $D-2$ transverse components and

$$
N=\sum_{k=1}^{\infty}\boldsymbol\alpha_{-k}\cdot\boldsymbol\alpha_k.
$$

The center-of-mass [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) remain $\{x^m,p_n\}=\delta^m_n$, and the transverse oscillator [Poisson brackets](../../../classical-mechanics.md#poisson-bracket) are $\{\alpha_j^a,\alpha_k^b\}=-ij\delta^{ab}\delta_{j+k,0}$. Other independent brackets vanish. With $\hbar=1$, [canonical quantization](../../../quantum-mechanics.md#canonical-quantization) gives the [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation)

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_j^a,\alpha_k^b]=j\delta^{ab}\delta_{j+k,0},\qquad
(\alpha_k^a)^\dagger=\alpha_{-k}^a.
$$

The oscillator [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) at [momentum](../../../classical-mechanics.md#momentum) $p$ is defined by $\alpha_k^a|0;p\rangle=0$ for $k>0$. It is the ground state of one string, rather than the empty spacetime vacuum. Set $a_k^a=\alpha_k^a/\sqrt{k}$ for $k>0$. The [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) prescription gives the [string level operator](../../../string-theory.md#string-level-operator)

$$
\widehat N=\sum_{k>0,a}\alpha_{-k}^a\alpha_k^a
=\sum_{k>0,a}k\,(a_k^a)^\dagger a_k^a,\qquad \widehat N|0;p\rangle=0.
$$

A [Fock state](../../../quantum-field-theory.md#fock-state) basis is obtained by applying $\prod_{k,a}((a_k^a)^\dagger)^{n_{ka}}/\sqrt{n_{ka}!}$ to $|0;p\rangle$, with [string level operator](../../../string-theory.md#string-level-operator) eigenvalue $N=\sum_{k,a}k n_{ka}$. In particular, its level-one states are

$$
\boxed{\alpha_{-1}^a|0;p\rangle,\qquad a=1,\ldots,D-2.}
$$

They transform as the transverse vector of the [little group](../../../special-relativity.md#little-group) rotation subgroup $SO(D-2)$, precisely the [vector-particle polarizations](../../../special-relativity.md#vector-particle-polarization) of a massless vector. A massive vector would instead require $D-1$ [vector-particle polarizations](../../../special-relativity.md#vector-particle-polarization). This conclusion uses a quantization compatible with the [Lorentz group](../../../special-relativity.md#lorentz-group) of the [bosonic string theory](../../../string-theory.md#bosonic-string-theory).

The classical mass constraint alone has no quantum [zero-point energy](../../../quantum-mechanics.md#zero-point-energy) shift. Its quantum version includes the [normal-ordering constant of a string](../../../string-theory.md#normal-ordering-constant-of-a-string) $a$:

$$
(p^2+2\pi T(\widehat N-a))|\mathrm{phys}\rangle=0,\qquad
M^2=2\pi T(N-a).
$$

Masslessness at level one fixes $a=1$, so

$$
\boxed{M_1^2=0,\qquad M_0^2=-2\pi T.}
$$

Thus **the ground state is a [tachyon](../../../physics.md#tachyon)**. Without the quantum ordering shift, the displayed classical constraint would give $M_1^2=2\pi T$ and would not support the stated massless interpretation. In the usual transverse vacuum regularization, $a=(D-2)/24$; consistency with $a=1$ also gives the [critical dimension of string theory](../../../string-theory.md#critical-dimension-of-string-theory) $D=26$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For [covariant quantization of the bosonic string](../../../string-theory.md#covariant-quantization-of-the-bosonic-string),

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_j^m,\alpha_k^n]=j\eta^{mn}\delta_{j+k,0},\qquad
(\alpha_k^m)^\dagger=\alpha_{-k}^m.
$$

All other commutators between independent [canonical variables](../../../classical-mechanics.md#canonical-variables) vanish. The covariant [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) obeys $\alpha_k^m|0;p\rangle=0$ for every $k>0$ and every $m$. [Normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) moves these annihilating [string oscillators](../../../string-theory.md#string-oscillator) to the right and gives

$$
\widehat L_j=\frac12\sum_{k\in\mathbb Z}:\alpha_{j-k}\cdot\alpha_k:,
\qquad
\widehat L_0=\frac{p^2}{2\pi T}+\widehat N_{\mathrm{cov}},\qquad
\widehat N_{\mathrm{cov}}=\sum_{k>0}\alpha_{-k}\cdot\alpha_k.
$$

Then $\widehat N_{\mathrm{cov}}|0;p\rangle=0$. Its commutator $[\widehat N_{\mathrm{cov}},\alpha_{-k}^m]=k\alpha_{-k}^m$ grades a [Fock state](../../../quantum-field-theory.md#fock-state) basis by $N=\sum k n_{km}$, although its [inner product](../../../linear-algebra.md#inner-product) is indefinite because of the timelike oscillator.

The quantum [Virasoro algebra](../../../string-theory.md#virasoro-algebra) has [central charge](../../../string-theory.md#central-charge) $D$:

$$
\boxed{[\widehat L_j,\widehat L_k]=(j-k)\widehat L_{j+k}
+\frac D{12}j(j^2-1)\delta_{j+k,0}.}
$$

The [Virasoro central extension](../../../string-theory.md#virasoro-central-extension) comes from [commutators](../../../lie-algebra.md#commutator) needed to order infinite oscillator sums; it is a quantum effect absent from the classical [Poisson brackets](../../../classical-mechanics.md#poisson-bracket). Replacing a classical [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) by a [commutator](../../../lie-algebra.md#commutator) cannot recover that term without a regularized ordering calculation.

If a state were annihilated by every nonzero $\widehat L_j$, the $j=1,k=-1$ [commutator](../../../lie-algebra.md#commutator) would imply $\widehat L_0|\psi\rangle=0$. The $j=2,k=-2$ commutator would then imply $(D/2)|\psi\rangle=0$. For $D>0$, **only the zero vector is annihilated by all nonzero [Virasoro constraints](../../../string-theory.md#virasoro-constraint)**. This explains why only positive modes annihilate a [physical string state](../../../string-theory.md#physical-string-state).

The vacuum is a [physical string state](../../../string-theory.md#physical-string-state) when $p^2=2\pi Ta$. At level one all states have the form $|A;p\rangle=A_m\alpha_{-1}^m|0;p\rangle$. Since $[\widehat L_j,\alpha_k^m]=-k\alpha_{j+k}^m$, the positive-mode [Virasoro constraints](../../../string-theory.md#virasoro-constraint) give

$$
\widehat L_1|A;p\rangle=\frac{A\cdot p}{\sqrt{\pi T}}|0;p\rangle,\qquad
\widehat L_j|A;p\rangle=0\quad(j\geq2).
$$

Thus the complete level-one conditions and norm are

$$
\boxed{p^2=2\pi T(a-1),\qquad A\cdot p=0,\qquad
\langle A;p|A;p\rangle=A_m^*\eta^{mn}A_n,}
$$

with the common vacuum normalization suppressed.

For $a>1$, choose spacelike [momentum](../../../classical-mechanics.md#momentum) $p^m=(0,k,0,\ldots)$, $k^2=2\pi T(a-1)$. A purely timelike polarization has $A\cdot p=0$ and norm $-1$. Hence **a negative-norm [physical string state](../../../string-theory.md#physical-string-state) exists when $a>1$**.

For $a<1$, the [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) gives $M^2=2\pi T(1-a)>0$. In a rest frame, $A\cdot p=0$ forces $A_0=0$, leaving $D-1$ positive-norm [vector-particle polarizations](../../../special-relativity.md#vector-particle-polarization), those of a massive vector.

For $a=1$ and nonzero null [momentum](../../../classical-mechanics.md#momentum), $A\cdot p=0$ leaves a null direction $A_m\propto p_m$. The corresponding [null string state](../../../string-theory.md#null-string-state) is $p\cdot\alpha_{-1}|0;p\rangle=\sqrt{\pi T}\widehat L_{-1}|0;p\rangle$. It is orthogonal to every [physical string state](../../../string-theory.md#physical-string-state) because $\widehat L_1$ annihilates them. Quotienting by this [gauge redundancy](../../../relativistic-quantum-field.md#gauge-redundancy), $A_m\sim A_m+\zeta p_m$, leaves $D-2$ positive [vector-particle polarizations](../../../special-relativity.md#vector-particle-polarization). Thus **the level-one spectrum agrees with [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory) at $a=1$**. This level-one argument alone does not establish consistency or absence of negative norms at all higher levels.

## 3

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use $\delta F=\epsilon\{F,\varphi\}$ with the canonical [Poisson bracket](../../../classical-mechanics.md#poisson-bracket). The [first-class constraint](../../../classical-mechanics.md#first-class-constraint) generates

$$
\boxed{\delta x^m=\epsilon p^m,\qquad \delta p_m=0,\qquad \delta e=\dot\epsilon.}
$$

Indeed the variation of the [relativistic particle phase-space action](../../../classical-mechanics.md#relativistic-particle-phase-space-action) is

$$
\delta I=\int dt\,\left\{\frac12\frac{d}{dt}
[\epsilon(p^2-M^2)]+(\dot\epsilon-\delta e)\varphi\right\}.
$$

The transformation is therefore a [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) when its parameter vanishes at the time endpoints, or suitable boundary conditions remove the total derivative.

On a fixed interval of parameter length $\Delta t$, the [proper-time modulus](../../../classical-mechanics.md#proper-time-modulus)

$$
s=\frac1{\Delta t}\int_{t_i}^{t_f}e(t)\,dt
$$

is unchanged by these [gauge transformations](../../../electromagnetism.md#gauge-transformation). Choosing $\epsilon(t)=\int_{t_i}^{t}(s-e(u))\,du$ sets $e+\delta e=s$, with $\epsilon(t_i)=\epsilon(t_f)=0$. Thus **the nonconstant part of the [worldline einbein](../../../classical-mechanics.md#worldline-einbein) can be fixed, but its constant modulus must still be integrated over**. Fixing $e=1$ as well would remove inequivalent values of the [proper-time modulus](../../../classical-mechanics.md#proper-time-modulus); it is legitimate only if the parameter interval is allowed to vary instead. The name proper-time modulus refers to the Schwinger proper-time parameter; after eliminating $p$, the geometric proper length for a massive on-shell trajectory is $M\int e\,dt$ in this normalization.

For the [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) functional $F=e-s$, its variation is $\delta F=\dot\epsilon$. The [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) is consequently

$$
\Delta_{\mathrm{FP}}=\det\bigl[\partial_t\delta(t-t')\bigr].
$$

The [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral) represents this determinant using anticommuting [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) $b,c$:

$$
\boxed{I_{\mathrm{FP}}=i\int dt\,b\dot c,\qquad
\int\mathcal Db\,\mathcal Dc\,e^{iI_{\mathrm{FP}}}\ \propto\ \det(\partial_t).}
$$

The phase and normalization of the determinant depend on the measure convention. Its domain carries the chosen boundary conditions: on an interval the constant modulus is excluded from the gauge-fixed directions, and on a periodic [worldline](../../../special-relativity.md#world-line) the constant ghost [zero mode in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory) is removed with the residual gauge volume treated separately. A bare determinant with such zero modes left in would vanish.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Jacobi identity for the Poisson bracket](../../../classical-mechanics.md#jacobi-identity-for-the-poisson-bracket) implies

$$
\bigl(f_{ij}{}^l f_{kl}{}^m+f_{jk}{}^l f_{il}{}^m
+f_{ki}{}^l f_{jl}{}^m\bigr)\varphi_m=0.
$$

For [first-class constraints](../../../classical-mechanics.md#first-class-constraint) with [linearly independent](../../../vector-space.md#linear-independence) differentials this gives $f_{[ij}{}^l f_{k]l}{}^m=0$, the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) for the [structure constants](../../../algebra.md#structure-constant) of the [constraint algebra](../../../classical-mechanics.md#constraint-algebra). Independence is an implicit assumption: for constraints obeying identities or vanishing identically, only the contracted identity follows, and arbitrary coefficients multiplying such constraints need not satisfy a [Lie algebra](../../../lie-algebra.md) identity.

With $G=\epsilon^i\varphi_i$ and $\delta F=\{F,G\}$, the [canonical variables](../../../classical-mechanics.md#canonical-variables) transform as

$$
\boxed{\delta q^I=\epsilon^i\frac{\partial\varphi_i}{\partial p_I},\qquad
\delta p_I=-\epsilon^i\frac{\partial\varphi_i}{\partial q^I}.}
$$

To fix the sign convention, vary the [phase-space action](../../../classical-mechanics.md#phase-space-action) directly:

$$
\delta I=\bigl[p_I\delta q^I-\epsilon^i\varphi_i\bigr]_{t_i}^{t_f}
+\int dt\,\bigl(\dot\epsilon^i+\epsilon^j\lambda^k f_{jk}{}^i-\delta\lambda^i\bigr)\varphi_i.
$$

Thus action invariance requires $\delta\lambda^i=\dot\epsilon^i+\epsilon^j\lambda^k f_{jk}{}^i$. For $F^i=\lambda^i-\bar\lambda^i$, the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) is that of

$$
\mathcal M^i{}_j=\delta^i_j\partial_t+\bar\lambda^k f_{jk}{}^i.
$$

Using anticommuting [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost), the invariant-convention result is

$$
\boxed{I_{\mathrm{FP}}=i\int dt\,b_i
\bigl(\dot c^i+c^j\bar\lambda^k f_{jk}{}^i\bigr).}
$$

**The original PDF has a sign error in the stated multiplier transformation; the TeX transcription has the consistent plus sign.** Keeping the PDF's displayed minus sign mechanically would instead give $i\int dt\,b_i(\dot c^i-c^j\bar\lambda^k f_{jk}{}^i)$. That expression exponentiates the determinant of the printed transformation, but that transformation does not preserve the stated [action](../../../classical-mechanics.md#action) with the canonical convention above. It cannot be used as the invariant result without changing another convention consistently.

As for the particle, constant multiplier moduli and any residual [zero mode in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory) must be handled separately; the constant [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) is understood locally on the [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the classically equivalent [Polyakov action](../../../string-theory.md#polyakov-action), fix [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl invariance](../../../string-theory.md#weyl-transformation), and perform a [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) of the [string worldsheet](../../../string-theory.md#worldsheet). In complex coordinates, the [worldsheet ghost action](../../../string-theory.md#worldsheet-ghost-action) for the [closed string](../../../string-theory.md#closed-string) is

$$
\boxed{S_{bc}=\frac1{2\pi}\int d^2z\,
\bigl(b_{zz}\bar\partial c^z+\bar b_{\bar z\bar z}\partial\bar c^{\bar z}\bigr).}
$$

The [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field) are anticommuting. Their [conformal weights](../../../string-theory.md#conformal-weight) are $b:(2,0)$, $c:(-1,0)$ and $\bar b:(0,2)$, $\bar c:(0,-1)$. The two chiral sectors are counted separately.

In either chiral sector, each embedding coordinate is a [free boson conformal field theory](../../../string-theory.md#free-boson-conformal-field-theory) with [central charge](../../../string-theory.md#central-charge) one. For the [bc system](../../../string-theory.md#bc-system), putting $J=2$ in $c_{bc}=-2(6J^2-6J+1)$ gives $c_{bc}=-26$. Cancellation of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) requires

$$
\boxed{c_{\mathrm{tot}}=D-26=0,\qquad D=26.}
$$

The antiholomorphic sector gives the same equation, rather than doubling the required [critical dimension of string theory](../../../string-theory.md#critical-dimension-of-string-theory). This dimension count assumes flat target spacetime with just the embedding fields; more general internal [conformal field theories](../../../string-theory.md#conformal-field-theory) change the matter accounting.

For the [spinning string](../../../string-theory.md#spinning-string), the [worldsheet Majorana fermions](../../../string-theory.md#worldsheet-majorana-fermion) have [conformal weight](../../../string-theory.md#conformal-weight) $1/2$. At $J=1/2$, the complex anticommuting [bc system](../../../string-theory.md#bc-system) has $c=1$; a real [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) contributes half of this. Hence $D$ real [worldsheet Majorana fermions](../../../string-theory.md#worldsheet-majorana-fermion) contribute $D/2$ per chiral sector. [Ramond sector](../../../string-theory.md#ramond-sector) versus [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector) changes their mode numbers and vacuum energies, not this local [central charge](../../../string-theory.md#central-charge).

The additional local [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry) has a fermionic gauge parameter, so its [superconformal ghosts](../../../string-theory.md#superconformal-ghost) are commuting fields forming a [beta-gamma system](../../../string-theory.md#beta-gamma-system), with [conformal weights](../../../string-theory.md#conformal-weight) $\beta:3/2$ and $\gamma:-1/2$ in the holomorphic sector. Commuting statistics reverse the sign of the [bc system](../../../string-theory.md#bc-system) formula, giving

$$
c_{\beta\gamma}=2\left(6\left(\frac32\right)^2-6\left(\frac32\right)+1\right)=11.
$$

Together with the reparameterization [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field), their total [central charge](../../../string-theory.md#central-charge) is $-26+11=-15$. Thus

$$
\boxed{c_{\mathrm{tot}}=D+\frac D2-26+11=0,\qquad D=10.}
$$

These cancellations make the [string worldsheet](../../../string-theory.md#worldsheet) gauge symmetries compatible with quantization; in the [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry) formulation they enter the nilpotence condition for the [BRST operator](../../../string-theory.md#brst-operator).

## 4

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [closed string](../../../string-theory.md#closed-string) already contains the particle required for [quantum gravity](../../../quantum-theory.md#quantum-gravity). For [bosonic string theory](../../../string-theory.md#bosonic-string-theory) in its [critical dimension of string theory](../../../string-theory.md#critical-dimension-of-string-theory), the [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) and [closed-string level matching](../../../string-theory.md#closed-string-level-matching) are

$$
M^2=\frac4{\alpha'}(N-1),\qquad N=\widetilde N,
\qquad \alpha'=\frac1{2\pi T}.
$$

At $N=\widetilde N=1$, the states $\epsilon_{mn}\alpha_{-1}^m\widetilde\alpha_{-1}^n|0;k\rangle$ are massless. After imposing the [Virasoro constraints](../../../string-theory.md#virasoro-constraint) and quotienting [null string states](../../../string-theory.md#null-string-state), the transverse [polarization tensor](../../../string-theory.md#polarization-tensor) decomposes into symmetric trace-free, antisymmetric and scalar pieces under $SO(D-2)$. They describe a [graviton](../../../quantum-theory.md#graviton), the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) and the [dilaton](../../../string-theory.md#dilaton). In particular, **the symmetric trace-free sector is a massless spin-two [graviton](../../../quantum-theory.md#graviton)**. Its number of [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) is $D(D-3)/2$.

The [state–operator correspondence](../../../string-theory.md#state-operator-correspondence) associates each [physical string state](../../../string-theory.md#physical-string-state) with a [string vertex operator](../../../string-theory.md#string-vertex-operator). For example, the matter part of a [massless closed-string vertex operator](../../../string-theory.md#massless-closed-string-vertex-operator) is

$$
V_{\epsilon,k}(z,\bar z)=\epsilon_{mn}:\partial X^m\bar\partial X^n e^{ik\cdot X}:,
\qquad k^2=0,\qquad k^m\epsilon_{mn}=k^n\epsilon_{mn}=0.
$$

Its [conformal weights](../../../string-theory.md#conformal-weight) are $(1,1)$, so its integrated form $\int d^2z\,V_{\epsilon,k}$ is invariant under changes of [string worldsheet](../../../string-theory.md#worldsheet) coordinates. At fixed insertion positions it is accompanied by $c\bar c$ from the [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field). Physical vertices represent [BRST cohomology](../../../relativistic-quantum-field.md#brst-cohomology) classes; longitudinal changes of the [polarization tensor](../../../string-theory.md#polarization-tensor) are [BRST-exact operators](../../../relativistic-quantum-field.md#brst-exact-operator) and decouple from physical [scattering amplitudes](../../../quantum-mechanics.md#scattering-amplitude). For the [graviton](../../../quantum-theory.md#graviton), this [string-state gauge redundancy](../../../string-theory.md#string-state-gauge-redundancy) becomes the linearized target-space [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $h_{mn}\mapsto h_{mn}+\partial_m\xi_n+\partial_n\xi_m$.

The [Polyakov path integral](../../../string-theory.md#polyakov-path-integral) computes a [closed-string scattering amplitude](../../../string-theory.md#closed-string-scattering-amplitude) by inserting the external [string vertex operators](../../../string-theory.md#string-vertex-operator), integrating their unfixed positions and the inequivalent [worldsheet moduli](../../../string-theory.md#worldsheet-moduli), and including the [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field). On a [Riemann sphere](../../../complex-analysis.md#riemann-sphere) three positions are fixed by the residual conformal group. For example, contractions of [tachyon vertex operators](../../../string-theory.md#tachyon-vertex-operator) produce the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor), whose position integral gives the [Virasoro–Shapiro amplitude](../../../string-theory.md#virasoro-shapiro-amplitude).

The [string dual resonance](../../../string-theory.md#string-dual-resonance) property means that one [crossing-symmetric scattering amplitude](../../../quantum-mechanics.md#crossing-symmetry) has equivalent expansions in the different channels: its poles exhibit intermediate string states in each channel, rather than separate channel contributions being added again. The [scattering-amplitude factorization](../../../quantum-mechanics.md#scattering-amplitude-factorization) at a [pole](../../../isolated-singularity.md#pole) identifies the intermediate particle and its couplings. Set $8\pi T=1$, so $\alpha'=4$ and the closed-string [tachyon](../../../physics.md#tachyon) has $M^2=-1$. For four such external states the [Mandelstam variables](../../../special-relativity.md#mandelstam-variables) obey $s+t+u=-4$. The [Virasoro–Shapiro amplitude](../../../string-theory.md#virasoro-shapiro-amplitude) has generic $s$-channel [poles](../../../isolated-singularity.md#pole) at $s=-1,0,1,\ldots$, exactly the [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum) in these units.

The massless [pole](../../../isolated-singularity.md#pole) gives an especially direct check. With overall normalization $C$ and $u=-4-s-t$, the [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence) gives

$$
\lim_{s\to0}sA(s,t)
=C\frac{\Gamma(-1-t)\Gamma(3+t)}{\Gamma(-2-t)\Gamma(2+t)}
=-C(t+2)^2.
$$

Thus

$$
\boxed{A(s,t)=-\frac{C(t+2)^2}{s}+O(1)\qquad(s\to0).}
$$

The quadratic [residue](../../../analysis.md#residue) in $t$ contains a spin-two exchange. A scalar exchange alone could not give this angular dependence. Combined with the known massless spectrum and [scattering-amplitude factorization](../../../quantum-mechanics.md#scattering-amplitude-factorization), it identifies exchange of the [graviton](../../../quantum-theory.md#graviton), with possible scalar contributions from the [dilaton](../../../string-theory.md#dilaton); the antisymmetric [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) does not couple to two identical scalar [tachyons](../../../physics.md#tachyon) here. Consequently the [graviton](../../../quantum-theory.md#graviton) participates in interactions, rather than being an isolated free state.

Decoupling longitudinal [graviton](../../../quantum-theory.md#graviton) polarizations forces a universal coupling to the conserved [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor). Consistency of this massless spin-two [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) extends the linearized coupling to the nonlinear dynamics of [general relativity](../../../general-relativity.md). At distances large compared with $\sqrt{\alpha'}$, the gravitational sector of the effective [action](../../../classical-mechanics.md#action) begins with the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action), alongside [dilaton](../../../string-theory.md#dilaton) and [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) terms and higher-derivative string corrections. The infinite tower of string states supplies the short-distance completion of this [quantum gravity](../../../quantum-theory.md#quantum-gravity) expansion.

Interactions are organized by [string worldsheet](../../../string-theory.md#worldsheet) topology. A constant [dilaton](../../../string-theory.md#dilaton) gives the [string coupling](../../../string-theory.md#string-coupling) $g_s=e^{\Phi_0}$, and a connected oriented surface of [genus](../../../topology.md#genus-of-a-surface) $g$ has [Euler characteristic](../../../homology.md#euler-characteristic) $\chi=2-2g$. Its weight is $g_s^{-\chi}$; with $n$ normalized external vertices,

$$
\boxed{\mathcal A_n=\sum_{g=0}^{\infty}g_s^{2g-2+n}\mathcal A_{g,n}.}
$$

The [sphere](../../../geometry-and-topology.md#sphere) is tree order, the [torus](../../../topology.md#torus) is one loop, and each additional handle adds a factor $g_s^2$. Each coefficient is an integral over [worldsheet moduli](../../../string-theory.md#worldsheet-moduli), so this is [string perturbation theory](../../../string-theory.md#string-perturbation-theory) in $g_s$, with an independent low-energy expansion in $\alpha'$.

For the one-loop vacuum contribution, [torus modular invariance](../../../string-theory.md#torus-modular-invariance) identifies $\tau$ with $(a\tau+b)/(c\tau+d)$, $ad-bc=1$. Integration is over the [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group),

$$
\mathcal F=\{\tau=\tau_1+i\tau_2:\ |\tau_1|\leq\tfrac12,\ |\tau|\geq1,\ \tau_2>0\},
\qquad \tau_2\geq\frac{\sqrt3}{2}.
$$

The potential short-proper-time region $\tau_2\to0$, responsible for a point-particle [ultraviolet divergence](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence), is absent. It would count metrics already represented elsewhere in $\mathcal F$. [Torus modular invariance](../../../string-theory.md#torus-modular-invariance) is therefore the geometric reason for one-loop ultraviolet finiteness. More explicitly, in $D=26$ the vacuum integrand is proportional to $d^2\tau\,\tau_2^{-14}|\eta(\tau)|^{-48}$, with $\eta$ the [Dedekind eta function](../../../string-theory.md#dedekind-eta-function); the complete expression is invariant under the [modular group](../../../modular-function.md#modular-group).

**Ultraviolet finiteness does not make the bosonic one-loop vacuum energy finite.** The remaining long-tube region $\tau_2\to\infty$ is an [infrared divergence](../../../quantum-field-theory.md#infrared-divergence) from the [tachyon](../../../physics.md#tachyon): $|\eta(\tau)|^{-48}\sim e^{4\pi\tau_2}$. It signals instability of the bosonic vacuum. Tachyon-free consistent backgrounds remove this particular obstruction, though other infrared effects must still be treated. The ultraviolet improvement comes from the extended string and the complete spectrum together with the worldsheet gauge identifications; the [genus](../../../topology.md#genus-of-a-surface) expansion remains a perturbative description of [quantum gravity](../../../quantum-theory.md#quantum-gravity).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
