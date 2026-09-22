# Paper 306

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_306.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_306.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) of each component of the [string embedding map](../../../string-theory.md#string-embedding-map) is the [wave equation](../../../wave-equation.md) $(\partial_\tau^2-\partial_\sigma^2)X^\mu=0$. Its left- and right-moving solutions are identified by the endpoint [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition), so the resulting [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) is

$$
X^\mu(\sigma,\tau)=x^\mu+2\alpha'p^\mu\tau
+i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^\mu}{n}
e^{-in\tau}\cos(n\sigma),
\qquad \alpha_{-n}^\mu=(\alpha_n^\mu)^\dagger.
$$

Indeed, the [Fourier cosine series](../../../fourier-series.md#fourier-cosine-series) makes $\partial_\sigma X^\mu$ vanish at $\sigma=0,\pi$. The canonical momentum density is $\Pi_\mu=(2\pi\alpha')^{-1}\dot X_\mu$. Imposing the equal-time [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) $[X^\mu(\sigma),\Pi_\nu(\sigma')]=i\delta^\mu_\nu\delta(\sigma-\sigma')$ gives the [covariant quantization of the bosonic string](../../../string-theory.md#covariant-quantization-of-the-bosonic-string)

$$
[x^\mu,p^\nu]=i\eta^{\mu\nu},
\qquad
[\alpha_m^\mu,\alpha_n^\nu]=m\,\delta_{m+n,0}\eta^{\mu\nu},
\qquad
[x,x]=[p,p]=0,
$$

with $\alpha_0^\mu=\sqrt{2\alpha'}p^\mu$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

An infinitesimal [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) is $\delta X^\mu=\omega^\mu{}_{\nu}X^\nu$ with $\omega_{\mu\nu}=-\omega_{\nu\mu}$. Applying [Noether theorem](../../../calculus-of-variations.md#noether-theorem) to this continuous symmetry gives the conserved [Lorentz current](../../../quantum-field-theory.md#lorentz-current)

$$
J_\alpha^{\mu\nu}=\frac1{2\pi\alpha'}
\left(X^\mu\partial_\alpha X^\nu-X^\nu\partial_\alpha X^\mu\right),
\qquad \partial^\alpha J_\alpha^{\mu\nu}=0.
$$

Its [Noether charge](../../../quantum-field-theory.md#noether-charge) is $M^{\mu\nu}=\int_0^\pi d\sigma\,J_\tau^{\mu\nu}$. Substituting the [open-string mode expansion](../../../string-theory.md#open-string-mode-expansion) and using [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the cosine modes yields

$$
M^{\mu\nu}=x^\mu p^\nu-x^\nu p^\mu
-i\sum_{n=1}^{\infty}\frac1n
\left(\alpha_{-n}^\mu\alpha_n^\nu-
\alpha_{-n}^\nu\alpha_n^\mu\right).
$$

The first term is orbital angular momentum; the sum is the contribution of the [string oscillators](../../../string-theory.md#string-oscillator).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

It is cleaner to use the action of the charge than to expand every double sum. The commutators from part a give, for $v^\rho=x^\rho,p^\rho$, or any $\alpha_n^\rho$,

$$
[M^{\mu\nu},v^\rho]
=i\left(\eta^{\mu\rho}v^\nu-\eta^{\nu\rho}v^\mu\right).
$$

Thus $M^{\mu\nu}$ acts on every mode in the [vector representation](../../../representation-theory.md#vector-representation) of the [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra). Apply the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) to the action of $[M^{\mu\nu},M^{\kappa\lambda}]$ on every mode. The result agrees with the action of

$$
i\left(\eta^{\mu\kappa}M^{\nu\lambda}-\eta^{\nu\kappa}M^{\mu\lambda}
+\eta^{\nu\lambda}M^{\mu\kappa}-\eta^{\mu\lambda}M^{\nu\kappa}\right).
$$

There is no extra scalar term: the orbital and oscillator pieces commute with one another, and direct use of their [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) gives no central contribution. Hence the displayed operators obey precisely the standard [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra).

## 2

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The universal [stress-tensor operator-product expansion](../../../string-theory.md#stress-tensor-operator-product-expansion) in a [two-dimensional conformal field theory](../../../string-theory.md#two-dimensional-conformal-field-theory) is

$$
T(z)T(w)\sim
\frac{c/2}{(z-w)^4}
+\frac{2T(w)}{(z-w)^2}
+\frac{\partial T(w)}{z-w}.
$$

Its fourth-order coefficient defines the [central charge](../../../string-theory.md#central-charge) $c$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Differentiating $X(z)X(w)\sim-(\alpha'/2)\log(z-w)$ gives the contractions needed for [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem). The free-boson part of $T$ supplies $1/[2(z-w)^4]$, corresponding to [central charge](../../../string-theory.md#central-charge) one. The cross-contractions between $:\!\partial X\partial X\!:$ and $\partial^2X$ produce the required lower poles but no fourth-order scalar term. Finally,

$$
\partial_z^2\partial_w^2\left[-\frac{\alpha'}2\log(z-w)\right]
=\frac{3\alpha'}{(z-w)^4},
$$

so the product of the two improvement terms contributes $3\alpha'q^2/(z-w)^4$. Matching this with $c/[2(z-w)^4]$ in the [stress-tensor operator-product expansion](../../../string-theory.md#stress-tensor-operator-product-expansion) gives the [linear dilaton conformal field theory](../../../string-theory.md#linear-dilaton-conformal-field-theory)

$$
\boxed{c=1+6\alpha'q^2}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The first term of the action is the [free boson conformal field theory](../../../string-theory.md#free-boson-conformal-field-theory). For the curvature coupling, insert the supplied [first variation](../../../calculus-of-variations.md#first-variation) of $\sqrt gR^{(2)}$, integrate by parts twice and discard the boundary term. Its metric variation is the stress-tensor improvement

$$
-q\left(\nabla_\alpha\nabla_\beta X-g_{\alpha\beta}\nabla^2X\right)
$$

in the conventions of the question. In a locally flat complex coordinate, the holomorphic component of the complete [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) is therefore

$$
T(z)=-\frac1{\alpha'}:\!\partial X\partial X\!:(z)-q:\!\partial^2X\!:(z),
$$

as required. Thus the coupling $q\int\sqrt g\,XR^{(2)}$ makes $X$ a [background-charge scalar field](../../../string-theory.md#background-charge-scalar-field), equivalently a worldsheet coordinate in a [linear dilaton conformal field theory](../../../string-theory.md#linear-dilaton-conformal-field-theory).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take $D$ embedding coordinates and give one coordinate the background charge $q$. The remaining $D-1$ free bosons contribute $D-1$, while the distinguished coordinate contributes $1+6\alpha'q^2$, so the matter [central charge](../../../string-theory.md#central-charge) is

$$
c_{\rm matter}=D+6\alpha'q^2.
$$

The [worldsheet ghosts](../../../string-theory.md#worldsheet-ghost-field) contributes $-26$. Cancellation of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) therefore requires

$$
\boxed{q^2=\frac{26-D}{6\alpha'}},
$$

which is real for $D<26$ and produces a noncritical bosonic string.

In target-space language the [dilaton](../../../string-theory.md#dilaton) is linear in this coordinate, so the local [string coupling](../../../string-theory.md#string-coupling) $g_s=e^\Phi$ changes exponentially. One end of the target direction is weakly coupled and the other is strongly coupled. Consequently [string perturbation theory](../../../string-theory.md#string-perturbation-theory) is trustworthy only in the weak-coupling region, rather than throughout the full background.

## 3

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A local operator $\mathcal O(w,\bar w)$ is a [primary operator](../../../string-theory.md#primary-field) of [conformal weights](../../../string-theory.md#conformal-weight) $(h,\widetilde h)$ when its [operator product expansions](../../../string-theory.md#operator-product-expansion) with the holomorphic and antiholomorphic stress tensors are

$$
T(z)\mathcal O(w,\bar w)\sim
\frac{h\mathcal O(w,\bar w)}{(z-w)^2}
+\frac{\partial\mathcal O(w,\bar w)}{z-w},
$$



$$
\bar T(\bar z)\mathcal O(w,\bar w)\sim
\frac{\widetilde h\mathcal O(w,\bar w)}{(\bar z-\bar w)^2}
+\frac{\bar\partial\mathcal O(w,\bar w)}{\bar z-\bar w},
$$

with no more singular poles. Equivalently, under a local [conformal transformation](../../../geometry-and-topology.md#conformal-map) it transforms covariantly with holomorphic exponent $h$ and antiholomorphic exponent $\widetilde h$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let

$$
V=\epsilon_{\mu\nu}:\!\partial X^\mu\bar\partial X^\nu e^{ik\cdot X}\!:.
$$

The exponential is a [primary operator](../../../string-theory.md#primary-field) with [conformal weights](../../../string-theory.md#conformal-weight) $(\alpha'k^2/4,\alpha'k^2/4)$. In the $T(z)V(w,\bar w)$ OPE, contracting one derivative in $T$ with $\partial X^\mu$ and the other with the exponential produces a third-order pole proportional to $k^\mu\epsilon_{\mu\nu}$. Its antiholomorphic counterpart is proportional to $\epsilon_{\mu\nu}k^\nu$. Therefore $V$ is primary exactly when its [polarization tensor](../../../string-theory.md#polarization-tensor) is transverse in both indices,

$$
\boxed{k^\mu\epsilon_{\mu\nu}=0,
\qquad \epsilon_{\mu\nu}k^\nu=0}.
$$

The remaining second-order poles give

$$
\boxed{(h,\widetilde h)=
\left(1+\frac{\alpha'k^2}{4},
1+\frac{\alpha'k^2}{4}\right)}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The matter part of the [massless closed-string vertex operator](../../../string-theory.md#massless-closed-string-vertex-operator) is

$$
V_\epsilon=\epsilon_{\mu\nu}:\!\partial X^\mu\bar\partial X^\nu e^{ik\cdot X}\!:,
\qquad k^2=0,
\qquad k^\mu\epsilon_{\mu\nu}=\epsilon_{\mu\nu}k^\nu=0.
$$

Its symmetric trace-free polarization is the graviton, while its antisymmetric polarization is the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), or B-field. The [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) $k^2=0$ and transversality make $V_\epsilon$ a [primary operator](../../../string-theory.md#primary-field) of [conformal weights](../../../string-theory.md#conformal-weight) $(1,1)$, as required for an [integrated string vertex operator](../../../string-theory.md#integrated-string-vertex-operator).

The graviton polarization has the linearized [gauge redundancy](../../../relativistic-quantum-field.md#gauge-redundancy)

$$
\epsilon_{\mu\nu}\sim\epsilon_{\mu\nu}+k_\mu\xi_\nu+k_\nu\xi_\mu,
$$

while the antisymmetric polarization obeys

$$
\epsilon_{\mu\nu}\sim\epsilon_{\mu\nu}+k_\mu\Lambda_\nu-k_\nu\Lambda_\mu.
$$

In either case the change in the integrated vertex is a worldsheet [total derivative](../../../calculus.md#total-derivative), hence vanishes on a closed worldsheet; in covariant language it is [BRST-exact](../../../relativistic-quantum-field.md#brst-cohomology). This [string-state gauge redundancy](../../../string-theory.md#string-state-gauge-redundancy) is the vertex-operator form of linearized target-space diffeomorphism or two-form gauge invariance.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $E_{\mu\nu}=\eta_{\mu\nu}$, transversality would require $k^\mu\eta_{\mu\nu}=k_\nu=0$. Hence the operator has a third-order stress-tensor pole and is not a [primary operator](../../../string-theory.md#primary-field) for any nonzero $k$.

For

$$
E_{\mu\nu}=\eta_{\mu\nu}+\xi_\mu k_\nu+k_\mu\xi_\nu,
$$

the two transversality conditions coincide and reduce to

$$
\boxed{k^2\xi_\nu+(1+k\cdot\xi)k_\nu=0}.
$$

If $k^2=0$, this says $k\cdot\xi=-1$, with arbitrary additional component transverse to $k$. If $k^2\ne0$, it forces

$$
\boxed{\xi_\mu=-\frac{k_\mu}{2k^2}},
$$

so $E_{\mu\nu}=\eta_{\mu\nu}-k_\mu k_\nu/k^2$ is the [transverse projection operator](../../../linear-algebra.md#transverse-projection-operator). Once this condition removes the third-order poles, the [conformal weights](../../../string-theory.md#conformal-weight) are again $(1+\alpha'k^2/4,1+\alpha'k^2/4)$; in the null case they are $(1,1)$.

## 4

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The target metric is a coupling of the [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model). Quantum consistency requires the gauge-fixed worldsheet theory to preserve [Weyl invariance](../../../string-theory.md#weyl-transformation), so its [sigma-model beta functions](../../../string-theory.md#sigma-model-beta-function) must vanish. With no B-field or varying dilaton, the metric beta function begins as

$$
\beta^G_{\mu\nu}=\alpha'R_{\mu\nu}+O(\alpha'^2).
$$

Therefore vanishing of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) requires

$$
\boxed{R_{\mu\nu}=0}
$$

to leading order in $\alpha'$: the target-space metric must be Ricci-flat at this order.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The $p$-dependent part of the first-order action can be completed to a square:

$$
\pi\alpha'V^{-1}p^\alpha p_\alpha+i p^\alpha\partial_\alpha Z
=\pi\alpha'V^{-1}
\left(p^\alpha+\frac{iV}{2\pi\alpha'}\partial^\alpha Z\right)
\left(p_\alpha+\frac{iV}{2\pi\alpha'}\partial_\alpha Z\right)
+\frac{V}{4\pi\alpha'}\partial^\alpha Z\partial_\alpha Z.
$$

The [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) over $p$ therefore leaves

$$
S_{\rm eff}[Y,Z]=\frac1{4\pi\alpha'}\int d^2\sigma
\left(G_{ij}(Y)\partial^\alpha Y^i\partial_\alpha Y^j
+V(Y)\partial^\alpha Z\partial_\alpha Z\right),
$$

after the stipulated omission of its [functional determinant](../../../quantum-field-theory.md#functional-determinant). Identifying $X^\mu=(Y^i,Z)$ gives exactly $S_1[X]$, establishing the classical equivalence.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Integrating by parts makes the $Z$ dependence $-i\int Z\,\partial_\alpha p^\alpha$. Its [functional integral](../../../quantum-field-theory.md#functional-measure) imposes the constraint $\partial_\alpha p^\alpha=0$. On the simply connected plane, the [Poincaré lemma](../../../differential-form.md#poincare-lemma) therefore permits the local and global parametrization

$$
p^\alpha=\frac1{2\pi\alpha'}\epsilon^{\alpha\beta}\partial_\beta\widetilde Z.
$$

Substitution into $S_2$ gives

$$
S_{\rm dual}[Y,\widetilde Z]
=\frac1{4\pi\alpha'}\int d^2\sigma
\left(G_{ij}(Y)\partial^\alpha Y^i\partial_\alpha Y^j
+V(Y)^{-1}\partial^\alpha\widetilde Z\partial_\alpha\widetilde Z\right).
$$

This is the [Buscher procedure](../../../string-theory.md#buscher-procedure) for the translation isometry in $z$, and its [T-duality](../../../string-theory.md#t-duality) replaces $G_{zz}=V$ by $\widetilde G_{\widetilde z\widetilde z}=V^{-1}$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The classical elimination in parts b and c discarded the field-dependent [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) determinant. At one loop that determinant is a local curvature coupling and supplies the [Buscher rules](../../../string-theory.md#buscher-rules) dilaton shift

$$
\boxed{\widetilde\Phi=\Phi-\frac12\log V}.
$$

The metric alone consequently need not obey $\widetilde R_{\mu\nu}=0$. The relevant leading [sigma-model beta function](../../../string-theory.md#sigma-model-beta-function) in the dual background instead contains

$$
\beta^{\widetilde G}_{\mu\nu}
=\alpha'\left(\widetilde R_{\mu\nu}
+2\widetilde\nabla_\mu\widetilde\nabla_\nu\widetilde\Phi\right)+\cdots.
$$

The new dilaton term cancels the failure of the dual metric to be Ricci-flat, so the complete metric-dilaton background remains conformal and physically [T-dual](../../../string-theory.md#t-duality) to the original one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
