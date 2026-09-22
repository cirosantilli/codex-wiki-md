# Paper 307

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_307.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_307.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [ii](#2/ii-2)
    - [Solution](#2/ii-2/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [N = 1 quotient metric](#2/n-1-quotient-metric)
    - [Solution](#2/n-1-quotient-metric/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [ii](#3/ii-2)
    - [Solution](#3/ii-2/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
  - [vi](#4/vi)
    - [Solution](#4/vi/solution)
  - [vii](#4/vii)
    - [Solution](#4/vii/solution)

## 1

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Kähler potential](../../../supersymmetry.md#kahler-potential) $K(\Phi,\Phi^\dagger)$ is a real function integrated over all four fermionic coordinates, $\int d^4\theta\,K$. Its complex Hessian gives the scalar [Kähler metric](../../../complex-geometry.md#kahler-metric) and therefore the kinetic terms. The [superpotential](../../../supersymmetry.md#superpotential) $W(\Phi)$ is holomorphic and is integrated over chiral superspace, $\int d^2\theta\,W+\mathrm{h.c.}$; its derivatives determine Yukawa couplings and the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential).

For the canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) $K=\Phi^\dagger\Phi$, extracting the $\theta^2\bar\theta^2$ component of the supplied [chiral-superfield component expansion](../../../supersymmetry.md#chiral-superfield-component-expansion) and integrating by parts gives the bosonic action

$$
\int d^4x\,d^4\theta\,\Phi^\dagger\Phi
=\int d^4x\left(-\partial_\mu\phi^*\partial^\mu\phi+F^*F\right),
$$

in the mostly-plus convention. Extracting the $\theta^2$ component of a holomorphic function gives

$$
\int d^4x\,d^2\theta\,W(\Phi)
=\int d^4x\left(FW'(\phi)-\frac12W''(\phi)\psi\psi\right),
$$

so its bosonic term is $FW'(\phi)$, with the Hermitian conjugate understood in a real action. For several fields, eliminating each algebraic [auxiliary field](../../../supersymmetry.md#auxiliary-field) by $F_i^*=-W_i$ produces $V_F=\sum_i|W_i|^2$.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For $W=X^2Z$, the [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential) is

$$
V=|W_X|^2+|W_Z|^2
=4|X|^2|Z|^2+|X|^4.
$$

Both terms vanish exactly when $X=0$, while $Z$ is arbitrary. Thus the [supersymmetric vacua](../../../supersymmetry.md#supersymmetric-vacuum) form one complex line,

$$
\boxed{X=0,\qquad Z\in\mathbb C,\qquad V_{\rm vac}=0}.
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For $W=XYZ$,

$$
V=|YZ|^2+|XZ|^2+|XY|^2.
$$

The [F-flatness](../../../supersymmetry.md#f-flatness) equations require at least two of $X,Y,Z$ to vanish. The [vacuum space](../../../supersymmetry.md#vacuum-moduli-space-of-a-supersymmetric-gauge-theory) is therefore the union of the three coordinate axes in $\mathbb C^3$,

$$
\boxed{\{Y=Z=0\}\cup\{X=Z=0\}\cup\{X=Y=0\}},
$$

and every point on it has zero vacuum energy.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For

$$
W=\alpha Y+\beta YX^2+\gamma XZ,
$$

the three F-terms are

$$
W_X=2\beta XY+\gamma Z,
\qquad W_Y=\alpha+\beta X^2,
\qquad W_Z=\gamma X.
$$

The equation $W_Z=0$ forces $X=0$, after which $W_Y=\alpha\ne0$; hence no [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) exists. Minimizing over $Z$ sets $Z=-2\beta XY/\gamma$, leaving

$$
V(X)=|\alpha+\beta X^2|^2+|\gamma X|^2.
$$

The two real quadratic eigenvalues about $X=0$ are $|\gamma|^2\pm2|\alpha\beta|$, so the stated hierarchy makes $X=0$ stable. The vacua are

$$
\boxed{X=Z=0,\qquad Y\text{ arbitrary},\qquad V_{\rm vac}=|\alpha|^2}.
$$

This is an [O'Raifeartaigh model](../../../supersymmetry.md#o-raifeartaigh-model): supersymmetry is spontaneously broken and $Y$ is a classical [pseudomodulus](../../../supersymmetry.md#pseudomodulus).

## 2

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write the scalar components as $\phi_i,\widetilde\phi_i,x$. The [superpotential](../../../supersymmetry.md#superpotential) gives

$$
W_x=\sum_i\widetilde\phi_i\phi_i,
\qquad W_{\phi_i}=\widetilde\phi_i(x-m_i),
\qquad W_{\widetilde\phi_i}=(x-m_i)\phi_i.
$$

Choosing the sign of the [Fayet–Iliopoulos term](../../../supersymmetry.md#fayet-iliopoulos-term) so that positive $\zeta$ favors the positively charged fields, the full [Supersymmetric quantum electrodynamics](../../../supersymmetry.md#supersymmetric-quantum-electrodynamics) potential is

$$
\boxed{
V=\sum_i|x-m_i|^2\left(|\phi_i|^2+|\widetilde\phi_i|^2\right)
+\left|\sum_i\widetilde\phi_i\phi_i\right|^2
+\frac{g^2}{2}\left(\sum_i|\phi_i|^2-\sum_i|\widetilde\phi_i|^2-\zeta\right)^2}.
$$

Changing the FI sign convention exchanges $\phi$ with $\widetilde\phi$ in the descriptions below.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $m_i=0$ and first take $\zeta>0$. The mass terms and [D-flatness](../../../supersymmetry.md#d-flatness) require $x=0$ and $\sum_i|\phi_i|^2-\sum_i|\widetilde\phi_i|^2=\zeta$, while [F-flatness](../../../supersymmetry.md#f-flatness) adds $\sum_i\widetilde\phi_i\phi_i=0$. Dividing by the U(1) gauge action gives the [Higgs branch](../../../supersymmetry.md#higgs-branch)

$$
\boxed{\mathcal M_H=T^*\mathbb {CP}^{N-1}},
$$

with complex dimension $2N-2$. For $\zeta<0$, the same result follows after exchanging $\phi$ and $\widetilde\phi$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Suppose $\zeta>0$ and all $m_i$ are distinct. A nonzero $\phi_j$ forces $x=m_j$. Distinctness then makes every other charged field vanish, and $\sum_i\widetilde\phi_i\phi_i=0$ forces $\widetilde\phi_j=0$. The [D-flatness](../../../supersymmetry.md#d-flatness) equation fixes $|\phi_j|^2=\zeta$, while its phase is removed by the gauge group. There is therefore one isolated [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) for each flavor,

$$
\boxed{x=m_j,\quad |\phi_j|^2=\zeta,\quad
\widetilde\phi_j=0,\qquad j=1,\ldots,N},
$$

for a total of $N$ vacua. Negative $\zeta$ gives the analogous vacua with $\widetilde\phi_j$ nonzero.

<h3 id="2/ii-2">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii-2/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii-2)

For $\zeta=0$ and distinct masses, any nonzero charged field can occur only at one $x=m_j$. At such a point, [D-flatness](../../../supersymmetry.md#d-flatness) gives $|\phi_j|=|\widetilde\phi_j|$, whereas [F-flatness](../../../supersymmetry.md#f-flatness) gives $\widetilde\phi_j\phi_j=0$; together they force both fields to vanish. Thus only the [Coulomb branch](../../../supersymmetry.md#coulomb-branch) remains,

$$
\boxed{\phi_i=\widetilde\phi_i=0,\qquad x\in\mathbb C},
$$

of complex dimension one. The points $x=m_i$ are special because the corresponding charged multiplets become massless there.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

When every $m_i$ and $\zeta$ vanishes, the [Coulomb branch](../../../supersymmetry.md#coulomb-branch) again has $\phi_i=\widetilde\phi_i=0$ and arbitrary $x$. A [Higgs branch](../../../supersymmetry.md#higgs-branch) also occurs at $x=0$: it is the zero-level quotient of

$$
\sum_i\widetilde\phi_i\phi_i=0,
\qquad
\sum_i|\phi_i|^2-\sum_i|\widetilde\phi_i|^2=0
$$

by U(1), and has complex dimension $2N-2$ for $N>1$. The two branches meet at the origin. For $N=1$, the F- and D-flat equations force both charged fields to vanish, so the Higgs branch collapses to that intersection point.

<h3 id="2/n-1-quotient-metric">N = 1 quotient metric</h3>

↑ **Parent:** [2](#2)

<h4 id="2/n-1-quotient-metric/solution">Solution</h4>

↑ **Parent:** [N = 1 quotient metric](#2/n-1-quotient-metric)

There is a conflict in the printed question: with dynamical $X$ and the displayed [superpotential](../../../supersymmetry.md#superpotential), $F_X=\widetilde\phi\phi=M$ forces $M=0$, so the $N=1$ theory has no vacuum branch parametrized by nonzero $M$. The natural intended calculation is the [Kähler quotient](../../../complex-geometry.md#kahler-quotient) of the $N=1$ D-flat SQED matter fields before imposing that extra F-term.

On this quotient, $|\phi|=|\widetilde\phi|$ and the gauge-invariant coordinate is $M=\widetilde\phi\phi$. Hence $|\phi|^2=|\widetilde\phi|^2=|M|$, and the canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) descends to

$$
\boxed{K(M,\overline M)=2\sqrt{M\overline M}=2|M|}.
$$

The associated [Kähler metric](../../../complex-geometry.md#kahler-metric) is

$$
\boxed{g_{M\overline M}=\partial_M\partial_{\overline M}K
=\frac1{2|M|}}.
$$

It is smooth for $M\ne0$ and has a conical singularity at $M=0$, locally $\mathbb C/\mathbb Z_2$. Physically, the charged fields become massless and the U(1) gauge symmetry is restored there, so integrating out the vector multiplet to obtain a sigma-model metric ceases to be valid.

## 3

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The transformation of the [holomorphic strong-coupling scale](../../../supersymmetry.md#holomorphic-strong-coupling-scale) is fixed by the mixed $SU(2)^2U(1)$ anomaly. The baryon-number contributions of $\Phi$ and $\widetilde\Phi$ cancel, so $\Lambda^{b_0}$ is neutral under $U(1)_B$. Under $U(1)_A$, all $2N_f$ doublets have charge one and [Dynkin index](../../../semisimple-lie-algebra.md#dynkin-index) one, giving axial charge $2N_f$. For the [R-symmetry](../../../supersymmetry.md#r-symmetry), each matter fermion has charge $(1-2/N_f)-1=-2/N_f$, so the matter contribution is $-4$; the gaugino has R-charge one and contributes $I(\mathrm{adj})=4$, giving zero total anomaly. Thus

$$
\boxed{
\begin{array}{c|ccc}
&U(1)_B&U(1)_A&U(1)_R\\ \hline
\Lambda^{6-N_f}&0&2N_f&0
\end{array}}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For $N_f=1$, antisymmetry makes the would-be baryons vanish, and the only generator of the [chiral ring of a supersymmetric gauge theory](../../../supersymmetry.md#chiral-ring-of-a-supersymmetric-gauge-theory) is the [meson operator in supersymmetric quantum chromodynamics](../../../supersymmetry.md#meson-operator-in-supersymmetric-quantum-chromodynamics) $M=\widetilde\Phi\Phi$. It obeys no classical constraint. Holomorphy, mass dimension and all three U(1) charges uniquely permit the [Affleck–Dine–Seiberg superpotential](../../../supersymmetry.md#affleck-dine-seiberg-superpotential)

$$
\boxed{W_{\rm dyn}=\frac{\Lambda^5}{M}}
$$

up to a nonzero constant absorbed into $\Lambda$. Since $\partial_MW=-\Lambda^5/M^2$ never vanishes at finite $M$, there is no finite supersymmetric ground state. Instead the potential approaches zero as $|M|\to\infty$: the theory has a supersymmetric runaway vacuum at infinity.

<h3 id="3/ii-2">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii-2/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii-2)

For $N_f=2$, the gauge-invariant chiral fields are the four mesons $M_i{}^j=\widetilde\Phi_i\Phi^j$ and the baryons

$$
B=\epsilon_{ab}\Phi_1^a\Phi_2^b,
\qquad
\widetilde B=\epsilon^{ab}\widetilde\Phi_{1a}\widetilde\Phi_{2b}.
$$

Classically they obey

$$
\boxed{\det M-B\widetilde B=0}
$$

up to the sign chosen in the definitions. No ordinary superpotential has the required R-charge. Nonperturbative dynamics instead produces the [quantum-deformed moduli space](../../../supersymmetry.md#quantum-deformed-moduli-space)

$$
\boxed{\det M-B\widetilde B=\Lambda^4}.
$$

The right-hand side has exactly the axial charge, dimension and other symmetry properties required to deform the classical relation.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For $N_f=3$, the infrared fields at the origin are the nine mesons $M_i{}^j$ and three baryons plus three antibaryons, for fifteen chiral multiplets. Every elementary quark superfield has R-charge $1/3$, so its fermion has charge $-2/3$. In the ultraviolet there are twelve quark Weyl fermions and three adjoint gauginos. Hence the two [anomalies](../../../relativistic-quantum-field.md#t-hooft-anomaly) are

$$
\operatorname{Tr}R=3+12\left(-\frac23\right)=-5,
$$



$$
\operatorname{Tr}R^3=3+12\left(-\frac23\right)^3=-\frac59.
$$

Each meson or baryon superfield contains two quarks and has R-charge $2/3$, so each composite fermion has charge $-1/3$. The unconstrained infrared fields therefore give

$$
\operatorname{Tr}R=15\left(-\frac13\right)=-5,
\qquad
\operatorname{Tr}R^3=15\left(-\frac13\right)^3=-\frac59.
$$

Both results agree, establishing the requested ['t Hooft anomaly matching](../../../relativistic-quantum-field.md#t-hooft-anomaly-matching). This smooth composite description is the $SU(2)$, $N_f=3$ example of [s-confinement](../../../supersymmetry.md#s-confinement).

## 4

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Two theories are [Seiberg duals](../../../supersymmetry.md#seiberg-duality) when they are distinct ultraviolet gauge theories that flow to the same infrared quantum field theory. Their gauge-invariant operator spectra, global symmetries, ['t Hooft anomalies](../../../relativistic-quantum-field.md#t-hooft-anomaly) and responses to deformations agree, even though one description may be strongly coupled where the other is weakly coupled.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Quantum consistency requires cancellation of the $SU(N)^3$ [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly). The two-index [symmetric square](../../../linear-algebra.md#symmetric-square) has [cubic anomaly coefficient](../../../semisimple-lie-algebra.md#cubic-anomaly-coefficient) $A(S)=N+4$, whereas each antifundamental has coefficient $-1$. Therefore

$$
\boxed{p=N+4}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The mixed $SU(N)^2U(1)_R$ anomaly receives $I(\mathrm{adj})=2N$ from the gaugino. A chiral multiplet of R-charge $r$ contains a fermion of charge $r-1$. With

$$
R[S]=\frac{2-N}{N+2},
\qquad R[\widetilde\Phi]=1,
$$

the symmetric-tensor fermion contributes

$$
I(S)(R[S]-1)
=(N+2)\left(\frac{2-N}{N+2}-1\right)=-2N,
$$

while every antifundamental fermion contributes zero. The total is $2N-2N=0$, so this is a nonanomalous [R-symmetry](../../../supersymmetry.md#r-symmetry) of the quantum theory.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Using the supplied [Dynkin indices](../../../semisimple-lie-algebra.md#dynkin-index) and $p=N+4$, the [one-loop beta function of a supersymmetric gauge theory](../../../supersymmetry.md#one-loop-beta-function-of-a-supersymmetric-gauge-theory) is

$$
b_0=\frac32(2N)-\frac12\left[(N+2)+p\right]
=3N-\frac12(2N+6)=2N-3.
$$

**Thus $b_0>0$ for every nontrivial $SU(N)$ in this family, and the electric theory is [asymptotically free](../../../perturbative-quantum-field-theory.md#asymptotic-freedom).**

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

In the proposed Spin(8) theory, the gaugino contributes $I(\mathrm{adj})=6$ to the mixed gauge-R anomaly. The $p$ fields $q$ have superfield R-charge one, so their fermions contribute zero. The spinor $t$ has fermion R-charge $-5-1=-6$ and index one, giving $-6$. The singlets $M$ and $U$ do not enter the gauge anomaly. Hence

$$
\boxed{\mathcal A_{\operatorname{Spin}(8)^2U(1)_R}=6-6=0},
$$

and the proposed [R-symmetry](../../../supersymmetry.md#r-symmetry) survives quantization.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

Gauge invariance, $SU(p)$ flavor symmetry and R-charge two permit

$$
\boxed{W=M^{ij}q_iq_j+Utt},
$$

with the Spin(8) vector and spinor indices contracted by their invariant bilinear forms. Indeed, $R[Mqq]=0+1+1=2$ and $R[Utt]=12-5-5=2$. Powers of the matching scale can be inserted to give fields whichever canonical mass dimensions are chosen.

<h3 id="4/vi">vi</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#4/vi)

Only the $p$ Spin(8) vectors $q$ and the one spinor $t$ contribute to the magnetic gauge beta function. The supplied indices give

$$
b_0^{\rm magnetic}
=\frac32(6)-\frac12(p+1)
=\frac{17-p}{2}=\frac{13-N}{2}.
$$

The magnetic theory is infrared free when $b_0^{\rm magnetic}<0$, namely

$$
\boxed{N>13}.
$$

At $N=13$ the one-loop coefficient vanishes and higher-order dynamics decides the flow. For $N>13$, [Seiberg duality](../../../supersymmetry.md#seiberg-duality) says that the strongly coupled low-energy limit of the asymptotically free electric $SU(N)$ theory is described by the weakly coupled Spin(8) fields and the superpotential from part v.

<h3 id="4/vii">vii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#4/vii)

Choose the flavor orientation in which each electric $\widetilde\Phi$ is a fundamental of $SU(p)$. Its $N$ color components then give

$$
\mathcal A^{\rm electric}_{SU(p)^3}=N.
$$

In the magnetic theory, the eight Spin(8) components of $q$ transform in the antifundamental and contribute $-8$. The singlet $M$ transforms in the symmetric representation of $SU(p)$, whose [cubic anomaly coefficient](../../../semisimple-lie-algebra.md#cubic-anomaly-coefficient) is $p+4$, while $t$ and $U$ are flavor singlets. Therefore

$$
\mathcal A^{\rm magnetic}_{SU(p)^3}=-8+(p+4)=p-4=N,
$$

where $p=N+4$ was used. The two $SU(p)^3$ ['t Hooft anomalies](../../../relativistic-quantum-field.md#t-hooft-anomaly) match, as required by [Seiberg duality](../../../supersymmetry.md#seiberg-duality).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
