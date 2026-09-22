# Paper 304

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_304.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_304.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)

## 1

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) contains the following [diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram). For $\Gamma_2$, there are the tree inverse propagator, the one-loop tadpole at order $\lambda$, and at order $\lambda^2$ the two-loop sunset and the two-loop tadpole with a tadpole insertion. For $\Gamma_4$, there are the tree vertex $-i\lambda$ and, at order $\lambda^2$, the three one-loop bubble diagrams in the $s$, $t$, and $u$ channels. Disconnected and one-particle-reducible graphs do not occur in the quantum effective action.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

After [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation), the zero-momentum bubble integral with [cutoff regularization](../../../perturbative-quantum-field-theory.md#cutoff-regularization) is

$$
I(0)=\int_{|k|<\Lambda}\frac{d^4k}{(2\pi)^4}\frac1{(k^2+m^2)^2}
=\frac1{16\pi^2}\left[\log\frac{\Lambda^2+m^2}{m^2}+\frac{m^2}{\Lambda^2+m^2}-1\right].
$$

The three channels contribute $3\lambda^2I(0)/2$. For $\Lambda\gg m$, this is $\frac{3\lambda^2}{32\pi^2}[\log(\Lambda^2/m^2)-1]$, so the zero-momentum [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) is enforced by

$$
\delta_\lambda=-\frac{3\lambda^2}{32\pi^2}\log\frac{\Lambda^2}{e m^2},
$$

and hence $F=e m^2$. Keeping the exact cutoff expression merely replaces $F$ by the finite cutoff-dependent quantity defined by $\log(\Lambda^2/F)=16\pi^2I(0)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Introducing a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) and subtracting at zero external momentum give

$$
\Gamma_4(s,t,u)=\lambda+\frac{\lambda^2}{32\pi^2}
\sum_{q^2=s,t,u}\int_0^1dx\,
\log\frac{m^2}{m^2-x(1-x)q^2-i\epsilon}+O(\lambda^3).
$$

The bare coupling $\lambda_0=\lambda+\delta_\lambda$ is independent of the [renormalization scale](../../../perturbative-quantum-field-theory.md#renormalization-scale). Differentiating its logarithmic counterterm at fixed $\lambda_0$ gives the leading [beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics)

$$
\boxed{\beta_\lambda=\mu\frac{d\lambda}{d\mu}=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3)}.
$$

## 2

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Completing the square in the [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) and choosing

$$
\mathcal N^{-1}=\int\mathcal D\phi\,
\exp\left(i\int d^4x\,\mathcal L_b\right)
$$

normalizes $Z_0[0]=1$. The result is

$$
Z_0[J]=\exp\left[-\frac12\int d^4x,d^4y\,J(x)D_F(x-y)J(y)\right],
$$

where the [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator) in the convention of the question is

$$
\boxed{D_F(x-y)=\int\frac{d^4p}{(2\pi)^4}\frac{i,e^{-ip\cdot(x-y)}}{p^2-M^2+i\epsilon}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The analogous [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral), normalized by $Z_0[0,0]=1$, gives

$$
Z_0[\bar\eta,\eta]=\exp\left[-\int d^4x,d^4y\,
\bar\eta(x)S_F(x-y)\eta(y)\right],
$$

with the free [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator)

$$
S_F(x-y)=\int\frac{d^4p}{(2\pi)^4}
\frac{i(\not p+m)e^{-ip\cdot(x-y)}}{p^2-m^2+i\epsilon}.
$$

Indeed $(i\not\partial_x-m)S_F(x-y)=i\delta^{(4)}(x-y)$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

With left [functional derivatives](../../../calculus-of-variations.md#functional-derivative) for the Grassmann sources, replace fields in the interaction by $\phi\mapsto i^{-1}\delta/\delta J$, $\psi\mapsto i^{-1}\delta/\delta\bar\eta$, and $\bar\psi\mapsto-i^{-1}\delta/\delta\eta$. Thus

$$
Z[\bar\eta,\eta,J]=
\exp\left[-ig\int d^4x
\left(-\frac1i\frac\delta{\delta\eta(x)}\right)
\left(\frac1i\frac\delta{\delta J(x)}\right)
\left(\frac1i\frac\delta{\delta\bar\eta(x)}\right)
\right]Z_{0,f}[\bar\eta,\eta]Z_{0,b}[J].
$$

The ordering displayed fixes the Grassmann signs and makes this an explicit source functional with no dynamical fields.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For momenta much smaller than $M$,

$$
\frac{i}{p^2-M^2+i\epsilon}=-\frac{i}{M^2}+O(p^2/M^4),
\qquad
D_F(x-y)=-\frac{i}{M^2}\delta^{(4)}(x-y)+O(M^{-4}).
$$

Expanding the source functional to order $g^2$, equivalently integrating out the heavy scalar by its field equation, produces

$$
\mathcal L_{\rm eff}=\bar\psi(i\not\partial-m)\psi
+\frac{g^2}{2M^2}(\bar\psi\psi)^2+O(M^{-4},g^4).
$$

**Thus the four-spinor coefficient is $g^2/(2M^2)$ in this normalization. Since $[\psi]=3/2$ and $[g]=0$ in four dimensions, $(\bar\psi\psi)^2$ has dimension six and its coefficient has the required dimension $-2$.**

## 3

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The first three terms are the scalar kinetic, mass, and $n$-point interaction terms. The remaining terms are the field-strength, mass, and coupling [counterterms](../../../perturbative-quantum-field-theory.md#counterterm). The momentum-space rules are

$$
\frac{i}{p^2-m^2+i\epsilon},\qquad -i\lambda,
\qquad i(\delta_Zp^2-\delta_{m^2}),\qquad -i\delta_\lambda,
$$

for a propagator, an $n$-leg interaction vertex, a two-leg counterterm insertion, and an $n$-leg counterterm vertex, respectively, together with momentum conservation at every vertex.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $d=6-\epsilon$. The one-loop two-point bubble has symmetry factor $1/2$ and, after a Feynman parameter and momentum shift, its pole is proportional to

$$
-\frac{2}{(4\pi)^3\epsilon}\int_0^1dx\,[m^2+x(1-x)p_E^2]
=-\frac{2}{(4\pi)^3\epsilon}\left(m^2+\frac{p_E^2}{6}\right).
$$

Cancelling the pole in the [minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#minimal-subtraction-scheme) gives, with $\epsilon=6-d$,

$$
\boxed{\delta_Z=-\frac{\lambda^2}{6(4\pi)^3\epsilon},\qquad
\delta_{m^2}=-\frac{\lambda^2m^2}{(4\pi)^3\epsilon}}.
$$

If one defines dimensional regularization by $d=6-2\epsilon$, these same poles are written with $2\epsilon$ in place of $\epsilon$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The scalar has canonical dimension $[\phi]=(d-2)/2$, so

$$
[\lambda]=d-6\frac{d-2}{2}=6-2d.
$$

The $\phi^6$ coupling is therefore marginal in $d=3$. Its leading two-point correction is the order-$\lambda$ diagram with one six-leg vertex, two external legs, and the remaining four legs paired into two tadpole loops. This diagram is independent of external momentum, so it renormalizes the mass but has no $p^2$ pole and does not contribute to $\delta_Z$.

## 4

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Substitution of the gauge transformations and $UU^\dagger=I$ gives

$$
D_\mu'\phi'=U(D_\mu\phi)U^\dagger.
$$

A direct commutator calculation gives

$$
[D_\mu,D_\nu]\phi=-ig[F_{\mu\nu},\phi].
$$

Covariance of the left side then implies $F'_{\mu\nu}=UF_{\mu\nu}U^\dagger$. The [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace) makes the traces of $F_{\mu\nu}F^{\mu\nu}$, $D_\mu\phi D^\mu\phi$, and $\phi^3$ invariant, so the Lagrangian is [gauge invariant](../../../relativistic-quantum-field.md#gauge-invariance).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The product of generators satisfies

$$
T_aT_b=\frac1{2N}\delta_{ab}I
+\frac12(d_{ab}{}^c+if_{ab}{}^c)T_c,
$$

and therefore

$$
\operatorname{Tr}(T_aT_bT_c)=\frac14(d_{abc}+if_{abc}).
$$

Because $\phi^a\phi^b\phi^c$ is symmetric, its contraction with the antisymmetric [structure constant of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) $f_{abc}$ vanishes. Hence

$$
\boxed{-\frac1{3!}\operatorname{Tr}(\phi^3)
=-\frac1{24}d_{abc}\phi^a\phi^b\phi^c.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

For the Grassmann-odd ghost $c$, the [BRST transformations](../../../relativistic-quantum-field.md#brst-symmetry) are

$$
QA_\mu=D_\mu c=\partial_\mu c-ig[A_\mu,c],
\qquad
Q\phi=ig[c,\phi],
\qquad
Qc=igc^2,
$$

up to a simultaneous convention-dependent sign for $Q$ and $c$. The ghost transformation makes the [BRST charge](../../../relativistic-quantum-field.md#brst-charge) nilpotent: $Q^2A_\mu=Q^2\phi=0$.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Gauge invariance gives $Q\int\mathcal L=0$. Nilpotence gives $Q^2\Psi=0$, and therefore

$$
QS=Q\int\mathcal L+Q^2\Psi=0.
$$

**Thus writing the gauge-fixing contribution as a BRST-exact term makes the complete action [BRST invariant](../../../relativistic-quantum-field.md#brst-symmetry).**

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

An infinitesimal change of gauge-fixing fermion, $\Psi\mapsto\Psi+\delta\Psi$, changes the action by the BRST-exact term $Q\delta\Psi$. If $\mathcal O$ is gauge invariant, then $Q\mathcal O=0$. BRST invariance of the measure gives the [BRST Ward identity](../../../relativistic-quantum-field.md#brst-ward-identity) $\langle QX\rangle=0$, so the normalized variation is

$$
\delta\langle\mathcal O\rangle
=i\langle\mathcal O,Q\delta\Psi\rangle_c
=i\langle Q(\mathcal O\,\delta\Psi)\rangle_c=0.
$$

**Therefore correlation functions of gauge-invariant operators do not depend on the choice of gauge, provided there is no BRST anomaly or boundary contribution.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
