# Paper 357

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_357.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_357.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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

↑ **Parent:** [Paper 357](paper-357.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Expanding the [spatial projection tensor](../../../numerical-relativity.md#spatial-projection-tensor) gives

$$
\Theta_\mu
=\perp^\rho{}_\mu Z_\rho
=Z_\mu+n_\mu n^\rho Z_\rho
=Z_\mu-n_\mu\Theta.
$$

Rearrangement yields the normal-plus-spatial decomposition

$$
\boxed{Z_\mu=\Theta_\mu+n_\mu\Theta.}
$$

It also makes $n^\mu\Theta_\mu=0$ immediate.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The definition of the [extrinsic curvature of a spatial hypersurface](../../../numerical-relativity.md#extrinsic-curvature-of-a-spatial-hypersurface) and $\perp^\rho{}_\mu=\delta^\rho{}_\mu+n^\rho n_\mu$ give

$$
K_{\mu\nu}
=-\left(\delta^\rho{}_\mu+n^\rho n_\mu\right)
\nabla_\rho n_\nu
=-\nabla_\mu n_\nu-n_\mu a_\nu,
$$

where $a_\nu=n^\rho\nabla_\rho n_\nu$ is the [normal acceleration](../../../numerical-relativity.md#normal-acceleration). Hence

$$
\boxed{-\nabla_\mu n_\nu=K_{\mu\nu}+n_\mu a_\nu.}
$$

Differentiating $n^\nu n_\nu=-1$ shows $n^\nu a_\nu=0$, so the acceleration is spatial as required.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The inverse spacetime metric decomposes as

$$
g^{\mu\nu}=\perp^{\mu\nu}-n^\mu n^\nu.
$$

Contracting the [covariant derivative](../../../general-relativity.md#covariant-derivative) of $Z_\nu$ and recognizing the fully projected contraction as its [spatial covariant derivative](../../../numerical-relativity.md#spatial-covariant-derivative) gives

$$
\boxed{
\nabla^\mu Z_\mu
=-n^\mu n^\nu\nabla_\mu Z_\nu+D^\mu Z_\mu.
}
$$

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

Insert $Z_\mu=\Theta_\mu+n_\mu\Theta$ from part (i) into the projected divergence:

$$
D^\mu Z_\mu
=D^\mu\Theta_\mu
+\perp^{\mu\nu}\nabla_\mu(n_\nu\Theta).
$$

The term containing $\nabla_\mu\Theta$ vanishes because $\perp^{\mu\nu}n_\nu=0$. The remaining contraction is

$$
\Theta\perp^{\mu\nu}\nabla_\mu n_\nu=-K\Theta
$$

by the definition of the [extrinsic curvature of a spatial hypersurface](../../../numerical-relativity.md#extrinsic-curvature-of-a-spatial-hypersurface). Therefore

$$
\boxed{D^\mu Z_\mu=D^\mu\Theta_\mu-K\Theta.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

First take the spacetime trace of the generalized field equation. Since $n_\mu Z^\mu=-\Theta$ and spacetime has dimension four, this gives

$$
{}^{(4)}R+2\nabla_\mu Z^\mu-2\Theta=-8\pi T.
$$

Next contract twice with the unit normal. The result is

$$
R_{\mu\nu}n^\mu n^\nu
+2n^\mu n^\nu\nabla_\mu Z_\nu-\Theta
=8\pi\rho+4\pi T.
$$

Adding the trace equation to twice this normal projection cancels $T$. The [Scalar Gauss equation](../../../numerical-relativity.md#scalar-gauss-equation) then converts the curvature terms to

$$
{}^{(3)}R+K^2-K_{\mu\nu}K^{\mu\nu}.
$$

For the derivative terms, part (iii) gives

$$
2\nabla_\mu Z^\mu+4n^\mu n^\nu\nabla_\mu Z_\nu
=2D^\mu Z_\mu+2n^\mu n^\nu\nabla_\mu Z_\nu.
$$

Differentiating $n^\nu Z_\nu=-\Theta$ along $n^\mu$ yields

$$
n^\mu n^\nu\nabla_\mu Z_\nu
=-n^\mu\nabla_\mu\Theta-Z_\nu a^\nu.
$$

Combining these identities produces

$$
\boxed{
{}^{(3)}R+K^2-K_{\mu\nu}K^{\mu\nu}
-2n^\mu\nabla_\mu\Theta-2Z_\mu a^\mu
-4\Theta+2D^\mu Z_\mu=16\pi\rho.
}
$$

Because $\Theta$ is a [scalar field](../../../quantum-field-theory.md#scalar-field) and $n^\mu=\alpha^{-1}(1,-\beta^i)$,

$$
n^\mu\nabla_\mu\Theta
=\frac1\alpha(\partial_t-\beta^m\partial_m)\Theta.
$$

The [normal acceleration](../../../numerical-relativity.md#normal-acceleration) is spatial, so $Z_\mu a^\mu=\Theta_\mu a^\mu$. Part (iv) also gives $D^\mu Z_\mu=D^\mu\Theta_\mu-K\Theta$. Solving the preceding constraint for $\partial_t\Theta$ gives

$$
\partial_t\Theta=\beta^m\partial_m\Theta+\frac\alpha2
\left[
{}^{(3)}R+K(K-2\Theta)-K_{\mu\nu}K^{\mu\nu}
-2\Theta_\mu a^\mu-4\Theta
+2D^\mu\Theta_\mu-16\pi\rho
\right].
$$

Thus the constants in this [Z4 formulation](../../../numerical-relativity.md#z4-formulation) evolution equation are

$$
\boxed{d_1=-2,\qquad d_2=-2,\qquad d_3=2,\qquad d_4=-16\pi.}
$$

## 2

↑ **Parent:** [Paper 357](paper-357.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Set $A=1-2M/R=(R-2M)/R$ and

$$
F(R)=\frac{RM}{(R-M)(R-2M)},
\qquad dT=dt-F\,dR.
$$

Substitution into the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) gives

$$
ds^2=-A\,dt^2+2AF\,dt\,dR
+\left(A^{-1}-AF^2\right)dR^2+R^2d\Omega^2.
$$

The cross coefficient and radial coefficient simplify to

$$
AF=\frac{M}{R-M},
\qquad
A^{-1}-AF^2=\frac{R^2}{(R-M)^2}.
$$

Therefore

$$
\boxed{
ds^2=-\left(1-\frac{2M}{R}\right)dt^2
+\frac{2M}{R-M}\,dt\,dR
+\frac{R^2}{(R-M)^2}\,dR^2+R^2d\Omega^2.
}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

With $R=r+M$ and $dR=dr$,

$$
1-\frac{2M}{R}=\frac{r-M}{r+M},
\qquad
\frac{R^2}{(R-M)^2}=\left(\frac{r+M}{r}\right)^2.
$$

Defining the [conformal factor](../../../general-relativity.md#conformal-factor) by

$$
\psi^4=\left(\frac{r+M}{r}\right)^2,
$$

also gives $R^2=\psi^4r^2$. Hence

$$
\boxed{
ds^2=-\frac{r-M}{r+M}\,dt^2
+\frac{2M}{r}\,dt\,dr
+\psi^4\left(dr^2+r^2d\Omega^2\right).
}
$$

The constant-time spatial metric is therefore [conformally flat](../../../general-relativity.md#conformally-flat-metric).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Comparison with the [3+1 decomposition of spacetime](../../../numerical-relativity.md#3-plus-1-decomposition-of-spacetime) gives the diagonal spatial metric

$$
\boxed{
\gamma_{ij}
=\operatorname{diag}\left(
\frac{(r+M)^2}{r^2},\,
(r+M)^2,\,
(r+M)^2\sin^2\theta
\right).
}
$$

The mixed metric coefficient is $\beta_r=g_{tr}=M/r$. Raising its index with $\gamma^{rr}=r^2/(r+M)^2$ yields the [shift vector](../../../numerical-relativity.md#shift-vector)

$$
\boxed{
\beta^r=\frac{Mr}{(r+M)^2},
\qquad \beta^\theta=\beta^\phi=0.
}
$$

Now

$$
\beta_i\beta^i=\frac{M^2}{(r+M)^2}
$$

and $g_{tt}=-\alpha^2+\beta_i\beta^i=-(r-M)/(r+M)$. The positive [lapse function](../../../numerical-relativity.md#lapse-function) is consequently

$$
\boxed{\alpha=\frac{r}{r+M}.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The spatial metric is stationary and only $\beta^r=b(r)=Mr/(r+M)^2$ is nonzero. The evolution equation therefore says

$$
2\alpha K_{ij}=(\mathcal L_\beta\gamma)_{ij},
$$

the [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) of the spatial metric along the [shift vector](../../../numerical-relativity.md#shift-vector). For the radial component,

$$
2\alpha K_{rr}
=b\,\partial_r\gamma_{rr}
+2\gamma_{rr}\partial_rb
=-\frac{2M}{r(r+M)},
$$

so

$$
\boxed{K_{rr}=-\frac{M}{r^2}.}
$$

For the angular components,

$$
2\alpha K_{\theta\theta}
=b\,\partial_r(r+M)^2
=\frac{2Mr}{r+M},
$$

and spherical symmetry supplies

$$
\boxed{
K_{\theta\theta}=M,\qquad
K_{\phi\phi}=M\sin^2\theta.
}
$$

All off-diagonal components vanish.

Contracting with the inverse spatial metric gives the [mean curvature](../../../second-fundamental-form.md#mean-curvature)

$$
\begin{aligned}
K&=\gamma^{rr}K_{rr}
+\gamma^{\theta\theta}K_{\theta\theta}
+\gamma^{\phi\phi}K_{\phi\phi}\\
&=-\frac{M}{(r+M)^2}
+\frac{M}{(r+M)^2}
+\frac{M}{(r+M)^2}.
\end{aligned}
$$

Thus

$$
\boxed{K=\frac{M}{(r+M)^2}.}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Stationarity makes $\partial_t\alpha=0$, while

$$
\partial_r\alpha=\frac{M}{(r+M)^2}.
$$

The left side of the [Bona--Masso slicing condition](../../../numerical-relativity.md#bona-masso-slicing-condition) is therefore

$$
-\beta^r\partial_r\alpha
=-\frac{M^2r}{(r+M)^4}.
$$

Its right side is

$$
-\alpha^2f(\alpha)K
=-\frac{Mr^2}{(r+M)^4}f(\alpha).
$$

Equality requires

$$
f=\frac Mr.
$$

Since $\alpha=r/(r+M)$, this is the [Stationary Schwarzschild Bona--Masso slicing function](../../../numerical-relativity.md#stationary-schwarzschild-bona-masso-slicing-function)

$$
\boxed{f(\alpha)=\frac{1-\alpha}{\alpha}.}
$$

**Consequently $\lim_{\alpha\to1}f(\alpha)=0$, as expected in the asymptotically flat region $r\to\infty$.**

## 3

↑ **Parent:** [Paper 357](paper-357.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) invert to

$$
t=\frac{u+v}{2},\qquad z=\frac{v-u}{2}.
$$

Thus

$$
-dt^2+dz^2=-du\,dv
$$

and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) becomes

$$
\boxed{ds^2=-du\,dv+dx^2+dy^2.}
$$

The [coordinate basis](../../../differential-geometry.md#coordinate-basis) transforms by the chain rule:

$$
\boxed{
\partial_t=\partial_u+\partial_v,\qquad
\partial_z=-\partial_u+\partial_v,
}
$$

or equivalently

$$
\boxed{
\partial_u=\frac12(\partial_t-\partial_z),\qquad
\partial_v=\frac12(\partial_t+\partial_z).
}
$$

In the $(z,t)$ diagram, $\partial_t$ points vertically upward and $\partial_z$ horizontally right. The vector $\partial_u$ points along the future-left null ray and $\partial_v$ along the future-right null ray; their factors of one half affect length in the coordinate drawing but not direction.

Using these derivative relations, the [Minkowski wave operator in null coordinates](../../../special-relativity.md#minkowski-wave-operator-in-null-coordinates) is

$$
\boxed{
\Box=-\partial_t^2+\partial_z^2+\partial_x^2+\partial_y^2
=-4\partial_u\partial_v+\partial_x^2+\partial_y^2.
}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The phase is

$$
p_\rho x^\rho=-\omega t+\omega z=-\omega u.
$$

Because the [transverse-traceless gauge](../../../general-relativity.md#transverse-traceless-gauge) perturbation has no component along

$$
k=\frac1{\sqrt2}(\partial_t-\partial_z),
$$

only the third term of the [linearized Riemann curvature operator](../../../general-relativity.md#linearized-riemann-curvature-operator) contributes to the required contraction:

$$
\Psi_4
=-\frac12(k^\rho\partial_\rho)^2
\left(h_{\mu\nu}\bar m^\mu\bar m^\nu\right).
$$

The derivatives and transverse polarization contraction are

$$
k^\rho\partial_\rho e^{-i\omega u}
=-i\sqrt2\,\omega e^{-i\omega u},
$$



$$
H_{\mu\nu}\bar m^\mu\bar m^\nu
=H_+-iH_\times,
\qquad
\bar m=\frac1{\sqrt2}(\partial_x-i\partial_y).
$$

Therefore the [Newman--Penrose scalar Psi4](../../../general-relativity.md#newman-penrose-scalar-psi4) is

$$
\boxed{
\Psi_4
=\omega^2(H_+-iH_\times)e^{-i\omega u}.
}
$$

Its real and imaginary parts encode the plus and cross [gravitational wave polarizations](../../../general-relativity.md#gravitational-wave-polarization), up to the stated [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) and [complex null tetrad](../../../general-relativity.md#complex-null-tetrad) conventions.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Only the transverse coordinates occur in the perturbation, so its tensor components are unchanged by replacing $(t,z)$ with $(u,v)$. The [plane gravitational wave in linearized gravity](../../../general-relativity.md#plane-gravitational-wave-in-linearized-gravity) is

$$
h_{\mu\nu}dx^\mu dx^\nu
=e^{-i\omega u}
\left[
H_+(dx^2-dy^2)+2H_\times\,dx\,dy
\right].
$$

Every component depends on $u$ alone. The [Minkowski wave operator in null coordinates](../../../special-relativity.md#minkowski-wave-operator-in-null-coordinates) therefore gives

$$
\Box h_{\mu\nu}
=-4\partial_u\underbrace{\partial_vh_{\mu\nu}}_{0}
+\underbrace{\partial_x^2h_{\mu\nu}}_{0}
+\underbrace{\partial_y^2h_{\mu\nu}}_{0}
=0.
$$

**Thus the field satisfies the vacuum [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations).**

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Using the stated [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) in the definition of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor), the two nontrivial contractions are

$$
\begin{aligned}
R^x{}_{uxu}
&=-\partial_u\left(\frac{f'}f\right)
-\left(\frac{f'}f\right)^2
=-\frac{f''}f,\\
R^y{}_{uyu}
&=-\partial_u\left(\frac{g'}g\right)
-\left(\frac{g'}g\right)^2
=-\frac{g''}g.
\end{aligned}
$$

Hence

$$
R_{uu}=R^\alpha{}_{u\alpha u}
=-\frac{f''}f-\frac{g''}g,
$$

and the vacuum [Einstein field equations](../../../general-relativity.md#einstein-field-equations) reduce to

$$
\boxed{\frac{f''}f+\frac{g''}g=0.}
$$

This is the diagonal [Rosen coordinates for a plane gravitational wave](../../../general-relativity.md#rosen-coordinates-for-a-plane-gravitational-wave) equation.

For the plus-polarized wave, set

$$
H(u)=H_+e^{-i\omega u}.
$$

Comparison of the transverse metric components gives, to [linear order](../../../algebra.md#linear-order),

$$
f(u)^2=1+H(u),\qquad
g(u)^2=1-H(u),
$$

or

$$
f(u)=1+\frac12H(u)+O(H_+^2),
\qquad
g(u)=1-\frac12H(u)+O(H_+^2).
$$

Therefore

$$
\frac{f''}f+\frac{g''}g
=\frac12H''-\frac12H''+O(H_+^2)
=O(H_+^2).
$$

The [Vacuum Einstein equations](../../../general-relativity.md#vacuum-einstein-equations) are consequently satisfied at linear order. A real gravitational wave is obtained by taking the real part of the complex plane-wave notation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
