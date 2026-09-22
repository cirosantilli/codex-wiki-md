# Paper 313

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_313.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_313.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
\boxed{\phi_{tt}-\phi_{xx}+U'(\phi)=0}.
$$

Time-translation invariance gives the conserved energy

$$
\boxed{E=\int_{\mathbb R}\left[\frac12\phi_t^2+\frac12\phi_x^2+U(\phi)\right]dx}.
$$

Indeed, after integrating the spatial term by parts and imposing finite-energy boundary conditions,

$$
\frac{dE}{dt}
=\int_{\mathbb R}\phi_t(\phi_{tt}-\phi_{xx}+U'(\phi))\,dx=0.
$$

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The potential is even, so field reflection has $\alpha=-1$; spatial reflection has $\beta=-1$. If $K(x)=\phi^{(0,1)}(x)$, the four oriented interpolating solutions, allowing a common translation, are

$$
\phi^{(0,1)}(x)=K(x),\qquad
\phi^{(1,0)}(x)=K(-x),
$$



$$
\phi^{(0,-1)}(x)=-K(x),\qquad
\phi^{(-1,0)}(x)=-K(-x).
$$

The first and third are kinks under this orientation convention, and spatial reflection gives their antikinks.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

On the sector $0\leq\phi\leq1$, choose the [superpotential](../../../supersymmetry.md#superpotential)

$$
W'(\phi)=\phi^2(1-\phi^2),
\qquad
\boxed{W(\phi)=\frac{\phi^3}{3}-\frac{\phi^5}{5}}.
$$

The static energy has the [Bogomolny bound](../../../quantum-field-theory.md#bogomolny-bound) completion

$$
E=\frac12\int_{\mathbb R}(\phi'-W')^2dx
+W(1)-W(0)\geq W(1)-W(0).
$$

Equality holds for $\phi'=W'$, and therefore

$$
\boxed{E[\phi^{(0,1)}]=\frac13-\frac15=\frac2{15}}.
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The first-order Bogomolny equation is

$$
\frac{d\phi}{dx}=\phi^2(1-\phi^2).
$$

Partial fractions and one integration give

$$
x-A=\int\frac{d\phi}{\phi^2(1-\phi^2)}
=-\frac1\phi+\frac12\log\frac{1+\phi}{1-\phi}.
$$

Thus

$$
\boxed{\frac12\log\frac{1+\phi}{1-\phi}-\frac1\phi=x-A}.
$$

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

As $x\to-\infty$, the term $-1/\phi$ dominates the implicit equation, so

$$
\phi(x)\sim\frac1{A-x}.
$$

As $x\to+\infty$, put $\delta=1-\phi$. Then

$$
x-A=\frac12\log\frac2\delta-1+o(1),
$$

and hence

$$
\phi(x)\sim1-e^{-2(x-b)},
\qquad
\boxed{b=A-1+\frac12\log2}.
$$

The profile rises monotonically from $0$ to $1$, with an algebraic left tail and an exponential right tail.

## 2

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Hodge star operator](../../../differential-form.md#hodge-star-operator) is defined by

$$
\alpha\wedge\star\beta=\langle\alpha,\beta\rangle_\eta\,\mathrm{vol}.
$$

On two-forms in oriented Euclidean four-space, $\star^2=1$ and the wedge product is symmetric. Therefore

$$
\star\omega\wedge\star\omega
=\omega\wedge\star^2\omega
=\boxed{\omega\wedge\omega}.
$$

For an anti-self-dual curvature $F=-\star F$, the [Yang-Mills instanton](../../../classical-field-theory-soliton.md#yang-mills-instanton) action becomes purely topological. With

$$
c_2=-\frac1{8\pi^2}\int_{\mathbb R^4}\operatorname{Tr}(F\wedge F),
$$

the standard positive-action convention gives

$$
\boxed{S_{\rm YM}=8\pi^2c_2}.
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $D_\mu=\partial_\mu+A_\mu$. A [Lax pair](../../../integrable-systems.md#lax-pair) with spectral parameter $\lambda$ is

$$
\boxed{L(\lambda)=D_w-\lambda D_{\bar z},
\qquad
M(\lambda)=D_z+\lambda D_{\bar w}}.
$$

The coefficients of $[L,M]=0$ at orders $1,\lambda,\lambda^2$ are respectively

$$
F_{wz}=0,\qquad F_{w\bar w}+F_{z\bar z}=0,\qquad F_{\bar w\bar z}=0,
$$

which are precisely the anti-self-dual Yang-Mills equations.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The equation $F_{wz}=0$ says that the partial connection $D_w,D_z$ is flat. Its compatibility condition therefore guarantees a local $G$-valued solution $g$ of

$$
\partial_wg=-A_wg,\qquad \partial_zg=-A_zg.
$$

After the associated [gauge transformation](../../../electromagnetism.md#gauge-transformation), both transformed components vanish:

$$
\boxed{A_w=A_z=0}.
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

In this gauge, $F_{\bar w\bar z}=0$ says that the remaining partial connection is flat. Hence locally

$$
A_{\bar w}=J^{-1}\partial_{\bar w}J,
\qquad
A_{\bar z}=J^{-1}\partial_{\bar z}J,
$$

or

$$
\boxed{A=J^{-1}\partial_{\bar w}J\,d\bar w
+J^{-1}\partial_{\bar z}J\,d\bar z}.
$$

The remaining curvature equation then becomes

$$
\boxed{\partial_w(J^{-1}\partial_{\bar w}J)
+\partial_z(J^{-1}\partial_{\bar z}J)=0}.
$$

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

For Maxwell theory the group is Abelian, so write $J=e^\chi$. The reduced equation loses its commutators and becomes

$$
\partial_w\partial_{\bar w}\chi
+\partial_z\partial_{\bar z}\chi=0.
$$

Since the Euclidean [Laplacian](../../../calculus.md#laplacian) is

$$
\Delta_{\mathbb R^4}=4(\partial_w\partial_{\bar w}
+\partial_z\partial_{\bar z}),
$$

the anti-self-dual Maxwell equations in this gauge are equivalent to

$$
\boxed{\Delta_{\mathbb R^4}\chi=0}.
$$

## 3

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a smooth map $\phi:M_1\to M_2$ between connected oriented closed manifolds of equal dimension and a volume form $\omega$ on $M_2$, the [topological degree](../../../geometry-and-topology.md#topological-degree) is defined by

$$
\boxed{\deg\phi=\frac{\int_{M_1}\phi^*\omega}{\int_{M_2}\omega}}.
$$

The standard area form on the unit sphere is

$$
\omega=\frac12\epsilon_{abc}\phi_a\,d\phi_b\wedge d\phi_c.
$$

Since $\int_{S^2}\omega=\operatorname{vol}(S^2)$, this gives

$$
\boxed{\deg\phi=\frac1{2\operatorname{vol}(S^2)}
\int_{S^2}\epsilon_{abc}\phi_a\,d\phi_b\wedge d\phi_c}.
$$

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a generic target value $y\in\mathbb{CP}^1$, its finite preimages solve

$$
P(z)-yQ(z)=0.
$$

When $m\ne n$ this has $\max(m,n)$ roots after the missing roots or poles at infinity are counted; when $m=n$, a generic $y$ again gives degree $m$. Holomorphic maps preserve orientation at regular preimages, so every local sign is positive. Hence

$$
\boxed{\deg f=\max(m,n)}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For $f(z)=z^m$,

$$
i\,df\wedge d\bar f=2m^2r^{2m-2}r\,dr\wedge d\theta.
$$

The pullback area is therefore

$$
\int_{\mathbb C}\frac{i\,df\wedge d\bar f}{(1+|f|^2)^2}
=4\pi m^2\int_0^\infty\frac{r^{2m-1}}{(1+r^{2m})^2}\,dr
=2\pi m.
$$

The same form integrates to $2\pi$ on the target sphere, so

$$
\boxed{\deg f=m}.
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Using $z=x+iy$, the energy is

$$
E=\frac12\int_{\mathbb R^2}
(|\partial_x\phi|^2+|\partial_y\phi|^2)\,dx\,dy.
$$

Because $|\phi|=1$, both derivatives are tangent to $S^2$ and $|\phi\times\partial_y\phi|=|\partial_y\phi|$. Completing the square gives

$$
E=\frac12\int|\partial_x\phi\mp\phi\times\partial_y\phi|^2\,dx\,dy
\left|\int\phi\mathbin\cdot
(\partial_x\phi\times\partial_y\phi)\,dx\,dy\right|.
$$

The final integral is $4\pi|\deg\phi|$ by the [topological degree](../../../geometry-and-topology.md#topological-degree) formula. Thus

$$
\boxed{E\geq4\pi|\deg\phi|},
\qquad
\boxed{c=4\pi}.
$$

Equality holds exactly when the appropriate first-order Bogomolny equation is satisfied:

$$
\boxed{\partial_x\phi=\pm\phi\times\partial_y\phi},
$$

with the sign chosen to match the degree.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
