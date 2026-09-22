# Paper 2

↑ **Parent:** [2024](../2024.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2024/papernst_ib_2_2024.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2024/papernst_ib_2_2024.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)
  - [d](#8/d)
    - [Solution](#8/d/solution)
  - [e](#8/e)
    - [Solution](#8/e/solution)
  - [f](#8/f)
    - [Solution](#8/f/solution)
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
  - [c](#9/c)
    - [Solution](#9/c/solution)
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

Substitution into the [diffusive flux](../../mathematical-physics.md#diffusive-flux) gives

$$
J(x,t)=-e^{-\lambda t}D(x)\bigl(u'(x)+\beta V'(x)u(x)\bigr).
$$

The [continuity equation](../../mathematical-physics.md#continuity-equation) for this [drift-diffusion equation with a potential](../../diffusion-equation.md#drift-diffusion-equation-with-a-potential) therefore reduces, after cancelling the nonzero exponential, to

$$
\boxed{\bigl[D(u'+\beta V'u)\bigr]'=-\lambda u.}
$$

The reflecting [boundary conditions](../../differential-equation.md#boundary-condition) become $D(u'+\beta V'u)=0$ at both endpoints. Thus each solution of this [eigenvalue problem](../../linear-operator-theory.md#eigenvalue-problem) supplies a separated solution of the original [diffusion equation](../../diffusion-equation.md).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [product rule](../../calculus.md#product-rule) makes the drift term cancel:

$$
u'+\beta V'u=e^{-\beta V}y'.
$$

Consequently the transformed [eigenvalue problem](../../linear-operator-theory.md#eigenvalue-problem) is

$$
-\bigl(De^{-\beta V}y'\bigr)'=\lambda e^{-\beta V}y,
\qquad
\boxed{p=De^{-\beta V},\quad q=0,\quad w=e^{-\beta V}.}
$$

Both $p$ and the weight $w$ are positive, as required for this [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For sufficiently smooth functions satisfying the same [boundary conditions](../../differential-equation.md#boundary-condition), [integration by parts](../../calculus.md#integration-by-parts) gives the boundary form

$$
\begin{aligned}
\langle f,\mathcal Lg\rangle-\langle\mathcal Lf,g\rangle
&=\int_{-L}^L\left[-f^*(pg')'+(pf^{*\prime})'g\right]dx\\
&=\left[p\bigl(f^{*\prime}g-f^*g'\bigr)\right]_{-L}^{L}.
\end{aligned}
$$

The stated endpoint relation annihilates this expression. This proves the required [self-adjoint differential operator](../../sturm-liouville-theory.md#self-adjoint-differential-operator) identity; for the usual regular [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem), separated real [boundary conditions](../../differential-equation.md#boundary-condition) give a self-adjoint realization on its domain.

In this problem the transformed [diffusive flux](../../mathematical-physics.md#diffusive-flux) is $J=-e^{-\lambda t}py'$. Thus the physical [boundary conditions](../../differential-equation.md#boundary-condition) are

$$
\boxed{py'(\pm L)=0,}
$$

equivalently $y'(\pm L)=0$ when the endpoint values of $p$ are positive. In particular $pf'=pg'=0$ at the endpoints, which makes the boundary form vanish directly. The [inner product](../../inner-product.md) used here is the ordinary integral; the weight $w$ enters the [generalized eigenvalue problem](../../linear-operator-theory.md#generalized-eigenvalue-problem), not this boundary-form calculation.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Apply the identity from (c) to the two real [eigenfunctions](../../linear-operator-theory.md#eigenfunction). The equations of their [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) give

$$
0=\int_{-L}^L\left(f_n\mathcal Lf_m-f_m\mathcal Lf_n\right)dx
=(\lambda_m-\lambda_n)\int_{-L}^Lwf_nf_m\,dx.
$$

Since the [eigenvalues](../../linear-operator-theory.md#eigenvalue) differ,

$$
\boxed{\int_{-L}^Lw(x)f_n(x)f_m(x)\,dx=0.}
$$

This is [orthogonality](../../inner-product.md#orthogonal-vectors) in the [weighted inner product](../../inner-product.md#weighted-inner-product).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For an admissible nonzero real trial function, [integration by parts](../../calculus.md#integration-by-parts) and the zero-[flux](../../mathematical-physics.md#flux) [boundary conditions](../../differential-equation.md#boundary-condition) reduce the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) to

$$
\frac{\int_{-L}^Ly\mathcal Ly\,dx}{\int_{-L}^Lwy^2\,dx}
=\frac{\int_{-L}^Lp(y')^2\,dx}{\int_{-L}^Lwy^2\,dx}\geq0.
$$

A nonzero constant trial function attains zero. Positivity of $p$ also shows that equality requires $y'=0$. Hence

$$
\boxed{\lambda_0=0,\qquad f_0(x)=C,\qquad c_{\rm eq}(x)=C e^{-\beta V(x)}.}
$$

If the conserved total amount is $M=\int_{-L}^Lc\,dx$, the normalized [stationary solution](../../differential-equation.md#stationary-solution) is

$$
\boxed{c_{\rm eq}(x)=\frac{M e^{-\beta V(x)}}{\int_{-L}^Le^{-\beta V(s)}\,ds}.}
$$

Its [diffusive flux](../../mathematical-physics.md#diffusive-flux) vanishes everywhere. The [Boltzmann distribution](../../thermodynamics.md#boltzmann-distribution) fixes the spatial profile, while the [diffusivity](../../brownian-motion.md#diffusion-coefficient) affects the relaxation toward it. Boundedness of $V$ makes the normalization finite on this finite interval.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the [harmonic extension in a circular sector](../../partial-differential-equation.md#harmonic-extension-in-a-circular-sector), write a separated [harmonic function](../../partial-differential-equation.md#harmonic-function) as $F(r)H(\theta)$. The [Laplace equation in polar coordinates](../../partial-differential-equation.md#laplace-equation-in-polar-coordinates) yields

$$
\frac{r(rF')'}{F}=-\frac{H''}{H}=\nu^2.
$$

The angular [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) select the [Fourier sine basis](../../fourier-series.md#fourier-sine-basis)

$$
H_n(\theta)=\sin\frac{n\theta}{2\alpha},\qquad \nu_n=\frac{n}{2\alpha},\quad n=1,2,\ldots.
$$

Indeed, the angular equation has no nonzero solution with nonpositive $\nu^2$: multiplying $-H''=\nu^2H$ by $H$ and integrating gives $\int(H')^2=\nu^2\int H^2$. The radial [Cauchy-Euler equation](../../linear-ordinary-differential-equation.md#cauchy-euler-equation) has solutions $r^{\nu_n}$ and $r^{-\nu_n}$. Boundedness at the vertex excludes the latter, so [superposition](../../vector-space.md#superposition-principle) gives

$$
\boxed{\Phi(r,\theta)=\sum_{n=1}^\infty A_n r^{n/(2\alpha)}\sin\frac{n\theta}{2\alpha}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Fourier orthogonality](../../fourier-series.md#fourier-orthogonality) relation on this angular interval is

$$
\int_0^{2\pi\alpha}\sin\frac{n\theta}{2\alpha}\sin\frac{m\theta}{2\alpha}\,d\theta
=\pi\alpha\,\delta_{nm}.
$$

Projecting the outer [boundary condition](../../differential-equation.md#boundary-condition) onto each angular [eigenfunction](../../linear-operator-theory.md#eigenfunction) gives

$$
\boxed{A_n=\frac{R^{-n/(2\alpha)}}{\pi\alpha}\int_0^{2\pi\alpha}\varphi(\theta)\sin\frac{n\theta}{2\alpha}\,d\theta.}
$$

The solution is **unique** in the class of bounded [harmonic functions](../../partial-differential-equation.md#harmonic-function) with the prescribed boundary trace. For continuous boundary data, the difference of two solutions is zero on the boundary and bounded at the vertex, so the [maximum principle for harmonic functions](../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) makes it zero throughout the sector. Equivalently all its [Fourier sine series](../../fourier-series.md#fourier-sine-series) coefficients vanish. The usual convergence interpretation applies if the data are only piecewise smooth.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Reflecting the solution across $\theta=\pi\alpha$ preserves its [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) and outer boundary data, so uniqueness makes the solution reflection-symmetric. Since

$$
\sin\frac{n(2\pi\alpha-\theta)}{2\alpha}=(-1)^{n+1}\sin\frac{n\theta}{2\alpha},
$$

only odd angular [Fourier modes](../../fourier-analysis.md#fourier-mode) survive. Put $\rho=(r/R)^{1/(2\alpha)}$ and $\psi=\theta/(2\alpha)$. On the symmetry axis $\psi=\pi/2$, comparison of the convergent [power series](../../sequence-and-series.md#power-series) gives

$$
A_{2j+1}R^{(2j+1)/(2\alpha)}(-1)^j=\frac1{(2j+1)!}.
$$

Thus

$$
\boxed{\Phi(r,\theta)=\sum_{j=0}^{\infty}\frac{(-1)^j\rho^{2j+1}}{(2j+1)!}\sin\bigl((2j+1)\psi\bigr).}
$$

This is the [imaginary part](../../complex-analysis.md#imaginary-part) of $\sin(\rho e^{i\psi})$, so a useful closed form is

$$
\boxed{\Phi(r,\theta)=\cos\bigl(\rho\cos\psi\bigr)\sinh\bigl(\rho\sin\psi\bigr).}
$$

At either straight edge $\sin\psi=0$, while on the symmetry axis the formula is $\sinh\rho$. Every term is [harmonic](../../partial-differential-equation.md#harmonic-function) in the sector, and the factorial denominator gives convergence up to $r=R$, verifying the full solution.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [fundamental solution of the Laplace equation](../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation) satisfies $\Delta_{\mathbf r}G_0=\delta(\mathbf r-\mathbf r')$ in the sense of [distributions](../../distribution-theory.md#distribution-mathematical-analysis), without a boundary condition. Choose it rotationally symmetric about the source. Away from the source, with $s=|\mathbf r-\mathbf r'|$, the radial [Laplace equation](../../partial-differential-equation.md#laplace-equation) is $(sG_0')'=0$, giving $G_0=A\log s+B$.

Integrating over a small disc around the source and using the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) fixes the normalization:

$$
1=\int_{s<\varepsilon}\Delta G_0\,dS
=\int_{s=\varepsilon}\frac{\partial G_0}{\partial s}\,dC
=\frac A\varepsilon\,2\pi\varepsilon=2\pi A.
$$

Therefore

$$
\boxed{G_0(\mathbf r;\mathbf r')=\frac1{2\pi}\log|\mathbf r-\mathbf r'|+B.}
$$

The additive constant is arbitrary; adding other entire [harmonic functions](../../partial-differential-equation.md#harmonic-function) is also possible if rotational symmetry is not imposed. The positive sign here follows from the convention $\Delta G_0=+\delta$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function) is the solution, with the source point held fixed, of

$$
\boxed{\Delta_{\mathbf r}G(\mathbf r;\mathbf r')=\delta(\mathbf r-\mathbf r')\text{ in }S,\qquad G(\mathbf r;\mathbf r')=0\text{ on }C.}
$$

Its singularity is the logarithmic one found in (a); subtracting that [fundamental solution](../../distribution-theory.md#fundamental-solution-of-a-linear-differential-operator) leaves a [harmonic function](../../partial-differential-equation.md#harmonic-function). An unbounded region also requires a condition at infinity, here boundedness.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[Green's second identity](../../partial-differential-equation.md#green-second-identity), with the outward [normal derivative](../../differential-geometry.md#normal-derivative), is

$$
\int_S(u\Delta v-v\Delta u)\,dS
=\oint_C\left(u\frac{\partial v}{\partial n}-v\frac{\partial u}{\partial n}\right)dC.
$$

Set $u=\Phi$ and $v=G(\cdot;\mathbf r')$, interpreting the logarithmic singularity by a small excised disc or [distribution theory](../../distribution-theory.md). The volume integral is $\Phi(\mathbf r')$ because $\Delta\Phi=0$ and $\Delta G=\delta$. On the boundary $G=0$ and $\Phi=f$, leaving

$$
\boxed{\Phi(\mathbf r')=\oint_C f(\mathbf r)\frac{\partial G(\mathbf r;\mathbf r')}{\partial n}\,dC.}
$$

For the exterior problem below, apply the identity first in a large truncated region. For bounded [harmonic functions](../../partial-differential-equation.md#harmonic-function) the extra circle at infinity contributes zero: $G$ tends to a constant, its radial derivative is $O(r^{-2})$, and a bounded exterior [harmonic function](../../partial-differential-equation.md#harmonic-function) also has radial derivative $O(r^{-2})$. This is the condition under which the same boundary representation applies there.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $s=|\mathbf r'|>0$ and $\mathbf p=\mathbf r'/s^2$. For $|\mathbf r|=1$, expanding both squared [Euclidean distances](../../topological-analysis.md#euclidean-distance) gives

$$
\begin{aligned}
s^2|\mathbf r-\mathbf p|^2
&=s^2-2\mathbf r\cdot\mathbf r'+1\\
&=|\mathbf r-\mathbf r'|^2.
\end{aligned}
$$

Taking nonnegative square roots proves

$$
\boxed{|\mathbf r-\mathbf r'|=|\mathbf r'|\,|\mathbf r-\mathbf p|.}
$$

This is the distance identity behind [inversion in a circle](../../group-theory.md#inversion-in-a-circle) and the [method of images](../../mathematics.md#method-of-images) for a circular boundary.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For a source in the exterior, its inverse point $\mathbf p$ lies strictly inside the excluded disc. The [method of images](../../mathematics.md#method-of-images) construction of the [bounded exterior disk Green function](../../green-s-function.md#bounded-exterior-disk-green-function) therefore allows an opposite logarithmic source there without adding a singularity to the domain. The candidate [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function) is

$$
\boxed{G(\mathbf r;\mathbf r')=\frac1{2\pi}\left(\log|\mathbf r-\mathbf r'|-\log|\mathbf r-\mathbf p|-\log|\mathbf r'|\right).}
$$

Its [Laplacian](../../multivariable-calculus.md#laplacian) in the exterior is exactly $\delta(\mathbf r-\mathbf r')$, since the image singularity is outside that domain. The identity in (d) makes $G=0$ on the unit circle. Moreover

$$
\lim_{|\mathbf r|\to\infty}G(\mathbf r;\mathbf r')=-\frac1{2\pi}\log|\mathbf r'|,
$$

so it obeys the required boundedness condition. These checks establish the stated logarithm-of-a-ratio expression with $A=1/(2\pi)$. Bounded exterior [Dirichlet uniqueness for the Poisson equation](../../analysis.md#dirichlet-uniqueness-for-the-poisson-equation) follows by [inversion in a circle](../../group-theory.md#inversion-in-a-circle) and removal of the bounded singularity at the origin.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

The outward normal of the exterior region points **into the excluded disc**, so it is $-\mathbf r$ on the unit circle. Differentiating the [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function) from (e), and writing $s=|\mathbf r'|$ and $d=|\mathbf r-\mathbf r'|$, gives

$$
\begin{aligned}
\frac{\partial G}{\partial n}
&=\frac1{2\pi}\left[-\frac{1-\mathbf r\cdot\mathbf r'}{d^2}+\frac{1-\mathbf r\cdot\mathbf p}{|\mathbf r-\mathbf p|^2}\right]\\
&=\frac{s^2-1}{2\pi|\mathbf r-\mathbf r'|^2}.
\end{aligned}
$$

Here $|\mathbf r-\mathbf p|^2=d^2/s^2$ was used. The concentrated boundary data have unit integral, so the boundary representation evaluates this exterior [Poisson kernel](../../partial-differential-equation.md#poisson-kernel) at $\mathbf r=(-1,0)$. Thus the bounded solution on either part of the exterior $x$-axis is

$$
\boxed{\Phi(x',0)=\frac{x'^2-1}{2\pi(x'+1)^2}=\frac{x'-1}{2\pi(x'+1)},\qquad |x'|>1.}
$$

It is positive on both intervals, diverges as $x'\to-1^-$ at the boundary source, and tends to $1/(2\pi)$ as $|x'|\to\infty$. Boundedness at infinity selects this solution; otherwise one could add an arbitrary multiple of $\log|\mathbf r'|$ without changing the circle's boundary data.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $f=u+iv$ and $z=x+iy$. For a positively oriented, piecewise smooth simple closed [contour](../../complex-analysis.md#complex-integration-contour) bounding a region where $u,v$ have continuous first [partial derivatives](../../multivariable-calculus.md#partial-derivative), [Green's theorem](../../multivariable-calculus.md#green-theorem) gives

$$
\begin{aligned}
\oint_C f(z)\,dz
&=\oint_C(u\,dx-v\,dy)+i\oint_C(v\,dx+u\,dy)\\
&=\iint_S(-v_x-u_y)\,dx\,dy+i\iint_S(u_x-v_y)\,dx\,dy.
\end{aligned}
$$

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) are $u_x=v_y$ and $u_y=-v_x$, so both integrands vanish:

$$
\boxed{\oint_C f(z)\,dz=0.}
$$

This proves [Cauchy's integral theorem](../../complex-analysis.md#cauchy-s-integral-theorem) under the standard regularity assumptions for [Green's theorem](../../multivariable-calculus.md#green-theorem). More general admissible [contours](../../complex-analysis.md#complex-integration-contour) follow by subdivision; every enclosed region must be free of singularities.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [simple pole](../../isolated-singularity.md#simple-pole) at $z_0$ means that $f$ is [holomorphic](../../holomorphic-function.md) in a punctured neighbourhood and $(z-z_0)f(z)$ extends holomorphically to a nonzero value at $z_0$. Equivalently its [Laurent series](../../analysis.md#laurent-series) begins with $a_{-1}/(z-z_0)$ and has no higher negative powers. The [residue](../../analysis.md#residue) is

$$
\boxed{\operatorname{Res}(f,z_0)=\lim_{z\to z_0}(z-z_0)f(z).}
$$

In particular, if $f=g/h$ with $g(z_0)\ne0$, $h(z_0)=0$ and $h'(z_0)\ne0$, this becomes $\operatorname{Res}(f,z_0)=g(z_0)/h'(z_0)$. The associated [residue theorem](../../analysis.md#residue-theorem) is

$$
\boxed{\oint_C f(z)\,dz=2\pi i\sum_{z_j\text{ inside }C}\operatorname{Res}(f,z_j)}
$$

for a positively oriented simple [contour](../../complex-analysis.md#complex-integration-contour) with no poles on it.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The exponential numerator is entire and never zero. The denominator vanishes precisely when $e^{2z}=-1$, giving

$$
z_n=i\pi\left(n+\tfrac12\right),\qquad n\in\mathbb Z.
$$

At these points $\sinh z_n=i(-1)^n\ne0$, so every zero of the denominator is simple and hence every singularity is a [simple pole](../../isolated-singularity.md#simple-pole). Using the [residue](../../analysis.md#residue) formula in (b),

$$
\boxed{\operatorname{Res}(f,z_n)=\frac{e^{-ikz_n}}{\sinh z_n}=\frac{(-1)^n}{i}\exp\left[k\pi\left(n+\tfrac12\right)\right].}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use the counterclockwise rectangular [contour](../../complex-analysis.md#complex-integration-contour) with vertices $-R,R,R+i\pi,-R+i\pi$. It encloses just the [simple pole](../../isolated-singularity.md#simple-pole) $i\pi/2$, whose [residue](../../analysis.md#residue) is $e^{k\pi/2}/i$. Let $I_R=\int_{-R}^R e^{-ikx}/\cosh x\,dx$. The identity

$$
f(x+i\pi)=-e^{k\pi}f(x)
$$

makes the top edge, traversed right to left, contribute $e^{k\pi}I_R$. On either vertical edge,

$$
|\cosh(\pm R+iy)|^2=\sinh^2R+\cos^2y,\qquad |e^{-ik(\pm R+iy)}|=e^{ky}\leq e^{|k|\pi}.
$$

Thus the sum of the vertical integrals tends to zero, with absolute value at most $2\pi e^{|k|\pi}/\sinh R$. The [residue theorem](../../analysis.md#residue-theorem) and $R\to\infty$ now give

$$
(1+e^{k\pi})I=2\pi e^{k\pi/2},\qquad
\boxed{I=\pi\operatorname{sech}\frac{k\pi}{2}.}
$$

The argument works for every fixed real $k$, including zero and negative values, and gives the [Fourier transform of the hyperbolic secant](../../fourier-transform.md#fourier-transform-of-the-hyperbolic-secant) with the convention $\widetilde f(k)=\int e^{-ikx}f(x)\,dx$.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use the [Fourier transform](../../fourier-transform.md) convention

$$
\widetilde f(\omega)=\int_{-\infty}^{\infty}e^{-i\omega t}f(t)\,dt,\qquad
f(t)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{i\omega t}\widetilde f(\omega)\,d\omega.
$$

The [convolution](../../fourier-analysis.md#convolution) is $(f*g)(t)=\int_{-\infty}^{\infty}f(\tau)g(t-\tau)\,d\tau$. For integrable $f,g$, [Fubini's theorem](../../measure-theory.md#fubini-s-theorem) and the substitution $s=t-\tau$ give

$$
\begin{aligned}
\widetilde{f*g}(\omega)
&=\int_{\mathbb R}\int_{\mathbb R}e^{-i\omega t}f(\tau)g(t-\tau)\,d\tau\,dt\\
&=\left(\int_{\mathbb R}e^{-i\omega\tau}f(\tau)\,d\tau\right)\left(\int_{\mathbb R}e^{-i\omega s}g(s)\,ds\right).
\end{aligned}
$$

Hence the [convolution theorem](../../fourier-analysis.md#convolution-theorem) is

$$
\boxed{\widetilde{f*g}(\omega)=\widetilde f(\omega)\widetilde g(\omega).}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Take the causal solution, extending the input and output by zero before the device starts at $t=0$. The two zero [initial conditions](../../differential-equation.md#initial-condition) ensure that this extension adds no impulsive terms to the first two [distributional derivatives](../../distribution-theory.md#distributional-derivative). The [Fourier transform of a derivative](../../fourier-analysis.md#fourier-transform-of-a-derivative) is multiplication by $i\omega$, so

$$
\left[(p+i\omega)^2+q^2\right]\widetilde\phi(\omega)=\widetilde I(\omega).
$$

Factoring the quadratic and taking [partial fraction decomposition](../../isolated-singularity.md#partial-fraction-decomposition) yields

$$
\boxed{\widetilde\phi=\widetilde R\widetilde I,\qquad
\widetilde R(\omega)=\frac1{2iq}\left(\frac1{p+i\omega-iq}-\frac1{p+i\omega+iq}\right).}
$$

The inverse [Fourier transform](../../fourier-transform.md) follows directly by integrating decaying exponentials:

$$
\boxed{R(t)=H(t)\frac{e^{-pt}\sin(qt)}q,}
$$

where $H$ is the [Heaviside step function](../../integral-transform.md#heaviside-step-function). This [damped-oscillator impulse response](../../analysis.md#causal-green-function-of-a-damped-oscillator) has $R(0^+)=0$ and $R'(0^+)=1$, as required for a unit impulse.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [convolution theorem](../../fourier-analysis.md#convolution-theorem) gives the causal response

$$
\phi(t)=\frac{I_0}q\int_0^{\min(t,1)}e^{-p(t-\tau)}\sin\bigl(q(t-\tau)\bigr)\,d\tau\quad(t>0).
$$

Define the integrated [impulse response](../../green-s-function.md#impulse-response), for $s\geq0$, by

$$
F(s)=\frac{1-e^{-ps}\cos(qs)-(p/q)e^{-ps}\sin(qs)}{p^2+q^2}.
$$

Direct differentiation gives $F'(s)=e^{-ps}\sin(qs)/q$ and $F(0)=F'(0)=0$. Thus

$$
\boxed{\phi(t)=\begin{cases}
0,&t\leq0,\\
I_0F(t),&0<t\leq1,\\
I_0\bigl[F(t)-F(t-1)\bigr],&t>1.
\end{cases}}
$$

In particular, after switch-off the answer is

$$
\boxed{\phi(t)=\frac{I_0}{p^2+q^2}\left\{
e^{-p(t-1)}\left[\cos q(t-1)+\frac pq\sin q(t-1)\right]
-e^{-pt}\left[\cos qt+\frac pq\sin qt\right]\right\},\quad t>1.}
$$

The response and its first [derivative](../../calculus.md#derivative) are continuous at both switching times, and the post-pulse motion is a freely decaying [damped harmonic oscillator](../../analysis.md#damped-harmonic-oscillator). The expression described as valid for $t<1$ in the paper is understood for $0<t<1$; before the pulse the causal output is zero.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Use the same [Fourier transform](../../fourier-transform.md) convention, now in the sense of [tempered distributions](../../fourier-analysis.md#tempered-distribution), since the homogeneous oscillations are not integrable. Transforming gives

$$
\bigl[q^2-(\omega+r)^2\bigr]\widetilde\phi(\omega)=0.
$$

Since $q>0$, the two roots are distinct. A [distribution](../../distribution-theory.md#distribution-mathematical-analysis) annihilated by this polynomial is a linear combination of [Dirac delta distributions](../../distribution-theory.md#dirac-delta-function) at its roots:

$$
\widetilde\phi(\omega)=2\pi A\delta(\omega+r-q)+2\pi B\delta(\omega+r+q).
$$

[Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) therefore gives

$$
\boxed{\phi(t)=A e^{i(q-r)t}+B e^{-i(q+r)t}
=e^{-irt}\bigl(C\cos qt+D\sin qt\bigr).}
$$

The constants may be complex. Differentiating the factor $e^{-irt}$ also verifies that the original [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) reduces to $\ddot\psi+q^2\psi=0$ for $\phi=e^{-irt}\psi$.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For a Cartesian coordinate change $x'_i=R_{ij}x_j$ with $R$ an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix), a rank-$n$ [tensor](../../multilinear-algebra.md#tensor) obeys

$$
\boxed{T'_{i_1\cdots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\cdots j_n},}
$$

with repeated indices summed according to [Einstein notation](../../multilinear-algebra.md#einstein-notation). A [tensor](../../multilinear-algebra.md#tensor) is **isotropic** if $T'_{i_1\cdots i_n}=T_{i_1\cdots i_n}$ for every proper [rotation matrix](../../linear-algebra.md#rotation-matrix) $R$. Under proper rotations the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) is an [isotropic third-rank tensor](../../multilinear-algebra.md#isotropic-third-rank-tensor); if reflections are included, it is a [pseudotensor](../../multilinear-algebra.md#pseudotensor). The convention using proper rotations is the one relevant to the rank-three classification here.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Under a proper [rotation matrix](../../linear-algebra.md#rotation-matrix) $R$, the product of coordinates transforms as a rank-$n$ [tensor](../../multilinear-algebra.md#tensor). The unit ball is unchanged by the substitution $\mathbf y=R\mathbf x$, whose [Jacobian determinant](../../multivariable-calculus.md#jacobian-determinant) is one. Hence

$$
\begin{aligned}
R_{i_1j_1}\cdots R_{i_nj_n}S_{j_1\cdots j_n}
&=\int_B(R\mathbf x)_{i_1}\cdots(R\mathbf x)_{i_n}\,dV_{\mathbf x}\\
&=\int_B y_{i_1}\cdots y_{i_n}\,dV_{\mathbf y}=S_{i_1\cdots i_n}.
\end{aligned}
$$

Thus $S$ is an [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor). An [isotropic second-rank tensor](../../multilinear-algebra.md#isotropic-second-rank-tensor) has the form $S_{ij}=A\delta_{ij}$. Taking the [trace](../../linear-algebra.md#matrix-trace) and using [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system),

$$
3A=\int_B|\mathbf x|^2\,dV=4\pi\int_0^1r^4\,dr=\frac{4\pi}5.
$$

Therefore the [isotropic second moment of a ball](../../multilinear-algebra.md#isotropic-second-moment-of-a-ball) is

$$
\boxed{S_{ij}=\frac{4\pi}{15}\delta_{ij}.}
$$

An [isotropic third-rank tensor](../../multilinear-algebra.md#isotropic-third-rank-tensor) has the form $B\epsilon_{ijk}$, but $S_{ijk}$ is symmetric in every pair of indices, forcing $B=0$. Alternatively, $\mathbf x\mapsto-\mathbf x$ makes its integrand odd on the ball. Thus

$$
\boxed{S_{ijk}=0.}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Choose an [orthonormal basis](../../inner-product.md#orthonormal-basis) with $\mathbf n=\mathbf e_3$. A half-turn about $\mathbf n$ kills all mixed axial-transverse components. Commutation with a quarter-turn makes the transverse block a scalar [identity matrix](../../vector-space.md#identity-matrix) plus an [antisymmetric matrix](../../linear-algebra.md#skew-symmetric-matrix). The resulting [oriented-axis invariant Cartesian tensor](../../multilinear-algebra.md#oriented-axis-invariant-cartesian-tensor), in coordinate-free form, is

$$
\boxed{\sigma_{ij}=a(\delta_{ij}-n_in_j)+d\,n_in_j+h\epsilon_{ikj}n_k,}
$$

with real constants $a,d,h$. The [Kronecker delta](../../multilinear-algebra.md#kronecker-delta), the [outer product](../../vector-space.md#outer-product) $n_in_j$, and the displayed [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) contraction are invariant under every proper rotation about $\mathbf n$, so this form is also sufficient. In the chosen basis,

$$
\sigma=\begin{pmatrix}a&-h&0\\h&a&0\\0&0&d\end{pmatrix}.
$$

The antisymmetric part must be retained unless further symmetry is imposed.

Decompose the [electric field](../../electric-field.md) as $\mathbf E=\mathbf E_\perp+\mathbf E_\parallel$, where $\mathbf E_\parallel=(\mathbf n\cdot\mathbf E)\mathbf n$. The [electric current density](../../electric-charge.md#current-density) is

$$
\mathbf J=a\mathbf E_\perp+d\mathbf E_\parallel+h\mathbf n\times\mathbf E_\perp.
$$

For a nonzero real [electric field](../../electric-field.md), the [alignment of current and field in an axisymmetric conductor](../../multilinear-algebra.md#alignment-of-current-and-field-in-an-axisymmetric-conductor) gives the complete classification of [collinearity](../../euclidean-geometry.md#collinearity):

- If $\mathbf E_\perp=0$, then $\boxed{\mathbf J=d\mathbf E}$, with no additional symmetry required.
- If $\mathbf E_\parallel=0$, then $\boxed{\mathbf J\parallel\mathbf E\ \Longleftrightarrow\ h=0}$. Within this family $h=0$ is exactly the condition that the [conductivity tensor](../../electric-charge.md#conductivity-tensor) is symmetric; then $\mathbf J=a\mathbf E$. An additional half-turn symmetry about a transverse axis is one way to force $h=0$.
- If both components are nonzero, then $\boxed{\mathbf J\parallel\mathbf E\ \Longleftrightarrow\ h=0\text{ and }a=d}$. These conditions give the [isotropic second-rank tensor](../../multilinear-algebra.md#isotropic-second-rank-tensor) $\sigma=aI$, and then $\mathbf J=a\mathbf E$ for every direction.

For completeness, if $\mathbf E_\perp\ne0$ and $\mathbf J=\lambda\mathbf E$, taking the [dot product](../../inner-product.md#dot-product) with $\mathbf n\times\mathbf E_\perp$ forces $h=0$. The transverse equation then gives $\lambda=a$, while a nonzero axial component gives $\lambda=d$. This proves there are no missing directions. Zero current is included as the zero scalar multiple; if “parallel” requires a direction for $\mathbf J$, exclude cases where that scalar is zero. For a strictly anisotropic crystal the last possibility is absent.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

An axial [electric field](../../electric-field.md) produces $\mathbf J=d\mathbf E$, so the observation sets $d=0$ and imposes no restriction on the transverse or antisymmetric parts. Thus

$$
\boxed{\sigma_{ij}=a(\delta_{ij}-n_in_j)+h\epsilon_{ikj}n_k.}
$$

A symmetric [conductivity tensor](../../electric-charge.md#conductivity-tensor) would further require $h=0$, but axial rotational invariance alone does not require this.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Use the bead [angles](../../geometry-and-topology.md#angle) $\theta_1,\theta_2,\theta_3$ as [generalized coordinates](../../lagrangian-mechanics.md#generalized-coordinate). The straight-line spring length between two beads follows from the [law of cosines](../../euclidean-geometry.md#law-of-cosines):

$$
\ell_{ij}=\sqrt{2-2\cos(\theta_i-\theta_j)}.
$$

The hoop is horizontal, so the [gravitational potential energy](../../energy.md#gravitational-energy) is constant and can be omitted. The [kinetic energy](../../energy.md#kinetic-energy) is $(m/2)\sum_i\dot\theta_i^2$, giving the [Lagrangian](../../calculus-of-variations.md#lagrangian)

$$
\boxed{L=\frac m2\sum_{i=1}^3\dot\theta_i^2-\frac k2\sum_{i<j}\left[\sqrt{2-2\cos(\theta_i-\theta_j)}-\sqrt3\right]^2.}
$$

At $\theta_i^0=\Theta+2\pi(i-1)/3$, every spring has its natural length, so the [potential energy](../../energy.md#potential-energy) is zero and its first [derivatives](../../calculus.md#derivative) vanish. This is an [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) for every constant $\Theta$. It is stable against relative displacement because each spring energy is nonnegative; the overall rotation is a neutral direction.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Put $\theta_i=\theta_i^0+\eta_i$. Differentiating the spring length gives

$$
\delta\ell_{ij}=\frac{\sin(\theta_i^0-\theta_j^0)}{\sqrt3}(\eta_i-\eta_j),\qquad
(\delta\ell_{ij})^2=\frac14(\eta_i-\eta_j)^2.
$$

The springs are unextended at [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), so the quadratic [potential energy](../../energy.md#potential-energy) contains only the squares of these first-order extensions:

$$
U_2=\frac k8\left[(\eta_1-\eta_2)^2+(\eta_2-\eta_3)^2+(\eta_3-\eta_1)^2\right].
$$

The linearized [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) are therefore

$$
m\ddot{\boldsymbol\eta}+\frac k4
\begin{pmatrix}2&-1&-1\\-1&2&-1\\-1&-1&2\end{pmatrix}\boldsymbol\eta=0.
$$

The [stiffness matrix](../../finite-element-method.md#stiffness-matrix) is $(k/4)(3I-\mathbf 1\mathbf 1^T)$. Its [eigenvector](../../linear-operator-theory.md#eigenvector) $\mathbf 1=(1,1,1)^T$ has zero [eigenvalue](../../linear-operator-theory.md#eigenvalue), and every vector whose components sum to zero has [eigenvalue](../../linear-operator-theory.md#eigenvalue) $3k/4$. One convenient orthonormal set of [normal modes](../../wave-equation.md#normal-mode) is

$$
\boxed{\begin{aligned}
\mathbf v_0&=\frac1{\sqrt3}(1,1,1)^T,&\omega_0&=0,\\
\mathbf v_1&=\frac1{\sqrt2}(1,-1,0)^T,&\omega_1&=\sqrt{\frac{3k}{4m}},\\
\mathbf v_2&=\frac1{\sqrt6}(1,1,-2)^T,&\omega_2&=\sqrt{\frac{3k}{4m}}.
\end{aligned}}
$$

Any orthonormal basis of the sum-zero plane is equally valid for the two degenerate [normal modes](../../wave-equation.md#normal-mode). The general small motion is

$$
\boldsymbol\eta(t)=(A_0+B_0t)\mathbf v_0+\sum_{j=1}^2\left[A_j\cos(\omega_1t)+B_j\sin(\omega_1t)\right]\mathbf v_j.
$$

The linear drift in the [zero mode](../../linear-operator-theory.md#zero-mode) describes a slow uniform rotation. These are [angular frequencies](../../lagrangian-mechanics.md#angular-frequency); the ordinary [frequencies](../../wave.md#frequency) of the two vibrational modes are $\omega_1/(2\pi)$.

<a id="7/b/image-tangential-displacement-patterns-of-the-three-bead-normal-modes"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2-q7-normal-modes.png)

**[Figure 1](#7/b/image-tangential-displacement-patterns-of-the-three-bead-normal-modes). Tangential displacement patterns of the three bead normal modes**. Arrows show the signs and relative sizes of the angular displacements in one choice of orthonormal [normal modes](../../wave-equation.md#normal-mode). The equal-arrow pattern is a rigid rotation, while the two sum-zero patterns have equal nonzero [angular frequency](../../lagrangian-mechanics.md#angular-frequency).

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

A common shift of all three [angles](../../geometry-and-topology.md#angle) leaves every spring length unchanged. This continuous rotational [symmetry](../../physics.md#symmetry-physics) gives the [zero mode](../../linear-operator-theory.md#zero-mode): there is no restoring force against rigid rotation.

The equilateral [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) also has the [dihedral group](../../finite-group-theory.md#dihedral-group) symmetry $D_3$. Its action on the three angular displacements preserves the uniform one-dimensional subspace and the two-dimensional sum-zero subspace. The latter is an [irreducible representation](../../representation-theory.md#irreducible-representation) over the [real numbers](../../arithmetic.md#real-number); a reflection may reverse all angular signs as well as exchange bead labels, which does not change these invariant subspaces. The symmetric [stiffness matrix](../../finite-element-method.md#stiffness-matrix) must act as a scalar on the sum-zero subspace, explaining the equal vibrational [angular frequencies](../../lagrangian-mechanics.md#angular-frequency). Directly, each sum-zero vector satisfies $(3I-\mathbf1\mathbf1^T)\mathbf v=3\mathbf v$. This is an example of [degenerate normal modes from permutation symmetry](../../lagrangian-mechanics.md#degenerate-normal-modes-from-permutation-symmetry), and of [normal modes of three equal masses with a symmetric gap potential](../../lagrangian-mechanics.md#normal-modes-of-three-equal-masses-with-a-symmetric-gap-potential).

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

The [group order](../../group.md#order-of-a-finite-group) is its [cardinality](../../cardinal-number.md#cardinality), $\boxed{|G|=\#\{g:g\in G\}}$. The [order of a group element](../../group-theory.md#order-of-a-group-element) $g$ is

$$
\boxed{\operatorname{ord}(g)=\min\{n\geq1:g^n=e\},}
$$

where $e$ is the [identity element](../../algebraic-operation.md#identity-element). In a [finite group](../../group.md#finite-group) such an $n$ always exists, since two nonnegative powers of $g$ must coincide.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

[Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) states that for a [subgroup](../../group.md#subgroup) $H$ of a [finite group](../../group.md#finite-group) $G$,

$$
\boxed{|G|=[G:H]\,|H|,\qquad |H|\mid |G|.}
$$

The left [cosets](../../group-theory.md#coset) of $H$ partition $G$, and multiplication by a coset representative is a [bijection](../../function.md#bijection) from $H$ onto that coset, explaining the formula. If $|G|=p$ is [prime](../../prime-number.md), then $|H|$ is either $1$ or $p$, so $H=\{e\}$ or $H=G$. Thus the correct conclusion is **no proper nontrivial subgroup**. The [trivial subgroup](../../group.md#trivial-subgroup) $\{e\}$ is proper for every group of prime order, so the wording in the question needs this qualification.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Let $d=\operatorname{ord}(g)$. The powers

$$
\langle g\rangle=\{e,g,\ldots,g^{d-1}\}
$$

are distinct: equality of two with exponents between $0$ and $d-1$ would give a smaller positive power equal to $e$. Reducing exponents modulo $d$ proves closure and supplies inverses, so this is a [cyclic subgroup](../../group.md#cyclic-subgroup) of [group order](../../group.md#order-of-a-finite-group) $d$. [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) now gives

$$
\boxed{\operatorname{ord}(g)=|\langle g\rangle|\mid |G|.}
$$

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

Choose $g\ne e$ in a group of prime [group order](../../group.md#order-of-a-finite-group) $p$. Its [order of a group element](../../group-theory.md#order-of-a-group-element) divides $p$ by (c) and is not $1$, hence equals $p$. Consequently its [cyclic subgroup](../../group.md#cyclic-subgroup) already contains all elements of $G$:

$$
\boxed{G=\langle g\rangle\cong C_p.}
$$

Thus every nonidentity element is a [group generator](../../group.md#generator-of-a-group).

<h3 id="8/e">e</h3>

↑ **Parent:** [8](#8)

<h4 id="8/e/solution">Solution</h4>

↑ **Parent:** [E](#8/e)

By (d), every group of [group order](../../group.md#order-of-a-finite-group) three is a [cyclic group](../../group.md#cyclic-group). Writing its elements as $e,a,a^2$, every product is determined by $a^3=e$; the [multiplication table](../../arithmetic.md#multiplication-table) is

$$
\begin{array}{c|ccc}
\cdot&e&a&a^2\\\hline
e&e&a&a^2\\
a&a&a^2&e\\
a^2&a^2&e&a
\end{array}
$$

The map $a^j\mapsto j\pmod3$ is a bijective [group homomorphism](../../group-theory.md#group-homomorphism) to addition modulo three. Therefore

$$
\boxed{G\cong\mathbb Z_3,}
$$

so there is exactly one such [group](../../group.md) **up to isomorphism**.

<h3 id="8/f">f</h3>

↑ **Parent:** [8](#8)

<h4 id="8/f/solution">Solution</h4>

↑ **Parent:** [F](#8/f)

Closure of the componentwise operation follows from closure in each factor. For three pairs, [associativity](../../algebraic-operation.md#associative-property) holds coordinatewise:

$$
\bigl((g_1,g_2)(h_1,h_2)\bigr)(k_1,k_2)
=\bigl((g_1h_1)k_1,(g_2h_2)k_2\bigr)
=\bigl(g_1(h_1k_1),g_2(h_2k_2)\bigr).
$$

The [identity element](../../algebraic-operation.md#identity-element) is $(e_1,e_2)$ and the [inverse element](../../algebraic-operation.md#inverse-element) of $(g_1,g_2)$ is $(g_1^{-1},g_2^{-1})$. These verify all [group axioms](../../group.md#group-axioms) for the [direct product of groups](../../group-theory.md#direct-product-of-groups). Counting independent choices gives

$$
\boxed{|G_1\times G_2|=|G_1|\,|G_2|.}
$$

The subset $N=G_1\times\{e_2\}$ contains the identity and is closed under products and inverses, so it is a [subgroup](../../group.md#subgroup). For any $x=(a,b)$ in the product and $(g,e_2)\in N$,

$$
x(g,e_2)x^{-1}=(aga^{-1},be_2b^{-1})=(aga^{-1},e_2)\in N.
$$

Conjugation by $x^{-1}$ gives the reverse inclusion, and hence

$$
\boxed{xNx^{-1}=N,\qquad N\mathrel{\trianglelefteq}G_1\times G_2.}
$$

This is the definition of a [normal subgroup](../../group-theory.md#normal-subgroup).

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Both [subgroups](../../group.md#subgroup) contain the [identity element](../../algebraic-operation.md#identity-element), so $H\cap K$ is nonempty. If $x,y\in H\cap K$, then $xy\in H$ and $xy\in K$, so $xy\in H\cap K$. Similarly $x^{-1}$ belongs to both subgroups and hence to their intersection. [Associativity](../../algebraic-operation.md#associative-property) is inherited from $G$. Thus

$$
\boxed{H\cap K\leq G.}
$$

This verifies the [group axioms](../../group.md#group-axioms); finiteness is unnecessary.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

In additive notation every element $(a,b)\in\mathbb Z_2\times\mathbb Z_4$ obeys $4(a,b)=(0,0)$. Its [order of a group element](../../group-theory.md#order-of-a-group-element) therefore divides four, whereas $1\in\mathbb Z_8$ has order eight. A [group isomorphism](../../algebra.md#group-isomorphism) preserves element orders, so

$$
\boxed{\mathbb Z_2\times\mathbb Z_4\not\cong\mathbb Z_8.}
$$

For the second product, define the [group homomorphism](../../group-theory.md#group-homomorphism)

$$
\Psi:\mathbb Z_6\longrightarrow\mathbb Z_2\times\mathbb Z_3,\qquad
[t]_6\longmapsto([t]_2,[t]_3).
$$

It is well-defined because multiples of six are divisible by both two and three. Its [kernel](../../kernel-of-a-linear-map.md) contains only zero: simultaneous divisibility by two and three implies divisibility by six. Thus $\Psi$ is injective, and equal finite [group orders](../../group.md#order-of-a-finite-group) make it surjective. Explicitly the six images are

$$
(0,0),(1,1),(0,2),(1,0),(0,1),(1,2).
$$

Therefore

$$
\boxed{\mathbb Z_2\times\mathbb Z_3\cong\mathbb Z_6.}
$$

For general positive integers $n,m$, the [order of a direct-product element](../../group-theory.md#order-of-a-direct-product-element) is the [least common multiple](../../divisibility.md#least-common-multiple) of its component orders. Hence every element order divides $\operatorname{lcm}(n,m)=nm/\gcd(n,m)$, while $(1,1)$ attains this order. It generates the whole product precisely when $n,m$ are [coprime](../../divisibility.md#coprime-integers):

$$
\boxed{\mathbb Z_n\times\mathbb Z_m\cong\mathbb Z_{nm}\quad\Longleftrightarrow\quad\gcd(n,m)=1.}
$$

This is the [cyclicity of a product of two finite cyclic groups](../../group-theory.md#cyclicity-of-a-product-of-two-finite-cyclic-groups), with the explicit isomorphism furnished by the [Chinese remainder theorem](../../mathematics.md#chinese-remainder-theorem).

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

The [center of a group](../../group-theory.md#center-of-a-group) contains $e$. If $z,w$ lie in the center, then for every $g\in G$,

$$
g(zw)g^{-1}=(gzg^{-1})(gwg^{-1})=zw,
\qquad
gz^{-1}g^{-1}=(gzg^{-1})^{-1}=z^{-1}.
$$

It is therefore closed under the [group operation](../../group.md#group-operation) and [inverse elements](../../algebraic-operation.md#inverse-element), and inherits [associativity](../../algebraic-operation.md#associative-property), proving it is a [subgroup](../../group.md#subgroup). Each of its elements commutes with every element of $G$, in particular with every other central element. Hence

$$
\boxed{Z(G)\leq G\text{ and }zw=wz\text{ for all }z,w\in Z(G).}
$$

Thus the center is an [abelian subgroup](../../group.md#abelian-subgroup).

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

A [group homomorphism](../../group-theory.md#group-homomorphism) preserves multiplication:

$$
\boxed{\Phi(g_1g_2)=\Phi(g_1)\Phi(g_2)\quad\text{for every }g_1,g_2\in G.}
$$

It automatically sends the [identity element](../../algebraic-operation.md#identity-element) to the identity and sends [inverse elements](../../algebraic-operation.md#inverse-element) to inverses. A [group isomorphism](../../algebra.md#group-isomorphism) is a **bijective group homomorphism**. For finite groups this requires equal [group orders](../../group.md#order-of-a-finite-group), and, once those orders agree, either injectivity or surjectivity of the [group homomorphism](../../group-theory.md#group-homomorphism) is sufficient. Equal orders alone do not suffice.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Here $a^2=-I$, $a^3=-a$ and $a^4=I$, so $K$ is a [cyclic group of order four](../../group.md#cyclic-group-of-order-four). Its [multiplication table](../../arithmetic.md#multiplication-table) is

$$
\boxed{\begin{array}{c|rrrr}
\cdot&I&-I&a&-a\\\hline
I&I&-I&a&-a\\
-I&-I&I&-a&a\\
a&a&-a&-I&I\\
-a&-a&a&I&-I
\end{array}}
$$

Write the specified image of $a$ as $A$. Direct matrix multiplication gives

$$
A^2=-I_2,\qquad A^3=-A,\qquad A^4=I_2.
$$

A [group representation](../../representation-theory.md#group-representation) is a [group homomorphism](../../group-theory.md#group-homomorphism) to a [general linear group](../../group-theory.md#general-linear-group), so the images of all powers of $a$ are forced:

$$
\boxed{\begin{aligned}
\Phi(I)&=\begin{pmatrix}1&0\\0&1\end{pmatrix},\\
\Phi(-I)&=\begin{pmatrix}-1&0\\0&-1\end{pmatrix},\\
\Phi(-a)&=\begin{pmatrix}0&-i\\-i&0\end{pmatrix}.
\end{aligned}}
$$

All four images are invertible. Defining $\Phi(a^j)=A^j$ is well-defined modulo four because $A^4=I_2$, and $A^{j+\ell}=A^jA^\ell$ verifies every product in the table. These observations prove both existence and uniqueness of this [representation](../../representation-theory.md#group-representation) with the prescribed image.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Distinguish the [quaternion group](../../finite-group-theory.md#quaternion-group) generators $\mathbf i,\mathbf j,\mathbf k$ from the complex scalar $i$. Denote their proposed image matrices by

$$
A=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad
B=\begin{pmatrix}0&i\\i&0\end{pmatrix},\qquad
C=\begin{pmatrix}i&0\\0&-i\end{pmatrix}.
$$

Direct multiplication gives

$$
A^2=B^2=C^2=-I_2,\qquad
AB=C,\quad BC=A,\quad CA=B,\qquad
BA=-C,\quad CB=-A,\quad AC=-B.
$$

For example $AB=\operatorname{diag}(i,-i)=C$ and $ABC=C^2=-I_2$. Sending $I$ to $I_2$ and each negative quaternion element to the negative of its positive image now reproduces every quaternion product. The matrices all have [determinant](../../multilinear-algebra.md#determinant) one and are invertible, so this is a [group representation](../../representation-theory.md#group-representation) in $GL(2,\mathbb C)$.

The eight matrices $\pm I_2,\pm A,\pm B,\pm C$ are distinct. Therefore the [group homomorphism](../../group-theory.md#group-homomorphism) is injective, and the representation is **faithful**; equivalently its [kernel](../../kernel-of-a-linear-map.md) is $\{I\}$.

The [character of a representation](../../representation-theory.md#character-of-a-representation) is the [trace](../../linear-algebra.md#matrix-trace) of its representing matrix. Consequently

$$
\boxed{\chi(I)=2,\qquad\chi(-I)=-2,\qquad
\chi(\pm\mathbf i)=\chi(\pm\mathbf j)=\chi(\pm\mathbf k)=0.}
$$

These are constant on the five [conjugacy classes](../../group-action.md#conjugacy-class) $\{I\}$, $\{-I\}$, $\{\pm\mathbf i\}$, $\{\pm\mathbf j\}$, $\{\pm\mathbf k\}$.

The complete list of [subgroups](../../group.md#subgroup) is

$$
\boxed{\begin{array}{c|c}
\text{subgroup}&\text{order}\\\hline
\{I\}&1\\
\{I,-I\}&2\\
\langle\mathbf i\rangle=\{I,-I,\mathbf i,-\mathbf i\}&4\\
\langle\mathbf j\rangle=\{I,-I,\mathbf j,-\mathbf j\}&4\\
\langle\mathbf k\rangle=\{I,-I,\mathbf k,-\mathbf k\}&4\\
Q&8
\end{array}}
$$

To see completeness, [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) allows only orders $1,2,4,8$. The only element of order two is $-I$, which fixes the order-two subgroup. Every noncentral element has order four and generates the corresponding listed [cyclic subgroup](../../group.md#cyclic-subgroup). Any order-four subgroup contains such an element, because there are only two central elements; it must equal the [cyclic subgroup](../../group.md#cyclic-subgroup) generated by that element. This accounts for all possibilities.

## ↑ Ancestors (10)

1. [2024](../2024.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
