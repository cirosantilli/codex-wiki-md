# Paper 354

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_354.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_354.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)

## 1

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

By the [state–operator correspondence](../../../string-theory.md#state-operator-correspondence), a CFT operator of [scaling dimension](../../../string-theory.md#scaling-dimension) $\Delta$ creates a cylinder state of energy $E=\Delta/R$. The identity gives the vacuum; the first nontrivial low-energy single-trace operator is the conserved [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor), with $\Delta=3$ in three dimensions; and one translation raises the dimension by one. Taking the scheme-dependent vacuum energy to vanish,

$$
\boxed{E_0=0,
\qquad E_1=\frac3R,
\qquad E_2=\frac4R.}
$$

All other single-trace primaries are heavy by assumption, while the first two-graviton state begins at $6/R$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The vacuum is unique, so $N_0=1$. The stress tensor is the spin-$2$ irreducible representation of $SU(2)$ and has $2j+1=5$ states. At the next level, a translation of spin $1$ gives

$$
1\otimes2=3\oplus2\oplus1.
$$

Stress-tensor conservation makes the spin-$1$ divergence a null [conformal descendant](../../../string-theory.md#conformal-descendant), leaving dimensions $7+5$. Hence

$$
\boxed{N_0=1,
\qquad N_1=5,
\qquad N_2=12.}
$$

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The corresponding rotation representations are

$$
\boxed{
E_0:j=0,
\qquad
E_1:j=2,
\qquad
E_2:j=2\ \text{and}\ 3.}
$$

The would-be $j=1$ representation at $E_2$ is absent because it is the null descendant expressing conservation of the stress tensor.

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

The [AdS/CFT correspondence](../../../string-theory.md#ads-cft-correspondence) maps the vacuum to empty anti-de Sitter spacetime and the stress-tensor conformal family to one-graviton normal modes. Therefore

$$
\boxed{n_g(E_0)=0,
\qquad n_g(E_1)=1,
\qquad n_g(E_2)=1.}
$$

The distinction between $E_1$ and $E_2$ is a different excitation within the same one-particle conformal family, not an additional graviton.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

At spacelike separation $x_{12}^2>0$, conformal symmetry fixes the [scalar-primary two-point function](../../../string-theory.md#scalar-primary-two-point-function) to

$$
\langle\mathcal O(x_1)\mathcal O(x_2)\rangle
=\frac{C_{\mathcal O}}{(x_{12}^2)^\Delta}.
$$

Applying the [d'Alembertian](../../../wave-equation.md#d-alembert-operator) at $x_2$ gives

$$
\boxed{F_0
=\frac{2C_{\mathcal O}\Delta(2\Delta+2-d)}
{(x_{12}^2)^{\Delta+1}}}
$$

away from contact terms. Thus, up to a real multiplicative constant, $F_0\propto(x_{12}^2)^{-\Delta-1}$. The scalar [conformal unitarity bound](../../../string-theory.md#conformal-unitarity-bound) makes the coefficient nonnegative and makes it vanish when the bound is saturated, as expected for the null free-field equation of motion.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

With

$$
Z[J]=\int\mathcal D\varphi\,
\exp\left(iS+i\int d^dx\,J\mathcal O\right),
$$

the time-ordered vacuum correlator can be written, in this source convention, as

$$
\boxed{F_0(x_1,x_2)=
-\left.\square_{x_2}
\frac1{Z[J]}
\frac{\delta^2Z[J]}{\delta J(x_1)\delta J(x_2)}
\right|_{J=0}.}
$$

Equivalent formulas in terms of the connected generating functional differ only by the standard factors of $i$.

A constant source deforms the action by $J\int d^dx\,\mathcal O$. Since $[J]=d-\Delta$, a nonzero $J$ introduces no scale only if

$$
\boxed{\Delta=d.}
$$

This marginality is necessary; for the deformed theory to remain a CFT for every $J$, the operator must additionally be [exactly marginal](../../../string-theory.md#exactly-marginal-operator), with vanishing beta function.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

For a bulk scalar with $m^2=\Delta(\Delta-d)$ in unit-radius Poincaré AdS, the [AdS scalar-field boundary asymptotics](../../../string-theory.md#ads-scalar-field-boundary-asymptotics) are

$$
\phi(x,z)=z^{d-\Delta}J(x)+z^\Delta A(x)+\cdots,
\qquad
\langle\mathcal O(x)\rangle\propto A(x).
$$

Thus $J$ and $\mathcal O$ are, up to normalization and local counterterms, the nonnormalizable and normalizable boundary coefficients respectively.

For $d=3$, $\Delta=1$, and $J=0$, alternative quantization gives

$$
\mathcal O(x)\propto\lim_{z\to0}z^{-1}\phi(x,z),
\qquad m^2=-2.
$$

The bulk [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) is

$$
\left[z^2\partial_z^2-2z\partial_z+z^2\square_x+2\right]\phi=0,
$$

so

$$
\square_x\phi=
\left(-\partial_z^2+\frac2z\partial_z-\frac2{z^2}\right)\phi.
$$

At separated points in any state,

$$
\boxed{
F=\lim_{z_1,z_2\to0}\frac1{z_1z_2}
\left\langle
\phi(x_1,z_1)
\left(-\partial_{z_2}^2+\frac2{z_2}\partial_{z_2}
-\frac2{z_2^2}\right)
\phi(x_2,z_2)
\right\rangle.}
$$

This contains only radial bulk derivatives, as required.

## 2

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The horizon is the largest positive root of $f(r_H)=0$. With $x=r_H^2$,

$$
0=1+\frac{x}{L^2}-\frac\mu x
\quad\Longleftrightarrow\quad
x^2+L^2x-\mu L^2=0.
$$

Choosing the positive root gives

$$
\boxed{r_H^2=\frac{L^2}{2}
\left(\sqrt{1+\frac{4\mu}{L^2}}-1\right).}
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

After Wick rotation $t=-it_E$, the near-horizon metric has

$$
ds_E^2\simeq f'(r_H)(r-r_H)dt_E^2
+\frac{dr^2}{f'(r_H)(r-r_H)}.
$$

Regularity at the origin of this polar plane requires the [Euclidean black-hole regularity condition](../../../general-relativity.md#euclidean-black-hole-regularity-condition) $\beta_H=4\pi/f'(r_H)$. Since

$$
\mu=r_H^2\left(1+\frac{r_H^2}{L^2}\right),
\qquad
f'(r_H)=\frac2{r_H}+\frac{4r_H}{L^2},
$$

we obtain

$$
\boxed{\beta_H=
\frac{2\pi L^2r_H}{2r_H^2+L^2}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Keep the smooth $\beta=\beta_H$ geometry fixed away from the horizon but identify Euclidean time with arbitrary period $\beta$. The horizon then has deficit angle $2\pi(1-\beta/\beta_H)$. Its delta-function curvature contributes

$$
\int_{\mathcal M}\sqrt g\,R\big|_{\rm tip}
=4\pi\left(1-\frac\beta{\beta_H}\right)A,
$$

and hence

$$
I_{\rm tip}=-\frac{A}{4G_N}
\left(1-\frac\beta{\beta_H}\right).
$$

Using $\log Z=-I_{\rm grav}$,

$$
\boxed{S_{\rm BH}
=\left.(1-\beta\partial_\beta)\log Z\right|_{\beta_H}
=\frac{A}{4G_N}
=\frac{2\pi^2r_H^3}{4G_N}.}
$$

All smooth bulk terms, including the cosmological-constant volume term, are proportional to the Euclidean time period and are annihilated by $1-\beta\partial_\beta$. The asymptotic [Gibbons–Hawking–York boundary term](../../../general-relativity.md#gibbons-hawking-york-boundary-term) and holographic counterterms are likewise smooth and linear in $\beta$. Only the curvature singularity at the fixed point of the Euclidean time circle survives.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Varying the boundary period and filling it by the corresponding smooth Euclidean saddle computes the same canonical partition function. Because each bulk metric obeys the Einstein equation, the implicit first-order metric variation of the on-shell action reduces to boundary terms; regularity relates the varied horizon radius to the varied period. The thermodynamic identity

$$
S=\beta E-I_E
=(1-\beta\partial_\beta)\log Z
$$

then yields the same [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy). The conical method is an off-shell way to isolate the local horizon term, while the smooth-saddle method packages that term into the variation of the entire solution.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The two-sided eternal black hole is dual to the [thermofield double state](../../../string-theory.md#thermofield-double-state)

$$
|\Psi_\beta\rangle
=\frac1{\sqrt{Z(\beta)}}
\sum_n e^{-\beta E_n/2}|n\rangle_L^*|n\rangle_R.
$$

Tracing out the left CFT gives

$$
\rho_R=\operatorname{Tr}_L|\Psi_\beta\rangle\langle\Psi_\beta|
=\frac{e^{-\beta H_R}}{Z(\beta)}.
$$

Thus the geometric period $\beta$ is the boundary inverse temperature, and $S_{\rm BH}$ is the [Von Neumann entropy](../../../von-neumann-entropy.md) $S_R=-\operatorname{Tr}(\rho_R\log\rho_R)$, equivalently the entanglement entropy between the two CFTs.

The [modular Hamiltonian](../../../string-theory.md#modular-hamiltonian) of this thermal state is

$$
K_R=-\log\rho_R=\beta H_R+\log Z.
$$

For any first-order state variation with $\operatorname{Tr}\delta\rho=0$,

$$
\delta S_R
=-\operatorname{Tr}(\delta\rho\log\rho_R)
=\operatorname{Tr}(\delta\rho K_R)
=\boxed{\beta\operatorname{Tr}(\delta\rho H_R)
=\beta\,\delta\langle E\rangle_\rho.}
$$

This is the [first law of entanglement entropy](../../../string-theory.md#first-law-of-entanglement-entropy).

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

The shell is created by a unitary $U_R$ acting only on the right CFT. Therefore $\rho_R\mapsto U_R\rho_RU_R^\dagger$ and its eigenvalues, hence the exact left--right entanglement entropy, do not change. The [Hubeny–Rangamani–Takayanagi surface](../../../string-theory.md#hubeny-rangamani-takayanagi-surface) homologous to the complete right boundary remains the old extremal bifurcation surface in the portion of the bulk preceding the shell, behind the enlarged late-time event horizon. Its entropy is

$$
\boxed{S_{L:R}=\frac{A(\mu)}{4G_N},}
$$

not $A(\mu')/(4G_N)$.

The larger late-time horizon area $A(\mu')$ instead gives the coarse-grained thermodynamic entropy of the final equilibrium black hole. It counts the entropy obtained after discarding detailed information about the coherent unitary excitation. The distinction between the unchanged HRT area and the increased final horizon area is the bulk counterpart of fine-grained entropy conservation under unitary evolution alongside thermodynamic entropy production after coarse graining.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
