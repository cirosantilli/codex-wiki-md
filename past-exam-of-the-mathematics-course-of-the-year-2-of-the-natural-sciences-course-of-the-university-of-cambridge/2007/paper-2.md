# Paper 2

↑ **Parent:** [2007](../2007.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2007/PaperNST_IB_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2007/PaperNST_IB_2.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [Grounded hemisphere](#2/grounded-hemisphere)
    - [Solution](#2/grounded-hemisphere/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $\Phi(r,\theta)=R(r)Y(\theta)$ in [Laplace's equation](../../partial-differential-equation.md#laplace-equation), multiply by $r^2/(RY)$, and separate the two variables:

$$
\frac{(r^2R')'}R=-\frac{(\sin\theta\,Y')'}{Y\sin\theta}=\lambda.
$$

With $s=\cos\theta$, the angular equation becomes $(1-s^2)Y_{ss}-2sY_s+\lambda Y=0$. Requiring a smooth [axisymmetric harmonic function](../../partial-differential-equation.md#axisymmetric-harmonic-function) at both poles selects $\lambda=n(n+1)$ and the [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) $Y=P_n(s)$, for nonnegative [integers](../../integer.md) $n$. The radial [Cauchy-Euler equation](../../linear-ordinary-differential-equation.md#cauchy-euler-equation) has solutions $r^n$ and $r^{-n-1}$. [Superposition](../../vector-space.md#superposition-principle) over the angular [eigenfunctions](../../linear-operator-theory.md#eigenfunction) therefore gives

$$
\Phi(r,\theta)=\sum_{n=0}^{\infty}(A_nr^n+B_nr^{-n-1})P_n(\cos\theta),\qquad (1-s^2)P_n''-2sP_n'+n(n+1)P_n=0.
$$

This expansion assumes regularity on each whole angular [sphere](../../euclidean-geometry.md#sphere); without it, singular angular solutions would also be possible. The boundary data in the shell involve only the $n=0,1$ modes. Define the [spherical-shell harmonic interpolation](../../partial-differential-equation.md#axisymmetric-harmonic-interpolation-between-concentric-spheres) weights

$$
p_0=\frac{a(b-r)}{r(b-a)},\quad q_0=\frac{b(r-a)}{r(b-a)},\qquad p_1=\frac{a^2(b^3-r^3)}{r^2(b^3-a^3)},\quad q_1=\frac{b^2(r^3-a^3)}{r^2(b^3-a^3)}.
$$

Each $p_n$ equals one at the inner boundary and zero at the outer one, and $q_n$ does the reverse. Hence the steady [temperature](../../temperature.md) is

$$
\boxed{T(r,\theta)=T_0p_0(r)+T_2q_0(r)+[T_1p_1(r)+T_3q_1(r)]\cos\theta.}
$$

Each term is a [harmonic function](../../partial-differential-equation.md#harmonic-function), and substitution verifies both prescribed boundary values. Uniqueness follows from the [maximum principle for harmonic functions](../../partial-differential-equation.md#maximum-principle-for-harmonic-functions).

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For $s=|\mathbf x-\mathbf x_0|>0$, the radial [Laplacian](../../multivariable-calculus.md#laplacian) gives $\nabla^2(1/s)=s^{-2}\partial_s(s^2\partial_s(1/s))=0$. The outward [flux](../../mathematical-physics.md#flux) of $\nabla[-1/(4\pi s)]$ through a small [sphere](../../euclidean-geometry.md#sphere) centred at the source is $[1/(4\pi s^2)]4\pi s^2=1$. Applying [Green's second identity](../../partial-differential-equation.md#green-second-identity) to a smooth [test function](../../distribution-theory.md#test-function) outside that small sphere and shrinking its radius therefore gives the distributional identity

$$
\boxed{\nabla^2\left(-\frac1{4\pi|\mathbf x-\mathbf x_0|}\right)=\delta(\mathbf x-\mathbf x_0).}
$$

The kernel tends to zero at infinity. Thus it is the [fundamental solution](../../distribution-theory.md#fundamental-solution-of-a-linear-differential-operator) with the sign convention $\Delta G=+\delta$. The sign will reverse when converting it into the [electrostatic potential](../../electric-field.md#electric-potential) of a positive [point charge](../../electric-field.md#point-charge) through [Poisson's equation](../../partial-differential-equation.md#poisson-s-equation).

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $\mathbf x_0^-=(x_0,y_0,-z_0)$ be the reflection of the source across the plane. The [method of images](../../mathematics.md#method-of-images) gives the [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function)

$$
\boxed{G_H(\mathbf x;\mathbf x_0)=-\frac1{4\pi}\left(\frac1{|\mathbf x-\mathbf x_0|}-\frac1{|\mathbf x-\mathbf x_0^-|}\right).}
$$

The two source distances agree on $z=0$, so the boundary value vanishes. The reflected source lies outside the upper half-space, leaving only the required [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function) inside. Both terms vanish at infinity.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Put $r_0=|\mathbf x_0|$ and $\mathbf x_0^*=a^2\mathbf x_0/r_0^2$ for $0<r_0<a$. The [Dirichlet Green function inside a sphere](../../green-s-function.md#dirichlet-green-function-inside-a-sphere) is

$$
\boxed{G_B(\mathbf x;\mathbf x_0)=-\frac1{4\pi}\left(\frac1{|\mathbf x-\mathbf x_0|}-\frac{a/r_0}{|\mathbf x-\mathbf x_0^*|}\right).}
$$

On $|\mathbf x|=a$, the distance identity $|\mathbf x-\mathbf x_0^*|=(a/r_0)|\mathbf x-\mathbf x_0|$ cancels the two terms. The inverse point lies outside the [sphere](../../euclidean-geometry.md#sphere), so it introduces no interior source. This weighted inversion is the [Kelvin transform](../../partial-differential-equation.md#kelvin-transform). For a central source, take the limit to get $G_B(\mathbf x;0)=-(4\pi)^{-1}(1/|\mathbf x|-1/a)$.

<h3 id="2/grounded-hemisphere">Grounded hemisphere</h3>

↑ **Parent:** [2](#2)

<h4 id="2/grounded-hemisphere/solution">Solution</h4>

↑ **Parent:** [Grounded hemisphere](#2/grounded-hemisphere)

Reflect the source across the equatorial plane and subtract the two ball kernels. This gives the [Dirichlet Green function inside a hemisphere](../../green-s-function.md#dirichlet-green-function-inside-a-hemisphere) $G_{\rm hemi}(\mathbf x;\mathbf x_0)=G_B(\mathbf x;\mathbf x_0)-G_B(\mathbf x;\mathbf x_0^-)$. It is zero on the spherical boundary because each ball kernel is zero there, and on the plane because reflection makes their values equal.

For a [point charge](../../electric-field.md#point-charge) $e$, [Poisson's equation](../../partial-differential-equation.md#poisson-s-equation) in SI units is $\Delta V=-e\delta(\mathbf x-\mathbf x_0)/\varepsilon_0$, so $V=-eG_{\rm hemi}/\varepsilon_0$. Writing $\mathbf x_0^{*-}$ for the reflected inverse point gives

$$
\boxed{V(\mathbf x)=\frac{e}{4\pi\varepsilon_0}\left[\frac1{|\mathbf x-\mathbf x_0|}-\frac1{|\mathbf x-\mathbf x_0^-|}-\frac{a/r_0}{|\mathbf x-\mathbf x_0^*|}+\frac{a/r_0}{|\mathbf x-\mathbf x_0^{*-}|}\right].}
$$

The construction uses the real charge, its negative reflected image, a negative inversion image of magnitude $ea/r_0$, and its positive reflected image. Reflection and inversion commute. All three images lie outside the open upper half-ball, and the prescribed zero boundary values determine the [electrostatic potential](../../electric-field.md#electric-potential) uniquely.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

At a point of complex [differentiability](../../analysis.md#differentiability), the [complex derivative](../../holomorphic-function.md#complex-derivative) is independent of the direction of approach. Taking increments along the real axis gives $f'=u_x+iv_x$; taking imaginary increments gives $f'=v_y-iu_y$. Equality of their [real parts](../../complex-analysis.md#real-part) and [imaginary parts](../../complex-analysis.md#imaginary-part) proves the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) $u_x=v_y$ and $u_y=-v_x$.

For the specified [real part](../../complex-analysis.md#real-part), observe that $z^2e^z$ has exactly that real part. Equivalently, integrating $v_y=u_x$ and checking $v_x=-u_y$ gives

$$
v=e^x[(x^2-y^2)\sin y+2xy\cos y]+C.
$$

Thus

$$
\boxed{f(z)=z^2e^z+iC,\qquad C\in\mathbb R.}
$$

The freedom is only a constant imaginary part: the difference of two such [holomorphic functions](../../holomorphic-function.md) has zero real part, so its [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) make it constant on each connected domain.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The square-root factor gives an algebraic [branch point](../../complex-analysis.md#branch-point) at $z=0$. The logarithm is locally analytic there but has value an odd multiple of $i\pi$, which is nonzero, so it cannot cancel that branching. The zero and pole of $(z-1)/(z+1)$ give logarithmic [branch points](../../complex-analysis.md#branch-point) at $z=1$ and $z=-1$, respectively. Thus the finite singularities are

$$
\boxed{z=0,\quad1,\quad-1\quad\text{(all branch points; no finite poles).}}
$$

Infinity is also a [branch point](../../complex-analysis.md#branch-point). On the logarithm branch tending to zero there, $\log[(z-1)/(z+1)]=-2/z+O(z^{-3})$, so the product behaves as $-2z^{-1/2}$. Other logarithm branches add $2\pi ik\sqrt z$ and retain branching. A chosen [branch cut](../../analysis.md#branch-cut) joins or separates these branch points; its ordinary interior points are not additional branch points of the underlying multivalued [function](../../function.md).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The denominator factors as $(z+2-i)(z+2+i)$. Neither root cancels against the numerator, and both are simple, so the finite singularities are

$$
\boxed{z=-2+i,\quad z=-2-i\quad\text{(simple poles).}}
$$

This is a [rational function](../../isolated-singularity.md#rational-function), so it has no [branch points](../../complex-analysis.md#branch-point). At infinity, putting $w=1/z$ gives $w/(1+4w+5w^2)$, analytic at zero; infinity is therefore a [removable singularity](../../isolated-singularity.md#removable-singularity) with value zero.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [residue theorem](../../analysis.md#residue-theorem) states that the [contour integral](../../complex-analysis.md#contour-integral) of a [meromorphic function](../../isolated-singularity.md#meromorphic-function) around a positively oriented simple closed contour equals $2\pi i$ times the sum of its enclosed [residues](../../analysis.md#residue), provided there are no singularities on the contour. The roots of $1+z^n$ are $z_k=e^{(2k+1)i\pi/n}$, $k=0,\ldots,n-1$. They are simple [poles](../../isolated-singularity.md#pole), with [residues](../../analysis.md#residue) $1/(nz_k^{n-1})=-z_k/n$.

Use the sector contour of angle $2\pi/n$, running outward along the positive axis and inward along the rotated ray. It encloses only $z_0=e^{i\pi/n}$. The large-arc contribution is $O(R^{1-n})$, hence vanishes. With $J=\int_0^\infty dx/(1+x^n)$, the two ray contributions give

$$
(1-e^{2\pi i/n})J=-\frac{2\pi i}{n}e^{i\pi/n}.
$$

Since $1-e^{2i\alpha}=-2ie^{i\alpha}\sin\alpha$,

$$
\boxed{J=\frac\pi{n\sin(\pi/n)}.}
$$

For the second integral, use $z^{n/2}/(1+z^n)$ on a branch continuous across the sector away from zero, with a small inner arc of radius $\epsilon$. Its large arc is $O(R^{1-n/2})$ and its small arc is $O(\epsilon^{1+n/2})$, both vanishing for $n\geq3$. On the rotated ray, $z^{n/2}$ changes by $e^{i\pi}=-1$, so the two radial contributions add rather than subtract. The enclosed [residue](../../analysis.md#residue) is $z_0^{1-n/2}/n=-ie^{i\pi/n}/n$. Consequently

$$
(1+e^{2\pi i/n})I=\frac{2\pi}{n}e^{i\pi/n},\qquad\boxed{I=\frac\pi{n\cos(\pi/n)}}.
$$

Both answers are instances of the [Mellin integral of a reciprocal binomial](../../integral-transform.md#mellin-integral-of-a-reciprocal-binomial). The direct contour argument also tracks the branch needed when $n$ is odd.

<a id="4/image-a-sector-encloses-exactly-one-root-of-the-denominator"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2-sector-contour.png)

**[Figure 1](#4/image-a-sector-encloses-exactly-one-root-of-the-denominator). A sector encloses exactly one root of the denominator**. An original illustrative contour for $n=5$, with outward and inward rays, an outer arc, and the inner indentation needed for a fractional power. Only the root at angle $\pi/n$ is enclosed.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The unilateral [Laplace transform](../../integral-transform.md#laplace-transform) is $\bar f(p)=\int_0^\infty e^{-pt}f(t)dt$ in its [region of absolute convergence of a Laplace transform](../../integral-transform.md#region-of-absolute-convergence-of-a-laplace-transform). Under the usual inversion hypotheses, the [Bromwich inversion formula](../../integral-transform.md#bromwich-inversion-formula) is

$$
f(t)=\frac1{2\pi i}\lim_{R\to\infty}\int_{c-iR}^{c+iR}e^{pt}\bar f(p)dp.
$$

The vertical [Bromwich contour](../../complex-analysis.md#bromwich-contour) is directed upward, with $c$ inside the transform's convergence half-plane and to the right of all its singularities. At discontinuities the standard symmetric inversion gives the mean of the one-sided values.

For a piecewise continuously [differentiable](../../analysis.md#differentiable-function) $f$ with an integrable transformed [derivative](../../calculus.md#derivative), [integration by parts](../../calculus.md#integration-by-parts) gives the [Laplace transform of a derivative](../../integral-transform.md#laplace-transform-of-a-derivative):

$$
\int_0^\infty e^{-pt}f'(t)dt=\left[e^{-pt}f(t)\right]_0^\infty+p\int_0^\infty e^{-pt}f(t)dt=\boxed{p\bar f(p)-f(0)}.
$$

Here the upper endpoint vanishes by the given decay condition, and right continuity at zero supplies the lower endpoint.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Set $a_n=1-1/(2n)$, $b_n=1+1/(2n)$. The finite pulse has [Laplace transform](../../integral-transform.md#laplace-transform) $\bar S_n(p)=n(e^{-pa_n}-e^{-pb_n})/p$. Since $f(0)=0$, transforming the equation gives

$$
\bar f(p)=\frac{n(e^{-pa_n}-e^{-pb_n})}{p(p-1)}.
$$

The [partial fraction decomposition](../../isolated-singularity.md#partial-fraction-decomposition) $1/[p(p-1)]=1/(p-1)-1/p$ has inverse $e^t-1$. By the [Laplace transform time-shift rule](../../integral-transform.md#laplace-transform-time-shift-rule),

$$
f(t)=n[(e^{t-a_n}-1)H(t-a_n)-(e^{t-b_n}-1)H(t-b_n)].
$$

This [finite-pulse response of a first-order linear equation](../../linear-ordinary-differential-equation.md#finite-pulse-response-of-a-first-order-linear-equation) gives the requested outer regions:

$$
\boxed{f(t)=0\quad(t<a_n),\qquad f(t)=2n\sinh\left(\frac1{2n}\right)e^{t-1}\quad(t>b_n).}
$$

For completeness, while the pulse is active the solution is $n(e^{t-a_n}-1)$. It is continuous at both switching times. After the forcing stops it grows as $e^t$, because the homogeneous equation is $f'=f$. The apparent pole at $p=0$ in the full transform is removable; the [Bromwich contour](../../complex-analysis.md#bromwich-contour) may be taken with $c>1$.

<a id="5/ii/image-a-unit-area-pulse-excites-an-exponentially-growing-response"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2-pulse-response.png)

**[Figure 2](#5/ii/image-a-unit-area-pulse-excites-an-exponentially-growing-response). A unit-area pulse excites an exponentially growing response**. Original calculated responses for two pulse widths and their limiting impulse response. The lower panel shows the prescribed rectangular inputs; their areas are both one.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A two-index [Cartesian tensor](../../multilinear-algebra.md#cartesian-tensor) has components transforming as $T'_{ij}=R_{ik}R_{jl}T_{kl}$ under an orthogonal change of [orthonormal basis](../../inner-product.md#orthonormal-basis). The tensor order here counts indices, rather than the [matrix rank](../../vector-space.md#matrix-rank). Its [scalar, symmetric-traceless and axial tensor decomposition](../../multilinear-algebra.md#scalar-symmetric-traceless-and-axial-tensor-decomposition) follows by setting

$$
Y=\frac{T_{kk}}3,\qquad\Omega_{ij}=\frac{T_{ij}-T_{ji}}2,\qquad S_{ij}=\frac{T_{ij}+T_{ji}}2-Y\delta_{ij}.
$$

Then $T_{ij}=Y\delta_{ij}+\Omega_{ij}+S_{ij}$, with $\Omega$ antisymmetric and $S$ symmetric and traceless. There are **three independent antisymmetric components** and **five independent symmetric traceless components**: three off-diagonal entries and two independent diagonal ones in the latter case.

For the symmetric tensor relative to a nonzero [vector](../../vector-space.md#vector) $A$, put $q=A_iA_i>0$, $s=A_iT_{ij}A_j$, and $t=T_{ii}$. The [symmetric tensor decomposition relative to an axis](../../multilinear-algebra.md#symmetric-tensor-decomposition-relative-to-an-axis) gives

$$
\boxed{\alpha=\frac12\left(t-\frac sq\right),\qquad\beta=\frac{3s/q-t}{2q},\qquad B_i=\frac{T_{ij}A_j}{q}-\frac{sA_i}{q^2}.}
$$

In particular $A_iB_i=s/q-s/q=0$. Define the [orthogonal projection](../../hilbert-space.md#orthogonal-projection) $P_{ij}=\delta_{ij}-A_iA_j/q$ onto the plane perpendicular to $A$, and set

$$
\boxed{C_{ij}=P_{ik}T_{kl}P_{lj}-\alpha P_{ij}.}
$$

This [tensor](../../multilinear-algebra.md#tensor) is symmetric and kills $A$. Its [trace](../../linear-algebra.md#matrix-trace) is $t-s/q-2\alpha=0$. To verify the full decomposition, set $u=A/\sqrt q$ and split $T$ into its longitudinal component $(u^TTu)uu^T$, two mixed components, and $PTP$. The mixed terms are exactly $BA^T+AB^T$, and $\alpha+\beta q=s/q$ gives the longitudinal coefficient. Thus all requested constraints and the reconstruction hold.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

For a conservative system near a stable equilibrium, the quadratic [Lagrangian](../../calculus-of-variations.md#lagrangian) has the form $L=\frac12\dot q^TM\dot q-\frac12q^TKq$, with symmetric [mass matrix](../../finite-element-method.md#mass-matrix) $M$ and [stiffness matrix](../../finite-element-method.md#stiffness-matrix) $K$. A [normal mode](../../wave-equation.md#normal-mode) $q=v e^{i\omega t}$ satisfies the [generalized eigenvalue problem for small oscillations](../../lagrangian-mechanics.md#generalized-eigenvalue-problem-for-small-oscillations) $(K-\omega^2M)v=0$, so the frequency equation is $\det(K-\omega^2M)=0$.

To quadratic order, vertical [velocities](../../classical-mechanics.md#velocity) contribute only fourth-order corrections to the [kinetic energy](../../energy.md#kinetic-energy), leaving $T=(\dot x^2+\dot y^2+\dot z^2)/2$. A string of length $\ell$ with small horizontal difference $d$ shortens its vertical projection by $d^2/(2\ell)$. The upper segment carries all three masses, the middle segment two, and the lower segment one. Hence their increases in [gravitational potential energy](../../energy.md#gravitational-energy) sum to

$$
V=3g\frac{x^2}{2(3a)}+2g\frac{(y-x)^2}{2(2b)}+g\frac{(z-y)^2}{2c}=\frac g2\left[\frac{x^2}{a}+\frac{(x-y)^2}{b}+\frac{(y-z)^2}{c}\right].
$$

Subtracting $V$ from $T$ gives the stated approximate [Lagrangian](../../calculus-of-variations.md#lagrangian). Here $M=I$ and

$$
K=g\begin{pmatrix}a^{-1}+b^{-1}&-b^{-1}&0\\-b^{-1}&b^{-1}+c^{-1}&-c^{-1}\\0&-c^{-1}&c^{-1}\end{pmatrix}.
$$

For a mode with middle displacement zero, write $v=(X,0,Z)^T$. The middle row requires $X/b+Z/c=0$, so $Z=-cX/b$. A nonzero mode then has $X,Z\ne0$, and the outer rows require $\omega^2/g=a^{-1}+b^{-1}=c^{-1}$. Therefore the necessary and sufficient condition is

$$
\boxed{\frac1a+\frac1b-\frac1c=0.}
$$

When it holds, the [mode shape](../../wave-equation.md#mode-shape) is $(1,0,-c/b)$ with $\omega=\sqrt{g/c}$. This is the force-cancellation mechanism of the [stationary middle mass in a three-mass spring chain](../../wave-equation.md#stationary-middle-mass-in-a-three-mass-spring-chain), applied to the equivalent quadratic stiffnesses here.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

[Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) states that the [group order](../../group.md#order-of-a-finite-group) of a finite [group](../../group.md) divides the [group order](../../group.md#order-of-a-finite-group); more precisely $|G|=[G:H]|H|$.

If every element squares to the [identity element](../../algebraic-operation.md#identity-element), every element is its own [inverse element](../../algebraic-operation.md#inverse-element), and $ab=(ab)^{-1}=b^{-1}a^{-1}=ba$. Thus a [group of exponent two is abelian](../../group.md#group-of-exponent-two-is-abelian). For distinct nonidentity $a,b$, the four elements $1,a,b,ab$ are distinct: for example $ab=1$ would imply $a=b$, and $ab=a$ would imply $b=1$. Products remain in this set because $a,b$ commute and square to one. Thus they form a [Klein four-group](../../finite-group-theory.md#klein-four-group) [subgroup](../../group.md#subgroup) of order four.

Now let $|G|=2p$ with odd [prime number](../../prime-number.md) $p$. By [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem), every [element order](../../group-theory.md#order-of-a-group-element) is one of $1,2,p,2p$. If an element has order $2p$, its square has order $p$. If no element had order $p$, all nonidentity elements would therefore have order two. There are at least two distinct such elements, producing a subgroup of order four. This contradicts $4\nmid2p$. Hence **there is an element of order $p$**.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

A [group homomorphism](../../group-theory.md#group-homomorphism) satisfies $\varphi(g_1g_2)=\varphi(g_1)\varphi(g_2)$; a bijective one is a [group isomorphism](../../algebra.md#group-isomorphism). Its [kernel of a group homomorphism](../../group-theory.md#kernel-of-a-group-homomorphism) is $K=\{g:\varphi(g)=1_H\}$. It is a [subgroup](../../group.md#subgroup), and for $k\in K$, $g\in G$,

$$
\varphi(gkg^{-1})=\varphi(g)\varphi(k)\varphi(g)^{-1}=1_H.
$$

Thus $gKg^{-1}\subseteq K$, and applying the same argument to $g^{-1}$ gives equality. Therefore $K$ is a [normal subgroup](../../group-theory.md#normal-subgroup).

Write $B_n=\begin{pmatrix}1&n\\0&1\end{pmatrix}$. Direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives $B_nB_m=B_{n+m}$, $B_0=I$ and $B_n^{-1}=B_{-n}$. Consequently these matrices form the [integer shear group](../../group.md#integer-shear-group), a [subgroup](../../group.md#subgroup) of $GL(2,\mathbb R)$. It is an [infinite cyclic group](../../group.md#infinite-cyclic-group), generated by $B_1$, since $B_1^n=B_n$ and no nonzero integer power is the identity.

The map $n\mapsto B_n$ is a bijective [group homomorphism](../../group-theory.md#group-homomorphism) from the additive [group of integers](../../group.md#additive-group-of-integers), proving the required [group isomorphism](../../algebra.md#group-isomorphism). **There are proper subgroups**: for example $\{B_{2n}:n\in\mathbb Z\}$ omits $B_1$. In fact every subgroup is $\{B_{mn}:n\in\mathbb Z\}$ for an integer $m\geq0$, by the classification of [subgroups of an infinite cyclic group](../../group.md#subgroup-of-an-infinite-cyclic-group); $m=0$ gives the trivial subgroup and $m=1$ the whole group.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

A real two-dimensional [group representation](../../representation-theory.md#group-representation) is a [group homomorphism](../../group-theory.md#group-homomorphism) $D:G\to GL(2,\mathbb R)$, so $D(AB)=D(A)D(B)$ and $D(I)=I$.

Substitute $\tilde x=\alpha x+\beta y$ and $\tilde y=\gamma x+\delta y$ into the quadratic expression. Its coefficients of $x^2$ and $y^2$ are $\alpha^2\hat a+\gamma^2\hat b$ and $\beta^2\hat a+\delta^2\hat b$. The cross term is zero for every matrix in this particular [cyclic group](../../group.md#cyclic-group), because each has one nonzero entry per row. Thus

$$
\boxed{M(A)=\begin{pmatrix}\alpha^2&\gamma^2\\\beta^2&\delta^2\end{pmatrix}.}
$$

Let $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ generate the group. For $A=\pm I$, $M=I$; for $A=\pm J$, $M=S:=\begin{pmatrix}0&1\\1&0\end{pmatrix}$. Since $S^2=I$, each $M$ is its own inverse and $D(J^k)=S^k$. The group law is respected: $S^{k+l}=S^kS^l$, and $S^4=I$ makes it independent of the representative modulo four. This proves that $D=M^{-1}$ is a [group representation](../../representation-theory.md#group-representation).

This [quarter-turn action on diagonal quadratic forms](../../representation-theory.md#quarter-turn-action-on-diagonal-quadratic-forms) has

$$
\boxed{\ker D=\{I,-I\},}
$$

so it is **not faithful**. Quadratic forms cannot distinguish a simultaneous sign reversal of both coordinates. The invariant coefficient directions $(1,1)$ and $(1,-1)$ correspond to the fixed form $x^2+y^2$ and the form $x^2-y^2$ whose sign changes under a quarter-turn.

## ↑ Ancestors (10)

1. [2007](../2007.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
