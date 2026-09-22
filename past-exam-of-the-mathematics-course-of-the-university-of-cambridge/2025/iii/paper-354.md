# Paper 354

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_354.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_354.pdf)

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
  - [c](#2/c)
    - [Solution](#2/c/solution)

## 1

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $|\mathcal O\rangle$ be the state associated with a scalar [conformal primary operator](../../../string-theory.md#conformal-primary-operator) of [scaling dimension](../../../string-theory.md#scaling-dimension) $\Delta$. In radial quantization,

$$
K_a|\mathcal O\rangle=0,\qquad
M_{ab}|\mathcal O\rangle=0,\qquad
D|\mathcal O\rangle=i\Delta|\mathcal O\rangle,
$$

and $P_a^\dagger=-K_a$. The norm of a level-one [conformal descendant](../../../string-theory.md#conformal-descendant) is

$$
\langle\mathcal O|(-K_a)P_b|\mathcal O\rangle
=-\langle\mathcal O|[K_a,P_b]|\mathcal O\rangle
=2\Delta\,\delta_{ab}.
$$

Unitarity first gives $\Delta\geq0$. If $\Delta=0$, every $P_a|\mathcal O\rangle$ is null, so the local operator is translation invariant and belongs to the identity conformal family. Excluding the identity therefore gives $\Delta>0$.

Now consider the scalar level-two descendant $P^2|\mathcal O\rangle$. The [conformal algebra](../../../string-theory.md#conformal-algebra) and the scalar-primary conditions give

$$
[K_a,P^2]|\mathcal O\rangle
=-2(2\Delta-d+2)P_a|\mathcal O\rangle.
$$

Applying the second $K_a$ and summing over $a$ yields

$$
\|P^2|\mathcal O\rangle\|^2
=\langle\mathcal O|K^2P^2|\mathcal O\rangle
=8d\Delta\left(\Delta-\frac{d-2}{2}\right)
\langle\mathcal O|\mathcal O\rangle.
$$

Positivity of this norm, together with $\Delta>0$, proves the scalar [conformal unitarity bound](../../../string-theory.md#conformal-unitarity-bound)

$$
\boxed{\Delta\geq\frac{d-2}{2}}.
$$

At equality the level-two descendant is null; in position space this is the free scalar equation of motion.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For the Poincaré metric on $\operatorname{AdS}_6$,

$$
\sqrt{|g|}=z^{-6},\qquad g^{ab}=z^2\eta^{ab}.
$$

The massless [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation), evaluated with the [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator), is

$$
\nabla^2\phi
=z^6\partial_z(z^{-4}\partial_z\phi)+z^2\Box_5\phi=0,
$$

or

$$
\boxed{z^2\phi_{zz}-4z\phi_z+z^2\Box_5\phi=0}.
$$

A boundary power $\phi\sim z^\alpha$ obeys the indicial equation

$$
\alpha(\alpha-5)=0.
$$

Thus

$$
\phi(z,x)=J(x)+z^5A(x)+\cdots.
$$

The constant branch is the nonnormalizable source and the $z^5$ branch is the normalizable response. Since $m^2=\Delta(\Delta-d)=0$ with $d=5$, the roots are $\Delta_-=0$ and $\Delta_+=5$. Only standard quantization is unitary here: the putative alternative operator of dimension zero would be the identity, whereas the field is a nontrivial fluctuating operator. The permissible conformally invariant source-free boundary condition is therefore Dirichlet,

$$
\boxed{J=0,\qquad \phi=O(z^5)}.
$$

More generally one may prescribe $J$ as an external source. The [holographic dictionary](../../../string-theory.md#holographic-dictionary) gives

$$
\boxed{[\mathcal O]=5,\qquad [J]=d-\Delta=0}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For a boundary-independent source, the [AdS scalar-field boundary asymptotics](../../../string-theory.md#ads-scalar-field-boundary-asymptotics) reduce to

$$
\phi(z)=J+z^5A+o(z^5).
$$

One may therefore extract the source and response directly:

$$
\boxed{J=\lim_{z\to0}\phi(z)},
\qquad
\boxed{A=\lim_{z\to0}z^{-5}\bigl(\phi(z)-J\bigr)
=\frac15\lim_{z\to0}z^{-4}\partial_z\phi}.
$$

The operator expectation value is proportional to $A$; choosing the boundary-operator normalization $\mathcal O=A$ gives the requested expressions. A conventional action normalization can instead multiply this relation by the fixed factor $2\Delta-d=5$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

When $J(x)$ varies, the radial wave equation recursively generates local derivative terms before the normalizable response. Substituting

$$
\phi=J+z^2\phi_{(2)}+z^4\phi_{(4)}+z^5A+\cdots
$$

into

$$
z^2\phi_{zz}-4z\phi_z+z^2\Box_5\phi=0
$$

gives

$$
\phi_{(2)}=\frac16\Box_5J,
\qquad
\phi_{(4)}=\frac1{24}\Box_5^2J.
$$

Because the boundary dimension is odd, no logarithmic term is required. [Holographic renormalization](../../../string-theory.md#holographic-renormalization) subtracts these source-dependent pieces, leaving

$$
\boxed{
\mathcal O(x)=
\lim_{z\to0}z^{-5}
\left[
\phi(z,x)-J(x)
-\frac{z^2}{6}\Box_5J(x)
-\frac{z^4}{24}\Box_5^2J(x)
\right]}
$$

in the normalization $\mathcal O=A$. Equivalently,

$$
\boxed{
\mathcal O(x)=\frac15\lim_{z\to0}z^{-4}
\left[
\partial_z\phi
-\frac z3\Box_5J
-\frac{z^3}{6}\Box_5^2J
\right]}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [state–operator correspondence](../../../string-theory.md#state-operator-correspondence) maps $\mathcal O$ to the lowest one-particle state on $S^4\times\mathbb R$. On a sphere of radius $r$, cylinder energy equals scaling dimension divided by $r$. The primary has $\Delta=5$.

A translation generator raises the dimension by one and transforms as a vector of $SO(5)$. States with no angular momentum arise from scalar descendant pairs $P^2$, so the allowed descendants are

$$
(P^2)^n\mathcal O,\qquad n=0,1,2,\ldots.
$$

Their dimensions are $5+2n$, and hence the one-quantum, zero-angular-momentum energies are

$$
\boxed{E_n=\frac{5+2n}{r},\qquad n=0,1,2,\ldots}.
$$

These are the $l=0$ normal-mode energies of a massless scalar in global [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime).

## 2

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Ryu–Takayanagi formula](../../../string-theory.md#ryu-takayanagi-formula) gives the leading entropy of a static boundary region:

$$
S(D_1)=\frac{\operatorname{Area}(\gamma_{D_1})}{4G}.
$$

On the $t=0$ slice of Poincaré $\operatorname{AdS}_4$,

$$
ds^2=\frac{dz^2+d\rho^2+\rho^2d\theta^2}{z^2}.
$$

The [minimal surface](../../../second-fundamental-form.md#minimal-surface) anchored on a boundary circle of radius $R_1$ is the hemisphere

$$
z^2+\rho^2=R_1^2.
$$

Cutting it off at $z=\epsilon$, its area is

$$
\begin{aligned}
A_\epsilon
&=2\pi R_1\int_0^{\sqrt{R_1^2-\epsilon^2}}
\frac{\rho\,d\rho}{(R_1^2-\rho^2)^{3/2}}\\
&=2\pi\left(\frac{R_1}{\epsilon}-1\right).
\end{aligned}
$$

Therefore

$$
\boxed{
S(D_1)=\frac{\pi R_1}{2G\epsilon}
-\frac{\pi}{2G}}.
$$

The universal requirement was the perimeter-law divergence $\pi R_1/(2G\epsilon)$; the finite constant depends on the stated pure $\operatorname{AdS}_4$ vacuum geometry and equals $-\pi/(2G)$ here. Since $G\sim N^{-3/2}$, both terms are of order $N^{3/2}$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $\gamma_1$ and $\gamma_2$ be the individual Ryu–Takayanagi surfaces for $D_1$ and $D_2$. Their disconnected union $\gamma_1\cup\gamma_2$ is homologous to $D_1\cup D_2$ and is therefore an admissible competitor in the minimization that defines $\gamma_{12}$. Minimality gives

$$
\operatorname{Area}(\gamma_{12})
\leq\operatorname{Area}(\gamma_1)
+\operatorname{Area}(\gamma_2).
$$

Dividing by $4G$ proves

$$
S(D_1\cup D_2)\leq S(D_1)+S(D_2),
$$

and hence the leading [holographic mutual information](../../../string-theory.md#holographic-mutual-information) obeys

$$
\boxed{I_c\geq0}.
$$

This is the geometric realization of the nonnegativity of [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

There are two competing extremal-surface topologies. The disconnected candidate $\gamma_1\cup\gamma_2$ has area independent of the separation $L$ and gives $I_c=0$. A connected surface joining the two boundary circles can have smaller area when the gap is small; as $L\to0$, short-distance entanglement across the nearby boundaries makes $I_c$ positive and divergent.

Increasing $L$ makes the connected candidate less favorable. At a critical separation $L=C(R_1,R_2)$ its area equals the disconnected area, and beyond that point the disconnected candidate is minimal. This [entanglement-wedge phase transition](../../../string-theory.md#entanglement-wedge-phase-transition) gives

$$
\boxed{I_c>0\quad(L<C),
\qquad
I_c=0\quad(L>C).}
$$

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Write $S_{\rm conn}(L)$ for the connected candidate and

$$
S_{\rm disc}=S(D_1)+S(D_2)
$$

for the $L$-independent disconnected candidate. The physical entropy is the lower envelope

$$
\boxed{S(D_1\cup D_2)=\min\{S_{\rm conn}(L),S_{\rm disc}\}}.
$$

Near $L=C$, the connected branch rises to meet the horizontal disconnected branch. The entropy is continuous but generically has a kink there: its derivative jumps from the positive slope of $S_{\rm conn}$ to zero. Correspondingly, $I_c=S_{\rm disc}-S(D_1\cup D_2)$ falls to zero and remains zero.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A pair of boundary circles has one dimensionless invariant under the [conformal field theory](../../../string-theory.md#conformal-field-theory) group. If their radii are $R_1,R_2$ and their center separation is

$$
d=R_1+R_2+L,
$$

a convenient invariant is the [inversive distance](../../../geometry-and-topology.md#inversive-distance)

$$
\chi=\frac{d^2-R_1^2-R_2^2}{2R_1R_2}.
$$

The choice between connected and disconnected bulk surfaces can depend only on $\chi$. Let the transition occur at the single theory-independent numerical value $\chi=X$, with $X>1$. Then

$$
(R_1+R_2+C)^2=R_1^2+R_2^2+2XR_1R_2,
$$

so

$$
\boxed{
C(R_1,R_2)
=\sqrt{R_1^2+R_2^2+2XR_1R_2}-R_1-R_2}.
$$

All dependence on the two radii is fixed by conformal symmetry; only the pure number $X$ requires the explicit minimal-surface calculation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
