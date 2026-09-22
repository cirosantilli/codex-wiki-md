# Paper 304

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20304.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20304.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
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

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The first two terms are the [kinetic term](../../../quantum-field-theory.md#kinetic-term) and [mass term](../../../quantum-field-theory.md#mass-term) of a [real scalar field](../../../scalar-field-theory.md#real-scalar-field); together they determine the free [quantum field theory propagator](../../../quantum-field-theory.md#propagator). The term $-\lambda\phi^4/4!$ is its quartic [field interaction term](../../../quantum-field-theory.md#field-interaction-term). The remaining three terms are [counterterms](../../../perturbative-quantum-field-theory.md#counterterm): $\delta_Z$ renormalizes the field normalization, $\delta_m$ renormalizes the mass, and $\delta_\lambda$ renormalizes the quartic coupling. Their regulator dependence cancels the ultraviolet divergences of loop diagrams, while their finite parts implement the chosen [renormalization conditions](../../../perturbative-quantum-field-theory.md#renormalization-condition).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Through order $\lambda^2$, the quartic [one-particle-irreducible Feynman diagrams](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-feynman-diagram) are the tree-level four-point vertex, the local $\delta_\lambda$ counterterm vertex, and three one-loop bubble diagrams. The bubbles have two quartic vertices and differ by whether the momentum through the loop is the $s$, $t$, or $u$ [Mandelstam variables](../../../special-relativity.md#mandelstam-variables); each has symmetry factor $1/2$. External-leg self-energies are not part of the 1PI four-point vertex, and $\delta_Z$ begins beyond the required order in this theory.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For a bubble carrying momentum $p$, a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) and a shift of the loop momentum give, after Wick rotation and [cutoff regularization](../../../perturbative-quantum-field-theory.md#cutoff-regularization),

$$
B(p^2)=\int_0^1dx\int_{|\ell_E|<\Lambda}
\frac{d^4\ell_E}{(2\pi)^4}
\frac1{[\ell_E^2+F(p^2)]^2}
=\frac1{16\pi^2}\int_0^1dx
\left[\log\frac{\Lambda^2}{F(p^2)}-1\right]
+O(\Lambda^{-2}),
$$

where $F(p^2)=m^2-x(1-x)p^2-i0$. The [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) therefore contains

$$
\Gamma_4(s,t,u)=\lambda+\delta_\lambda
-\frac{\lambda^2}{2}\{B(s)+B(t)+B(u)\}+O(\lambda^3).
$$

The [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) $\Gamma_4(M^2,M^2,M^2)=\lambda$ fixes

$$
\delta_\lambda=\frac{3\lambda^2}{2}B(M^2)+O(\lambda^3).
$$

Substitution cancels both the cutoff and the scheme-dependent constant and leaves

$$
\Gamma_4(s,t,u)=\lambda-\frac{\lambda^2}{32\pi^2}
\int_0^1dx\log\left[
\frac{F(M^2)^3}{F(s)F(t)F(u)}
\right]+O(\lambda^3),
$$

as required.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Regard $\lambda$ as a [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) $\lambda(M)$. At fixed $s,t,u$ and to order $\lambda^2$, differentiating the one-loop answer with respect to $\log M$ gives

$$
0=\frac{d\Gamma_4}{d\log M}
=\frac{d\lambda}{d\log M}
-\frac{\lambda^2}{32\pi^2}\int_0^1 6\,dx+O(\lambda^3),
$$

because $m\ll M$ implies $F(M^2)\simeq-x(1-x)M^2$. Thus the [beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) is

$$
\beta(\lambda)=\frac{d\lambda}{d\log M}
=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3).
$$

Solving this [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) with $\lambda(M_0)=\lambda_0$ gives

$$
\frac1{\lambda(M)}=\frac1{\lambda_0}
-\frac3{16\pi^2}\log\frac{M}{M_0},
\qquad
\lambda(M)=\frac{\lambda_0}{1-\dfrac{3\lambda_0}{16\pi^2}\log(M/M_0)}
$$

to leading-logarithmic order.

## 2

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The leading contributions to $\delta_2$ and $\delta_m$ come from the one-loop electron self-energy: one internal electron line and one internal photon line join two electron-photon vertices. Its coefficients of $\gamma^\mu p_\mu$ and $m$ determine the field-strength and mass counterterms. The leading contribution to $\delta_1$ comes from the one-loop electron-photon vertex correction, with two internal electron propagators and one internal photon propagator, together with the corresponding local counterterm vertices. The [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) gives $\delta_1=\delta_2$ in a gauge-invariant scheme.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Use [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) with $d=4-\epsilon$ and choose [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge). Combining the electron and photon denominators with a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter), shifting the loop momentum, and discarding the odd term leaves the numerator

$$
(2-d)(1-x)\gamma^\mu p_\mu+dm.
$$

The pole of the rotationally symmetric integral consequently gives

$$
\Sigma_{\rm pole}(p)
=\frac{e^2}{8\pi^2\epsilon}
\int_0^1dx\,[-2(1-x)\gamma^\mu p_\mu+4m]
=\frac{e^2}{8\pi^2\epsilon}(-\gamma^\mu p_\mu+4m).
$$

With the inverse-propagator convention

$$
S^{-1}(p)=\gamma^\mu p_\mu-m+\delta_2\gamma^\mu p_\mu-\delta_m-\Sigma(p),
$$

the [minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#minimal-subtraction-scheme) chooses the counterterm pole to equal $\Sigma_{\rm pole}$. Hence

$$
\boxed{\delta_2=-\frac{e^2}{8\pi^2\epsilon},
\qquad
\delta_m=-\frac{me^2}{2\pi^2\epsilon}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The leading two-point diagram has one sextic vertex, two external legs, and its remaining four legs paired into two tadpole loops; it determines the mass counterterm. The leading six-point diagram has two sextic vertices joined by three internal lines, leaving three external legs at each vertex; it is a two-loop diagram and determines the coupling counterterm. The corresponding local $\delta_m$ and $\delta_\lambda$ vertices complete the counterterm calculation.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For the two-point graph, $L=2$ and $I=2$, so its [superficial degree of divergence](../../../perturbative-quantum-field-theory.md#superficial-degree-of-divergence) in three dimensions is

$$
D=3L-2I=2.
$$

Its additive mass-squared counterterm is therefore proportional to $\lambda\Lambda^2$; writing that counterterm as $m^2\delta_m$ gives the dimensionless scaling $\delta_m\sim\lambda\Lambda^2/m^2$, or $\Lambda^2/m^2$ when coupling factors are suppressed as in the question. For the six-point graph, $L=2$ and $I=3$, so $D=0$ and its ultraviolet divergence is logarithmic:

$$
\delta_\lambda\sim\lambda^2\log(\Lambda/m).
$$

Suppressing powers of $\lambda$ yields the two stated estimates.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The only two-point diagram through second [loop order](../../../perturbative-quantum-field-theory.md#loop-order) is the double tadpole from one sextic vertex. It has no route by which the external momentum can pass through an internal propagator, so its value is independent of $p$ and renormalizes only the mass. A field-strength counterterm is determined by the coefficient of $p^2$ in the two-point 1PI function, hence $\delta_Z=0$ at one and two loops. The first momentum-dependent two-point topology uses two sextic vertices joined by five internal lines and has four loops.

## 3

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Complete the square in the heavy variable:

$$
S(\phi,\chi)=\frac12m^2\phi^2
+\frac12M^2\left(\chi+\frac{\lambda\phi^2}{M^2}\right)^2
-\frac{\lambda^2}{2M^2}\phi^4.
$$

The shifted [Gaussian integral](../../../calculus.md#gaussian-integral) is independent of $\phi$. For $M>0$, choosing $N=M/\sqrt{2\pi}$ removes it and gives

$$
\boxed{W(\phi)=\frac12m^2\phi^2-\frac{\lambda^2}{2M^2}\phi^4,
\qquad
\widetilde\lambda=-\frac{\lambda^2}{2M^2}.}
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The induced four-$\phi$ interaction is the tree-level diagram with two $\lambda\phi^2\chi$ vertices joined by one internal $\chi$ propagator. The zero-dimensional propagator is $M^{-2}$, and the second-order expansion of the exponential supplies the factor $1/2$. The resulting effective-action coefficient is therefore $-\lambda^2/(2M^2)$, exactly the value of $\widetilde\lambda$ found by the [Gaussian integral](../../../calculus.md#gaussian-integral).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Let $K_M=-\partial^2+M^2$ and let $\Delta_M=K_M^{-1}$ be its Euclidean [quantum field theory propagator](../../../quantum-field-theory.md#propagator). With the source-sign convention suited to the expression in the question, define

$$
Z_0[J]=N_0\int\mathcal D\chi\,
\exp\left[-S_2[\chi]-\int d^dx\,J(x)\chi(x)\right]
=\exp\left[\frac12\int d^dx\,d^dy\,
J(x)\Delta_M(x-y)J(y)\right],
$$

where $N_0$ makes $Z_0[0]=1$. Since inserting $\chi(x)$ is equivalent to acting with $-\delta/\delta J(x)$, the [integral over $\chi$](../../../quantum-field-theory.md#integrating-out-a-field) gives

$$
\boxed{W[\phi]=S_1[\phi]-\log\left.
\left\{\exp\left[-S_3\left(\phi,-\frac{\delta}{\delta J}\right)\right]Z_0[J]\right\}\right|_{J=0}.}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The interaction is linear in the Gaussian field $\chi$, so completing the functional square makes its order-$\lambda^2$ contribution exact:

$$
W[\phi]=S_1[\phi]-\frac{\lambda^2}{2}
\int d^dx\,d^dy\,\phi^2(x)\Delta_M(x-y)\phi^2(y).
$$

In momentum space, $\Delta_M(p)=(p^2+M^2)^{-1}$. If every external momentum satisfies $p^2\ll M^2$, the [derivative expansion](../../../quantum-field-theory.md#derivative-expansion)

$$
\Delta_M(p)=\frac1{M^2}-\frac{p^2}{M^4}+O(M^{-6}p^4)
$$

starts with the local effective interaction

$$
-\frac{\lambda^2}{2M^2}\int d^dx\,\phi^4(x),
$$

which is the field-theory version of the zero-dimensional result.

## 4

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a gauge orbit near a root $\alpha_0$ of $G(A^\alpha)=0$, functional linearization gives

$$
G(A^\alpha)=\left.\frac{\delta G(A^\alpha)}{\delta\alpha}\right|_{\alpha_0}
(\alpha-\alpha_0)+O((\alpha-\alpha_0)^2).
$$

The multidimensional delta-function change-of-variables formula therefore gives

$$
\int\mathcal D\alpha\,\delta[G(A^\alpha)]
=\det\left(\left.\frac{\delta G(A^\alpha)}{\delta\alpha}\right|_{G=0}\right)^{-1}.
$$

Comparison with the defining identity proves

$$
\Delta_{\rm FP}[A]=\det\left(\left.\frac{\delta G(A^\alpha)}{\delta\alpha}\right|_{G=0}\right),
$$

up to the usual field-independent normalization and a choice of determinant sign on the gauge patch.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For [axial gauge](../../../relativistic-quantum-field.md#axial-gauge),

$$
\frac{\delta G^a(x)}{\delta\alpha^b(y)}
=n^\mu D_\mu^{ab}(x)\delta^{(4)}(x-y),
$$

so the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) is $\det(n^\mu D_\mu)$. Representing it with a [Faddeev-Popov ghost field](../../../relativistic-quantum-field.md#faddeev-popov-ghost) pair gives

$$
S_{\rm gh}=\int d^4x\,\bar c^a n^\mu D_\mu^{ab}c^b.
$$

The delta functional sets $\omega=n\mathbin\cdot A$ in its Gaussian weight, and hence

$$
S_{\rm gf}=-\frac1{2\xi}\int d^4x\,(n^\mu A_\mu^a)^2.
$$

Substitution yields

$$
Z[J]=N\int\mathcal DA\,\mathcal D\bar c\,\mathcal Dc\,
e^{,iS[A]+iS_{\rm gh}+iS_{\rm gf}+i\int J^\mu A_\mu}.
$$

In the strict axial-gauge limit $n\mathbin\cdot A=0$, $n\mathbin\cdot D=n\mathbin\cdot\partial$, so the ghost determinant is independent of $A$ and can be absorbed into $N$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write the gauge-fixing and ghost action as the [BRST transformation](../../../relativistic-quantum-field.md#brst-symmetry) of the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion):

$$
S_{\rm gf}+S_{\rm gh}=s\int d^4x\,
\bar c^a\left(n^\mu A_\mu^a-\frac\xi2B^a\right),
$$

with harmless rescalings of $B$ accommodating the convention $s\bar c^a=\xi B^a$ used in the question. The gauge-invariant action obeys $sS[A]=0$, while nilpotence gives

$$
s(S_{\rm gf}+S_{\rm gh})=s^2\Psi_n=0.
$$

**Thus the entire gauge-fixed action is [BRST invariant](../../../relativistic-quantum-field.md#brst-symmetry). Eliminating the auxiliary field $B^a$ by its algebraic field equation reproduces the axial gauge-fixing term and the ghost action found in part (b).**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Changing $n^\mu$ to $u^\mu$ changes the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion) by

$$
\Psi_u-\Psi_n=\int d^4x\,\bar c^a(u-n)^\mu A_\mu^a.
$$

The corresponding change of the action is the BRST-exact term $s(\Psi_u-\Psi_n)$. For a BRST-closed observable $\mathcal O$, invariance of the functional measure implies that the variation of its expectation value is the expectation of a total BRST variation and vanishes:

$$
\delta\langle\mathcal O\rangle
\mathrel\propto\langle s[\mathcal O(\Psi_u-\Psi_n)]\rangle=0.
$$

**Therefore physical states and observables, which are classes in [BRST cohomology](../../../relativistic-quantum-field.md#brst-cohomology), do not depend on the fixed axial-gauge vector, provided there is no BRST anomaly or boundary contribution.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
