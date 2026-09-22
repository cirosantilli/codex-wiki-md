# Paper 311

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_311.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_311.pdf)

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
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)

## 1

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $f(r)=1-r_+^2/r^2$ and let a dot denote differentiation with respect to an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\tau$. The time-translation and $z$-translation [Killing vector fields](../../../general-relativity.md#killing-vector-field), together with rotational symmetry of the unit $S^3$, give the [conserved quantities](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector)

$$
E=f\dot t,
\qquad
P=\dot z,
\qquad
J^2=r^4\lVert\dot\Omega_3\rVert^2.
$$

Define $\varepsilon=-g_{ab}\dot x^a\dot x^b$, so $\varepsilon=1,0,-1$ for timelike, null and spacelike geodesics respectively. The normalization equation becomes

$$
-\frac{E^2}{f}+\frac{\dot r^2}{f}+\frac{J^2}{r^2}+P^2=-\varepsilon.
$$

It therefore has the [effective potential](../../../physics.md#effective-potential) form

$$
\frac12\dot r^2+\widetilde V(r)=0,
\qquad
\boxed{\widetilde V(r)=\frac12\left[f(r)\left(\varepsilon+P^2+\frac{J^2}{r^2}\right)-E^2\right]}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For radial [null geodesics](../../../special-relativity.md#null-geodesic), $d\Omega_3=dz=0$ and $ds^2=0$, so

$$
\frac{dt}{dr}=\pm\frac1{f(r)}.
$$

Introduce the tortoise coordinate by

$$
\frac{dr_\star}{dr}=\frac1f,
\qquad
\boxed{r_\star=r+\frac{r_+}{2}\log\left|\frac{r-r_+}{r+r_+}\right|}
$$

up to an additive constant. The plus sign gives $d(t-r_\star)=0$ on outgoing rays, while the minus sign gives $d(t+r_\star)=0$ on ingoing rays. Hence

$$
\boxed{u=t-r_\star},
\qquad
\boxed{v=t+r_\star}
$$

are respectively constant on the stated radial null families.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The normal to a surface of constant $r$ has squared norm

$$
g^{ab}(\partial_ar)(\partial_br)=g^{rr}=f(r),
$$

which vanishes at $r=r_+$. Thus this surface is a [null hypersurface](../../../general-relativity.md#null-hypersurface). The stationary [Killing vector field](../../../general-relativity.md#killing-vector-field)

$$
K=\partial_t
$$

has $K^2=g_{tt}=-f$, so it becomes null there and generates a [Killing horizon](../../../general-relativity.md#killing-horizon). Since $f$ has a simple zero, its [surface gravity](../../../general-relativity.md#surface-gravity) is

$$
\boxed{\kappa=\frac12f'(r_+)=\frac1{r_+}}.
$$

A horizon cross-section has topology $S^3\times S^1$, where the circle is the periodic $z$ direction. Including a complete generator, the null hypersurface has topology

$$
\boxed{\mathbb R\times S^3\times S^1}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Using $v=t+r_\star$ puts the [black string](../../../general-relativity.md#black-string) metric into regular ingoing form,

$$
ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega_3^2+dz^2.
$$

Its inverse metric gives

$$
\nabla^ar=(\partial_v)^a+f(\partial_r)^a,
\qquad
(\nabla r)^2=f.
$$

For $r<r_+$, $f<0$, so $\nabla r$ is timelike. It is future-directed by continuity from the future horizon, where it equals the future generator $\partial_v$. If $X$ is any future-directed causal tangent, then

$$
X(r)=g(X,\nabla r)<0.
$$

Thus $r$ decreases strictly along every future-directed causal curve in the interior. No such curve can cross back through $r=r_+$ or reach [future null infinity](../../../general-relativity.md#future-null-infinity). The region $r<r_+$ is consequently outside the causal past of future null infinity and is part of the [black hole](../../../general-relativity.md#black-hole) region.

## 2

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose an auxiliary null vector $N^a$ with $U\mathbin\cdot N=-1$. The [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) is

$$
P^a{}_b=\delta^a_b+U^aN_b+N^aU_b,
$$

and the [optical tensor](../../../geodesic-congruence.md#optical-tensor) is $\widehat B_{ab}=P_a{}^cP_b{}^dB_{cd}$ for $B_{ab}=\nabla_bU_a$. Because the screen is two-dimensional, its irreducible decomposition is

$$
\widehat B_{ab}=\frac12\theta P_{ab}+\widehat\sigma_{ab}+\widehat\omega_{ab},
$$

where

$$
\boxed{\theta=P^{ab}\widehat B_{ab}},
\qquad
\boxed{\widehat\sigma_{ab}=\widehat B_{(ab)}-\frac12\theta P_{ab}},
\qquad
\boxed{\widehat\omega_{ab}=\widehat B_{[ab]}}.
$$

These are respectively the [null expansion](../../../geodesic-congruence.md#null-expansion), [null shear](../../../geodesic-congruence.md#null-shear), and [null twist](../../../geodesic-congruence.md#null-twist), also called rotation.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Affine geodesic motion gives $U^c\nabla_cU_a=0$. Commuting the two [covariant derivatives](../../../general-relativity.md#covariant-derivative) and applying the product rule yields

$$
\begin{aligned}
U^c\nabla_cB_{ab}
&=U^c\nabla_c\nabla_bU_a\\
&=\nabla_b(U^c\nabla_cU_a)
-(\nabla_bU^c)(\nabla_cU_a)
+R_{cba}{}^dU_dU^c\\
&=-B^c{}_bB_{ac}+R_{cba}{}^dU_dU^c.
\end{aligned}
$$

This proves the required transport identity. The curvature term is symmetric after screen projection, so taking the antisymmetric screen part and inserting the optical decomposition gives the [null-twist propagation equation](../../../geodesic-congruence.md#null-twist-propagation-equation)

$$
\boxed{U^c\nabla_c\widehat\omega_{ab}
=-\theta\widehat\omega_{ab}
+2\widehat\sigma_{c[a}\widehat\omega_{b]}{}^c}.
$$

In particular, an initially twist-free congruence remains twist-free.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Choose a spacelike two-dimensional cross-section $S$ of the [null hypersurface](../../../general-relativity.md#null-hypersurface) $\mathcal N$ and coordinates $y^i$ on $S$. Extend $y^i$ along the null generators, and choose their parameter $\lambda$ to be affine, so $U=\partial_\lambda$ on $\mathcal N$. At every point choose the other null normal $L$ with $g(U,L)=1$, shoot out the affinely parametrized null geodesic with tangent $L$, and call its affine parameter $r$. Transport $(\lambda,y^i)$ along those transverse geodesics.

This construction gives [Gaussian null coordinates](../../../general-relativity.md#gaussian-null-coordinates). The hypersurface is $r=0$, and the coordinate conditions imply

$$
g_{rr}=g_{ri}=0,
\qquad
g_{r\lambda}=1,
\qquad
g_{\lambda\lambda}|_{r=0}=g_{\lambda i}|_{r=0}=0.
$$

Because $\lambda$ is affine on the generators, $\partial_rg_{\lambda\lambda}|_{r=0}=0$. Smoothness then factors the remaining components as $g_{\lambda\lambda}=r^2F$ and $g_{\lambda i}=rh_i$, giving

$$
\boxed{ds^2=2\,dr\,d\lambda+r^2F\,d\lambda^2+2rh_i\,d\lambda\,dy^i+h_{ij}\,dy^i\,dy^j}.
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

On $r=0$, the screen metric is $h_{ij}$ and $U=\partial_\lambda$. Therefore the [null expansion](../../../geodesic-congruence.md#null-expansion) is

$$
\theta=\frac12h^{ij}\frac{\partial h_{ij}}{\partial\lambda}.
$$

The derivative formula for the [determinant](../../../linear-algebra.md#determinant) gives

$$
\frac{\partial h}{\partial\lambda}
=h\,h^{ij}\frac{\partial h_{ij}}{\partial\lambda},
$$

and hence

$$
\boxed{\frac{\partial\sqrt h}{\partial\lambda}=\theta\sqrt h}.
$$

**Thus $\theta$ is the fractional rate of change of an infinitesimal transverse area carried along the generators: positive expansion enlarges the beam and negative expansion focuses it.**

## 3

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [asymptotically flat spacetime](../../../general-relativity.md#asymptotically-flat-spacetime) at [future null infinity](../../../general-relativity.md#future-null-infinity) admits a smooth [conformal completion](../../../general-relativity.md#conformal-completion) $(\overline{\mathcal M},\bar g)$ with the following properties. The physical spacetime $\mathcal M$ is the interior of $\overline{\mathcal M}$, its metric obeys

$$
\bar g_{ab}=\Omega^2g_{ab},
$$

and the boundary component $\mathcal I^+$ satisfies $\Omega=0$ and $d\Omega\ne0$. Every future-directed outgoing null geodesic has an endpoint there, the generators of $\mathcal I^+$ are complete, and in four spacetime dimensions $\mathcal I^+\simeq\mathbb R\times S^2$. The physical [Einstein field equations](../../../general-relativity.md#einstein-field-equations) are vacuum in a neighborhood of this boundary.

Let $n_a=\bar\nabla_a\Omega$. Multiplying the supplied conformal Ricci relation by $\Omega^2$, using $R_{ab}=0$, and taking the limit to $\mathcal I^+$ gives

$$
0=-3\bar g_{ab}n^cn_c,
\qquad
\boxed{n^an_a=0\quad\hbox{on }\mathcal I^+}.
$$

The boundary normal is therefore null. Since a null normal is also tangent to its hypersurface, $n^a$ generates $\mathcal I^+$.

Smoothness makes $s=\Omega^{-1}n^2$ finite at the boundary. Multiplication of the same vacuum equation by $\Omega$ gives there

$$
2\bar\nabla_an_b+\bar g_{ab}(\bar\Box\Omega-3s)=0.
$$

Taking the trace yields $s=\tfrac12\bar\Box\Omega$, and substitution gives

$$
\bar\nabla_an_b=\frac14\bar g_{ab}\bar\Box\Omega.
$$

The remaining freedom $\Omega\mapsto\omega\Omega$ can be used to impose $\bar\Box\Omega=0$ on $\mathcal I^+$. In this conformal gauge, $\bar\nabla_an_b=0$ there, so the generators are affinely parametrized, expansion-free null geodesics of the unphysical metric.

Choose a generator coordinate $u$, the defining function $\Omega$, and angular coordinates $x^A$ whose leading metric $q_{AB}$ is the round metric on the [unit sphere](../../../topology.md#unit-sphere). After the conformal and coordinate choices above, the leading unphysical metric is

$$
\bar g=2\,du\,d\Omega+q_{AB}dx^Adx^B+O(\Omega),
$$

with the Minkowski term $-\Omega^2du^2$ entering at the next relevant order. Setting $r=\Omega^{-1}$ recovers the physical asymptotic form

$$
g=-du^2-2\,du\,dr+r^2q_{AB}dx^Adx^B
+\text{terms lower by powers of }r.
$$

The displayed leading metric is [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) in outgoing null coordinates. Smooth conformal extendibility controls the lower-order corrections, while the vacuum equations constrain them to the radiative Bondi--Sachs expansion. This is the precise sense in which the permitted spacetimes approach Minkowski spacetime near $\mathcal I^+$ while still allowing outgoing gravitational radiation.

## 4

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics) states that the area of spatial cross-sections of a future [event horizon](../../../general-relativity.md#event-horizon) cannot decrease toward the future, provided the [null energy condition](../../../general-relativity.md#null-energy-condition) and the standard global assumptions hold.

Let $k^a$ be an affinely parametrized horizon generator. It is hypersurface-orthogonal, so its [null twist](../../../geodesic-congruence.md#null-twist) vanishes. The [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) in $D$ dimensions and the Einstein equation give

$$
\frac{d\theta}{d\lambda}
=-\frac{\theta^2}{D-2}
-\widehat\sigma_{ab}\widehat\sigma^{ab}
-R_{ab}k^ak^b
\leq-\frac{\theta^2}{D-2}.
$$

If $\theta(\lambda_0)<0$, integration implies that $\theta$ diverges to $-\infty$ within affine distance at most $(D-2)/|\theta(\lambda_0)|$. The resulting focal point would make the generator leave the achronal boundary that defines the event horizon, contradicting its assumed future completeness. Hence $\theta\geq0$ everywhere. Since [null expansion](../../../geodesic-congruence.md#null-expansion) obeys

$$
\frac{dA}{d\lambda}=\theta A,
$$

every horizon area element, and therefore every complete cross-section area, is nondecreasing.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For this metric, $\sqrt{-g}=a^2$, while $g^{\eta\eta}=-a^{-2}$, $g^{zz}=a^{-2}$ and $g^{ij}=\delta^{ij}$. The massless [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) is consequently

$$
\Box\phi
=\frac1{a^2}(-\partial_\eta^2+\partial_z^2)\phi
+\delta^{ij}\partial_i\partial_j\phi=0.
$$

Insert the spatial [Fourier transform](../../../analysis.md#fourier-transform) given in the question. Each [wavenumber](../../../wave-equation.md#wavenumber) mode then satisfies

$$
\boxed{\Phi_{k_z\mathbf k}''
+\omega_{k_z\mathbf k}^2(\eta)\Phi_{k_z\mathbf k}=0},
\qquad
\boxed{\omega_{k_z\mathbf k}^2(\eta)=k_z^2+a(\eta)^2|\mathbf k|^2}.
$$

**Thus every field mode is a [simple harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) with a time-dependent [angular frequency](../../../classical-mechanics.md#angular-frequency).**

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

In the two constant regions define

$$
\omega_\pm=\sqrt{k_z^2+a_\pm^2|\mathbf k|^2}.
$$

The normalized [positive-frequency modes](../../../quantum-field-theory.md#positive-frequency-solution) are

$$
\boxed{u_\pm(\eta)=\frac{e^{-i\omega_\pm\eta}}{\sqrt{2\omega_\pm}}},
$$

up to the common spatial Fourier normalization. They satisfy the unit Wronskian condition

$$
i(u_\pm^*u_\pm'-u_\pm u_\pm^{*\prime})=1,
$$

which is the mode form of the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product). Because the mode equation contains no delta function at $\eta=0$, both $\Phi$ and $\Phi'$ are continuous there.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Continue the incoming positive-frequency mode through $\eta=0$ as

$$
u_-(\eta)=\alpha u_+(\eta)+\beta u_+^*(\eta)
\qquad(\eta>0).
$$

Continuity of the mode and its first derivative gives the [sudden frequency quench](../../../quantum-field-theory.md#sudden-frequency-quench) coefficients

$$
\alpha=\frac{\omega_++\omega_-}{2\sqrt{\omega_+\omega_-}},
\qquad
\beta=\frac{\omega_+-\omega_-}{2\sqrt{\omega_+\omega_-}}.
$$

The associated [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation) says that the incoming vacuum has expected outgoing occupation number

$$
\boxed{\langle N_{k_z\mathbf k}^{(+)}\rangle
=|\beta|^2
=\frac{(\omega_+-\omega_-)^2}{4\omega_+\omega_-}}.
$$

It vanishes when $a_+=a_-$, as required when there is no change of geometry.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
