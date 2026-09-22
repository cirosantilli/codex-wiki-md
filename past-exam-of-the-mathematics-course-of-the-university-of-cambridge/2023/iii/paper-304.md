# Paper 304

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_304.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_304.pdf)

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
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

After integration by parts, the quadratic action is

$$
S_0[x]=-\frac12\int dt\,x(t)(\partial_t^2+\omega^2)x(t).
$$

With the pole prescription appropriate to the conventions in the question, its inverse kernel is

$$
D(t)=\int\frac{dE}{2\pi}\frac{i\,e^{-iEt}}{\omega^2-E^2-i\epsilon}.
$$

For $t>0$ close the [contour](../../../complex-analysis.md#contour-integration) in the lower half-plane and for $t<0$ close it in the upper half-plane. The enclosed pole in each case gives

$$
D(t-t')=\frac1{2\omega}e^{i\omega|t-t'|},
$$

which equivalently satisfies $(\partial_t^2+\omega^2)D(t)=i\delta(t)$.

The source-dependent [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) is evaluated by translating the integration variable by the classical sourced solution. Completing the square gives

$$
Z_0[J]=Z_0[0]\exp\left[
-\frac12\int dt\,dt'\,J(t)D(t-t')J(t')
\right].
$$

Changes in the sign of the source term or of the path-integral phase move factors of $i$ between $D$ and the exponent but leave the contraction rules equivalent.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Replace each occurrence of $x(t)$ in the interaction by the [functional derivative](../../../calculus-of-variations.md#functional-derivative) that inserts it. In standard Minkowski source conventions,

$$
Z[J]
=\exp\left[
-\frac{i\lambda}{3!}\int dt
\left(\frac1i\frac{\delta}{\delta J(t)}\right)^3
\right]Z_0[J]
$$

and hence

$$
Z[J]
=\sum_{n=0}^\infty\frac1{n!}
\left[-\frac{i\lambda}{3!}\int dt
\left(\frac1i\frac{\delta}{\delta J(t)}\right)^3\right]^n
Z_0[J].
$$

The factors of $i$ are adjusted together if one uses the source convention of part a directly.

This is a [perturbation series](../../../perturbative-quantum-field-theory.md#perturbation-series), generally an asymptotic rather than convergent series because the number of [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-s-theorem) grows factorially. For real cubic coupling the potential is also unbounded on one side, so the real-axis theory does not possess a stable nonperturbative ground state without a contour prescription or further stabilizing interactions.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The time-domain [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) are:

- each internal line joining times $t,t'$ contributes $D(t-t')$;
- each cubic vertex contributes $-i\lambda$ and an integration $\int dt$;
- divide by the graph's [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor);
- attach the external times to the corresponding lines and retain connected graphs.

There is no order-$\lambda$ connected two-point correction. Through order $\lambda^2$, the two connected topologies are the two-vertex fish graph and the one-particle-reducible tadpole graph. With the displayed vertex convention,

$$
\begin{aligned}
\langle T x(t_1)x(t_2)\rangle_{\mathrm{conn}}
={}&D(t_1-t_2)\\
&+\frac{(-i\lambda)^2}{2}\int dt\,dt'\,
D(t_1-t)D(t-t')^2D(t'-t_2)\\
&+\frac{(-i\lambda)^2}{2}\int dt\,dt'\,
D(t_1-t)D(t_2-t)D(t-t')D(0)
+O(\lambda^4),
\end{aligned}
$$

up to the common factors of $i$ associated with the propagator convention. Vacuum normalization removes disconnected vacuum bubbles.

These integrals are ultraviolet finite in one time dimension: a harmonic-oscillator propagator behaves as $E^{-2}$ at large frequency, and the loop-frequency integrals have negative superficial degree of divergence. They are also infrared finite because $\omega>0$ supplies a gap. The cubic instability affects nonperturbative convergence but does not create a divergence in these fixed-order integrals.

## 2

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For massless [phi-fourth theory](../../../scalar-field-theory.md#quartic-interaction) in four dimensions, the momentum-space rules are

$$
\text{propagator: }\frac{i}{p^2+i\epsilon},
\qquad
\text{quartic vertex: }-i\lambda.
$$

Writing

$$
\mathcal L_{\mathrm{ct}}
=\frac12\delta_Z(\partial\phi)^2
-\frac12\delta m^2\phi^2
-\frac{\delta\lambda}{4!}\phi^4,
$$

the two-point counterterm insertion is $i(\delta_Zp^2-\delta m^2)$ and the four-point counterterm is $-i\delta\lambda$.

The renormalized [one-particle-irreducible correlation function](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-correlation-function) $\Gamma_4$ through order $\lambda^2$ contains the tree quartic vertex, the quartic counterterm, and three one-loop bubble diagrams. The bubbles are the $s$, $t$, and $u$ channels and each has symmetry factor $1/2$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For one channel with momentum $p$, introduce a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) and shift the loop momentum:

$$
\frac1{\ell^2(\ell+p)^2}
=\int_0^1dx\,
\frac1{\{(\ell+xp)^2+x(1-x)(-p^2)\}^2}.
$$

In $d=4-\epsilon$, with dimensional-regularization scale $\bar\mu$ before the usual modified-minimal-subtraction redefinition, the bubble at $p^2=-M^2$ is

$$
B(M)=\frac{i}{16\pi^2}
\left[
\frac2\epsilon-\gamma+\log4\pi
-\log\frac{M^2}{\bar\mu^2}
-\int_0^1dx\,\log\{x(1-x)\}
+O(\epsilon)
\right].
$$

Since $\int_0^1\log\{x(1-x)\}\,dx=-2$, summing the three equal channels gives the form displayed in the question, beginning with $6/\epsilon-3\gamma$.

Consequently

$$
-i\lambda_{\mathrm{eff}}
=-i\lambda
+\frac{i\,3\lambda^2}{32\pi^2}
\left[
\frac2\epsilon-\gamma+\log4\pi
-\log\frac{M^2}{\bar\mu^2}+2
\right]
-i\delta\lambda+O(\lambda^3).
$$

The [momentum-subtraction scheme](../../../perturbative-quantum-field-theory.md#momentum-subtraction-scheme) condition $\lambda_{\mathrm{eff}}(M)=\lambda$ is enforced by

$$
\delta\lambda
=\frac{3\lambda^2}{32\pi^2}
\left[
\frac2\epsilon-\gamma+\log4\pi
-\log\frac{M^2}{\bar\mu^2}+2
\right].
$$

Choosing $\bar\mu=M$ removes the logarithm. A minimal-subtraction scheme keeps only the pole and therefore defines a different finite renormalized coupling.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For a renormalized $n$-point one-particle-irreducible function, the [Callan-Symanzik equation](../../../perturbative-quantum-field-theory.md#callan-symanzik-equation) is

$$
\left(
M\frac{\partial}{\partial M}
+\beta(\lambda)\frac{\partial}{\partial\lambda}
+n\gamma_\phi(\lambda)
\right)\Gamma_R^{(n)}=0,
$$

with a convention-dependent sign on $\gamma_\phi$. At this order $\gamma_\phi=0$.

At a general Euclidean momentum scale $Q$, the one-loop four-point function contains

$$
\lambda_{\mathrm{eff}}(Q)
=\lambda(M)+\frac{3\lambda(M)^2}{32\pi^2}
\log\frac{Q^2}{M^2}+O(\lambda^3).
$$

Requiring a physical amplitude to be independent of the arbitrary subtraction scale gives

$$
0=M\frac d{dM}\lambda_{\mathrm{eff}}(Q)
=\beta(\lambda)-\frac{3\lambda^2}{16\pi^2}+O(\lambda^3),
$$

and therefore

$$
\boxed{\beta(\lambda)=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3).}
$$

## 3

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For the convention in the question, a finite [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) acts covariantly on the field strength:

$$
F_{\mu\nu}\mapsto F'_{\mu\nu}=UF_{\mu\nu}U^\dagger
$$

or with $U$ and $U^\dagger$ exchanged if the opposite convention is used for $D_\mu$. Cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace) gives

$$
\operatorname{Tr}(F'_{\mu\nu}F'^{\mu\nu})
=\operatorname{Tr}(UF_{\mu\nu}F^{\mu\nu}U^\dagger)
=\operatorname{Tr}(F_{\mu\nu}F^{\mu\nu}),
$$

so the [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) Lagrangian is gauge invariant.

The quadratic gauge-field operator has zero directions $A_\mu\sim A_\mu+D_\mu\alpha$ along each [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit). It therefore has no inverse on the full field space. [Gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) removes this degeneracy and produces a propagator, while the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) accounts for the corresponding Jacobian.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Requiring $D_\mu\phi$ to transform as $U^\dagger(D_\mu\phi)U$ and using the gauge-field transformation law gives

$$
D_\mu\phi=\partial_\mu\phi-ig[A_\mu,\phi].
$$

Indeed, differentiating $U^\dagger\phi U$ produces two inhomogeneous derivative terms, and those cancel against the inhomogeneous part of the transformed connection.

For $U=1+i\alpha^aT_a+O(\alpha^2)$,

$$
\phi'=U^\dagger\phi U
=\phi+i[\phi,\alpha^aT_a]+O(\alpha^2).
$$

If $[T_a,T_b]=if_{ab}{}^cT_c$, then

$$
\delta\phi^c=f_{ab}{}^c\alpha^a\phi^b.
$$

This is the infinitesimal [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

At lowest derivative order, a general invariant effective Lagrangian through fourth order in the fields has the schematic form

$$
\begin{aligned}
\mathcal L={}&-\frac12\operatorname{Tr}F_{\mu\nu}F^{\mu\nu}
+\operatorname{Tr}(D_\mu\phi D^\mu\phi)
-m_\phi^2\operatorname{Tr}\phi^2
-\lambda_{abcd}\phi^a\phi^b\phi^c\phi^d\\
&+\bar\psi(i\not D-m_\psi)\psi
-h_A\,\mathcal I_A(\bar\psi,\psi,\phi,\phi)
-G_B\,\mathcal J_B(\bar\psi,\psi,\bar\psi,\psi).
\end{aligned}
$$

Here $\lambda_{abcd}$ is any invariant symmetric rank-four tensor, the $\mathcal I_A$ run over invariant contractions such as $(\operatorname{Tr}\phi^2)\bar\psi\psi$ and $\bar\psi\phi^2\psi$, and the $\mathcal J_B$ run over gauge- and Lorentz-invariant four-fermion contractions. The two sign symmetries forbid scalar cubic terms and Yukawa terms $\bar\psi\phi\psi$. The covariant kinetic terms automatically contain the allowed cubic and quartic interactions involving $A_\mu$.

The canonical dimensions are

$$
[A_\mu]=[\phi]=\frac{d-2}{2},
\qquad
[\psi]=\frac{d-1}{2},
$$

and hence

$$
[g]=\frac{4-d}{2},
\quad
[\lambda]=4-d,
\quad
[h_A]=3-d,
\quad
[G_B]=2-d,
\quad
[m_\phi^2]=2,
\quad
[m_\psi]=1.
$$

A coupling is [relevant](../../../perturbative-quantum-field-theory.md#relevant-coupling), [marginal](../../../perturbative-quantum-field-theory.md#marginal-coupling), or [irrelevant](../../../perturbative-quantum-field-theory.md#irrelevant-coupling) when its dimension is positive, zero, or negative at the Gaussian fixed point. Thus gauge and scalar-quartic interactions are marginal in $d=4$, the mixed two-scalar fermion bilinear is marginal in $d=3$, and four-fermion interactions are marginal in $d=2$. Quantum corrections replace this engineering classification near an interacting fixed point by the eigenvalues of its RG stability matrix.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The one-loop four-scalar one-particle-irreducible diagrams, together with permutations of the external scalar labels, are:

- a scalar bubble with two scalar-quartic vertices;
- a gauge-scalar box with four $A\phi\phi$ vertices;
- a triangle with two $A\phi\phi$ vertices and one $AA\phi\phi$ seagull vertex;
- a gauge bubble with two $AA\phi\phi$ seagull vertices;
- when the mixed operators $\mathcal I_A$ are present, a fermion bubble with two $\phi^2\bar\psi\psi$ vertices.

The first four are forced by the scalar covariant derivative and scalar potential. There is no ordinary Yukawa fermion box because the imposed $\phi\mapsto-\phi$ symmetry forbids a one-scalar fermion vertex.

## 4

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Treat the [BRST transformation](../../../relativistic-quantum-field.md#brst-symmetry) $Q$ as an odd graded derivation. In matrix notation the first three transformations are

$$
QA_\mu=D_\mu c,
\qquad
Qc=-\frac{ig}{2}[c,c]_{\mathrm{graded}},
\qquad
Q\psi=igc\psi.
$$

Then

$$
Q^2A_\mu=D_\mu(Qc)-ig[QA_\mu,c]_{\mathrm{graded}}=0
$$

after substituting $Qc$ and using the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Similarly, the two terms in

$$
Q^2\psi=ig(Qc)\psi-igc(Q\psi)
$$

cancel because the ghost components anticommute and only the Lie-algebra commutator survives. Applying $Q$ once more to $Qc$ gives a sum proportional to $f^d{}_{e[a}f^e{}_{bc]}c^ac^bc^c$, which vanishes by Jacobi. Finally,

$$
Q^2\bar c^a=QB^a=0,
\qquad
Q^2B^a=0.
$$

**Thus $Q^2=0$ on every field.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The gauge-invariant Yang-Mills and matter part $\mathcal L_0$ is BRST invariant because a BRST variation is a gauge transformation with ghost-valued parameter. For the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion)

$$
\Psi=\bar c^a\left(G^a(A)-\frac{\xi}{2}B^a\right),
$$

the graded Leibniz rule gives

$$
Q\Psi
=B^aG^a-\frac{\xi}{2}B^aB^a
-\bar c^a\frac{\delta G^a}{\delta A_\mu^b}D_\mu^{bc}c^c,
$$

up to the common sign convention used to define the ghost term. This is precisely the gauge-fixing, auxiliary-field, and ghost sector of the displayed Lagrangian. Therefore

$$
\boxed{\mathcal L=\mathcal L_0+Q\Psi,
\qquad
Q\mathcal L=Q\mathcal L_0+Q^2\Psi=0.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Under $\Psi\mapsto\Psi+\delta\Psi$, the transition amplitude changes to first order by an insertion

$$
i\int d^4x\,\langle f|\{\widehat Q,\delta\Psi(x)\}|i\rangle.
$$

If

$$
\widehat Q|i\rangle=0,
\qquad
\widehat Q|f\rangle=0,
$$

with the corresponding condition on the bra, the two terms vanish after moving $\widehat Q$ to the external states. The amplitude is then independent of the gauge-fixing choice.

Conversely, invariance for arbitrary changes of the gauge-fixing fermion requires physical external states to be [BRST closed](../../../relativistic-quantum-field.md#brst-cohomology). States differing by a BRST-exact state have identical matrix elements against closed states, so the physical state space is the cohomology

$$
\boxed{\ker\widehat Q/\operatorname{im}\widehat Q.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
