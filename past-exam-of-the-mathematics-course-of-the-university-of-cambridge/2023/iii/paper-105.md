# Paper 105

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_105.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_105.pdf)

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
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
    - [v](#1/b/v)
      - [Solution](#1/b/v/solution)
    - [vi](#1/b/vi)
      - [Solution](#1/b/vi/solution)
    - [vii](#1/b/vii)
      - [Solution](#1/b/vii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Consider an analytic [quasilinear partial differential equation](../../../partial-differential-equation.md#quasilinear-partial-differential-equation)

$$
\sum_{i,j=1}^n a^{ij}(x,u,Du)\,\partial_i\partial_j u
=F(x,u,Du).
$$

Let the analytic initial hypersurface be $\Gamma=\{\phi=0\}$ and prescribe $u=u_0$ and one transverse derivative $\partial_Nu=u_1$ on $\Gamma$. The tangential derivatives of $u_0$ together with $u_1$ determine the full first jet $Du$ on $\Gamma$. The hypersurface is [non-characteristic](../../../partial-differential-equation.md#non-characteristic-hypersurface) at $x_0$ with respect to these data when

$$
\sum_{i,j}a^{ij}(x_0,u_0(x_0),Du(x_0))
\partial_i\phi(x_0)\partial_j\phi(x_0)\ne0.
$$

This is precisely the [principal symbol of a partial differential equation](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) evaluated on the conormal $d\phi(x_0)$.

The [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) then gives a unique real-analytic solution near $x_0$. In coordinates flattening $\Gamma$ to $x_n=0$, non-characteristicity lets the equation solve analytically for $\partial_n^2u$, after which the analytic equation and the two initial jets determine every higher Taylor coefficient.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [wave operator](../../../wave-equation.md#d-alembert-operator) has principal symbol

$$
p(\tau,\xi)=-\tau^2+|\xi|^2.
$$

The conormal to the initial plane is $dt$, and $p(dt)=-1\ne0$. The plane is therefore non-characteristic.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The principal symbol is $\tau^2+|\xi|^2$, so its value on $dt$ is $1$. The initial plane is non-characteristic.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

When the [heat equation](../../../diffusion-equation.md#heat-equation) is viewed as a second-order equation, its principal symbol contains only the spatial second derivatives:

$$
p(\tau,\xi)=-|\xi|^2
$$

up to an irrelevant sign. It vanishes on $dt$, so the initial plane is characteristic in this second-order sense. The equation remains a well-posed first-order evolution equation in time; these are different notions of order.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

The principal symbol is

$$
p(\tau,\xi)=\tau^2-(1+u^2)|\xi|^2.
$$

Its value on $dt$ is $1$, independently of the data, so the initial plane is non-characteristic everywhere.

<h4 id="1/b/v">v</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/v/solution">Solution</h5>

↑ **Parent:** [V](#1/b/v)

For $\phi(x)=|x|^2-1$, the conormal on the unit sphere is $d\phi=(0,2x)$. Hence

$$
p(d\phi)=4|x|^2=4
$$

on the sphere. It is non-characteristic at every point.

<h4 id="1/b/vi">vi</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#1/b/vi)

For $\phi=t-x_1$, the conormal is $dt-dx_1$, and

$$
p(d\phi)=-1+1=0.
$$

This null hyperplane is a [characteristic hypersurface](../../../partial-differential-equation.md#characteristic-hypersurface) of the wave equation.

<h4 id="1/b/vii">vii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/vii/solution">Solution</h5>

↑ **Parent:** [Vii](#1/b/vii)

The second-order principal symbol of the heat operator evaluated on $dt-dx_1$ is $-1$, up to the overall sign convention. Thus this tilted hypersurface is non-characteristic.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Introduce the [null coordinates](../../../partial-differential-equation.md#characteristic-coordinate)

$$
\xi=t-x,\qquad\eta=t+x.
$$

Then $\Box=-4\partial_\xi\partial_\eta$, so the equation becomes

$$
u_{\xi\eta}=-\frac14u.
$$

Write the compatible boundary values as

$$
a(\xi)=u(\xi,0),\qquad b(\eta)=u(0,\eta),\qquad a(0)=b(0)=c.
$$

Twice integrating the equation gives the equivalent [Volterra integral equation](../../../analysis.md#volterra-integral-equation)

$$
u(\xi,\eta)
=a(\xi)+b(\eta)-c
-\frac14\int_0^\xi\int_0^\eta u(s,r)\,dr\,ds.
$$

Let $T$ denote the double-integral operator including the factor $-1/4$, and put $g=a+b-c$. Successive approximation gives the [Neumann series](../../../banach-algebra.md#neumann-series)

$$
u=\sum_{m=0}^\infty T^mg.
$$

On a rectangle $|\xi|\leq R$, $|\eta|\leq R$,

$$
\|T^mg\|_\infty
\leq\frac{(R^2/4)^m}{(m!)^2}\|g\|_\infty.
$$

The series and its differentiated series converge locally uniformly. Since $a$ and $b$ are analytic, the sum is analytic and solves the equation and data near the origin.

If two solutions have the same data, their difference $w=Tw$. Iterating and using the same factorial estimate gives $\|w\|_\infty=0$ on every sufficiently small rectangle. This proves uniqueness. The argument is the [Analytic Goursat problem for a Klein--Gordon equation](../../../partial-differential-equation.md#analytic-goursat-problem-for-a-klein-gordon-equation).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The same Volterra series converges uniformly on the entire compact characteristic square $0\leq\xi,\eta\leq1$, because

$$
\sum_{m\geq0}\frac{1}{4^m(m!)^2}<\infty.
$$

The boundary functions are analytic on neighbourhoods of the compact axis segments, so finitely many complex neighbourhoods give uniform Cauchy estimates for their derivatives. Applying $T^m$ adds the two factorial denominators above, and the corresponding derivative series converges on a neighbourhood of every point of the closed square. Thus the local analytic solutions continue across the whole square and agree on overlaps by uniqueness.

Equivalently, the integral equation bounds $u$ and every differentiated equation on each smaller rectangle; no norm can blow up at a first missing corner. The local analytic existence theorem therefore extends the solution through that corner. This is [Global continuation for the analytic Goursat problem](../../../partial-differential-equation.md#global-continuation-for-the-analytic-goursat-problem).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For compatible $C^2$ boundary functions $a$ and $b$, use exactly the same Volterra series. The factorial estimate holds in the $C^2$ norm after differentiating the integral formula, so the series converges to a $C^2$ function on the full square. It satisfies

$$
u_{\xi\eta}=-u/4
$$

and the two boundary values. This directly proves existence. One can equivalently approximate $a,b$ in $C^2$ by compatible analytic functions; the same estimates make their analytic solutions Cauchy in $C^2$.

## 2

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The zero-boundary [Sobolev space](../../../sobolev-space.md) is

$$
H_0^1(\Omega)=\overline{C_c^\infty(\Omega)}^{\,H^1}.
$$

On it define

$$
(u,v)_{H_0^1}=\int_\Omega\nabla u\cdot\nabla v.
$$

If this quadratic form vanishes, then $\nabla u=0$. The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) gives

$$
\|u\|_{L^2}\leq C\|\nabla u\|_{L^2}=0,
$$

so $u=0$. It is therefore an inner product, and its norm is equivalent to the usual $H^1$ norm.

A function $u\in H_0^1(\Omega)$ is a [weak solution](../../../partial-differential-equation.md#weak-solution) when

$$
\int_\Omega\nabla u\cdot\nabla\varphi
=-\int_\Omega f\varphi
\qquad\text{for every }\varphi\in H_0^1(\Omega).
$$

This follows from [integration by parts](../../../calculus.md#integration-by-parts) and incorporates the homogeneous [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) through membership in $H_0^1$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The functional

$$
\ell(\varphi)=-\int_\Omega f\varphi
$$

is bounded on $H_0^1(\Omega)$ by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the Poincare inequality:

$$
|\ell(\varphi)|\leq C\|f\|_{L^2}\|\nabla\varphi\|_{L^2}.
$$

The [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem) therefore supplies a unique $u\in H_0^1(\Omega)$ satisfying

$$
(u,\varphi)_{H_0^1}=\ell(\varphi)
$$

for every test function. This is exactly the weak identity from part (a). Uniqueness also follows by testing the homogeneous difference with itself.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

After integration by parts, the weak formulation is

$$
\int_\Omega(\nabla u\cdot\nabla\varphi+u\varphi)
=-\int_\Omega f\varphi
\qquad(\varphi\in H_0^1(\Omega)).
$$

The left side is the inner product

$$
(u,\varphi)_*=\int_\Omega(\nabla u\cdot\nabla\varphi+u\varphi),
$$

which is positive definite and induces the usual $H^1$ norm. The right side is bounded in this norm. The Riesz representation theorem, equivalently the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem), gives a unique weak solution. This is the [weak Dirichlet problem for the massive Laplacian](../../../functional-analysis.md#weak-dirichlet-problem-for-the-massive-laplacian) with mass one and the signs multiplied by $-1$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Combined interior and boundary [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) for the Dirichlet Laplacian on a smooth bounded domain states that, for every integer $k\geq0$,

$$
\|u\|_{H^{k+2}(\Omega)}
\leq C_k\|f\|_{H^k(\Omega)}
$$

when $\Delta u=f$ and $u$ has zero boundary trace. More generally one first has an additional $\|u\|_{L^2}$ term, which uniqueness and the Poincare inequality remove here.

For the shifted equation, write $\Delta u=f+u$. The weak estimate gives $u\in H^1$. Applying the displayed estimate first with an $L^2$ right side gives $u\in H^2$. Repeating,

$$
f\in H^k,\quad u\in H^j
\quad\Longrightarrow\quad
u\in H^{\min(k,j)+2},
$$

until $u\in H^{k+2}$. The lower-order term is controlled at each stage, yielding

$$
\|u\|_{H^{k+2}}\leq C_k\|f\|_{H^k}.
$$

This is [boundary elliptic regularity for the shifted Dirichlet Laplacian](../../../distribution-theory.md#boundary-elliptic-regularity-for-the-shifted-dirichlet-laplacian).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

There is a sign issue in the printed problem. Part (c) constructs the inverse of $\Delta-1$, whereas the second equation printed in part (e) contains $\Delta+1$. The latter operator is invertible with homogeneous Dirichlet data only when $1$ is not a [Dirichlet Laplacian eigenvalue](../../../partial-differential-equation.md#dirichlet-laplacian-eigenvalue). Thus the assertion as printed needs this nonresonance hypothesis; with a minus sign it follows directly from parts (c) and (d).

Under either the intended minus sign or the stated nonresonance condition, let $G_0$ and $G_1$ be the bounded Dirichlet solution operators for the two linear equations. Choose $s>n/2$ and work with $u,v\in H^{s+2}(\Omega)\cap H_0^1(\Omega)$. Since $H^s(\Omega)$ is a [Sobolev algebra](../../../sobolev-space.md#sobolev-algebra),

$$
\|(\partial_{11}v)^2\|_{H^s}\leq C\|v\|_{H^{s+2}}^2,\qquad
\|(\partial_{22}u)^2\|_{H^s}\leq C\|u\|_{H^{s+2}}^2.
$$

Define

$$
\mathcal T(u,v)=
\left(
G_0\big((\partial_{11}v)^2+\varepsilon f\big),
G_1\big((\partial_{22}u)^2\big)
\right).
$$

Elliptic regularity gives, on a ball of radius $R$,

$$
\|\mathcal T(u,v)\|_{H^{s+2}\times H^{s+2}}
\leq C(R^2+\varepsilon\|f\|_{H^s}),
$$

and the difference estimate has Lipschitz constant at most $CR$. Choose $R$ small and then $\varepsilon_0$ so that $C(R^2+\varepsilon_0\|f\|_{H^s})\leq R$. The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) gives a solution for $0\leq\varepsilon<\varepsilon_0$. Repeated elliptic regularity and smoothness of $f$ bootstrap the solution to $C^\infty$.

## 3

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a smooth function $g$ define its [spherical mean](../../../analysis.md#spherical-mean)

$$
M_tg(x)=\frac1{4\pi}\int_{S^2}g(x+t\omega)\,d\omega.
$$

The [Kirchhoff formula](../../../wave-equation.md#kirchhoff-formula)

$$
u(t,x)=\partial_t\big(tM_tu_0(x)\big)+tM_tu_1(x)
$$

defines a smooth solution of the three-dimensional [wave equation](../../../wave-equation.md) for all positive and negative $t$ and has the prescribed data at $t=0$.

For uniqueness, apply the local [energy estimate](../../../partial-differential-equation.md#energy-estimate) to the difference of two solutions on a backward light cone. Its energy at the cone tip is bounded by the zero initial energy on the cone base, so the difference and its derivatives vanish. Covering spacetime by such cones proves uniqueness among $C^2$ solutions.

Compact support is unnecessary for existence or uniqueness: the sphere in the Kirchhoff formula is compact for each $(t,x)$, so arbitrary smooth data suffice, and the cone-energy proof is local.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Strong Huygens principle](../../../wave-equation.md#strong-huygens-principle) in three spatial dimensions says that the solution at $(t,x)$ depends only on the initial data on the sphere

$$
\{y:|y-x|=|t|\},
$$

rather than on the full ball bounded by that sphere. This follows immediately from the Kirchhoff formula and its time derivative. Consequently a disturbance has no tail inside the light cone: if the initial data are supported in a compact set $K$, then $u(t,x)=0$ whenever that sphere misses $K$. This is sharper than [finite propagation speed](../../../wave-equation.md#finite-propagation-speed), which only excludes influence from outside the ball.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $\mathcal Rg(s,\omega)$ be the [Radon transform](../../../analysis.md#radon-transform)

$$
\mathcal Rg(s,\omega)=\int_{y\cdot\omega=s}g(y)\,dA_y.
$$

Taking the large-radius limit in the Kirchhoff formula, with $\xi=t-r$ fixed for the outgoing limit and $\eta=t+r$ fixed for the incoming limit, gives the [radiation fields](../../../wave-equation.md#radiation-field)

$$
\psi_+(\xi,\omega)
=\frac1{4\pi}
\left[
\mathcal Ru_1(-\xi,\omega)
-\partial_s\mathcal Ru_0(-\xi,\omega)
\right],
$$



$$
\psi_-(\eta,\omega)
=-\frac1{4\pi}
\left[
\mathcal Ru_1(\eta,\omega)
+\partial_s\mathcal Ru_0(\eta,\omega)
\right].
$$

Indeed, the expanding spheres converge after multiplication by $r/t$ to the planes $y\cdot\omega=-\xi$ and $y\cdot\omega=\eta$, respectively.

The Radon transforms of smooth compactly supported functions are smooth. If the data are supported in a ball of radius $R$, these transforms vanish for $|s|>R$. Hence both radiation fields are well-defined smooth functions of compact support in the null-time variable.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For radial data, set

$$
f_0(r)=r\,u_0(|r|),\qquad f_1(r)=r\,u_1(|r|)
$$

on $\mathbb R$. The conditions at the origin say exactly that these are smooth odd compactly supported functions. The radial reduction $w(t,r)=ru(t,r)$ satisfies the one-dimensional wave equation, and the [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula) gives

$$
w(t,r)=\frac12\big(f_0(r-t)+f_0(r+t)\big)
+\frac12\int_{r-t}^{r+t}f_1(s)\,ds.
$$

In null coordinates this is

$$
w=\frac12\big(f_0(-\xi)+f_0(\eta)\big)
+\frac12\int_{-\xi}^{\eta}f_1(s)\,ds.
$$

The limits are therefore

$$
\psi_+(\xi)=
\frac12f_0(-\xi)+\frac12\int_{-\xi}^{\infty}f_1(s)\,ds,
$$



$$
\psi_-(\eta)=
\frac12f_0(\eta)-\frac12\int_{\eta}^{\infty}f_1(s)\,ds.
$$

They are smooth and compactly supported because $f_0,f_1$ are odd.

Write

$$
A(s)=\frac12f_0(s),\qquad
B(s)=\frac12\int_s^\infty f_1(q)\,dq.
$$

Then $A$ is an arbitrary odd test function and $B$ is an arbitrary even test function. Conversely, every odd $A\in C_c^\infty(\mathbb R)$ gives $f_0=2A$, and every even $B\in C_c^\infty(\mathbb R)$ gives $f_1=-2B'$. Thus both maps are injective and

$$
X_-=X_+=C_c^\infty(\mathbb R).
$$

Since

$$
\psi_-=A-B,\qquad
\psi_+=-A+B,
$$

the radial [scattering map](../../../wave-equation.md#scattering-map) is

$$
\boxed{S\psi=-\psi.}
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
