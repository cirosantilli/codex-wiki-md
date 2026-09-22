# Paper 337

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_337.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_337.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)

## 1

↑ **Parent:** [Paper 337](paper-337.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

After [integration by parts](../../../calculus.md#integration-by-parts), define the Euclidean quadratic operator

$$
K[\lambda]=-partial_\tau^2-v^2\nabla^2+i\lambda.
$$

The action can then be written as

$$
S=\frac1{2vg}\sum_{a=1}^N
\langle n_a,K[\lambda]n_a\rangle
-\frac{iN}{2vg}\int d^2x\,d\tau\,\lambda.
$$

Each component of $\mathbf n$ gives the same bosonic [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral), so

$$
\int\mathcal D\mathbf n\,
e^{-\frac1{2vg}\sum_a\langle n_a,Kn_a\rangle}
\propto(\det K)^{-N/2}.
$$

Discarding a $\lambda$-independent normalization, the remaining [functional determinant](../../../quantum-field-theory.md#functional-determinant) gives

$$
\boxed{
Z=\int\mathcal D\lambda\,e^{-\widetilde S[\lambda]},
\qquad
\widetilde S[\lambda]
=\frac N2\operatorname{Tr}\log K[\lambda]
-\frac{iN}{2vg}\int d^2x\,d\tau\,\lambda.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Every term in $\widetilde S$ is proportional to $N$. The [Large-N expansion](../../../quantum-field-theory.md#large-n-expansion) therefore suppresses fluctuations of the auxiliary field by powers of $1/N$, and the leading partition function comes from a [saddle-point approximation](../../../analysis.md#saddle-point-approximation).

Vary with respect to $i\lambda$ and use $\delta\operatorname{Tr}\log K=\operatorname{Tr}(K^{-1}\delta K)$. At a translation-invariant saddle $i\lambda=m^2$, the [gap equation](../../../quantum-field-theory.md#gap-equation) is

$$
\boxed{
\frac1{vg}
=T\sum_{n\in\mathbb Z}
\int\frac{d^2k}{(2\pi)^2}
\frac1{\omega_n^2+v^2k^2+m^2},
\qquad \omega_n=2\pi nT.}
$$

The frequencies are the bosonic [Matsubara frequencies](../../../quantum-field-theory.md#matsubara-frequency) imposed by periodicity around the imaginary-time thermal circle.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At zero temperature, the [Matsubara sum](../../../quantum-field-theory.md#bosonic-matsubara-sum) becomes a frequency integral:

$$
\frac1{vg}
=\int_{|\mathbf k|<\Lambda}\frac{d^2k}{(2\pi)^2}
\int_{-\infty}^{\infty}\frac{d\omega}{2\pi}
\frac1{\omega^2+v^2k^2+m^2}.
$$

The frequency integral is $1/(2\sqrt{v^2k^2+m^2})$, and radial momentum integration gives

$$
\frac1{vg}
=\frac{\sqrt{v^2\Lambda^2+m^2}-m}{4\pi v^2}.
$$

Define the [critical coupling](../../../quantum-field-theory.md#critical-coupling) by the massless equation

$$
\frac1{vg_c}=\frac{\Lambda}{4\pi v}.
$$

Taking the cutoff to infinity in the difference gives

$$
\frac1g-\frac1{g_c}=-\frac{m}{4\pi v},
$$

and hence

$$
\boxed{m=\frac{4\pi v(g-g_c)}{gg_c}.}
$$

A positive mass solution exists only for $g>g_c$. For $g<g_c$, the symmetric saddle cannot enforce the constraint with $m^2>0$; instead the $O(N)$ symmetry is [spontaneously broken](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) to $O(N-1)$, the field acquires [Néel order](../../../statistical-physics.md#neel-state), and the ordered phase contains massless [Goldstone bosons](../../../critical-phenomenon.md#goldstone-boson).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For fixed momentum put

$$
E_k=\sqrt{v^2k^2+m(T)^2}.
$$

In the contour formula, $F(z)=1/(E_k^2-z^2)$ has poles at $z=\pm E_k$. Deforming the contour onto those poles and using the oddness of $\coth(z/(2T))$ gives the standard [Bosonic Matsubara sum](../../../quantum-field-theory.md#bosonic-matsubara-sum)

$$
\boxed{
T\sum_{n\in\mathbb Z}
\frac1{\omega_n^2+E_k^2}
=\frac1{2E_k}\coth\left(\frac{E_k}{2T}\right).}
$$

Equivalently,

$$
\frac1{2E_k}\coth\left(\frac{E_k}{2T}\right)
=\frac{1+2n_B(E_k)}{2E_k},
$$

where $n_B(E)=1/(e^{E/T}-1)$ is the [Bose-Einstein distribution](../../../statistical-physics.md#bose-einstein-distribution). The first term is the zero-point fluctuation and the second is its thermal occupation.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The finite-temperature gap equation is

$$
\frac1{vg}
=\int_{|\mathbf k|<\Lambda}
\frac{d^2k}{(2\pi)^2}
\frac1{2E_k}\coth\left(\frac{E_k}{2T}\right).
$$

With $E=\sqrt{v^2k^2+m^2}$, the radial measure obeys $k\,dk=E\,dE/v^2$, so

$$
\frac1{vg}
=\frac{T}{2\pi v^2}
\left[
\log\sinh\left(\frac{E}{2T}\right)
\right]_{m}^{\sqrt{v^2\Lambda^2+m^2}}.
$$

As $\Lambda\to\infty$, subtraction of the massless, zero-temperature equation at $g_c$ leaves

$$
\frac1{vg}-\frac1{vg_c}
=-\frac{T}{2\pi v^2}
\log\left[2\sinh\left(\frac{m}{2T}\right)\right].
$$

The zero-temperature relation with $m=\Delta$ is

$$
\frac1{vg}-\frac1{vg_c}
=-\frac{\Delta}{4\pi v^2}.
$$

Equating the finite parts gives

$$
2\sinh\left(\frac{m}{2T}\right)=e^{\Delta/(2T)},
$$

and therefore

$$
\boxed{
m(T)=2T\operatorname{arsinh}
\left(\frac12e^{\Delta/(2T)}\right).}
$$

The subtraction is a [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition): it trades the cutoff-dependent bare coupling for the physical zero-temperature gap.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

When $T\ll\Delta$, the argument of the inverse hyperbolic sine is large. Using $\operatorname{arsinh}z=\log(2z)+1/(4z^2)+O(z^{-4})$ gives

$$
\boxed{
m(T)=\Delta+2T e^{-\Delta/T}
+O(Te^{-2\Delta/T}).}
$$

The mass remains the zero-temperature gap, with an exponentially small correction from thermally activated excitations.

When $T\gg\Delta$, expand around $z=1/2$. If

$$
\varphi=\frac{1+\sqrt5}{2}
$$

is the [golden ratio](../../../algebra.md#golden-ratio), then $\operatorname{arsinh}(1/2)=\log\varphi$, and

$$
\boxed{
m(T)=2T\log\varphi+\frac{\Delta}{\sqrt5}
+O\left(\frac{\Delta^2}{T}\right).}
$$

The leading value $m/T=2\log\varphi$ is universal. This is the [quantum-critical regime](../../../critical-phenomenon.md#quantum-critical-regime): temperature is the only leading energy scale and the [correlation length](../../../critical-phenomenon.md#correlation-length) is of order $v/T$.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The [analytic continuation](../../../complex-analysis.md#analytic-continuation) from bosonic imaginary frequency to a retarded frequency is $i\omega_n\mapsto\omega+i0^+$. Thus

$$
\boxed{
G_R(\omega,\mathbf k)
=\frac{vg}{N}
\frac1{v^2k^2+m(T)^2-(\omega+i0^+)^2}.}
$$

Writing $E_k=\sqrt{v^2k^2+m(T)^2}$ and using the [Sokhotski–Plemelj formula](../../../complex-analysis.md#sokhotski-plemelj-theorem) gives, in this sign convention,

$$
\boxed{
\operatorname{Im}G_R(\omega,\mathbf k)
=\frac{\pi vg}{2NE_k}
\left[\delta(\omega-E_k)-\delta(\omega+E_k)\right].}
$$

The opposite overall convention for the [retarded Green function](../../../quantum-field-theory.md#retarded-green-function) reverses this sign; the corresponding [spectral function](../../../quantum-field-theory.md#spectral-function) is conventionally chosen positive at positive frequency.

Near the [quantum critical point](../../../critical-phenomenon.md#quantum-critical-point), $m/T$ is a function only of $\Delta/T$. The Green function has the scaling form

$$
G_R(\omega,k;T,\Delta)
=\frac{vg}{N}T^{-2}
\mathcal G\left(\frac\omega T,
\frac{vk}{T},\frac\Delta T\right),
$$

with

$$
\mathcal G^{-1}
=\left(\frac{vk}{T}\right)^2
+\left[2\operatorname{arsinh}
\left(\frac12e^{\Delta/(2T)}\right)\right]^2
-\left(\frac{\omega+i0^+}{T}\right)^2.
$$

This is [quantum critical scaling](../../../critical-phenomenon.md#quantum-critical-scaling) with dynamical critical exponent $z=1$ and leading large-$N$ anomalous dimension $\eta=0$.

## 2

↑ **Parent:** [Paper 337](paper-337.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\eta_i=+1$ and $-1$ on the two sublattices of the square lattice. A unit-vector decomposition that separates staggered and uniform magnetization is

$$
\boxed{
\mathbf n_i
=\eta_i\widetilde{\mathbf n}(\mathbf x_i)
\sqrt{1-|\mathbf m(\mathbf x_i)|^2}
+\mathbf m(\mathbf x_i),}
$$

where

$$
|\widetilde{\mathbf n}|^2=1,
\qquad
\mathbf m\mathbin\cdot\widetilde{\mathbf n}=0,
\qquad
|\mathbf m|\ll1.
$$

The alternating part is the [Néel order parameter](../../../statistical-physics.md#neel-order-parameter), while $\mathbf m$ is the slowly varying [uniform magnetization](../../../statistical-physics.md#uniform-magnetization) generated by canting the two sublattices.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a smooth configuration, neighboring sites lie on opposite sublattices and contribute [Spin coherent-state Berry phases](../../../statistical-physics.md#spin-coherent-state-berry-phase) with opposite orientations. The terms $S\Gamma[\widetilde{\mathbf n}]$ and $S\Gamma[-\widetilde{\mathbf n}]$ therefore cancel pairwise modulo the quantized solid-angle ambiguity. Their smooth bulk contribution vanishes in the [continuum limit](../../../physics.md#continuum-limit).

Singular spacetime configurations can leave lattice Berry phases attached to hedgehog events, but those are outside the smooth sector used in this continuum derivation. Thus the order-parameter-only [Wess–Zumino term](../../../statistical-physics.md#wess-zumino-term) may be dropped here.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

At a site with background $\eta_i\widetilde{\mathbf n}$, the linear variation is $\delta\mathbf n_i=\mathbf m$. The supplied variation formula gives

$$
S\,\delta\Gamma[eta_i\widetilde{\mathbf n}]
=S\int dt\,mathbf m\mathbin\cdot
\left[(\eta_i\widetilde{\mathbf n})
\times(\eta_i\partial_t\widetilde{\mathbf n})\right]
=S\int dt\,mathbf m\mathbin\cdot
(\widetilde{\mathbf n}\times\partial_t\widetilde{\mathbf n}).
$$

Replacing the lattice sum by $a^{-2}\int d^2x$ yields

$$
\boxed{
I_{WZ}^{(1)}
=\frac S{a^2}\int dt\,d^2x\,
\mathbf m\mathbin\cdot
(\widetilde{\mathbf n}\times\partial_t\widetilde{\mathbf n}).}
$$

This [Berry-phase term](../../../statistical-physics.md#wess-zumino-term) makes the uniform canting field the momentum conjugate to rotations of the Néel order parameter.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For a nearest-neighbor bond in the positive coordinate direction $\mu$, smoothness and orthogonality give

$$
\mathbf n_i\mathbin\cdot\mathbf n_{i+\hat\mu}
=-1+2|\mathbf m|^2
+\frac{a^2}{2}|\partial_\mu\widetilde{\mathbf n}|^2
+\text{higher derivatives and powers of }\mathbf m.
$$

There are two such bonds per site on the square lattice. Omitting the constant ground-state energy,

$$
S^2J\sum_{\langle ij\rangle}
\mathbf n_i\mathbin\cdot\mathbf n_j
\longrightarrow
\int d^2x\left[
\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
+\frac{4JS^2}{a^2}|\mathbf m|^2
\right].
$$

The staggered part of the field coupling cancels between the two sublattices, whereas

$$
S\sum_i\mathbf B\mathbin\cdot\mathbf n_i
\longrightarrow
\frac S{a^2}\int d^2x\,
\mathbf B\mathbin\cdot\mathbf m.
$$

Including the overall minus sign of the Hamiltonian contribution to the real-time action, the continuum Lagrangian density is therefore

$$
\boxed{
\mathcal L
=\frac S{a^2}\mathbf m\mathbin\cdot
(\widetilde{\mathbf n}\times\partial_t\widetilde{\mathbf n})
-\frac{4JS^2}{a^2}|\mathbf m|^2
-\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
-\frac S{a^2}\mathbf B\mathbin\cdot\mathbf m.}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Set

$$
A=\frac S{a^2},
\qquad
C=\frac{4JS^2}{a^2},
\qquad
\mathbf q=\widetilde{\mathbf n}\times
\partial_t\widetilde{\mathbf n}-\mathbf B.
$$

After adding $\lambda\mathbf m\mathbin\cdot\widetilde{\mathbf n}$, the terms involving the massive canting field are

$$
\mathcal L_m=-C|\mathbf m|^2
+\mathbf m\mathbin\cdot(A\mathbf q+lambda\widetilde{\mathbf n}).
$$

Completing the square gives

$$
\mathcal L_m
=-C\left|
\mathbf m-\frac{A\mathbf q+lambda\widetilde{\mathbf n}}{2C}
\right|^2
+\frac{|A\mathbf q+lambda\widetilde{\mathbf n}|^2}{4C}.
$$

The [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) over $\mathbf m$ contributes only a field-independent determinant. Hence

$$
\boxed{
\mathcal L_{eff}(\widetilde{\mathbf n},\lambda)
=-\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
+\frac1{16Ja^2}
\left|
\mathbf q+\frac{a^2\lambda}{S}widetilde{\mathbf n}
\right|^2.}
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Because $\widetilde{\mathbf n}\mathbin\cdot
(\widetilde{\mathbf n}\times\partial_t\widetilde{\mathbf n})=0$, the component of $\mathbf q$ parallel to $\widetilde{\mathbf n}$ is $-\mathbf B\mathbin\cdot\widetilde{\mathbf n}$. The [Gaussian integral](../../../calculus.md#gaussian-integral) over $\lambda$ removes precisely this longitudinal component. Thus

$$
\mathcal L_{eff}
=-\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
+\frac1{16Ja^2}
\left|
\widetilde{\mathbf n}\times\partial_t\widetilde{\mathbf n}
-\mathbf B+(\mathbf B\mathbin\cdot\widetilde{\mathbf n})
\widetilde{\mathbf n}
\right|^2.
$$

Using the [vector triple-product identity](../../../calculus.md#vector-triple-product) and $|\widetilde{\mathbf n}|=1$, this becomes the $O(3)$ [nonlinear sigma model](../../../quantum-field-theory.md#nonlinear-sigma-model) in a background field:

$$
\boxed{
I_{eff}[\widetilde{\mathbf n}]
=\int dt\,d^2x\left[
-\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
+\frac1{16Ja^2}
|\partial_t\widetilde{\mathbf n}
-\mathbf B\times\widetilde{\mathbf n}|^2
\right].}
$$

The magnetic field acts as the temporal component of an $O(3)$ background gauge connection.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

Choose the orientation of spherical coordinates as

$$
\widetilde{\mathbf n}
=(\sin\theta\cos\phi,-\sin\theta\sin\phi,\cos\theta),
$$

which differs from the opposite azimuth convention only by $\phi\mapsto-\phi$. With $\mathbf B=B\widehat{\mathbf x}$, $\theta=\pi/2-\delta\theta$, and $\phi=\delta\phi$,

$$
\widetilde{\mathbf n}
=(1,-\delta\phi,\delta\theta)+O(\delta^2).
$$

Substitution into the effective action gives

$$
\boxed{
\mathcal L_{eff}
=-\alpha^2\left[(\nabla\delta\theta)^2
+(\nabla\delta\phi)^2\right]
+\beta^2\left[(\partial_t\delta\theta+B\delta\phi)^2
+(\partial_t\delta\phi-B\delta\theta)^2\right],}
$$

where

$$
\boxed{\alpha^2=\frac{JS^2}{2},
\qquad
\beta^2=\frac1{16Ja^2}.}
$$

Let $\psi=\delta\theta+i\delta\phi$ and define the zero-field [spin-wave velocity](../../../statistical-physics.md#spin-wave-velocity)

$$
c=\frac\alpha\beta=2\sqrt2\,JSa.
$$

The linearized equation is

$$
(\partial_t-iB)^2\psi-c^2\nabla^2\psi=0.
$$

For a plane wave, the two circular polarizations therefore obey

$$
\boxed{(\omega\pm B)^2=c^2k^2,}
$$

or, with signed-frequency branches, $\omega=ck\pm B$ and their negative-frequency partners. At $B=0$ these are the two degenerate, linearly dispersing [antiferromagnetic spin waves](../../../statistical-physics.md#antiferromagnetic-spin-wave). The field [Zeeman-splits](../../../statistical-physics.md#zeeman-splitting) the two opposite circular polarizations by shifting their frequencies in opposite directions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
