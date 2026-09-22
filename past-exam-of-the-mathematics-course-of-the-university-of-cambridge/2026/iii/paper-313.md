# Paper 313

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20313.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20313.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

With $D_i\phi=(\partial_i-iA_i)\phi$ and $B=F_{12}$, the critically coupled [Abelian Higgs model](../../../classical-field-theory-soliton.md#abelian-higgs-model) energy in the conventions of the question is

$$
E=\frac12\int_{\mathbb R^2}d^2x\left[
B^2+|D_1\phi|^2+|D_2\phi|^2
+\frac14(1-|\phi|^2)^2\right].
$$

Finite energy requires $|\phi|\to1$, $D_i\phi\to0$, and $B\to0$ at spatial infinity.

For the [Derrick theorem](../../../classical-field-theory-soliton.md#derrick-s-theorem) test, preserve gauge covariance by defining

$$
\phi_\lambda(x)=\phi(\lambda x),
\qquad
A_i^{(\lambda)}(x)=\lambda A_i(\lambda x).
$$

The magnetic, covariant-gradient, and potential energies scale as

$$
E_B(\lambda)=\lambda^2E_B,
\qquad
E_D(\lambda)=E_D,
\qquad
E_V(\lambda)=\lambda^{-2}E_V.
$$

Stationarity at $\lambda=1$ requires $E_B=E_V$, which is possible for a nonconstant finite-energy configuration. The oppositely scaling magnetic and potential terms therefore evade the usual Derrick obstruction and allow vortex solitons.

At infinity write $\phi\to e^{i\chi}$. The condition $D\phi\to0$ gives $A\to d\chi$, and the phase winding defines the [Abelian Higgs vortex](../../../classical-field-theory-soliton.md#nielsen-olesen-vortex) number

$$
N=\frac1{2\pi}\oint_{S^1_\infty}d\chi\in\mathbb Z.
$$

By [Stokes theorem](../../../calculus.md#stokes-theorem),

$$
\boxed{\int_{\mathbb R^2}F
=\oint_{S^1_\infty}A=2\pi N}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Away from zeros of $\phi$, write

$$
\phi=e^{u/2+i\chi},
\qquad
u=\log|\phi|^2.
$$

The first [Bogomolny vortex equation](../../../classical-field-theory-soliton.md#bogomolny-vortex-equation), $(D_x+iD_y)\phi=0$, gives

$$
A_x=\partial_x\chi+\frac12\partial_yu,
\qquad
A_y=\partial_y\chi-\frac12\partial_xu.
$$

If the zeros $z_r$ have multiplicities $N_r$, the phase curl and the logarithmic singularities give, distributionally,

$$
B=2\pi\sum_rN_r\delta^{(2)}(z-z_r)-\frac12\Delta u.
$$

Equating this with $\Omega(1-e^u)/2$ yields the [Taubes equation](../../../classical-field-theory-soliton.md#taubes-equation)

$$
\boxed{
\Delta u+\Omega(1-e^u)
=4\pi\sum_rN_r\delta^{(2)}(z-z_r)}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For a zero of order $N$ at the origin and no other zeros,

$$
u(r)=2N\log r+O(1)
\quad(r\to0),
\qquad
u(r)\to0
\quad(r\to\infty).
$$

Away from the zero, the flat [Taubes equation](../../../classical-field-theory-soliton.md#taubes-equation) is

$$
\Delta u=e^u-1.
$$

If $u$ had a positive interior maximum, then the [second-derivative test](../../../calculus.md#hessian-matrix) would give $\Delta u\leq0$ there, while $e^u-1>0$, a contradiction. The boundary values are $-\infty$ at the zero and $0$ at infinity, so the [maximum principle](../../../partial-differential-equation.md#maximum-principle-for-subharmonic-functions) gives $u\leq0$. Hence

$$
\boxed{|\phi|=e^{u/2}\leq1}.
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The surface area is

$$
\operatorname{Area}(\Sigma)
=\int_{\mathbb R^2}\frac{a^2}{(1+|z|^2)^2}\,dx\,dy
=2\pi a^2\int_0^\infty\frac{r\,dr}{(1+r^2)^2}
=\pi a^2.
$$

Integrating the [Taubes equation](../../../classical-field-theory-soliton.md#taubes-equation) over the compact surface eliminates the Laplacian and gives

$$
4\pi N=\int_\Sigma\Omega(1-e^u)d^2x
<\operatorname{Area}(\Sigma)
$$

for a nontrivial solution. For $N=2$, the [Bradlow bound](../../../classical-field-theory-soliton.md#bradlow-bound) therefore requires

$$
\boxed{\pi a^2>8\pi,
\qquad a^2>8}.
$$

Equality is the dissolved-vortex limit with identically vanishing Higgs field and does not give the stipulated ordinary two-vortex solution.

## 2

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the curvature $F=dA+A\wedge A$, define the [Second Chern form](../../../geometry-and-topology.md#second-chern-form)

$$
\boxed{C_2=\frac1{8\pi^2}\operatorname{Tr}(F\wedge F)}.
$$

Using the graded cyclicity of the trace and $d^2=0$,

$$
d\operatorname{Tr}(A\wedge dA)
=\operatorname{Tr}(dA\wedge dA),
$$

while

$$
d\operatorname{Tr}(A\wedge A\wedge A)
=3\operatorname{Tr}(dA\wedge A\wedge A).
$$

Expanding $\operatorname{Tr}(F\wedge F)$ gives the same two terms with coefficient two on $dA\wedge A\wedge A$; the quartic term has vanishing trace by graded cyclicity. Therefore

$$
C_2=dY,
\qquad
\boxed{Y=\frac1{8\pi^2}\operatorname{Tr}\left(
A\wedge dA+\frac23A\wedge A\wedge A\right)},
$$

so $\boxed{\alpha=2/3}$. This is the [Chern-Simons 3-form](../../../geometry-and-topology.md#chern-simons-3-form).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Set

$$
\omega=dg\,g^{-1},
\qquad
\widetilde A=gAg^{-1}-\omega.
$$

The right [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation) is $d\omega=\omega\wedge\omega$. Direct substitution gives

$$
\widetilde F=gFg^{-1},
$$

so trace invariance proves $\widetilde C_2=C_2$.

For the [Chern-Simons 3-form](../../../geometry-and-topology.md#chern-simons-3-form), expansion and graded cyclicity give

$$
Y(\widetilde A)-Y(A)
=\frac1{8\pi^2}d\operatorname{Tr}\bigl(
\omega\wedge gAg^{-1}\bigr)
+\frac1{24\pi^2}\operatorname{Tr}(\omega^3).
$$

Since cyclicity also gives

$$
\operatorname{Tr}(\omega\wedge gAg^{-1})
=\operatorname{Tr}(g^{-1}dg\wedge A),
$$

the required two-form may be chosen as

$$
\boxed{T=\frac1{8\pi^2}\operatorname{Tr}(g^{-1}dg\wedge A)}.
$$

Thus

$$
\boxed{
Y\longmapsto Y+dT
+\frac1{24\pi^2}\operatorname{Tr}[(dg\,g^{-1})^3]}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Finite Euclidean Yang-Mills action requires $F\to0$ sufficiently rapidly at spatial infinity. Consequently the connection approaches a pure gauge,

$$
A\longrightarrow-dg\,g^{-1}
$$

under the convention of the question. Compactifying the asymptotic boundary identifies it with $S^3_\infty$, while $SU(2)$ is itself topologically $S^3$. Thus $g|_{S^3_\infty}$ has an integer [topological degree](../../../geometry-and-topology.md#topological-degree).

By $C_2=dY$ and [Stokes theorem](../../../calculus.md#stokes-theorem), the [instanton number](../../../classical-field-theory-soliton.md#instanton-number) is

$$
k=\int_{\mathbb R^4}C_2
=\int_{S^3_\infty}Y(-dg\,g^{-1})
=\boxed{\frac1{24\pi^2}
\int_{S^3_\infty}\operatorname{Tr}[(dg\,g^{-1})^3]}
=\deg(g),
$$

up to the common simultaneous choice of trace and orientation signs. Smoothness and finite action are imposed in the interior, and $F=\pm{}^\star F$ selects an instanton or anti-instanton representative of the topological sector.

## 3

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a matrix [Lie group](../../../lie-theory.md#lie-group), the left-invariant [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) is

$$
\boxed{\rho=g^{-1}dg}.
$$

Differentiating $g^{-1}g=I$ gives $d(g^{-1})=-g^{-1}(dg)g^{-1}$. Hence

$$
d\rho=d(g^{-1})\wedge dg
=-g^{-1}dg\wedge g^{-1}dg
=-\rho\wedge\rho,
$$

and therefore

$$
\boxed{d\rho+\rho\wedge\rho=0}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Substitute $\rho=\sigma^\alpha T_\alpha$ into the [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation). Antisymmetry of the wedge product gives

$$
\rho\wedge\rho
=\frac12\sigma^\alpha\wedge\sigma^\beta
[T_\alpha,T_\beta]
=\frac12c^\gamma{}_{\alpha\beta}
\sigma^\alpha\wedge\sigma^\beta T_\gamma.
$$

Equating coefficients of $T_\gamma$ yields

$$
\boxed{d\sigma^\gamma
=-\frac12\sum_{\alpha,\beta}
c^\gamma{}_{\alpha\beta}\sigma^\alpha\wedge\sigma^\beta},
$$

so $\boxed{f^\gamma{}_{\alpha\beta}=-c^\gamma{}_{\alpha\beta}/2}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Represent the [real affine group](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line) by

$$
g(a,b)=
\begin{pmatrix}
e^a&b\\0&1
\end{pmatrix}.
$$

Matrix multiplication reproduces

$$
(a,b)(a',b')=(a+a',b+e^ab').
$$

The [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) is

$$
g^{-1}dg=
\begin{pmatrix}
da&e^{-a}db\\0&0
\end{pmatrix},
$$

so a basis of left-invariant one-forms is

$$
\boxed{\sigma^1=da,
\qquad \sigma^2=e^{-a}db}.
$$

The dual left-invariant vector fields are

$$
\boxed{E_1=\partial_a,
\qquad E_2=e^a\partial_b}.
$$

Indeed $\sigma^i(E_j)=\delta^i_j$, and left translation preserves the one-forms and vector fields.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The metric is the [left-invariant metric](../../../lie-theory.md#left-invariant-metric)

$$
g=da^2+e^{-2a}db^2.
$$

Its right-invariant vector fields are

$$
\boxed{R_1=\partial_a+b\partial_b,
\qquad R_2=\partial_b}.
$$

Their flows act by left translations, which preserve a left-invariant metric. Directly,

$$
\mathcal L_{R_1}g=0,
\qquad
\mathcal L_{R_2}g=0,
$$

so both are [Killing vector fields](../../../general-relativity.md#killing-vector-field) and generate one-parameter isometry groups.

There is an additional Killing field. Put $y=e^a>0$ and $x=b$; then

$$
g=\frac{dx^2+dy^2}{y^2},
$$

the [hyperbolic plane](../../../geometry-and-topology.md#hyperbolic-plane) of constant curvature $-1$. Its isometry algebra is three-dimensional, whereas the space of right-invariant fields here is two-dimensional. For example, the third independent Killing field can be written

$$
(b^2-e^{2a})\partial_b+2b\partial_a,
$$

which is not right invariant. Hence the answer is yes.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
