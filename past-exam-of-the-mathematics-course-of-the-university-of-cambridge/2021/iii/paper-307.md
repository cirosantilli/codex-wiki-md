# Paper 307

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_307.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_307.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Complex conjugation reverses the order of the Grassmann variables. Thus the conjugate of $i\bar\psi\dot\psi$ differs from itself only by integration by parts, while the remaining terms are manifestly real. The action is therefore real up to a boundary term.

Substituting the stated transformations into the Lagrangian, using anticommutation of $\psi,\bar\psi,\epsilon,\bar\epsilon$, and integrating the terms containing $\ddot x$ and $\dot\psi$ by parts leaves a total derivative. A convenient convention for the resulting [Noether charges](../../../quantum-field-theory.md#noether-charge) is

$$
\boxed{Q=\psi\left(p-ih'(x)\right),
\qquad
\bar Q=\bar\psi\left(p+ih'(x)\right)},
\qquad p=\dot x.
$$

Overall signs can be moved between the charges and the Grassmann transformation parameters. These charges generate the displayed transformations and obey the classical supersymmetry algebra.

Canonical quantization gives

$$
[x,p]=i,
\qquad
\{\psi,\bar\psi\}=1,
\qquad
\psi^2=\bar\psi^2=0,
$$

with all other elementary graded commutators zero. Represent $p=-i\,d/dx$, let $\psi$ act by exterior multiplication by $dx$, and let $\bar\psi$ act by contraction with $\partial_x$. The Hilbert space is then

$$
\mathcal H=L^2\Omega^0(\mathbb R)\oplus L^2\Omega^1(\mathbb R),
$$

the square-integrable complex differential forms on the line. Up to an inessential factor of $-i$, $Q$ is the [twisted de Rham differential](../../../quantum-mechanics.md#twisted-de-rham-differential)

$$
d_h=e^{-h}de^h=d+dh\wedge,
$$

and $\bar Q$ is its Hilbert-space adjoint. The Hamiltonian is $H=\{Q,\bar Q\}/2$, so a zero-energy state must be annihilated by both charges.

On zero-forms the zero-mode equation is $(d/dx+h')u=0$, giving $u=Ce^{-h}$. On one-forms it is $(-d/dx+h')v=0$, giving $v=Ce^h$. For $h=-x^4$, only the one-form is square integrable, so the unique ground state is

$$
\boxed{\Psi_0=C e^{-x^4}dx}.
$$

For a generic cubic polynomial, $h(x)$ tends to opposite infinities at the two ends of the real line. Each of $e^h$ and $e^{-h}$ therefore diverges at one end, so neither candidate is square integrable. There is consequently no normalizable zero-energy state.

## 2

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $\Lambda$ be a chiral gauge parameter. One consistent Abelian [supergauge transformation](../../../supersymmetry.md#supergauge-transformation) convention is

$$
\Phi_i\mapsto e^{-iq_i\Lambda}\Phi_i,
\qquad
\bar\Phi_i\mapsto\bar\Phi_i e^{iq_i\bar\Lambda},
\qquad
V\mapsto V+i(\Lambda-\bar\Lambda),
$$

for which $\bar\Phi_i e^{q_iV}\Phi_i$ is invariant. [Wess-Zumino gauge](../../../supersymmetry.md#wess-zumino-gauge) uses the nonordinary components of $\Lambda$ to remove the superfluous scalar and spinor components of $V$, leaving the photon, gauginos, complex scalar, and real auxiliary field of the two-dimensional vector multiplet. Ordinary $U(1)$ gauge transformations remain.

Define the field-strength multiplet, up to conventional normalization, by

$$
\boxed{\Sigma=\bar D_+D_-V}.
$$

Gauge invariance follows because chirality, antichirality, $\bar D_+^2=D_-^2=0$, and $\{\bar D_+,D_-\}=0$ annihilate the variation of $V$. The same identities give

$$
\bar D_+\Sigma=0,
\qquad
D_-\Sigma=0,
$$

so $\Sigma$ is a [twisted chiral superfield](../../../supersymmetry.md#twisted-chiral-superfield). The [Fayet–Iliopoulos term](../../../supersymmetry.md#fayet-iliopoulos-term) is a twisted F-term. In the standard axial convention its measure $d\theta^+d\bar\theta^-$ has axial charge $-2$, so invariance requires

$$
\boxed{q_A(\Sigma)=+2}.
$$

Reversing all axial-charge conventions reverses both signs but leaves this statement unchanged: the field and measure have opposite charges.

The charged matter fermions are chiral with respect to the axial symmetry. In a background with gauge flux, their [functional measure](../../../quantum-field-theory.md#functional-measure) has the two-dimensional axial anomaly

$$
\partial_\mu j_A^\mu=\frac1\pi\left(\sum_iq_i\right)F_{01}
$$

up to orientation and current normalization. Equivalently, a Fujikawa transformation multiplies the torus path integral by a phase proportional to $\alpha(\sum_iq_i)\int F$. Since the background flux may be nonzero, the continuous axial $U(1)$ survives quantum mechanically precisely when

$$
\boxed{\sum_iq_i=0}.
$$

## 3

↑ **Parent:** [Paper 307](paper-307.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Put $\theta=\theta^+$, $\bar\theta=\bar\theta^+$ and $y^+=x^++i\theta\bar\theta$. The general [two-dimensional N=(0,2) supersymmetry](../../../supersymmetry.md#two-dimensional-n-0-2-supersymmetry) chiral superfield is

$$
\boxed{\Phi(y^+,x^-,\theta)=\phi(y^+,x^-)+\sqrt2\theta\psi_+(y^+,x^-)}.
$$

In ordinary coordinates this is $\Phi=\phi+\sqrt2\theta\psi_++i\theta\bar\theta\partial_+\phi$. A supersymmetric kinetic action is

$$
\boxed{S_1=-\frac i2\int d^2x\,d\theta d\bar\theta\,
\bar\Phi\partial_-\Phi},
$$

whose component form, up to light-cone conventions and total derivatives, is

$$
S_1=\int d^2x\left[-\partial_\mu\bar\phi\partial^\mu\phi
+i\bar\psi_+\partial_-\psi_+\right].
$$

A [Fermi superfield](../../../supersymmetry.md#fermi-superfield) satisfying $\bar D_+\Lambda_-=f(\Phi)$ has expansion

$$
\boxed{\Lambda_-=\lambda_- -\sqrt2\theta G-\bar\theta f(\phi)
+\theta\bar\theta\left(i\partial_+\lambda_-
+\sqrt2\psi_+^i\partial_i f\right)}.
$$

Here $G$ is a complex bosonic [auxiliary field](../../../supersymmetry.md#auxiliary-field). With the normalization in the question, the component action is

$$
\begin{aligned}
S_2=\int d^2x\bigg[&i\bar\lambda_-\partial_+\lambda_-+|G|^2
-\frac12|f|^2\\
&-\frac1{\sqrt2}\left(\bar\lambda_-\psi_+^i\partial_i f
+\bar\psi_+^{\bar i}\partial_{\bar i}\bar f\,\lambda_-\right)
\bigg],
\end{aligned}
$$

up to equivalent sign conventions for the fermions.

The chiral integral in $S_3$ is supersymmetric only if its integrand is chiral. Applying $\bar D_+$ gives the necessary and sufficient condition

$$
\boxed{\sum_a f_a(\Phi)J^a(\Phi)=0},
$$

with every $J^a$ holomorphic and with gauge charges chosen so that each product $\Lambda_{-a}J^a$ is gauge invariant. Its component expansion couples $G_a$ linearly to $J^a$ and supplies the corresponding Yukawa term $\lambda_{-a}\psi_+^i\partial_iJ^a$.

Eliminating each $G_a$ by its algebraic field equation gives the nonnegative scalar potential. In the normalization displayed above and in the question,

$$
\boxed{V(\phi)=\frac12\sum_a|f_a(\phi)|^2
+2\sum_a|J^a(\phi)|^2}.
$$

If the conventional definitions $\bar D_+\Lambda_-^a=\sqrt2E_a$ and $S_J=-\int d\theta\,\Lambda_{-a}J^a/\sqrt2+\mathrm{h.c.}$ are used instead, the same result is written $V=\sum_a(|E_a|^2+|J^a|^2)$; the two forms differ only by the normalization of $f$ and $J$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
