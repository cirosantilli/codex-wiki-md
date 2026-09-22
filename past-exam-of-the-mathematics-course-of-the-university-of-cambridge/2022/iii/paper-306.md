# Paper 306

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_306.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_306.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
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
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) of the gauge-fixed [Polyakov action](../../../string-theory.md#polyakov-action) is the two-dimensional wave equation

$$
(\partial_\tau^2-\partial_\sigma^2)X^\mu=0.
$$

Its general solution is a sum of left- and right-moving functions. Periodicity in $\sigma$ and a Fourier expansion give the [closed-string mode expansion](../../../string-theory.md#closed-string-mode-expansion)

$$
X^\mu=x^\mu+\alpha'p^\mu\tau
+i\sqrt{\frac{\alpha'}2}\sum_{r\ne0}\frac1r
\left(\alpha_r^\mu e^{-ir(\tau-\sigma)}
+\widetilde\alpha_r^\mu e^{-ir(\tau+\sigma)}\right).
$$

The zero modes satisfy $\alpha_0^\mu=\widetilde\alpha_0^\mu=\sqrt{\alpha'/2},p^\mu$. Here $x^\mu$ and $p^\mu$ are the center-of-mass position and momentum, while the nonzero [string oscillators](../../../string-theory.md#string-oscillator) describe shape excitations.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A classical string must also satisfy the equations obtained by varying the worldsheet metric before imposing [conformal gauge](../../../string-theory.md#conformal-gauge). Vanishing of the worldsheet [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) gives

$$
T_{++}=\frac1{\alpha'}\partial_+X\mathbin\cdot\partial_+X=0,
\qquad
T_{--}=\frac1{\alpha'}\partial_-X\mathbin\cdot\partial_-X=0.
$$

In modes these are the [Virasoro constraints](../../../string-theory.md#virasoro-constraint)

$$
L_m=\frac12\sum_r\alpha_{m-r}\mathbin\cdot\alpha_r=0,
\qquad
\widetilde L_m=\frac12\sum_r\widetilde\alpha_{m-r}\mathbin\cdot\widetilde\alpha_r=0
$$

for every integer $m$. Reality of $X^\mu$ also requires

$$
(\alpha_r^\mu)^*=\alpha_{-r}^\mu,
\qquad
(\widetilde\alpha_r^\mu)^*=\widetilde\alpha_{-r}^\mu.
$$

Together with periodicity and the wave equation, these conditions remove the unphysical longitudinal worldsheet excitations.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a target circle of radius $R$, maps may wind, so the boundary condition is

$$
Y(\tau,\sigma+2\pi)=Y(\tau,\sigma)+2\pi Rw,
\qquad w\in\mathbb Z.
$$

Single-valued target-space wavefunctions quantize the center-of-mass momentum as $p_Y=n/R$, with $n\in\mathbb Z$. The [compact boson](../../../string-theory.md#compact-boson) expansion becomes

$$
Y=y+\alpha'\frac nR\tau+wR\sigma
+i\sqrt{\frac{\alpha'}2}\sum_{r\ne0}\frac1r
\left(\alpha_r e^{-ir(\tau-\sigma)}
+\widetilde\alpha_r e^{-ir(\tau+\sigma)}\right).
$$

Equivalently, its left- and right-moving zero-mode momenta are

$$
p_L=\frac nR+\frac{wR}{\alpha'},
\qquad
p_R=\frac nR-\frac{wR}{\alpha'}.
$$

The integers $n$ and $w$ are the [momentum and winding modes](../../../string-theory.md#momentum-and-winding-modes).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $M$ be the mass measured in the uncompactified 25-dimensional spacetime. The quantum zero-mode constraints are

$$
0=L_0-a=\frac{\alpha'}4(-M^2+p_L^2)+N-a,
\qquad
0=\widetilde L_0-a=\frac{\alpha'}4(-M^2+p_R^2)+\widetilde N-a.
$$

The [string level operators](../../../string-theory.md#string-level-operator)

$$
N=\sum_{r>0}\alpha_{-r}\mathbin\cdot\alpha_r,
\qquad
\widetilde N=\sum_{r>0}\widetilde\alpha_{-r}\mathbin\cdot\widetilde\alpha_r
$$

have nonnegative integer eigenvalues. Adding the constraints and using $(p_L^2+p_R^2)/2=n^2/R^2+w^2R^2/\alpha'^2$ gives

$$
\boxed{M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}
+\frac2{\alpha'}(N+\widetilde N-2a)}.
$$

Their difference gives [closed-string level matching](../../../string-theory.md#closed-string-level-matching), $N-\widetilde N+nw=0$ with the present left-right convention. The [normal-ordering constant of a string](../../../string-theory.md#normal-ordering-constant-of-a-string) $a$ is the regularized zero-point energy generated when oscillator products are normal ordered.

## 2

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The quadratic kinetic operator of the [beta-gamma system](../../../string-theory.md#beta-gamma-system) couples $\beta$ only to $\gamma$. Its Green-function equation is

$$
\bar\partial_z\langle\beta(z)\gamma(w)\rangle
=-2\pi\delta^{(2)}(z-w)
$$

in the stated normalization. Since $\bar\partial(1/(z-w))=2\pi\delta^{(2)}(z-w)$, the singular part is

$$
\boxed{\beta(z)\gamma(w)\sim-\frac1{z-w}}.
$$

The inverse kinetic matrix has no $\beta\beta$ or $\gamma\gamma$ entry, so those two [operator product expansions](../../../string-theory.md#operator-product-expansion) are nonsingular. For commuting fields, reversing the order gives $\gamma(z)\beta(w)\sim1/(z-w)$ after expanding about $w$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Applying [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) to the stated [holomorphic stress-energy tensor](../../../string-theory.md#holomorphic-stress-energy-tensor) gives

$$
T(z)\gamma(w)\sim
\frac{h\gamma(w)}{(z-w)^2}+\frac{\partial\gamma(w)}{z-w},
$$

and

$$
T(z)\beta(w)\sim
\frac{(1-h)\beta(w)}{(z-w)^2}+\frac{\partial\beta(w)}{z-w}.
$$

These are exactly the stress-tensor OPEs of [primary operators](../../../string-theory.md#primary-field). Hence $\gamma$ has holomorphic [conformal weight](../../../string-theory.md#conformal-weight) $h$ and $\beta$ has weight $1-h$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

In any two-dimensional conformal field theory,

$$
T(z)T(w)\sim\frac{c/2}{(z-w)^4}
+\frac{2T(w)}{(z-w)^2}+\frac{\partial T(w)}{z-w}.
$$

Double contractions in the bosonic [beta-gamma system](../../../string-theory.md#beta-gamma-system) give

$$
\boxed{c_{\beta\gamma}=2(6h^2-6h+1)}.
$$

The polynomial is unchanged by $h\mapsto1-h$, as required when the roles of the two fields are interchanged. If the fields anticommute, a closed fermionic contraction contributes an additional minus sign, giving the fermionic bc-system result

$$
\boxed{c_{bc}=-2(6h^2-6h+1)}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The $D$ free embedding scalars contribute $c_X=D$. The ordinary diffeomorphism ghosts contribute $c_{bc}=-26$. The fermionic $(m,n)$ pair has $h_n=0$ and contributes $-2$. Each of the $D/2$ fermionic $(\chi_a,\psi^a)$ pairs has $h_\psi=1/2$ and contributes $+1$. Each bosonic $(\beta_r,\gamma^r)$ pair has $h_\gamma=-1/2$ and contributes $+11$, and there are two such pairs. The total holomorphic [central charge](../../../string-theory.md#central-charge) is therefore

$$
c_{\rm tot}=D-26-2+\frac D2+22=\frac{3D}{2}-6.
$$

Cancellation of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) requires $c_{\rm tot}=0$, so

$$
\boxed{D=4}.
$$

The antiholomorphic sector gives the same condition.

## 3

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The unintegrated closed-string operator $c\widetilde c\,\mathcal O$ must have total conformal weight $(0,0)$ and ghost number $(1,1)$. Since $c$ and $\widetilde c$ have weights $(-1,0)$ and $(0,-1)$, the matter operator $\mathcal O$ must be a [Virasoro primary operator](../../../string-theory.md#primary-field) of weight

$$
(h,\widetilde h)=(1,1).
$$

Equivalently, the full operator must be a [BRST-closed operator](../../../relativistic-quantum-field.md#brst-closed-operator) and not a [BRST-exact operator](../../../relativistic-quantum-field.md#brst-exact-operator). For a momentum-dependent tensor operator, these requirements impose its target-space mass-shell, transversality, and gauge-equivalence conditions.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

At closed-string level $N=\widetilde N$, the [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum) is

$$
M^2=\frac4{\alpha'}(N-1).
$$

The state on the leading [Regge trajectory](../../../string-theory.md#regge-trajectory) uses only level-one oscillators and has maximal spin $J=N+\widetilde N=2N$. Eliminating $N$ gives

$$
\boxed{J=2+\frac{\alpha'M^2}{2}}.
$$

Because $N$ is unbounded, the spectrum contains infinitely many particles of increasing mass and spin. The intercept $J=2$ at $M^2=0$ includes the graviton.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The Riemann sphere has three complex [Conformal Killing vector fields](../../../general-relativity.md#conformal-killing-vector-field), forming the Möbius group $PSL(2,\mathbb C)$. Gauge fixing this residual conformal symmetry permits three insertion points to be fixed arbitrarily. Each unintegrated [string vertex operator](../../../string-theory.md#string-vertex-operator) contains $c\widetilde c$, and the three insertions exactly saturate the three holomorphic and three antiholomorphic ghost zero modes. Since every full vertex has weight $(0,0)$, the correlator is Möbius invariant and independent of the chosen three positions.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The free-boson worldsheet theory factorizes into independent holomorphic and antiholomorphic sectors. The factors $\partial X^\mu$ contract only in the holomorphic sector and produce one tensor $T^{\mu\kappa\rho}$, while the $\bar\partial X^\nu$ factors independently produce $T^{\nu\lambda\sigma}$. Their product is the closed-string version of left-right factorization, often summarized at tree level as closed-string kinematics being a square of open-string kinematics.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

In one chiral sector there are three derivatives $\partial X$. A nonzero Wick contraction can pair two derivatives with each other and contract the remaining derivative with an exponential; this gives a metric times one momentum and hence the terms linear in $k$. Alternatively, all three derivatives can contract with exponential operators, giving three momenta and the term proportional to $\alpha'k^3$. The same alternatives occur independently in the antiholomorphic sector.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

An [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) contains two derivatives, so its cubic graviton vertex produces only the $k\times k$ part of the product of the two $T$ tensors. The string amplitude also contains cross terms of order $\alpha'k^4$ and a term of order $\alpha'^2k^6$. These cannot arise from pure Einstein gravity. They require higher-curvature corrections, schematically

$$
S_{\rm eff}=\frac1{16\pi G_N}\int d^{26}x\sqrt{-g}
\left[R+\alpha'c_2R_{\mu\nu\rho\sigma}^2
+\alpha'^2c_3R^3+O(\alpha'^3\nabla^2R^3,\alpha'^3R^4)\right],
$$

with index contractions and coefficients fixed by string amplitudes up to [field redefinitions](../../../perturbative-quantum-field-theory.md#field-redefinition). The full bosonic-string effective action also contains the dilaton and Kalb-Ramond field. Thus Einstein gravity is only its leading low-energy approximation.

## 4

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In old covariant quantization, an open-string [physical string state](../../../string-theory.md#physical-string-state) obeys

$$
(L_0-1)|\psi\rangle=0,
\qquad
L_n|\psi\rangle=0\quad(n>0),
$$

with analogous left- and right-moving conditions for a closed string. A [spurious string state](../../../string-theory.md#spurious-string-state) is a [Virasoro descendant](../../../string-theory.md#virasoro-descendant) orthogonal to every physical state. A [null string state](../../../string-theory.md#null-string-state) is both physical and spurious; it has zero norm and zero inner product with every physical state, so quotienting by null states removes gauge redundancy without removing observable states.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $|s\rangle=L_{-1}|\chi\rangle$ with $L_n|\chi\rangle=0$ for every $n\ge0$. Since $[L_0,L_{-1}]=L_{-1}$, $|s\rangle$ has $L_0$ eigenvalue one. Moreover,

$$
L_1|s\rangle=[L_1,L_{-1}]|\chi\rangle=2L_0|\chi\rangle=0,
$$

and for $n>1$,

$$
L_n|s\rangle=(n+1)L_{n-1}|\chi\rangle=0.
$$

It is therefore physical. It is a Virasoro descendant and hence spurious, while its norm is

$$
\langle s|s\rangle=\langle\chi|L_1L_{-1}|\chi\rangle
=2\langle\chi|L_0|\chi\rangle=0.
$$

**Thus it is null.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Set

$$
|s\rangle=\left(L_{-2}+\frac32L_{-1}^2\right)|\phi\rangle.
$$

Its $L_0$ eigenvalue is $-1+2=1$. The Virasoro algebra gives

$$
L_1L_{-2}|\phi\rangle=3L_{-1}|\phi\rangle,
\qquad
L_1L_{-1}^2|\phi\rangle=-2L_{-1}|\phi\rangle,
$$

so $L_1|s\rangle=0$. At critical central charge $c=26$,

$$
L_2L_{-2}|\phi\rangle=(4L_0+13)|\phi\rangle=9|\phi\rangle,
\qquad
L_2L_{-1}^2|\phi\rangle=-6|\phi\rangle,
$$

so $L_2|s\rangle=0$. All $L_n$ with $n\ge3$ annihilate it directly. Hence $|s\rangle$ is physical and, being a positive-level Virasoro descendant, spurious; it is therefore a null state.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The zero-mode condition is automatic:

$$
L_0|\psi\rangle=\left(\frac12\alpha_0^2+2\right)|\psi\rangle=|\psi\rangle.
$$

Using $[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu$ and oscillator annihilation of the vacuum gives

$$
L_1|\psi\rangle
=2\left(t_{\mu\nu}\alpha_0^\nu+v_\mu\right)
\alpha_{-1}^\mu|0,p\rangle,
$$

which vanishes when $t_{\mu\nu}\alpha_0^\nu=-v_\mu$. Similarly,

$$
L_2|\psi\rangle
=\left(t^\mu{}_{\mu}+2v\mathbin\cdot\alpha_0\right)|0,p\rangle,
$$

which vanishes when $v\mathbin\cdot\alpha_0=-t^\mu{}_{\mu}/2$. Higher positive Virasoro modes annihilate a level-two state. These are precisely the stated physical-state conditions.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Using $\alpha_0^2=-2$, tracelessness and transversality of $\epsilon_{\mu\nu}$ gives

$$
t^\mu{}_{\mu}=\frac1{20}(3\alpha_0^2+26)t^\lambda{}_{\lambda}
=t^\lambda{}_{\lambda},
$$



$$
t_{\mu\nu}\alpha_0^\nu
=\frac1{20}(3\alpha_0^2+1)t^\lambda{}_{\lambda}\alpha_{0\mu}
=-\frac14t^\lambda{}_{\lambda}\alpha_{0\mu}=-v_\mu,
$$

and $v\mathbin\cdot\alpha_0=-t^\lambda{}_{\lambda}/2$, so the constraints hold.

On the momentum vacuum,

$$
L_{-1}|0,p\rangle=(\alpha_0\mathbin\cdot\alpha_{-1})|0,p\rangle,
$$



$$
L_{-2}|0,p\rangle
=\left(\alpha_0\mathbin\cdot\alpha_{-2}
+\frac12\alpha_{-1}\mathbin\cdot\alpha_{-1}\right)|0,p\rangle,
$$

and

$$
L_{-1}^2|0,p\rangle
=\left(\alpha_0\mathbin\cdot\alpha_{-2}
+(\alpha_0\mathbin\cdot\alpha_{-1})^2\right)|0,p\rangle.
$$

Therefore

$$
|\psi\rangle=\epsilon_{\mu\nu}\alpha_{-1}^\mu\alpha_{-1}^\nu|0,p\rangle+|n\rangle,
$$

where

$$
|n\rangle=\frac{t^\lambda{}_{\lambda}}{10}
\left(L_{-2}+\frac32L_{-1}^2\right)|0,p\rangle.
$$

The vacuum has $L_0|0,p\rangle=\alpha_0^2|0,p\rangle/2=-|0,p\rangle$ and is annihilated by positive modes, so part c proves that $|n\rangle$ is null. The physical content is consequently the transverse traceless tensor $\epsilon_{\mu\nu}$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
