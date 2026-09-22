# Paper 2

↑ **Parent:** [2018](../2018.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2018/papernst_ib_2_2018.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2018/papernst_ib_2_2018.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
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
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [i](#5/d/i)
      - [Solution](#5/d/i/solution)
    - [ii](#5/d/ii)
      - [Solution](#5/d/ii/solution)
    - [iii](#5/d/iii)
      - [Solution](#5/d/iii/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
    - [iv](#6/b/iv)
      - [Solution](#6/b/iv/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Seek a positive weight such that the [differential operator](../../analysis.md#differential-operator) becomes $-w^{-1}(py')'$. Matching the second [derivative](../../calculus.md#derivative) gives $p=w(1-x^2)$, while matching the first [derivative](../../calculus.md#derivative) requires $p'=-xw$. Consequently

$$
(1-x^2)w'-2xw=-xw,\qquad \frac{w'}w=\frac{x}{1-x^2}.
$$

Choosing the multiplicative constant to be one gives

$$
\boxed{w(x)=\frac1{\sqrt{1-x^2}},\qquad p(x)=\sqrt{1-x^2},\qquad -(py_n')'=n^2wy_n}.
$$

This is [Sturm-Liouville form](../../sturm-liouville-theory.md#sturm-liouville-form) with zero potential term. Multiply the equations for $y_n,y_m$ by $y_m,y_n$, subtract, and integrate. The [Lagrange identity for a Sturm-Liouville operator](../../sturm-liouville-theory.md#lagrange-identity-for-a-sturm-liouville-operator) gives

$$
(n^2-m^2)\int_{-1}^1wy_ny_m\,dx
=\left[p(y_ny_m'-y_my_n')\right]_{-1}^{1}=0.
$$

The boundary expression vanishes because $p\to0$ and the functions and their [derivatives](../../calculus.md#derivative) are finite. Since $n,m\geq0$ are distinct, their [eigenvalues](../../linear-operator-theory.md#eigenvalue) $n^2,m^2$ are distinct, proving

$$
\boxed{\int_{-1}^{1}\frac{y_n(x)y_m(x)}{\sqrt{1-x^2}}\,dx=0\quad(n\ne m)}.
$$

The endpoint singularities of the weight are integrable, so these [weighted inner products](../../inner-product.md#weighted-inner-product) exist.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $n=0$, a constant solution and its normalization give $y_0=1$. For $n=1$, substitute $y=ax+b$: the equation gives $b=0$, and the normalization gives $a=1$. For $n=2$, put $y=ax^2+bx+c$. Comparing coefficients gives $b=0$ and $c=-a/2$; then $y(1)=1$ fixes $a=2$. Thus

$$
\boxed{y_0=1,\qquad y_1=x,\qquad y_2=2x^2-1}.
$$

These are the first three [Chebyshev polynomials](../../numerical-analysis.md#chebyshev-polynomial). For their squared [weighted norms](../../inner-product.md#weighted-norm), use $x=\cos\theta$, which converts $dx/\sqrt{1-x^2}$ into $-d\theta$:

$$
\boxed{I_0=\int_0^\pi1\,d\theta=\pi,\qquad
I_1=\int_0^\pi\cos^2\theta\,d\theta=\frac\pi2}.
$$

More generally, $y_n(\cos\theta)=\cos(n\theta)$ makes their [orthogonality](../../inner-product.md#orthogonal-vectors) the usual [cosine](../../geometry-and-topology.md#cosine) [orthogonality](../../inner-product.md#orthogonal-vectors).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Let $L=-(1-x^2)D^2+xD$, so $Ly_n=n^2y_n$ and the forced equation is $(\gamma^2-L)Z=e^{\varepsilon x}$. The small-parameter [Taylor expansion](../../calculus.md#taylor-expansion) of the forcing is

$$
e^{\varepsilon x}=1+\varepsilon x+\frac{\varepsilon^2x^2}{2}+O(\varepsilon^3)
=y_0+\varepsilon y_1+\frac{\varepsilon^2}{4}(y_0+y_2)+O(\varepsilon^3).
$$

Each [Chebyshev polynomial](../../numerical-analysis.md#chebyshev-polynomial) can be inverted separately under $\gamma^2-L$. None of the required denominators vanishes because $\gamma$ is a real noninteger. Thus the [regular solution of a forced Chebyshev equation](../../numerical-analysis.md#regular-solution-of-a-forced-chebyshev-equation) has

$$
\boxed{A=\frac{y_0}{\gamma^2},\qquad
B=\frac{y_1}{\gamma^2-1},\qquad
C=\frac{y_0}{4\gamma^2}+\frac{y_2}{4(\gamma^2-4)}}.
$$

Here we select the same regular endpoint domain as in part (a), with finite function values and finite endpoint [derivatives](../../calculus.md#derivative). This qualification is needed: the printed forced equation alone does not state endpoint conditions. Without this selection one can add $c_1\cos(\gamma\arccos x)+c_2\sin(\gamma\arccos x)$, which remain finite but generally have singular endpoint [derivatives](../../calculus.md#derivative). With $x=\cos\theta$, regularity gives $Z_\theta(0)=Z_\theta(\pi)=0$; the corresponding homogeneous equation has only the zero solution for noninteger $\gamma$. This makes the displayed expansion unique.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Write the integral's multiplier in the [Chebyshev polynomial](../../numerical-analysis.md#chebyshev-polynomial) basis:

$$
(1-x^2)^{-1/2}+(1-x^2)^{1/2}
=w(2-x^2)=w\left(\frac32y_0-\frac12y_2\right).
$$

At $\gamma^2=5$, part (i) gives

$$
Z=\left(\frac15+\frac{\varepsilon^2}{20}\right)y_0
+\frac\varepsilon4y_1+\frac{\varepsilon^2}{4}y_2+O(\varepsilon^3).
$$

By [orthogonality](../../inner-product.md#orthogonal-vectors), the $y_1$ term and all cross terms vanish. Using $I_0=\pi$ and $I_2=\pi/2$, the integral is

$$
\frac32\pi\left(\frac15+\frac{\varepsilon^2}{20}\right)
-\frac12\frac\pi2\frac{\varepsilon^2}{4}+O(\varepsilon^3)
=\boxed{\frac{3\pi}{10}+\frac{\pi}{80}\varepsilon^2+O(\varepsilon^3)}.
$$

The remainder can be integrated against this integrable weight in the regular expansion, so it retains the stated order.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $\Psi=U(r)V(\phi)$ in the [Laplace equation](../../partial-differential-equation.md#laplace-equation) in [polar coordinates](../../multivariable-calculus.md#polar-coordinates). After multiplication by $r^2/(UV)$, [separation of variables](../../partial-differential-equation.md#separation-of-variables) gives

$$
\frac{r^2U''+rU'}U=-\frac{V''}V=n^2.
$$

The angular function is $2\pi$-periodic and single-valued, so its nonconstant modes are $\cos(n\phi),\sin(n\phi)$ with integer $n\geq1$. Their radial [Euler differential equation](../../linear-ordinary-differential-equation.md#cauchy-euler-equation) has solutions $r^n,r^{-n}$; finiteness at the origin excludes $r^{-n}$.

The zero angular mode has constant angular part and radial solutions $1,\log r$. The logarithmic term is again excluded at the origin. [Superposition](../../vector-space.md#superposition-principle) therefore yields

$$
\boxed{\Psi(r,\phi)=A_0+\sum_{n=1}^\infty r^n[A_n\cos(n\phi)+B_n\sin(n\phi)]}.
$$

This is the regular harmonic expansion inside the disk.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

On the boundary, integrate the expansion from part (a) over one angular period. Every nonconstant [sine](../../geometry-and-topology.md#sine) and [cosine](../../geometry-and-topology.md#cosine) has zero average, so

$$
\int_0^{2\pi}f(\phi)\,d\phi=2\pi A_0.
$$

All positive-power radial terms vanish at $r=0$, leaving $\Psi(0)=A_0$. Hence

$$
\boxed{\Psi(0)=\frac1{2\pi}\int_0^{2\pi}f(\phi)\,d\phi
=\frac1{2\pi R}\int_{r=R}f\,ds}.
$$

This is the [mean value property for harmonic functions](../../partial-differential-equation.md#mean-value-property-for-harmonic-functions). It is an average over arclength as well as over angle, since $ds=R\,d\phi$. The usual continuity or integrable-boundary-data hypotheses justify taking this angular average.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write the boundary [Fourier series](../../fourier-series.md) as $f=A_0+\sum_{n\geq1}(a_n\cos n\phi+b_n\sin n\phi)$. Since $R=2$, its coefficients obey $a_n=2^nA_n$ and $b_n=2^nB_n$. The mean is

$$
A_0=\frac1{2\pi}\left(\pi+\int_\pi^{2\pi}\cos^2\phi\,d\phi\right)=\frac34.
$$

For $n\geq1$, the integral of $\cos n\phi$ on the first semicircle is zero. On the second semicircle, use $\cos^2\phi=(1+\cos2\phi)/2$ and [cosine](../../geometry-and-topology.md#cosine) [orthogonality](../../inner-product.md#orthogonal-vectors). This gives $a_2=1/4$ and every other $a_n=0$.

For the [sine](../../geometry-and-topology.md#sine) coefficients, every even $n$ gives zero on both semicircles. For odd $n$, [product-to-sum formulas](../../geometry-and-topology.md#product-to-sum-formula) give

$$
\begin{aligned}
\pi b_n&=\int_0^\pi\sin n\phi\,d\phi+
\int_\pi^{2\pi}\frac{1+\cos2\phi}{2}\sin n\phi\,d\phi\\
&=\frac2n-\frac1n-\frac12\left(\frac1{n+2}+\frac1{n-2}\right)
=\frac{4}{n(4-n^2)}.
\end{aligned}
$$

Thus the requested radial-expansion coefficients are

$$
\boxed{A_0=\frac34,\qquad A_n=\begin{cases}1/16,&n=2,\\0,&n\ne2,\end{cases}\qquad
B_n=\begin{cases}\displaystyle\frac{4}{\pi\,2^n n(4-n^2)},&n\text{ odd},\\0,&n\text{ even}.\end{cases}}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For any interior point $\mathbf p$, choose a sufficiently small circle centred on $\mathbf p$ and wholly inside the disk. Translating the origin does not change the [Laplace equation](../../partial-differential-equation.md#laplace-equation), so part (b) gives

$$
\Psi(\mathbf p)=\frac1{2\pi}\int_0^{2\pi}\Psi(\mathbf p+\rho(\cos\theta,\sin\theta))\,d\theta.
$$

Suppose a real [harmonic function](../../partial-differential-equation.md#harmonic-function), continuous on the closed disk, attains its global maximum $M$ at an interior point. Every value on each such circle is at most $M$, and their average is $M$. By continuity, every value on the circle must therefore equal $M$. Varying its radius shows that a neighbourhood of the point also has value $M$.

Thus the set of points attaining $M$ is open in the disk, and it is closed by continuity. The disk is connected, so this set must be the whole disk. The function is constant and has the same maximum on the boundary. Otherwise the maximum cannot be interior. Compactness of the closed disk guarantees existence of a maximum, proving the [maximum principle for harmonic functions](../../partial-differential-equation.md#maximum-principle-for-harmonic-functions):

$$
\boxed{\max_{r\leq R}\Psi=\max_{r=R}\Psi}.
$$

Continuity up to the boundary is the standard hypothesis for this attained-maximum formulation.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the convention $\Delta G=+\delta^{(3)}$. The [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function) for this [Poisson equation](../../partial-differential-equation.md#poisson-s-equation) satisfies, for each source point $\mathbf r'\in V$,

$$
\boxed{\Delta_{\mathbf r}G(\mathbf r,\mathbf r')=\delta^{(3)}(\mathbf r-\mathbf r')\quad\text{in }V,
\qquad G(\mathbf r,\mathbf r')=0\quad\text{on }S}.
$$

It is a [harmonic function](../../partial-differential-equation.md#harmonic-function) away from its source, with a unit delta singularity there. Its [boundary condition](../../differential-equation.md#boundary-condition) is homogeneous even when the original potential has nonzero boundary values; those values enter through the boundary integral. This sign convention is the one giving the plus signs in the formula requested in part (b).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply [Green's second identity](../../partial-differential-equation.md#green-second-identity) to $\Phi(\mathbf r)$ and $G(\mathbf r,\mathbf r')$, differentiating in $\mathbf r$:

$$
\int_V(\Phi\Delta G-G\Delta\Phi)\,dV
=\int_S\left(\Phi\frac{\partial G}{\partial n}-G\frac{\partial\Phi}{\partial n}\right)dS.
$$

The volume terms become $\Phi(\mathbf r')-\int_VG\rho\,dV$. On the boundary $G=0$ and $\Phi=f$, so

$$
\boxed{\Phi(\mathbf r')=\int_V\rho(\mathbf r)G(\mathbf r,\mathbf r')\,dV
+\int_S f(\mathbf r)\frac{\partial G}{\partial n}(\mathbf r,\mathbf r')\,dS}.
$$

Here $\partial/\partial n$ is the outward [normal derivative](../../differential-geometry.md#normal-derivative) in the integration variable. One may justify the identity at the singularity by excising a small sphere around $\mathbf r'$; its unit flux supplies the evaluation $\Phi(\mathbf r')$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $\Delta G=+\delta^{(3)}$, the [fundamental solution of the Laplace equation](../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation) in three dimensions is

$$
\boxed{G_0(\mathbf r,\mathbf r')=-\frac1{4\pi|\mathbf r-\mathbf r'|}}.
$$

Its sign follows from the flux: on a small sphere of radius $\varepsilon$, its outward radial [derivative](../../calculus.md#derivative) is $1/(4\pi\varepsilon^2)$, with total flux one.

Let $s=|\mathbf r'|\in(0,1)$ and put the image point at $\mathbf r'^*=\mathbf r'/s^2$. The [method of images](../../mathematics.md#method-of-images) gives the [Dirichlet Green function inside a sphere](../../green-s-function.md#dirichlet-green-function-inside-a-sphere):

$$
\boxed{G_B(\mathbf r,\mathbf r')=-\frac1{4\pi}
\left[\frac1{|\mathbf r-\mathbf r'|}-\frac1{s|\mathbf r-\mathbf r'^*|}\right]}.
$$

The image lies outside the ball, so its potential is harmonic inside. On $|\mathbf r|=1$, the identity $|\mathbf r-\mathbf r'|=s|\mathbf r-\mathbf r'^*|$ makes the two terms cancel. The original source retains unit strength. For a source at the centre, take the limit:

$$
\boxed{G_B(\mathbf r,0)=-\frac1{4\pi}\left(\frac1{|\mathbf r|}-1\right)}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $\overline{\mathbf r'}=(x',y',-z')$ be reflection of the interior source across the equatorial plane. Using the ball [Green's function](../../green-s-function.md) from part (c), form

$$
\boxed{G_H(\mathbf r,\mathbf r')=G_B(\mathbf r,\mathbf r')-G_B(\mathbf r,\overline{\mathbf r'})}.
$$

Both terms vanish on the unit sphere. On the flat disk $z=0$, distances to reflected points coincide, and the same is true of their inversion images, so the difference is zero there as well. Only $\mathbf r'$ is inside the upper half-ball; the reflected source is in the lower half-ball, and both inversion images lie outside the full ball. Thus there is exactly one interior delta source, of the required strength.

Explicitly, with $s=|\mathbf r'|$ and stars denoting inversion in the unit sphere,

$$
\boxed{G_H=-\frac1{4\pi}\left[
\frac1{|\mathbf r-\mathbf r'|}-\frac1{s|\mathbf r-\mathbf r'^*|}
-\frac1{|\mathbf r-\overline{\mathbf r'}|}+\frac1{s|\mathbf r-\overline{\mathbf r'}^*|}
\right]}.
$$

This is the [Dirichlet Green function inside a hemisphere](../../green-s-function.md#dirichlet-green-function-inside-a-hemisphere), constructed from four image-source terms.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A sufficient [contour](../../complex-analysis.md#complex-integration-contour) setting for both results is a positively oriented, simple, closed, piecewise smooth [contour](../../complex-analysis.md#complex-integration-contour) $C$, with the function [holomorphic](../../holomorphic-function.md) on an open neighbourhood of $C$ and its entire interior. The [Cauchy integral theorem](../../complex-analysis.md#cauchy-s-integral-theorem) then states

$$
\boxed{\oint_C f(z)\,dz=0}.
$$

If $z_0$ is strictly inside $C$, the [Cauchy integral formula](../../analysis.md#cauchy-integral-formula) states

$$
\boxed{f(z_0)=\frac1{2\pi i}\oint_C\frac{f(z)}{z-z_0}\,dz}.
$$

The [contour](../../complex-analysis.md#complex-integration-contour) must not pass through $z_0$. Positive orientation means anticlockwise; reversing it reverses the sign of the [contour](../../complex-analysis.md#complex-integration-contour) integral. The holomorphy assumption throughout the interior excludes hidden singularities there.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The only denominator zero is $z_0=-1$, which lies strictly inside the given circle. The numerator is an [entire function](../../holomorphic-function.md#entire-function). Apply the [derivative](../../calculus.md#derivative) form of the [Cauchy integral formula](../../analysis.md#cauchy-integral-formula) with $n=6$:

$$
\oint_C\frac{\sin z}{(z+1)^7}\,dz
=\frac{2\pi i}{6!}\left.\frac{d^6}{dz^6}\sin z\right|_{z=-1}.
$$

The sixth [derivative](../../calculus.md#derivative) is $-\sin z$, so its value at $-1$ is $\sin1$. Consequently

$$
\boxed{\oint_C\frac{\sin z}{(z+1)^7}\,dz=\frac{\pi i\sin1}{360}}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For a positively oriented simple closed [contour](../../complex-analysis.md#complex-integration-contour), the [residue theorem](../../analysis.md#residue-theorem) states that the integral of a function holomorphic on and inside the [contour](../../complex-analysis.md#complex-integration-contour) except at finitely many isolated interior singularities is $2\pi i$ times the sum of its [residues](../../analysis.md#residue). There must be no singularity on the [contour](../../complex-analysis.md#complex-integration-contour).

Factor the denominator as $(z^2+z+1)(z^2-z+1)$. For $R>1$, the upper semicircle encloses the two [simple poles](../../isolated-singularity.md#simple-pole)

$$
a=\frac12+\frac{i\sqrt3}{2},\qquad b=-\frac12+\frac{i\sqrt3}{2}.
$$

The other two [poles](../../isolated-singularity.md#pole) are in the lower half-plane. Since $D'(z)=4z^3+2z=2z(2z^2+1)$,

$$
\operatorname{Res}_{a}g=\frac{e^{ia}}{2i\sqrt3\,a},\qquad
\operatorname{Res}_{b}g=-\frac{e^{ib}}{2i\sqrt3\,b}.
$$

Writing $h=\sqrt3/2$ and using $1/a=1/2-ih$, $1/b=-1/2-ih$, their numerator difference simplifies to

$$
\frac{e^{ia}}a-\frac{e^{ib}}b
=e^{-h}\left[\left(\frac12-ih\right)e^{i/2}+\left(\frac12+ih\right)e^{-i/2}\right]
=e^{-h}\left[\cos\frac12+\sqrt3\sin\frac12\right].
$$

Thus for every $R>1$ the closed-contour integral is

$$
\oint_{L_R\cup C_R}g(z)\,dz
=\frac\pi{\sqrt3}e^{-\sqrt3/2}\left[\cos\frac12+\sqrt3\sin\frac12\right].
$$

To remove the arc, on $C_R$ we have $|e^{iz}|=e^{-\operatorname{Im}z}\leq1$ and $|z^4+z^2+1|\geq R^4-R^2-1$. For sufficiently large $R$, the [complex line integral estimate](../../complex-analysis.md#complex-line-integral-estimate) gives

$$
\left|\int_{C_R}g(z)\,dz\right|
\leq\frac{\pi R}{R^4-R^2-1}\longrightarrow0.
$$

The real-line integral is absolutely convergent. Its imaginary part is zero by oddness of $\sin x/(x^4+x^2+1)$. Therefore

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{x^4+x^2+1}\,dx
=\frac\pi{\sqrt3}e^{-\sqrt3/2}\left[\cos\frac12+\sqrt3\sin\frac12\right]}.
$$

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A sufficient assumption is that $f$ is absolutely continuous, $f,f'\in L^1(\mathbb R)$, and $f(t)\to0$ at both infinities. [Integration by parts](../../calculus.md#integration-by-parts) in the [Fourier transform](../../fourier-transform.md) gives

$$
\widetilde{f'}(\omega)
=\left[f(t)e^{-i\omega t}\right]_{-\infty}^{\infty}
+i\omega\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt
=\boxed{i\omega\widetilde f(\omega)}.
$$

The decay assumption removes the boundary term, and integrability makes both transforms ordinary convergent integrals. The same [derivative](../../calculus.md#derivative) identity extends to [tempered distributions](../../fourier-analysis.md#tempered-distribution).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Apply the [Fourier transform of a derivative](../../fourier-analysis.md#fourier-transform-of-a-derivative) twice to the [damped harmonic oscillator](../../analysis.md#damped-harmonic-oscillator) equation. Under the corresponding convergence assumptions,

$$
(-\omega^2+2i\kappa\omega+\Omega^2)\widetilde y(\omega)=\widetilde f(\omega).
$$

Thus

$$
\boxed{\widetilde y(\omega)=\widetilde h(\omega)\widetilde f(\omega),\qquad
\widetilde h(\omega)=\frac1{\Omega^2-\omega^2+2i\kappa\omega}}.
$$

Since $\kappa,\Omega>0$, this denominator has no real zero: its imaginary part could vanish only at $\omega=0$, where its real part is positive. The transform therefore defines a regular response on the real frequency axis.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $\beta=\sqrt{\Omega^2-\kappa^2}$, interpreted as $i\sqrt{\kappa^2-\Omega^2}$ in the [overdamped](../../wave-equation.md#overdamping) case. Factoring the denominator gives

$$
\Omega^2-\omega^2+2i\kappa\omega=-(\omega-\omega_-)(\omega-\omega_+),\qquad
\boxed{\omega_\pm=i\kappa\pm\beta}.
$$

[Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) and the [convolution theorem](../../fourier-analysis.md#convolution-theorem) give

$$
\boxed{y(t)=\int_{-\infty}^{\infty}G(t-\xi)f(\xi)\,d\xi},
$$

where

$$
G(t)=-\frac1{2\pi}\int_{-\infty}^{\infty}
\frac{e^{i\omega t}}{(\omega-\omega_-)(\omega-\omega_+)}\,d\omega.
$$

Thus the requested numerator is

$$
\boxed{s(\omega,t)=-\frac1{2\pi}e^{i\omega t}}.
$$

For all positive $\kappa,\Omega$, both [poles](../../isolated-singularity.md#pole) lie in the upper half-plane. In the [overdamped](../../wave-equation.md#overdamping) case their imaginary parts are $\kappa\pm\sqrt{\kappa^2-\Omega^2}$, both positive. At equality they merge into a double [pole](../../isolated-singularity.md#pole).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/i">i</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/i/solution">Solution</h5>

↑ **Parent:** [I](#5/d/i)

For $t>0$, close the inverse-transform [contour](../../complex-analysis.md#complex-integration-contour) in the upper half-plane. There $|e^{i\omega t}|\leq1$; the rational factor is $O(|\omega|^{-2})$, so the arc integral vanishes. For $\Omega>\kappa$, write $\beta=\sqrt{\Omega^2-\kappa^2}>0$. The two [simple poles](../../isolated-singularity.md#simple-pole) are $i\kappa\pm\beta$, and the [residue theorem](../../analysis.md#residue-theorem) yields

$$
\begin{aligned}
G(t)&=-i\left[\frac{e^{i\omega_+t}}{\omega_+-\omega_-}
+\frac{e^{i\omega_-t}}{\omega_--\omega_+}\right]\\
&=-i e^{-\kappa t}\frac{e^{i\beta t}-e^{-i\beta t}}{2\beta}
=\boxed{e^{-\kappa t}\frac{\sin(\beta t)}\beta}.
\end{aligned}
$$

This [causal Green function of a damped oscillator](../../analysis.md#causal-green-function-of-a-damped-oscillator) has damped oscillations with envelope $e^{-\kappa t}$ and tends to zero as $t\to\infty$.

<h4 id="5/d/ii">ii</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/d/ii)

For $\kappa>\Omega$, put $\eta=\sqrt{\kappa^2-\Omega^2}$, so $0<\eta<\kappa$ and the [poles](../../isolated-singularity.md#pole) are $i(\kappa\pm\eta)$. Closing in the upper half-plane for $t>0$ again includes both [simple poles](../../isolated-singularity.md#simple-pole). The [residue theorem](../../analysis.md#residue-theorem) gives

$$
\boxed{G(t)=e^{-\kappa t}\frac{\sinh(\eta t)}\eta
=\frac{e^{-(\kappa-\eta)t}-e^{-(\kappa+\eta)t}}{2\eta}}.
$$

This [overdamped](../../wave-equation.md#overdamping) response has no oscillation. Its slow tail is $e^{-(\kappa-\eta)t}/(2\eta)$, and it tends to zero because $\eta<\kappa$.

<h4 id="5/d/iii">iii</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/d/iii)

At $\Omega=\kappa$, the inverse-transform denominator is $-(\omega-i\kappa)^2$. For $t>0$, its upper-half-plane double-pole [residue](../../analysis.md#residue) is the [derivative](../../calculus.md#derivative) of the exponential:

$$
G(t)=-i\left.\frac{d}{d\omega}e^{i\omega t}\right|_{\omega=i\kappa}
=\boxed{t e^{-\kappa t}}.
$$

It is also the continuous limit of both answers above as $\beta\to0$ or $\eta\to0$. This [critically damped](../../wave-equation.md#critical-damping) response tends to zero with a linear factor multiplying the exponential.

In all three cases, for $t<0$ close the [contour](../../complex-analysis.md#complex-integration-contour) in the lower half-plane, where $e^{i\omega t}$ decays. There are no [poles](../../isolated-singularity.md#pole) inside, so

$$
\boxed{G(t)=0\quad(t<0)}.
$$

At $t=0$ its continuous value is zero and $G'(0^+)=1$, producing the unit [derivative](../../calculus.md#derivative) jump required by $(D_t^2+2\kappa D_t+\Omega^2)G=\delta(t)$. Thus all three formulas are causal [Green's functions](../../green-s-function.md) and all decay to zero at late times.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

For the critically damped case, causality reduces the [convolution](../../fourier-analysis.md#convolution) to

$$
y(t)=\int_0^\infty s e^{-\kappa s}\cos[\kappa(t-s)]\,ds.
$$

Although the forcing is not integrable on the full real line, this integral converges absolutely because the [Green's function](../../green-s-function.md) is integrable. Thus the calculation is valid directly; the corresponding [Fourier transform](../../fourier-transform.md) can be interpreted as a [tempered distribution](../../fourier-analysis.md#tempered-distribution).

Use the [complex exponential](../../calculus.md#complex-exponential-function) and $\int_0^\infty s e^{-as}\,ds=a^{-2}$ for $\operatorname{Re}a>0$:

$$
y(t)=\operatorname{Re}\left[e^{i\kappa t}\int_0^\infty s e^{-\kappa(1+i)s}\,ds\right]
=\operatorname{Re}\left[\frac{e^{i\kappa t}}{\kappa^2(1+i)^2}\right].
$$

Since $(1+i)^2=2i$, the [convolution](../../fourier-analysis.md#convolution) response is

$$
\boxed{y(t)=\frac{\sin(\kappa t)}{2\kappa^2}}.
$$

This is the bounded steady response to the stated forcing acting for all time. Without an [initial condition](../../differential-equation.md#initial-condition) or the [convolution](../../fourier-analysis.md#convolution) selection, the general solution additionally contains $(C_1+C_2t)e^{-\kappa t}$. No switch-on at $t=0$ was specified, so zero initial displacement and [velocity](../../classical-mechanics.md#velocity) should not be imposed on this all-time forcing.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Split the [Cartesian second-rank tensor](../../multilinear-algebra.md#cartesian-second-rank-tensor) into symmetric and antisymmetric parts:

$$
S_{ij}=\frac{T_{ij}+T_{ji}}2,\qquad A_{ij}=\frac{T_{ij}-T_{ji}}2.
$$

Define $u_k=\frac12\epsilon_{kij}T_{ij}$. The symmetric part contributes zero to this contraction. The [epsilon-delta identity](../../multivariable-calculus.md#contraction-of-two-levi-civita-symbols) then gives

$$
\epsilon_{ijk}u_k=\frac12\epsilon_{ijk}\epsilon_{klm}T_{lm}
=\frac12(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})T_{lm}
=\frac{T_{ij}-T_{ji}}2=A_{ij}.
$$

Therefore

$$
\boxed{T_{ij}=S_{ij}+\epsilon_{ijk}u_k,\qquad
S_{ij}=\frac{T_{ij}+T_{ji}}2,\qquad u_k=\frac12\epsilon_{kij}T_{ij}}.
$$

The symmetric part and the three independent antisymmetric components determine these quantities uniquely. Under proper rotations $u$ is a [vector](../../vector-space.md#vector); under reflections it is an [axial vector](../../vector-space.md#pseudovector).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

Apply the [symmetric gradient and curl decomposition](../../multilinear-algebra.md#symmetric-gradient-and-curl-decomposition) separately to the [electric field](../../electric-field.md) and the [magnetic field](../../magnetic-field.md):

$$
\boxed{S^E_{ij}=\frac12(\partial_iE_j+\partial_jE_i),\qquad
S^B_{ij}=\frac12(\partial_iB_j+\partial_jB_i)}.
$$

The corresponding axial parts are

$$
\boxed{\mathbf u^E=\frac12\nabla\times\mathbf E=-\frac12\partial_t\mathbf B,
\qquad
\mathbf u^B=\frac12\nabla\times\mathbf B=\frac1{2c^2}\partial_t\mathbf E}.
$$

The second equalities use the vacuum [Maxwell equations](../../maxwell-equations.md). Their [divergence](../../multivariable-calculus.md#divergence) constraints also show that both symmetric [gradient](../../multivariable-calculus.md#gradient) [tensors](../../multilinear-algebra.md#tensor) are traceless.

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Differentiate $\mathbf u^E=\frac12\nabla\times\mathbf E$ with respect to time. The vacuum [Maxwell equations](../../maxwell-equations.md) give $\partial_t\mathbf E=c^2\nabla\times\mathbf B$, so

$$
\partial_t\mathbf u^E=\frac{c^2}{2}\nabla\times(\nabla\times\mathbf B).
$$

The [curl of the curl identity](../../multivariable-calculus.md#curl-of-the-curl-identity) is $\nabla\times(\nabla\times\mathbf B)=\nabla(\nabla\cdot\mathbf B)-\nabla^2\mathbf B$. Since $\nabla\cdot\mathbf B=0$,

$$
\boxed{\frac{\partial\mathbf u^E}{\partial t}=-\frac{c^2}{2}\nabla^2\mathbf B}.
$$

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

The same [Maxwell equations](../../maxwell-equations.md) give

$$
\partial_t\mathbf u^B=\frac12\nabla\times\partial_t\mathbf B
=-\frac12\nabla\times(\nabla\times\mathbf E)=\frac12\nabla^2\mathbf E,
$$

where the last equality uses $\nabla\cdot\mathbf E=0$. Combining with part (ii),

$$
\partial_t(u_i^E+u_i^B)=\frac12\nabla^2E_i-\frac{c^2}{2}\nabla^2B_i.
$$

The divergences of the symmetric gradients satisfy

$$
\partial_jS^E_{ij}=\frac12(\partial_i\partial_jE_j+\partial_j\partial_jE_i)=\frac12\nabla^2E_i,
\qquad \partial_jS^B_{ij}=\frac12\nabla^2B_i.
$$

Thus the local identity is $\partial_t(u_i^E+u_i^B)=\partial_j(S^E_{ij}-c^2S^B_{ij})$. Integrate over the fixed volume and apply the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) componentwise:

$$
\boxed{\frac\partial{\partial t}\int_V(u_i^E+u_i^B)\,dV
=\oint_A(S^E_{ij}-c^2S^B_{ij})\,dA_j}.
$$

Here $dA_j=n_jdA$ uses the outward [normal vector](../../differential-geometry.md#normal-vector).

<h4 id="6/b/iv">iv</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/b/iv)

The [divergence of a cross product](../../multivariable-calculus.md#divergence-of-a-cross-product) identity and the vacuum [Maxwell equations](../../maxwell-equations.md) imply

$$
\begin{aligned}
\nabla\cdot(\mathbf B\times\mathbf E)
&=\mathbf E\cdot(\nabla\times\mathbf B)-\mathbf B\cdot(\nabla\times\mathbf E)\\
&=\frac1{c^2}\mathbf E\cdot\partial_t\mathbf E+\mathbf B\cdot\partial_t\mathbf B\\
&=\partial_t\left(\frac{|\mathbf E|^2}{2c^2}+\frac{|\mathbf B|^2}{2}\right).
\end{aligned}
$$

The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) therefore gives the required balance with

$$
\boxed{\lambda=\frac12\left(\frac{|\mathbf E|^2}{c^2}+|\mathbf B|^2\right)},\qquad
\boxed{\frac\partial{\partial t}\int_V\lambda\,dV=\oint_A(\mathbf B\times\mathbf E)\cdot d\mathbf A}.
$$

An additive time-independent constant in $\lambda$ is immaterial. This is the vacuum [Poynting theorem](../../electromagnetic-wave.md#poynting-theorem) in the normalization of the given equations: equivalently $\partial_t\lambda+\nabla\cdot(\mathbf E\times\mathbf B)=0$. The order of the [cross product](../../vector-space.md#cross-product) accounts for the plus sign in the stated integral identity.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Choose [generalized coordinates](../../lagrangian-mechanics.md#generalized-coordinate) $q_i$ measured from a static [equilibrium point](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), and assume a conservative system with no velocity-dependent forces. Keeping terms of degree two in displacements and velocities gives the [small oscillation](../../lagrangian-mechanics.md#small-oscillation) [Lagrangian](../../calculus-of-variations.md#lagrangian)

$$
\boxed{\mathcal L=\frac12\dot{\mathbf q}^{\,T}A\dot{\mathbf q}-\frac12\mathbf q^TB\mathbf q}.
$$

Here $A$ is the positive-definite symmetric [mass](../../classical-mechanics.md#mass) [matrix](../../vector-space.md#matrix) evaluated at equilibrium, and $B$ is the symmetric [Hessian matrix](../../multivariable-calculus.md#hessian-matrix) of the [potential energy](../../energy.md#potential-energy) there. The linear potential term is zero by equilibrium, and an additive constant has been dropped. Coordinate-dependent corrections to the kinetic [matrix](../../vector-space.md#matrix) contribute only at higher order.

The [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) are $A\ddot{\mathbf q}+B\mathbf q=0$. For a [normal mode](../../wave-equation.md#normal-mode) $\mathbf q=\mathbf v e^{i\omega t}$, they give the [generalized eigenvalue problem](../../linear-operator-theory.md#generalized-eigenvalue-problem) $(B-\omega^2A)\mathbf v=0$. A nonzero [mode shape](../../wave-equation.md#mode-shape) exists exactly when

$$
\boxed{\det(B-\omega^2A)=0}.
$$

This is a degree-$n$ [polynomial](../../polynomial.md) in $\omega^2$. At a stable equilibrium its roots are nonnegative; zero roots correspond to [zero modes](../../linear-operator-theory.md#zero-mode).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

Choose positive $\phi$ so the bob is displaced to the right relative to the cart. Its [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system) are

$$
X=x+L\sin\phi,\qquad Y=-L\cos\phi.
$$

Differentiation gives $\dot X^2+\dot Y^2=\dot x^2+2L\cos\phi\,\dot x\dot\phi+L^2\dot\phi^2$. Thus the exact [kinetic energy](../../energy.md#kinetic-energy) and [potential energy](../../energy.md#potential-energy) are

$$
T=\frac12(m+M)\dot x^2+ML\cos\phi\,\dot x\dot\phi+\frac12ML^2\dot\phi^2,
\qquad V=\frac12kx^2+MgL(1-\cos\phi).
$$

Retain quadratic terms, using $\cos\phi=1+O(\phi^2)$ in the kinetic cross term and $1-\cos\phi=\phi^2/2+O(\phi^4)$ in the potential. The [Lagrangian](../../calculus-of-variations.md#lagrangian) is

$$
\boxed{\mathcal L=\frac12(m+M)\dot x^2+ML\dot x\dot\phi+\frac12ML^2\dot\phi^2
-\frac12kx^2-\frac12MgL\phi^2}.
$$

Its [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) give

$$
\boxed{(m+M)\ddot x+ML\ddot\phi+kx=0,\qquad
ML\ddot x+ML^2\ddot\phi+MgL\phi=0}.
$$

The kinetic cross term is essential: acceleration of the support couples the pendulum and cart. These equations define the [normal modes of a spring-mounted pendulum cart](../../lagrangian-mechanics.md#normal-modes-of-a-spring-mounted-pendulum-cart).

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

With the stated parameters, the [mass](../../classical-mechanics.md#mass) and restoring [matrices](../../vector-space.md#matrix) are

$$
A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad
B=\begin{pmatrix}2&0\\0&1\end{pmatrix}.
$$

The [generalized eigenvalue problem](../../linear-operator-theory.md#generalized-eigenvalue-problem) gives

$$
\det(B-\omega^2A)=(2-2\omega^2)(1-\omega^2)-\omega^4
=\omega^4-4\omega^2+2=0.
$$

Therefore the two normal [angular frequencies](../../lagrangian-mechanics.md#angular-frequency) are

$$
\boxed{\omega_{\mathrm{low}}=\sqrt{2-\sqrt2},\qquad
\omega_{\mathrm{high}}=\sqrt{2+\sqrt2}}.
$$

The second row of the modal equation is $-\omega^2x+(1-\omega^2)\phi=0$. It gives the [mode shapes](../../wave-equation.md#mode-shape)

$$
\boxed{\begin{aligned}
\omega_{\mathrm{low}}:&\quad (x,\phi)=a(1,\sqrt2)\cos(\omega_{\mathrm{low}}t+\delta),\\
\omega_{\mathrm{high}}:&\quad (x,\phi)=a(1,-\sqrt2)\cos(\omega_{\mathrm{high}}t+\delta).
\end{aligned}}
$$

Each [normal mode](../../wave-equation.md#normal-mode) has arbitrary small amplitude $a$ and phase $\delta$. The bob's horizontal displacement is $X=x+\phi$ to first order. Thus in the lower mode, bob and cart move in phase, with bob amplitude $1+\sqrt2$ times the cart amplitude. In the higher mode they move oppositely, because $X=(1-\sqrt2)x$; the bob amplitude is $\sqrt2-1$ times the cart amplitude. Its vertical displacement is quadratic in the angle and is absent at this order.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

Let $n=\operatorname{ord}(a)$, which is finite. A [group homomorphism](../../group-theory.md#group-homomorphism) preserves powers and the identity, so

$$
f(a)^n=f(a^n)=f(e)=e'.
$$

If $r=\operatorname{ord}(f(a))$, divide $n$ by $r$: $n=qr+s$ with $0\leq s<r$. Then $e'=f(a)^n=f(a)^s$, and minimality of $r$ forces $s=0$. Thus

$$
\boxed{\operatorname{ord}(f(a))\mid\operatorname{ord}(a),\qquad
\operatorname{ord}(f(a))\leq\operatorname{ord}(a)}.
$$

If $f$ is a [group isomorphism](../../algebra.md#group-isomorphism), apply the same argument to its inverse: $\operatorname{ord}(a)\leq\operatorname{ord}(f(a))$. The two inequalities yield

$$
\boxed{\operatorname{ord}(f(a))=\operatorname{ord}(a)}.
$$

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

The two products are conjugate:

$$
a^{-1}(ab)a=ba.
$$

[Conjugation](../../group-action.md#conjugation) by $a^{-1}$ is a [group automorphism](../../algebra.md#group-automorphism), so part (a) proves

$$
\boxed{\operatorname{ord}(ab)=\operatorname{ord}(ba)}.
$$

Directly, cancellation gives $(ba)^r=a^{-1}(ab)^ra$ for every positive integer $r$. Thus a power of one product is the identity exactly when the same power of the other is the identity. This proves that [conjugation preserves element order](../../group-theory.md#conjugation-preserves-element-order), even without the finiteness assumption.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

The hypothesis implies $g^2=e$ for every $g\in G$, including the identity, so $g^{-1}=g$. For arbitrary $a,b\in G$, their product also equals its own inverse. The inverse-of-a-product rule therefore gives

$$
ab=(ab)^{-1}=b^{-1}a^{-1}=ba.
$$

Thus **$G$ is an [abelian group](../../group.md#abelian-group)**. Finiteness is not needed for this implication; it holds for every [group](../../group.md) in which each element squares to the identity.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Assume (I). Existence of a decomposition is part of the hypothesis. If $h_1h_2=k_1k_2$ are two decompositions, multiply on the left by $k_1^{-1}$ and on the right by $h_2^{-1}$ to obtain

$$
k_1^{-1}h_1=k_2h_2^{-1}.
$$

The left side belongs to $H_1$ and the right side to $H_2$, since they are [subgroups](../../group.md#subgroup). Their common value belongs to $H_1\cap H_2=\{e\}$, so $h_1=k_1$ and $h_2=k_2$. This proves uniqueness, hence (II).

Conversely, assume (II). Existence immediately gives $G=H_1H_2$. If $a\in H_1\cap H_2$, then

$$
a=a\cdot e=e\cdot a
$$

are two allowed factorizations, because the identity is in each [subgroup](../../group.md#subgroup). Uniqueness makes their first components equal, so $a=e$. Thus $H_1\cap H_2=\{e\}$ and (I) follows.

Therefore **(I) and (II) are equivalent**. This is an [exact factorization of a group](../../group.md#exact-factorization-of-a-group). For finite [groups](../../group.md) it gives $|G|=|H_1||H_2|$, but it does not by itself identify $G$ with a [direct product of groups](../../group-theory.md#direct-product-of-groups); multiplication between the two factors can be noncommutative.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

The two diagonal generators are independent involutions, so

$$
H_1=\{\operatorname{diag}(\epsilon_1,\epsilon_2):\epsilon_1,\epsilon_2\in\{1,-1\}\},\qquad |H_1|=4.
$$

It is a [Klein four-group](../../finite-group-theory.md#klein-four-group). Write the swapping generator as $J=\begin{pmatrix}0&1\\1&0\end{pmatrix}$. Then $J^2=I$, so $H_2=\{I,J\}$ has order two. Moreover,

$$
J\operatorname{diag}(\epsilon_1,\epsilon_2)J
=\operatorname{diag}(\epsilon_2,\epsilon_1)\in H_1.
$$

Thus $J$ normalizes $H_1$. The set

$$
K=\{DJ^\eta:D\in H_1,\ \eta\in\{0,1\}\}
$$

is a [group](../../group.md): its products reduce using

$$
(DJ^\eta)(D'J^\zeta)=D(J^\eta D'J^{-\eta})J^{\eta+\zeta},
$$

and inverses reduce in the same way. It contains both generating [subgroups](../../group.md#subgroup), so minimality gives $G\subseteq K$; conversely every displayed product is in $G$, giving $G=K$.

There are four diagonal [matrices](../../vector-space.md#matrix) $D$ and four off-diagonal [matrices](../../vector-space.md#matrix) $DJ$, all distinct. Consequently

$$
\boxed{|G|=8}.
$$

Also $H_1\cap H_2=\{I\}$, since $J$ is not diagonal, and every element of $G$ has the form $DJ^\eta\in H_1H_2$. This proves condition (I), hence the [exact factorization of a group](../../group.md#exact-factorization-of-a-group). Here $H_1$ is a [normal subgroup](../../group-theory.md#normal-subgroup) and $G=H_1\rtimes H_2$ is a [semidirect product](../../group-theory.md#semidirect-product). Its [matrices](../../vector-space.md#matrix) are the two-dimensional [signed permutation matrices](../../vector-space.md#signed-permutation-matrix), also realizing the [dihedral group](../../finite-group-theory.md#dihedral-group) of the square.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

A [vector subspace](../../vector-space.md#vector-subspace) $W\subseteq\mathbb C^n$ is an [invariant subspace](../../representation-theory.md#invariant-subspace) for the [group representation](../../representation-theory.md#group-representation) $D$ if

$$
\boxed{D(g)W\subseteq W\quad\text{for every }g\in G}.
$$

Because $g^{-1}$ is also in the [group](../../group.md) and $D(g)$ is invertible, the inclusion is equivalently $D(g)W=W$ for every $g$.

For $n>0$, the representation is an [irreducible representation](../../representation-theory.md#irreducible-representation) when its only invariant [vector subspaces](../../vector-space.md#vector-subspace) are

$$
\boxed{W=\{0\}\quad\text{and}\quad W=\mathbb C^n}.
$$

Thus no nonzero proper subspace is preserved by all representing [matrices](../../vector-space.md#matrix).

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Every $D_2(g)$ is invertible because both inversion and the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) preserve invertibility. For $g,h\in G$, the [group homomorphism](../../group-theory.md#group-homomorphism) property of $D_1$ and reversal of multiplication under the adjoint give

$$
\begin{aligned}
D_2(gh)&=[D_1((gh)^{-1})]^\dagger\\
&=[D_1(h^{-1})D_1(g^{-1})]^\dagger\\
&=[D_1(g^{-1})]^\dagger[D_1(h^{-1})]^\dagger
=D_2(g)D_2(h).
\end{aligned}
$$

Also $D_2(e)=I$. Hence **$D_2$ is a [group representation](../../representation-theory.md#group-representation)**. It is the [inverse-adjoint representation](../../representation-theory.md#inverse-adjoint-representation) of $D_1$; the inverse and adjoint each reverse product order, so together they preserve it.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Use the standard [Hermitian inner product](../../linear-algebra.md#hermitian-inner-product) $\langle w,v\rangle=w^\dagger v$. Since $W$ is invariant under every $D_2(g)$, it is in particular invariant under

$$
D_2(g^{-1})=[D_1(g)]^\dagger.
$$

Let $v\in W^\perp$ and $w\in W$. Then

$$
\langle w,D_1(g)v\rangle
=\langle D_1(g)^\dagger w,v\rangle=0,
$$

because $D_1(g)^\dagger w\in W$ and $v$ is orthogonal to $W$. Thus $D_1(g)v$ is orthogonal to every $w\in W$, proving

$$
\boxed{D_1(g)W^\perp\subseteq W^\perp\quad(g\in G)}.
$$

Therefore $W^\perp$ is an [invariant subspace](../../representation-theory.md#invariant-subspace) for $D_1$. If $D_1$ is irreducible, $W^\perp$ is either $\{0\}$ or $\mathbb C^n$. In finite-dimensional [inner product space](../../inner-product.md#inner-product-space), $(W^\perp)^\perp=W$, so these alternatives force $W=\mathbb C^n$ or $W=\{0\}$. Hence

$$
\boxed{D_1\ \text{irreducible}\ \Longrightarrow\ D_2\ \text{irreducible}}.
$$

No unitarity of $D_1$ was assumed; the [inverse-adjoint representation](../../representation-theory.md#inverse-adjoint-representation) is exactly what makes this [orthogonal complement](../../hilbert-space.md#orthogonal-complement) argument work.

## ↑ Ancestors (10)

1. [2018](../2018.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
