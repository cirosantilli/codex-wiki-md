# Paper 354

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_354.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_354.pdf)

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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)

## 1

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Under the [state–operator correspondence](../../../string-theory.md#state-operator-correspondence), let $|O_{ij}\rangle$ be the state of the antisymmetric [conformal primary operator](../../../string-theory.md#conformal-primary-operator) $O_{ij}$. In radial quantization $P_i^\dagger=K_i$, while primarity gives $K_i|O_{jk}\rangle=0$. The norm of the level-one descendant obtained by taking a divergence is therefore determined by the [conformal algebra](../../../string-theory.md#conformal-algebra) commutator

$$
[K_a,P_b]=2i(\delta_{ab}D-M_{ab}).
$$

Using the two-form action of $M_{ab}$ gives, up to a positive normalization,

$$
\|P^i|O_{ij}\rangle\|^2
\propto(\Delta-d+2)\|O\|^2.
$$

Positivity of norm yields the two-form [conformal unitarity bound](../../../string-theory.md#conformal-unitarity-bound)

$$
\boxed{\Delta\geq d-2\qquad(d\geq4).}
$$

At saturation the descendant is null, and the operator obeys the conservation equation $\partial^iO_{ij}=0$.

In $d=3$, Hodge duality turns the two-form into the vector primary $V_k=\epsilon_{kij}O^{ij}/2$. The vector divergence descendant has norm proportional to $\Delta-d+1=\Delta-2$. Consequently the stronger bound is

$$
\boxed{\Delta\geq2\qquad(d=3),}
$$

rather than the formal two-form value $d-2=1$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Varying the two-form action gives the gauge-invariant equation

$$
\boxed{\nabla_aF^{abc}=0,\qquad F=dA.}
$$

Choose radial gauge $A_{zi}=0$ and boundary-transverse gauge $\partial^iA_{ij}=0$. In the Poincare patch of $\operatorname{AdS}_6$, $\sqrt{-g}=z^{-6}$, while raising the three indices of $F$ contributes $z^6$. The boundary components consequently obey

$$
\boxed{(\partial_z^2+\eta^{kl}\partial_k\partial_l)A_{ij}=0.}
$$

The near-boundary indicial equation is $\alpha(\alpha-1)=0$, so

$$
A_{ij}(z,x)=J_{ij}(x)+zA^{(1)}_{ij}(x)+\cdots.
$$

Under the bulk dilation $(z,x)\mapsto(\lambda z,\lambda x)$, a two-form component carries two powers of inverse length. Thus the leading coefficient has dimension $2$, while the coefficient of $z$ has dimension $3$:

$$
\boxed{\Delta_J=2,\qquad\Delta_O=3.}
$$

The leading freely specifiable, nonnormalizable coefficient is the CFT source $J_{ij}$. The subleading normalizable coefficient is its canonical response and determines $\langle O_{ij}\rangle$. This agrees with the saturated two-form unitarity bound $\Delta_O=d-2=3$ in the five-dimensional boundary CFT and with the [holographic dictionary](../../../string-theory.md#holographic-dictionary) for a massless bulk gauge field.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Translation invariance supplies the momentum-conserving delta function. Lorentz invariance, symmetry of $T_{ij}$, stress-tensor conservation, and tracelessness then fix the remaining tensor structure to the transverse traceless spin-two projector shown in the question, up to an overall theory-dependent coefficient. Since the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) has scaling dimension $d$, its momentum transform has dimension zero. The delta function has momentum dimension $-d$, so scale invariance requires

$$
\boxed{\beta=d.}
$$

For the Wightman function, the spectral condition restricts support to the appropriate future-directed timelike momenta, with convention-dependent distributions on the null boundary. It vanishes for spacelike momentum. A time-ordered or Euclidean correlator is obtained by analytic continuation and exists more broadly, but polynomial contact terms are renormalization-scheme dependent; in even dimensions the nonlocal power is accompanied by a logarithm.

In a large-$N$ holographic CFT, the single-trace state $T_{ij}(p)|0\rangle$ is dual at leading order to a one-graviton bulk state with the matching boundary momentum and polarization. Multiparticle intermediate states and graviton interactions enter at subleading orders in $1/N$.

## 2

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose a constant-time boundary interval whose endpoints differ by $\pi$ in $\phi$. Its [Ryu–Takayanagi formula](../../../string-theory.md#ryu-takayanagi-formula) surface is the diameter through $r=0$. Cutting it off at $r_c=\pi/2-\epsilon$, its length is

$$
\ell=2R_{\rm AdS}\int_0^{r_c}\frac{dr}{\cos r}
=2R_{\rm AdS}\log(\sec r_c+\tan r_c)
=2R_{\rm AdS}\log\frac2\epsilon+O(\epsilon^2).
$$

The [holographic entanglement entropy](../../../string-theory.md#holographic-entanglement-entropy) is therefore

$$
S=\frac\ell{4G}
=\frac{R_{\rm AdS}}{2G}\log\epsilon^{-1}+\text{finite}
=\boxed{\frac c3\log\epsilon^{-1}+\text{finite},}
$$

where the [Brown--Henneaux central charge](../../../string-theory.md#brown-henneaux-central-charge) $c=3R_{\rm AdS}/(2G)$ was used.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $R=R_{\rm AdS}$ and $r_c=\pi/2-\epsilon$. For $\operatorname{AdS}_3$, $\mathcal R=-6/R^2$ and $\Lambda=-1/R^2$, while

$$
\sqrt{-g}=R^3\frac{\sin r}{\cos^3r}.
$$

The bulk term is

$$
I_{\rm bulk}=-\frac{R\Delta t}{4G}(\sec^2r_c-1).
$$

With the inward normal $n^r=-\cos r/R$, the induced metric has $\sqrt{-h}=R^2\sin r/\cos^2r$ and

$$
K=-\frac1R\left(\frac{\cos^2r}{\sin r}+2\sin r\right).
$$

The [Gibbons–Hawking–York boundary term](../../../general-relativity.md#gibbons-hawking-york-boundary-term) is consequently

$$
I_{\rm GHY}=\frac{R\Delta t}{4G}(1+2\tan^2r_c).
$$

Thus, with the orientation and Lorentzian signs displayed in the question,

$$
\boxed{I_{\rm GR}=\frac{R\Delta t}{4G}\sec^2r_c
=\frac{R\Delta t}{4G}\csc^2\epsilon.}
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The divergence is local in the induced boundary metric and is cancelled by the leading [holographic renormalization](../../../string-theory.md#holographic-renormalization) counterterm

$$
\boxed{I_{\rm ct}=-\frac1{8\pi GR}\int_{\partial M}d^2y\sqrt{-h}.}
$$

On the regulated cylinder this is

$$
I_{\rm ct}=-\frac{R\Delta t}{4G}
\frac{\cos\epsilon}{\sin^2\epsilon}
=-\frac{R\Delta t}{4G}\left(\epsilon^{-2}-\frac16+O(\epsilon^2)\right),
$$

which cancels the $\epsilon^{-2}$ divergence of $I_{\rm GR}$. An overall sign changes if one uses the oppositely signed Euclidean generating functional; the local counterterm changes with it.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The stated finite value

$$
\frac1{\Delta t}I_{\rm ren}=-\frac c{12}
$$

is the [Casimir energy of a two-dimensional conformal field theory](../../../string-theory.md#casimir-energy-of-a-two-dimensional-conformal-field-theory) on the unit spatial circle. The plane-to-cylinder conformal map shifts the Hamiltonian by $-c/12$, so the global $\operatorname{AdS}_3$ vacuum is dual to the CFT cylinder vacuum rather than to a state of zero cylinder energy. The sign assigned directly to the Lorentzian on-shell action depends on whether it is identified with the action density or with the vacuum-energy generating functional; the universal boundary datum is the vacuum energy $E_0=-c/12$ supplied in the question.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
