# Paper 306

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_306.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_306.pdf)

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
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)
- [4](#4)
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

## 1

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Polyakov action](../../../string-theory.md#polyakov-action) contains the dilaton coupling

$$
S_\Phi=\frac1{4\pi}\int_\Sigma\sqrt h\,\Phi(X)R^{(2)}.
$$

For a constant [dilaton](../../../string-theory.md#dilaton) $\Phi_0$, the [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives $S_\Phi=\Phi_0\chi(\Sigma)$, so the path-integral weight contributes $e^{-\Phi_0\chi}=g_s^{-\chi}$ with [string coupling](../../../string-theory.md#string-coupling) $g_s=e^{\Phi_0}$. A connected closed oriented genus-$g$ worldsheet has $\chi=2-2g$. Including one conventional factor of $g_s$ for each of $n$ external closed-string vertices gives the [string genus expansion](../../../string-theory.md#string-genus-expansion)

$$
\boxed{\mathcal A_{g,n}\propto g_s^{,2g-2+n}}.
$$

For four external states on the sphere, this is $g_s^2$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The quadratic worldsheet action makes each $X^\mu$ a free boson. Its [Green function](../../../analysis.md#green-s-function) in the complex plane inverts the operator in the action and uses $\partial\bar\partial\log|z-w|^2=2\pi\delta^{(2)}(z-w)$ with the corresponding convention. The result is

$$
\boxed{\left\langle X^\mu(z,\bar z)X^\nu(w,\bar w)\right\rangle
=-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2}.
$$

An additive constant is physically irrelevant because it can be absorbed into the zero mode.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Split $X^\mu=x_0^\mu+X'^\mu$. Integrating the constant mode gives [momentum conservation](../../../classical-mechanics.md#momentum-conservation),

$$
\int d^{26}x_0\,e^{ix_0\cdot\sum_i p_i}
\propto\delta^{26}\!\left(\sum_i p_i\right).
$$

For the nonzero modes, [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) and the propagator give

$$
\left\langle\prod_{i=1}^4{}:e^{ip_i\cdot X(z_i)}:\right\rangle
=\exp\!\left[-\sum_{j<k}p_j\cdot p_k
\left\langle X(z_j)X(z_k)\right\rangle\right]
=\prod_{j<k}|z_j-z_k|^{\alpha'p_j\cdot p_k}.
$$

Thus, up to source-independent numerical normalization, the four-point amplitude is

$$
\boxed{
\mathcal A^{(4)}\sim
\frac{g_s^2\delta^{26}(\sum_i p_i)}{\operatorname{Vol}(SL(2,\mathbb C))}
\int\prod_{i=1}^4d^2z_i
\prod_{j<k}|z_j-z_k|^{\alpha'p_j\cdot p_k}}.
$$

The product is the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

For the [Möbius transformation](../../../group-theory.md#mobius-transformation) $z'=(az+b)/(cz+d)$ with $ad-bc=1$,

$$
z_j'-z_k'=\frac{z_j-z_k}{(cz_j+d)(cz_k+d)},
\qquad
d^2z_i'=\frac{d^2z_i}{|cz_i+d|^4}.
$$

The power of $|cz_i+d|$ contributed by every pair containing $i$ is

$$
-\alpha'\sum_{j\ne i}p_i\cdot p_j
=\alpha'p_i^2=4,
$$

where [momentum conservation](../../../classical-mechanics.md#momentum-conservation) and the mass-shell condition $p_i^2=4/\alpha'$ were used. The Koba-Nielsen factor therefore contributes $|cz_i+d|^4$ at each insertion, exactly cancelling the transformed measure. Hence the remaining integral is $SL(2,\mathbb C)$ invariant, and division by its volume removes the residual conformal-gauge redundancy.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Because the [gamma function](../../../complex-analysis.md#gamma-function) has simple poles at the nonpositive integers and no zeros, the $s$-dependent numerator $\Gamma(-\alpha's/4)$ has poles at

$$
-\frac{\alpha's}{4}=-n,
\qquad n=0,1,2,\ldots,
$$

or

$$
\boxed{s=M_n^2=\frac{4n}{\alpha'}}.
$$

Factorization of a scattering amplitude identifies each pole with an intermediate on-shell state. The [Type II superstring mass spectrum](../../../string-theory.md#type-ii-superstring-mass-spectrum) therefore contains a massless level at $n=0$ and an infinite equally spaced tower in squared mass for $n\geq1$. There is no negative-$M^2$ pole, consistently with the absence of a tachyon in [Type II superstring theory](../../../string-theory.md#type-ii-string-theory).

## 2

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The term $\widehat p^{,2}/2$ is the target-space zero-mode kinetic energy. The constant $-1/12$ is the [zero-point energy](../../../quantum-mechanics.md#zero-point-energy) of the left- and right-moving oscillators: each chiral boson contributes $-1/24$. Finally,

$$
\sum_{n\geq1}\alpha_{-n}\alpha_n,
\qquad
\sum_{n\geq1}\widetilde\alpha_{-n}\widetilde\alpha_n
$$

count the energies of the two independent sets of [string oscillators](../../../string-theory.md#string-oscillator); one excitation of mode $n$ has energy $n$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For $n>0$, define occupation numbers $N_n,\widetilde N_n\in\mathbb N_0$. A basis is

$$
\boxed{|p;\{N_n\},\{\widetilde N_n\}\rangle
\propto\prod_{n\geq1}(\alpha_{-n})^{N_n}
(\widetilde\alpha_{-n})^{\widetilde N_n}|p;0,0\rangle},
$$

where $\widehat p|p;0,0\rangle=p|p;0,0\rangle$ and positive oscillator modes annihilate the vacuum. Since $\alpha_{-n}\alpha_n$ has eigenvalue $nN_n$, the simultaneous eigenvalues are

$$
\boxed{H=\frac{p^2}{2}-\frac1{12}
+\sum_{n=1}^\infty n(N_n+\widetilde N_n)},
$$



$$
\boxed{P=\sum_{n=1}^\infty n(\widetilde N_n-N_n)}.
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Put $\tau=\tau_1+i\tau_2$ and $q=e^{2\pi i\tau}$. The torus partition function is the [trace](../../../linear-algebra.md#matrix-trace)

$$
Z(\tau,\bar\tau)=\operatorname{Tr}
e^{-2\pi\tau_2H+2\pi i\tau_1P}.
$$

The continuum momentum states have density $V/(2\pi)$, so their contribution is

$$
\frac V{2\pi}\int_{-\infty}^{\infty}dp\,e^{-\pi\tau_2p^2}
=\frac V{2\pi\sqrt{\tau_2}}.
$$

Each left-moving oscillator contributes $\sum_{N\geq0}q^{nN}=(1-q^n)^{-1}$, with the complex conjugate for the right mover. The zero-point factor combines these products into the [Dedekind eta function](../../../string-theory.md#dedekind-eta-function)

$$
\eta(\tau)=q^{1/24}\prod_{n=1}^{\infty}(1-q^n).
$$

Therefore the [torus partition function of a free boson](../../../string-theory.md#torus-partition-function-of-a-free-boson) is

$$
\boxed{Z(\tau,\bar\tau)=\frac V{2\pi\sqrt{\operatorname{Im}\tau}}
|\eta(\tau)|^{-2}}.
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For a [compact boson](../../../string-theory.md#compact-boson) $X\sim X+2\pi R$, a closed spatial circuit of the worldsheet may wind around the target circle:

$$
\boxed{X(\tau,\sigma+2\pi)=X(\tau,\sigma)+2\pi Rw,
\qquad w\in\mathbb Z}.
$$

Single-valued target-space wavefunctions quantize the zero-mode momentum as $p=n/R$, $n\in\mathbb Z$. In the convention

$$
p_L=\frac nR+wR,
\qquad
p_R=\frac nR-wR,
$$

the Hamiltonian and worldsheet momentum become

$$
\boxed{H=\frac12\left(\frac{n^2}{R^2}+w^2R^2\right)-\frac1{12}
+\sum_{k\geq1}k(N_k+\widetilde N_k)},
$$



$$
\boxed{P=nw+\sum_{k\geq1}k(\widetilde N_k-N_k)}.
$$

The $nw$ term is the zero-mode contribution to [closed-string level matching](../../../string-theory.md#closed-string-level-matching).

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

The momentum integral is replaced by the sum over [momentum and winding modes](../../../string-theory.md#momentum-and-winding-modes). Combining the zero modes with the oscillator trace gives

$$
\boxed{
Z_R(\tau,\bar\tau)=\frac1{|\eta(\tau)|^2}
\sum_{n,w\in\mathbb Z}
\exp\!\left[-\pi\tau_2\left(\frac{n^2}{R^2}+w^2R^2\right)
+2\pi i\tau_1nw\right]}.
$$

Equivalently,

$$
Z_R=\frac1{|\eta|^2}\sum_{n,w}
q^{p_L^2/4}\bar q^{p_R^2/4}
$$

with the left/right convention of part (iv). The answer is invariant under the [T-duality](../../../string-theory.md#t-duality) $R\leftrightarrow1/R$ accompanied by $n\leftrightarrow w$ in these units.

## 3

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

An operator $\mathcal O(w,\bar w)$ is a [primary operator](../../../string-theory.md#primary-field) of [conformal weights](../../../string-theory.md#conformal-weight) $(h,\widetilde h)$ when its OPEs with the stress tensors are

$$
T(z)\mathcal O(w,\bar w)\sim
\frac{h\mathcal O(w,\bar w)}{(z-w)^2}
+\frac{\partial_w\mathcal O(w,\bar w)}{z-w},
$$



$$
\bar T(\bar z)\mathcal O(w,\bar w)\sim
\frac{\widetilde h\mathcal O(w,\bar w)}{(\bar z-\bar w)^2}
+\frac{\partial_{\bar w}\mathcal O(w,\bar w)}{\bar z-\bar w},
$$

with no more singular terms. Its [scaling dimension](../../../string-theory.md#scaling-dimension) and two-dimensional spin are

$$
\boxed{\Delta=h+\widetilde h,
\qquad s=h-\widetilde h}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

[Normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) defines a composite field by subtracting all singular self-contractions before bringing its constituent points together. For example,

$$
{}:\!\partial X\partial X\!:(z)
=\lim_{w\to z}\left[
\partial X(z)\partial X(w)-
\langle\partial X(z)\partial X(w)\rangle\right].
$$

This makes $T$ and $\bar T$ well-defined local operators and is equivalent in oscillator language to placing creation operators to the left of annihilation operators.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Only the fermionic part of $T$ contracts with $\psi$. Applying [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) to $T_\psi(z)=-\tfrac12{}:\!\psi\partial\psi\!:(z)$ and using $\psi(z)\psi(w)\sim1/(z-w)$ gives

$$
T(z)\psi(w)\sim
\frac{\frac12\psi(w)}{(z-w)^2}
+\frac{\partial\psi(w)}{z-w}.
$$

There is no singular OPE with $\bar T(\bar z)$. Thus $\psi$ is a [primary operator](../../../string-theory.md#primary-field) with

$$
\boxed{(h,\widetilde h)=\left(\frac12,0\right)}.
$$

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The holomorphic free boson contributes [central charge](../../../string-theory.md#central-charge) $c_X=1$, while one real chiral free fermion contributes $c_\psi=1/2$. Equivalently, the double contractions in $T(z)T(w)$ give

$$
T(z)T(w)\sim\frac{3/4}{(z-w)^4}
+\frac{2T(w)}{(z-w)^2}+\frac{\partial T(w)}{z-w}.
$$

Since the fourth-order coefficient is $c/2$,

$$
\boxed{c=1+\frac12=\frac32}.
$$

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

The free equations of motion are $\bar\partial\psi=0$ and $\partial\bar\partial X=0$, hence

$$
\bar\partial G=i(\bar\partial\psi)\partial X+i\psi\bar\partial\partial X=0.
$$

Thus the [superconformal current](../../../string-theory.md#superconformal-current) $G=i\psi\partial X$ is holomorphic. Differentiating the boson OPE gives $\partial X(z)\partial X(w)\sim-1/(z-w)^2$. The double contraction in $G(z)G(w)$ is consequently $1/(z-w)^3$, while the single contractions combine into twice the full stress tensor. Therefore

$$
\boxed{G(z)G(w)\sim
\frac1{(z-w)^3}+\frac{2T(w)}{z-w}}.
$$

The leading coefficient equals $2c/3=1$ for $c=3/2$.

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

Extract a mode using

$$
G_m=\oint_0\frac{dz}{2\pi i}\,z^{m+1/2}G(z),
\qquad
L_k=\oint_0\frac{dw}{2\pi i}\,w^{k+1}T(w).
$$

In the radially ordered double contour for the anticommutator, the simple pole $2T(w)/(z-w)$ gives $2L_{m+n}$. Expanding $z^{m+1/2}$ about $w$, the third-order pole contributes one half of its second derivative,

$$
\frac12\left(m+\frac12\right)\left(m-\frac12\right)
w^{m-3/2}.
$$

The remaining contour is nonzero only for $m+n=0$. Restoring the general leading OPE coefficient $2c/3$ gives

$$
\boxed{
\{G_m,G_n\}=2L_{m+n}
+\frac c{12}(4m^2-1)\delta_{m,-n}}.
$$

This is the fermionic relation in the [N=1 super-Virasoro algebra](../../../string-theory.md#n-1-super-virasoro-algebra).

## 4

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

In Euclidean worldsheet signature, the [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model) action can be written

$$
\boxed{
S=\frac1{4\pi\alpha'}\int_\Sigma d^2\sigma\sqrt h\,
\left[h^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+i\epsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\alpha'\Phi(X)R^{(2)}(h)\right]}.
$$

The factor of $i$ in the B-field term is absent in Lorentzian signature. Here $G$ is the target metric, $B$ the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), and $\Phi$ the [dilaton](../../../string-theory.md#dilaton).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The worldsheet metric is a gauge variable, so quantum consistency requires the [Weyl transformation](../../../string-theory.md#weyl-transformation) to remain non-anomalous. The background fields are couplings of a two-dimensional quantum field theory, and their [sigma-model beta functions](../../../string-theory.md#sigma-model-beta-function) multiply the trace of the worldsheet stress tensor. Requiring every beta function to vanish gives, at the first nontrivial order in the derivative or $\alpha'$ expansion, precisely the stated metric, B-field and dilaton equations. They are also the Euler-Lagrange equations of the leading spacetime string-frame effective action

$$
\boxed{S_{\rm eff}\propto\int d^{26}x\sqrt{-G}\,e^{-2\Phi}
\left[R+4(\nabla\Phi)^2-\frac1{12}H^2+O(\alpha')\right].}
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Define the leading right-hand side of the dilaton equation by

$$
C=2\nabla^2\Phi-2(\nabla\Phi)^2+\frac12R-\frac1{24}H^2.
$$

Take a divergence of the metric equation. The contracted [Bianchi identity](../../../fiber-bundle.md#bianchi-identity), commutation of covariant derivatives on $\nabla_\nu\Phi$, the B-field equation $\nabla^\lambda H_{\lambda\mu\nu}=2\nabla^\lambda\Phi H_{\lambda\mu\nu}$, and the supplied H-field identity give

$$
0=\frac12\nabla_\nu R+2\nabla_\nu\nabla^2\Phi
+2R_{\nu\rho}\nabla^\rho\Phi
-\frac12\nabla^\rho\Phi H_{\rho\kappa\lambda}H_\nu{}^{\kappa\lambda}
-\frac1{24}\nabla_\nu H^2.
$$

The metric equation contracted with $\nabla^\rho\Phi$ says

$$
R_{\nu\rho}\nabla^\rho\Phi
=-2\nabla_\nu\nabla_\rho\Phi\nabla^\rho\Phi
+\frac14H_{\nu\kappa\lambda}H_\rho{}^{\kappa\lambda}\nabla^\rho\Phi.
$$

Substitution cancels the curvature, Hessian and H-field terms in $\nabla_\nu C$, leaving

$$
\boxed{\nabla_\nu C=0}.
$$

**Thus $C$ is constant on each connected component. The remaining constant is fixed by the central-charge deficit; it vanishes in the critical 26-dimensional bosonic theory at this order.**

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

First, the displayed equations are only the one-loop [sigma-model beta functions](../../../string-theory.md#sigma-model-beta-function). Higher worldsheet loops generate additional covariant terms with more curvatures, H-fields and derivatives, each accompanied by higher powers of $\alpha'$. Second, string scattering amplitudes contain momentum corrections from the finite string length and from integrating out the infinite tower of massive string states. Their low-energy expansion produces the same higher-derivative spacetime operators, such as curvature-squared and higher-curvature terms. Both arguments require $\alpha'$ corrections even though local field redefinitions can move individual correction terms between equations.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

Let $a=0,\ldots,p$ label directions tangent to the [D-brane](../../../string-theory.md#d-brane) and $i=p+1,\ldots,25$ label transverse directions. The endpoints obey Dirichlet conditions transversely,

$$
\boxed{\delta X^i=0\quad\text{or equivalently}\quad
X^i|_{\partial\Sigma}=x_0^i},
$$

and the boundary variation of the metric and constant B-field terms gives mixed tangential conditions

$$
\boxed{\eta_{ab}\partial_\sigma X^b
+b_{ab}\partial_\tau X^b=0
\quad\text{on }\partial\Sigma},
$$

up to the orientation sign at the two ends. A worldvolume gauge potential contributes $2\pi\alpha'F_{ab}$ in the same place, so the gauge-invariant condition contains $\mathcal F=b+2\pi\alpha'F$.

From the brane perspective, the pullback of the background B-field is therefore indistinguishable locally from a constant worldvolume electromagnetic field strength, modulo its two-form gauge symmetry and a compensating transformation of the brane gauge field. This is the [open-string boundary condition in a B-field](../../../string-theory.md#open-string-boundary-condition-in-a-b-field); sufficiently general constant $b$ also induces the familiar noncommutative deformation of D-brane endpoint coordinates.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
