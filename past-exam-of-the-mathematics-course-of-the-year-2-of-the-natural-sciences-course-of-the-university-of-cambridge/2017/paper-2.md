# Paper 2

↑ **Parent:** [2017](../2017.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2017/papernst_ib_2_0.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2017/papernst_ib_2_0.pdf)

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
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
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

The relevant [weighted inner product](../../inner-product.md#weighted-inner-product) is $\langle u,v\rangle_w=\int_0^1w(x)u(x)v(x)\,dx$. The normalized [eigenfunctions](../../linear-operator-theory.md#eigenfunction) of the [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) have the [orthonormality](../../inner-product.md#orthonormal-set) property

$$
\boxed{\int_0^1w(x)y_n(x)y_m(x)\,dx=\delta_{nm}.}
$$

Here $\delta_{nm}$ is the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta): the integral is one for $n=m$ and zero otherwise. The weight is $w$, rather than $p$ or the unweighted measure.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Projecting the [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) onto $y_m$ using the [weighted inner product](../../inner-product.md#weighted-inner-product) gives

$$
a_m=\langle f,y_m\rangle_w=\int_0^1w(x)f(x)y_m(x)\,dx.
$$

For the partial sum $f_N=\sum_{n=0}^Na_ny_n$, [orthonormality](../../inner-product.md#orthonormal-set) therefore gives

$$
\|f_N\|_w^2=\sum_{n,m=0}^Na_na_m\langle y_n,y_m\rangle_w=\sum_{n=0}^Na_n^2.
$$

For $f$ of finite [weighted norm](../../inner-product.md#weighted-norm), the given completeness means that $f_N\to f$ in that norm. The [triangle inequality](../../topological-analysis.md#triangle-inequality) implies $|\|f_N\|_w-\|f\|_w|\leq\|f_N-f\|_w\to0$. Taking the limit of the finite identity proves [Parseval's identity](../../fourier-analysis.md#parseval-identity):

$$
\boxed{\int_0^1w(x)f(x)^2\,dx=\sum_{n=0}^\infty a_n^2.}
$$

This argument justifies the limiting step without assuming that a double infinite series can be integrated term by term. As usual, the expansion is understood for [square-integrable functions](../../measure-theory.md#square-integrable-function) with respect to the weighted measure; the boundary and smoothness assumptions of the regular [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) provide the usual stronger interpretations when needed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Write $Y=\sum_{n\geq0}b_ny_n$ in the complete [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion). To determine $b_m$, multiply the differential equation by $y_m$ and integrate. The [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator) has the symmetry identity

$$
\int_0^1\big(y_m\mathcal LY-Y\mathcal Ly_m\big)\,dx=\big[p(Yy_m'-y_mY')\big]_0^1=0,
$$

because both functions obey the homogeneous [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition). Consequently

$$
\lambda_m\int_0^1wYy_m\,dx=\alpha\int_0^1wYy_m\,dx+\int_0^1wfy_m\,dx,
$$

so that $(\lambda_m-\alpha)b_m=a_m$. The stipulated exclusion of every [eigenvalue](../../linear-operator-theory.md#eigenvalue) makes all denominators nonzero, and gives

$$
\boxed{Y(x)=\sum_{n=0}^\infty\frac{a_n}{\lambda_n-\alpha}y_n(x).}
$$

This is the [resolvent operator](../../functional-analysis.md#resolvent-of-an-operator) applied to $f$ in the weighted space. The same projection shows [uniqueness](../../mathematical-logic.md#uniqueness): a homogeneous solution would have $(\lambda_m-\alpha)b_m=0$ for every $m$, hence would vanish by completeness. For the regular problem the formula gives the solution in the operator domain when $f$ is square-integrable.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Only two coefficients in the [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) are nonzero: $a_0=2$ and $a_1=2-\alpha$. Since $\alpha\ne2$, the result of part (i) simplifies to

$$
Y=\frac{2}{1-\alpha}y_0+\frac{2-\alpha}{2-\alpha}y_1=\frac{2}{1-\alpha}y_0+y_1.
$$

Using [Parseval's identity](../../fourier-analysis.md#parseval-identity), the prescribed [weighted norm](../../inner-product.md#weighted-norm) becomes

$$
\frac{4}{(1-\alpha)^2}+1=2.
$$

Thus $1-\alpha=\pm2$, so $\alpha=-1$ or $3$. Positivity selects

$$
\boxed{\alpha=3,\qquad Y=-y_0+y_1.}
$$

The standing nonresonance assumption still applies: this answer requires that $3$ is not one of the unspecified higher [eigenvalues](../../linear-operator-theory.md#eigenvalue). Their actual values are not supplied. If a higher [eigenvalue](../../linear-operator-theory.md#eigenvalue) were $3$, the stated exclusion would fail and the data would not have an admissible $\alpha$ under that exclusion.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use [separation of variables](../../partial-differential-equation.md#separation-of-variables) with $\Phi=M(\mu)N(\nu)$. A nonzero product gives

$$
\frac{M''}{M}=-\frac{N''}{N}=\lambda,\qquad M''-\lambda M=0,\qquad N''+\lambda N=0.
$$

The angular factor must be a [periodic function](../../function.md#periodic-function) of [period](../../mathematics.md#period-of-a-function) $2\pi$. If $\lambda<0$, its exponential solutions cannot be periodic unless they vanish. If $\lambda=0$, $N=c+d\nu$ forces $d=0$, while $M=A_0+B_0\mu$. If $\lambda>0$, periodicity requires $\sqrt\lambda=n\in\mathbb N$, giving angular factors $\cos(n\nu),\sin(n\nu)$ and radial factors $\cosh(n\mu),\sinh(n\mu)$.

Superposing these separated [harmonic functions](../../partial-differential-equation.md#harmonic-function) yields

$$
\boxed{\begin{aligned}
\Phi(\mu,\nu)={}&A_0+B_0\mu\\
&+\sum_{n=1}^\infty\Big\{[A_n\cosh(n\mu)+B_n\sinh(n\mu)]\cos(n\nu)\\
&\hspace{45mm}+[C_n\cosh(n\mu)+D_n\sinh(n\mu)]\sin(n\nu)\Big\}.
\end{aligned}}
$$

To see completeness, expand an arbitrary smooth [harmonic function](../../partial-differential-equation.md#harmonic-function) in a [Fourier series](../../fourier-series.md) in $\nu$ on each ellipse. Substitution into the equation forces every [Fourier coefficient](../../fourier-series.md#fourier-coefficient) to obey the corresponding radial equation above. The series is interpreted with the convergence needed for a [harmonic function](../../partial-differential-equation.md#harmonic-function), for example locally on compact subannuli. No boundedness condition at infinity or extension across $\mu=0$ has been imposed, so there is no reason to discard either radial branch in these [elliptic coordinates](../../geometry-and-topology.md#elliptic-coordinates).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $d=b-a$. In the [mixed Dirichlet-Neumann problem in an elliptic annulus](../../geometry-and-topology.md#mixed-dirichlet-neumann-problem-in-an-elliptic-annulus), the angular [Fourier modes](../../fourier-analysis.md#fourier-mode) separate. The outer data excite the $\cos\nu$ mode, while the inner derivative excites $\cos2\nu$.

For the first mode, a radial factor with zero derivative at $\mu=a$ is $\cosh(\mu-a)$. Normalizing its outer value gives $F_1(\mu)=\cosh(\mu-a)/\cosh d$. For the second mode, a radial factor vanishing at $\mu=b$ is $\sinh[2(b-\mu)]$. Its derivative at $a$ must be $-1$, fixing the coefficient to $1/[2\cosh(2d)]$. Therefore

$$
\boxed{\Phi(\mu,\nu)=\frac{\cosh(\mu-a)}{\cosh(b-a)}\cos\nu+\frac{\sinh[2(b-\mu)]}{2\cosh[2(b-a)]}\cos2\nu.}
$$

Each term satisfies [Laplace's equation](../../partial-differential-equation.md#laplace-equation); at $\mu=b$ the second term vanishes and the first is $\cos\nu$. At $\mu=a$, differentiating gives $0-\cos2\nu$, as required. All other modes, including the constant mode, vanish by the homogeneous mixed conditions. Alternatively, [integration by parts](../../calculus.md#integration-by-parts) applied to the difference of two solutions gives a zero integral of $|\nabla\Phi|^2$, proving [uniqueness](../../mathematical-logic.md#uniqueness).

**Boundary convention.** The calculation follows the explicitly printed coordinate derivative $\partial_\mu\Phi$. In [elliptic coordinates](../../geometry-and-topology.md#elliptic-coordinates), the [scale factor](../../cosmology.md#scale-factor-cosmology) is $h=\sqrt{\sinh^2\mu+\sin^2\nu}$ and the outward [unit normal](../../differential-geometry.md#unit-normal) at the inner boundary points toward decreasing $\mu$. A physical [normal derivative](../../differential-geometry.md#normal-derivative) there would be $-h^{-1}\partial_\mu\Phi$. Thus the phrase “normal derivative” in the source must be understood in its displayed coordinate sense; imposing the same numerical data on a unit-normal derivative would be a different problem.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Set $\kappa=|k|$. The differential operator in the [modified Helmholtz equation](../../partial-differential-equation.md#modified-helmholtz-equation) depends only on $k^2=\kappa^2$. Let $G$ be its decaying [Green function](../../green-s-function.md). Acting on the proposed integral with the operator, in the sense of [distributions](../../distribution-theory.md#distribution-mathematical-analysis), gives

$$
\begin{aligned}
(\nabla_{\mathbf r}^2-k^2)\phi(\mathbf r)
&=\int_{\mathbb R^3}(\nabla_{\mathbf r}^2-k^2)G(\mathbf r,\mathbf r')\rho(\mathbf r')\,d^3\mathbf r'\\
&=\int_{\mathbb R^3}\delta^{(3)}(\mathbf r-\mathbf r')\rho(\mathbf r')\,d^3\mathbf r'\\
&=\rho(\mathbf r).
\end{aligned}
$$

The last step is the sifting property of the [Dirac delta](../../distribution-theory.md#dirac-delta-function). Thus

$$
\boxed{\phi(\mathbf r)=\int_{\mathbb R^3}G(\mathbf r,\mathbf r')\rho(\mathbf r')\,d^3\mathbf r'.}
$$

For a regular rapidly decaying source, the $1/|\mathbf r-\mathbf r'|$ singularity of the kernel found in part (ii) is locally [integrable](../../measure-theory.md#integrability) in three dimensions, and its convolution with the source tends to zero at infinity. This verifies both the equation and the decay condition. The sign of the kernel below corresponds to $\nabla^2-k^2$; reversing the sign of the entire operator reverses the kernel.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

By translation and rotation invariance, use a radial [Green function](../../green-s-function.md) $G(R)$, where $R=|\mathbf r-\mathbf r'|$ is the [Euclidean distance](../../topological-analysis.md#euclidean-distance). Away from the source, the radial [modified Helmholtz equation](../../partial-differential-equation.md#modified-helmholtz-equation) is

$$
G''+\frac2R G'-k^2G=0.
$$

Writing $u=RG$ reduces this to $u''-\kappa^2u=0$, where $\kappa=|k|$. For $\kappa>0$, decay eliminates $e^{\kappa R}/R$, leaving $G=Ae^{-\kappa R}/R$. For $\kappa=0$, the two radial branches are a constant and $1/R$; decay again leaves $A/R$.

To fix the singular normalization, integrate the defining equation over a ball of radius $\varepsilon$ about $\mathbf r'$. The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives

$$
4\pi\varepsilon^2G'(\varepsilon)-k^2\int_{R<\varepsilon}G\,d^3\mathbf r=1.
$$

The volume term is $O(\varepsilon^2)$, whereas

$$
4\pi\varepsilon^2G'(\varepsilon)=-4\pi A e^{-\kappa\varepsilon}(1+\kappa\varepsilon)\longrightarrow-4\pi A.
$$

Consequently

$$
\boxed{A=-\frac1{4\pi},\qquad G(\mathbf r,\mathbf r')=-\frac{e^{-|k||\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|}.}
$$

**Source qualification.** The printed $e^{-kR}$ is the decaying branch only when $k\geq0$, although the source declares $k$ real. For negative $k$ it grows, so it cannot be the requested decaying [Green function](../../green-s-function.md). The absolute value above covers every real $k$ and reduces to the printed form for nonnegative $k$.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The domain is the three-dimensional upper [half-space](../../geometry-and-topology.md#half-space). Reflect the source point to $\mathbf r'^*=(x',y',-z')$. The [method of images](../../mathematics.md#method-of-images) places an opposite source at this reflected point, giving the [Dirichlet image kernel for the three-dimensional modified Helmholtz equation](../../green-s-function.md#dirichlet-image-kernel-for-the-three-dimensional-modified-helmholtz-equation)

$$
\boxed{G_D(\mathbf r,\mathbf r')=-\frac1{4\pi}\left[\frac{e^{-\kappa|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}-\frac{e^{-\kappa|\mathbf r-\mathbf r'^*|}}{|\mathbf r-\mathbf r'^*|}\right],\qquad\kappa=|k|.}
$$

On $z=0$, the two [Euclidean distances](../../topological-analysis.md#euclidean-distance) are equal, so the terms cancel exactly. The image lies outside the domain, so its contribution satisfies the homogeneous [modified Helmholtz equation](../../partial-differential-equation.md#modified-helmholtz-equation) everywhere inside; only the original source contributes a [Dirac delta](../../distribution-theory.md#dirac-delta-function). Both terms decay at infinity, including for $k=0$, and the homogeneous [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) follows.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

This is the [Dirichlet principle](../../calculus-of-variations.md#dirichlet-principle). Put $v=w-\psi$, so $v$ vanishes on the boundary. For real, sufficiently regular functions of finite [Dirichlet energy](../../differential-geometry.md#dirichlet-energy), [Green's first identity](../../partial-differential-equation.md#green-s-first-identity) gives

$$
\int_V\nabla\psi\cdot\nabla v\,dV=\int_Sv\,\partial_n\psi\,dS-\int_Vv\nabla^2\psi\,dV=0.
$$

The surface term is zero because $v=0$, and the volume term is zero because $\psi$ is a [harmonic function](../../partial-differential-equation.md#harmonic-function). Expanding the square of $\nabla w=\nabla\psi+\nabla v$ now gives the stronger identity

$$
\boxed{\int_V|\nabla w|^2\,dV=\int_V|\nabla\psi|^2\,dV+\int_V|\nabla(w-\psi)|^2\,dV\ \geq\ \int_V|\nabla\psi|^2\,dV.}
$$

Thus the [harmonic function](../../partial-differential-equation.md#harmonic-function) minimizes [Dirichlet energy](../../differential-geometry.md#dirichlet-energy) among functions with the same boundary values. Equality requires $\nabla v=0$, hence $v$ is constant on each connected component; the zero boundary value makes that constant zero on every component having boundary. For an unbounded domain one additionally needs the boundary term at infinity to vanish; the usual bounded regular-domain setting needs no such extra condition.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [simple zero](../../holomorphic-function.md#simple-zero) of an [analytic function](../../holomorphic-function.md) has a local factorization $f(z)=(z-z_0)u(z)$, where $u$ is an [analytic function](../../holomorphic-function.md) and $u(z_0)=f'(z_0)\ne0$. Since $1/u$ is also an [analytic function](../../holomorphic-function.md) near $z_0$, its [Taylor series](../../calculus.md#taylor-series) gives

$$
\frac1{f(z)}=\frac1{z-z_0}\left[\frac1{f'(z_0)}+O(z-z_0)\right].
$$

The nonzero coefficient of $(z-z_0)^{-1}$ proves that this is a [simple pole](../../isolated-singularity.md#simple-pole), with

$$
\boxed{\operatorname{Res}_{z=z_0}\frac1{f(z)}=\frac1{f'(z_0)}.}
$$

Multiplying by the [Taylor series](../../calculus.md#taylor-series) $g(z)=g(z_0)+O(z-z_0)$ similarly gives

$$
\boxed{\operatorname{Res}_{z=z_0}\frac{g(z)}{f(z)}=\frac{g(z_0)}{f'(z_0)}.}
$$

The assumption $g(z_0)\ne0$ ensures that the [pole](../../isolated-singularity.md#pole) is not canceled. In either formula the [residue](../../analysis.md#residue) is precisely the coefficient of $(z-z_0)^{-1}$ in the [Laurent series](../../analysis.md#laurent-series).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Clear the apparent negative power of $z$ to obtain the [rational function](../../isolated-singularity.md#rational-function)

$$
h(z)=\frac{-2iz}{z^2-2iaz-1}.
$$

Let $\Delta=\sqrt{a^2-1}>0$. Its denominator factors as $(z-z_-)(z-z_+)$, with

$$
\boxed{z_-=i(a-\Delta),\qquad z_+=i(a+\Delta).}
$$

These are distinct [simple poles](../../isolated-singularity.md#simple-pole). Since $(a-\Delta)(a+\Delta)=1$ and $a+\Delta>1$, we have $0<a-\Delta<1$: only $z_-$ lies inside the [unit circle](../../complex-analysis.md#complex-unit-circle). The apparent singularity at $z=0$ in the original expression is a [removable singularity](../../isolated-singularity.md#removable-singularity), with the continued value $h(0)=0$; it is not another pole.

Using the [residue](../../analysis.md#residue) formula from part (a), with denominator derivative $2z-2ia$, gives

$$
\boxed{\operatorname{Res}_{z=z_-}h=\frac{-2iz_-}{2z_--2ia}=\frac{i(a-\Delta)}{\Delta}.}
$$

There are no other finite singularities of the continued [rational function](../../isolated-singularity.md#rational-function).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

First use $\sin\theta/(a-\sin\theta)=a/(a-\sin\theta)-1$. If $J=\int_{-\pi}^{\pi}(a-\sin\theta)^{-1}\,d\theta$, the required integral is $aJ-2\pi$.

Set $z=e^{i\theta}$. The [unit circle](../../complex-analysis.md#complex-unit-circle) is traversed counterclockwise once, $d\theta=dz/(iz)$, and $\sin\theta=(z-z^{-1})/(2i)$. Thus

$$
J=\frac1i\oint_{|z|=1}\frac{h(z)}z\,dz.
$$

The function $h(z)/z=-2i/(z^2-2iaz-1)$ is regular at zero. Its only enclosed [pole](../../isolated-singularity.md#pole) is $z_-$ from part (b), and its [residue](../../analysis.md#residue) is

$$
\operatorname{Res}_{z=z_-}\frac{h(z)}z=\frac1{z_-}\operatorname{Res}_{z=z_-}h=\frac1\Delta.
$$

By the [residue theorem](../../analysis.md#residue-theorem), $J=(1/i)2\pi i/\Delta=2\pi/\Delta$. Therefore

$$
\boxed{\int_{-\pi}^{\pi}\frac{\sin\theta}{a-\sin\theta}\,d\theta=2\pi\left(\frac{a}{\sqrt{a^2-1}}-1\right).}
$$

As a sign and scale check, this is positive and behaves as $\pi/a^2$ for large $a$, in agreement with expanding the integrand and integrating its first nonzero, $\sin^2\theta/a^2$, term.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $F(\omega)=\widetilde f(\omega)$ to distinguish the [Fourier transform](../../fourier-transform.md) from the original function. [Integration by parts](../../calculus.md#integration-by-parts), using the stated decay, gives

$$
\widehat{f'}(\omega)=\big[f(t)e^{-i\omega t}\big]_{-\infty}^{\infty}+i\omega\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt=i\omega F(\omega).
$$

Applying the same argument to $f'$ gives $\widehat{f''}=i\omega\widehat{f'}=-\omega^2F$. Differentiation with respect to the frequency gives

$$
F'(\omega)=\int_{-\infty}^{\infty}(-it)f(t)e^{-i\omega t}\,dt=-i\widehat{tf}(\omega).
$$

Consequently

$$
\boxed{\widehat{f'}=i\omega F,\qquad\widehat{f''}=-\omega^2F,\qquad\widehat{tf}=iF'.}
$$

The classical steps require existence of the relevant integrals and justification for differentiation under the integral, for example sufficient integrability of $f$, its derivatives and $tf$. The same identities extend to [tempered distributions](../../fourier-analysis.md#tempered-distribution), which is the useful interpretation in part (c).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For the [Gaussian function](../../calculus.md#gaussian-function), direct differentiation gives $f'=-tf$. Applying the [Fourier transform](../../fourier-transform.md) identities from part (a),

$$
i\omega F=-iF',\qquad F'=-\omega F.
$$

Solving this first-order [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) gives

$$
\boxed{h(\omega)=-\omega,\qquad F(\omega)=C e^{-\omega^2/2}.}
$$

In fact, the normalization can also be fixed: the [Gaussian integral](../../integral.md#gaussian-integral) gives $F(0)=\int_{\mathbb R}e^{-t^2/2}\,dt=\sqrt{2\pi}$, so $C=\sqrt{2\pi}$ with the convention used here. The transform has the same Gaussian shape.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $Y=\widehat y$. Transform the three terms of the order-zero [Bessel differential equation](../../bessel-function.md#bessel-differential-equation) using part (a):

$$
\widehat{ty''}=i(-\omega^2Y)'=-i(2\omega Y+\omega^2Y'),\qquad\widehat{y'}=i\omega Y,\qquad\widehat{ty}=iY'.
$$

Adding and dividing by $i$ gives

$$
\boxed{(1-\omega^2)Y'-\omega Y=0.}
$$

On $-1<\omega<1$, [separation of variables](../../partial-differential-equation.md#separation-of-variables) gives $Y'/Y=\omega/(1-\omega^2)$, hence $Y=C/\sqrt{1-\omega^2}$. To obtain the usual solution regular at $t=0$, choose the compactly supported extension

$$
Y(\omega)=\frac{C\,\mathbf1_{(-1,1)}(\omega)}{\sqrt{1-\omega^2}}.
$$

This is a genuine [distributional weak solution](../../partial-differential-equation.md#weak-solution): the differential equation can be written $[(1-\omega^2)Y]'+\omega Y=0$, and $(1-\omega^2)Y=C\sqrt{1-\omega^2}\,\mathbf1_{(-1,1)}$ vanishes continuously at both endpoints. Thus differentiation produces no endpoint [Dirac delta](../../distribution-theory.md#dirac-delta-function) terms.

[Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) now gives

$$
y(t)=\frac{C}{2\pi}\int_{-1}^1\frac{e^{i\omega t}}{\sqrt{1-\omega^2}}\,d\omega.
$$

This integral is smooth at the origin and solves the original equation. Its value there is $C/2$. Normalizing $y(0)=1$ fixes $C=2$, and identifies the [Bessel function of the first kind](../../bessel-function.md#bessel-function-of-the-first-kind) of order zero:

$$
\boxed{J_0(t)=\frac1\pi\int_{-1}^1\frac{\cos(tu)}{\sqrt{1-u^2}}\,du=\frac1\pi\int_0^\pi\cos(t\cos\theta)\,d\theta.}
$$

The last equality uses $u=\cos\theta$. Without normalization, the regular solution is an arbitrary constant times this integral; this is the [Fourier transform of the Bessel function J0](../../bessel-function.md#fourier-transform-of-the-bessel-function-j0) pair.

**Regularity qualification.** The source specifies the differential equation but no condition at its singular point $t=0$. The transformed equation separately has solutions $C_\pm/\sqrt{\omega^2-1}$ on the two exterior intervals. Thus it does not, by itself, determine the support or a single global multiplicative constant. The compactly supported choice above constructs the regular Bessel branch. The other independent branch, the [Bessel function of the second kind](../../bessel-function.md#bessel-function-of-the-second-kind), is singular at the origin. Also $J_0$ is not absolutely integrable on the real line, so its transform is properly taken as a [tempered distribution](../../fourier-analysis.md#tempered-distribution), rather than relying on the stronger classical integrability assumptions of part (a).

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

In orthonormal [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system), a rank-$n$ [tensor](../../multilinear-algebra.md#tensor) has components transforming under a change of axes $R$ as

$$
\boxed{T'_{i_1\cdots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\cdots j_n},\qquad R^TR=I.}
$$

Repeated indices are summed. This is the [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law); for rank one it is precisely the transformation law of a [vector](../../vector-space.md#vector).

Use the [vector triple product](../../multivariable-calculus.md#vector-triple-product) to write the double [cross product](../../vector-space.md#cross-product) as

$$
W=u\times(\Omega\times u)=(u\cdot u)\Omega-(u\cdot\Omega)u.
$$

Both [dot products](../../inner-product.md#dot-product) are invariant under an orthogonal change of axes, while $u'=Ru$ and $\Omega'=R\Omega$. Therefore

$$
W'=(u\cdot u)R\Omega-(u\cdot\Omega)Ru=RW.
$$

Hence **$W$ is a vector**. This argument also avoids the sign issue for an individual [cross product](../../vector-space.md#cross-product) under an orientation-reversing orthogonal transformation: the double product has two such factors, whose signs cancel.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Take the centre of the ball as the origin. An orthogonal change of variables leaves both this domain and its volume measure invariant. Consequently its Cartesian moment integrals are [isotropic tensors](../../multilinear-algebra.md#isotropic-tensor). Equivalently, inversion $x\mapsto-x$ immediately makes every odd moment zero.

There is no nonzero invariant rank-one [vector](../../vector-space.md#vector), so

$$
\boxed{\int_Vx_i\,dV=0.}
$$

An [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor) of rank two is a scalar multiple of the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta), giving $\int_Vx_ix_j\,dV=\alpha\delta_{ij}$. Contract the indices and use [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system):

$$
3\alpha=\int_Vr^2\,dV=4\pi\int_0^a r^4\,dr=\frac{4\pi a^5}{5}.
$$

Thus the [Cartesian moments of a three-dimensional ball](../../geometry-and-topology.md#cartesian-moments-of-a-three-dimensional-ball) give

$$
\boxed{\alpha=\frac{4\pi a^5}{15},\qquad\int_Vx_ix_j\,dV=\frac{4\pi a^5}{15}\delta_{ij},\qquad\int_Vx_ix_jx_k\,dV=0.}
$$

For the last identity, one may also use the general rotation-invariant rank-three tensor $c\epsilon_{ijk}$: the moment is fully symmetric in its indices, whereas the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) is antisymmetric, forcing $c=0$.

The origin convention is necessary. For a ball centred at a nonzero vector $c$, its first moment would instead be $(4\pi a^3/3)c_i$, so the displayed claims implicitly refer to coordinates measured from its centre.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Use the [vector triple product](../../multivariable-calculus.md#vector-triple-product) expression from part (a). Put $s=\Omega\cdot x$ and $r^2=x\cdot x$. Since $u=\Omega+\beta x$,

$$
u\cdot u=\Omega^2+2\beta s+\beta^2r^2,\qquad u\cdot\Omega=\Omega^2+\beta s.
$$

Expanding $W=(u\cdot u)\Omega-(u\cdot\Omega)u$ and canceling the zeroth-order terms gives

$$
\boxed{W(x)=\beta\big[(\Omega\cdot x)\Omega-\Omega^2x\big]+\beta^2\big[r^2\Omega-(\Omega\cdot x)x\big].}
$$

The first bracket is odd in $x$ and integrates to zero over the centred ball. With $\alpha=4\pi a^5/15$, the [Cartesian moments of a three-dimensional ball](../../geometry-and-topology.md#cartesian-moments-of-a-three-dimensional-ball) give

$$
\int_Vr^2\,dV=3\alpha,\qquad\int_V(\Omega\cdot x)x_i\,dV=\Omega_j\int_Vx_jx_i\,dV=\alpha\Omega_i.
$$

Therefore

$$
\boxed{\int_VW_i\,dV=2\alpha\beta^2\Omega_i=\frac{8\pi a^5\beta^2}{15}\Omega_i.}
$$

The resulting [vector](../../vector-space.md#vector) is parallel to $\Omega$, as the rotational symmetry of the centred domain requires.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Use displacements $x_i$ from an [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), so the two spring extensions are $x_2-x_1$ and $x_3-x_2$. The [kinetic energy](../../energy.md#kinetic-energy) and [elastic potential energy](../../elasticity-physics.md#elastic-energy) are

$$
\boxed{T=\frac m2(\dot x_1^2+\mu\dot x_2^2+\dot x_3^2),\qquad V=\frac k2\big[(x_2-x_1)^2+(x_3-x_2)^2\big].}
$$

Thus $T=\dot x^TM\dot x/2$ and $V=x^TKx/2$, with the [small-oscillation mass and stiffness matrices](../../lagrangian-mechanics.md#small-oscillation-mass-and-stiffness-matrices)

$$
\boxed{M=m\begin{pmatrix}1&0&0\\0&\mu&0\\0&0&1\end{pmatrix},\qquad K=k\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.}
$$

If $x_i$ instead denote absolute positions, the appropriate natural spring lengths must first be subtracted from the differences in $V$. They do not affect the equations for displacements.

[Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) give $M\ddot x+Kx=0$, so a [normal mode](../../wave-equation.md#normal-mode) $x=ve^{i\omega t}$ obeys the [generalized eigenvalue problem for small oscillations](../../lagrangian-mechanics.md#generalized-eigenvalue-problem-for-small-oscillations) $Kv=\omega^2Mv$. Reflection symmetry separates antisymmetric shapes $(A,0,-A)^T$ from symmetric shapes $(A,B,A)^T$. In the antisymmetric sector the end equation is $kA=m\omega^2A$, giving $\omega^2=k/m$. In the symmetric sector the two independent equations are

$$
k(A-B)=m\omega^2A,\qquad2k(B-A)=\mu m\omega^2B.
$$

Twice the first plus the second gives $m\omega^2(2A+\mu B)=0$. If $\omega=0$, then $B=A$. Otherwise $B=-2A/\mu$, and substitution into the first equation gives $\omega^2=(k/m)(1+2/\mu)$. Thus the three independent shapes are:

$$
\begin{array}{c|c|c}
&v&\omega^2\\\hline
0&(1,1,1)^T&0\\
1&(1,0,-1)^T&k/m\\
2&(1,-2/\mu,1)^T&(k/m)(1+2/\mu)
\end{array}.
$$

For $v_0$ both springs retain their lengths, so this is uniform translation. For $v_1$ the end masses move oppositely and their forces on the middle mass cancel. For $v_2$ the end masses move together, while the middle mass moves oppositely so the [centre of mass](../../classical-mechanics.md#center-of-mass) remains fixed. Direct substitution verifies all three eigenpairs; for positive $m,k,\mu$ the three [eigenvalues](../../linear-operator-theory.md#eigenvalue) are distinct and exhaust the three degrees of freedom. These are the [normal modes of three masses connected by two equal springs](../../lagrangian-mechanics.md#normal-modes-of-three-masses-connected-by-two-equal-springs).

A useful normalization is the [weighted inner product](../../inner-product.md#weighted-inner-product) induced by $M$. Since the squared mass norms are $m(\mu+2)$, $2m$ and $m(2+4/\mu)$, respectively, take

$$
\boxed{q_0=\frac{v_0}{\sqrt{m(\mu+2)}},\quad q_1=\frac{v_1}{\sqrt{2m}},\quad q_2=\frac{v_2}{\sqrt{m(2+4/\mu)}},\qquad q_i^TMq_j=\delta_{ij}.}
$$

If ordinary Euclidean unit [eigenvectors](../../linear-operator-theory.md#eigenvector) are intended instead, divide $v_0,v_1,v_2$ by $\sqrt3,\sqrt2,\sqrt{2+4/\mu^2}$, respectively. The frequencies and physical motions are independent of this normalization choice. The zero-frequency coordinate has general motion $A+Bt$ rather than an oscillation.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Substitution of $\mu=2$ into the [normal modes of three masses connected by two equal springs](../../lagrangian-mechanics.md#normal-modes-of-three-masses-connected-by-two-equal-springs) gives

$$
\boxed{\Omega=\sqrt{\frac km},\qquad\omega_0=0,\quad\omega_1=\Omega,\quad\omega_2=\sqrt2\,\Omega.}
$$

The corresponding shapes are $v_0=(1,1,1)^T$, $v_1=(1,0,-1)^T$, $v_2=(1,-1,1)^T$. For example, $Kv_2=k(2,-4,2)^T=2(k/m)Mv_2$, verifying the third [eigenvalue](../../linear-operator-theory.md#eigenvalue) directly.

Their relevant [orthogonality](../../inner-product.md#orthogonal-vectors) uses the kinetic matrix $M=m\operatorname{diag}(1,2,1)$:

$$
\boxed{v_i^TMv_j=0\quad(i\ne j),\qquad\begin{pmatrix}v_0&v_1&v_2\end{pmatrix}^{\!T}M\begin{pmatrix}v_0&v_1&v_2\end{pmatrix}=m\operatorname{diag}(4,2,4).}
$$

This is [mass-matrix orthogonality of normal modes](../../lagrangian-mechanics.md#mass-matrix-orthogonality-of-normal-modes). It also follows by subtracting $v_i^TKv_j=\omega_j^2v_i^TMv_j$ from its transpose and using the symmetry of $K,M$. Ordinary [Euclidean inner products](../../inner-product.md#dot-product) need not vanish: in fact $v_0^Tv_2=1$.

<a id="7/b/image-the-three-normal-modes-for-a-free-spring-chain-with-middle-mass-2m-amplitudes-are-relative-and-the-zero-mode-is-translation"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2-2017-ib-normal-modes.png)

**[Figure 1](#7/b/image-the-three-normal-modes-for-a-free-spring-chain-with-middle-mass-2m-amplitudes-are-relative-and-the-zero-mode-is-translation). The three normal modes for a free spring chain with middle mass $2m$; amplitudes are relative and the zero mode is translation**.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Continue with $\mu=2$. Decompose the initial displacement into the [normal modes](../../wave-equation.md#normal-mode):

$$
(2\varepsilon,-\varepsilon,0)^T=\varepsilon v_1+\varepsilon v_2.
$$

There is no translational component. Because all initial velocities vanish, the oscillatory coordinates contain only cosines and the zero-frequency velocity is zero. Therefore

$$
\boxed{\begin{aligned}
x_1(t)&=\varepsilon\big[\cos(\Omega t)+\cos(\sqrt2\,\Omega t)\big],\\
x_2(t)&=-\varepsilon\cos(\sqrt2\,\Omega t),\\
x_3(t)&=\varepsilon\big[-\cos(\Omega t)+\cos(\sqrt2\,\Omega t)\big],\qquad \Omega=\sqrt{k/m}.
\end{aligned}}
$$

At $t=0$ these give the prescribed displacements and zero velocities. Each term separately satisfies $M\ddot x+Kx=0$. Also $x_1+2x_2+x_3=0$ for all $t$, so the [centre of mass](../../classical-mechanics.md#center-of-mass) remains at its original equilibrium position, consistent with the absence of external forces.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

Direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives $P^2=P-I$ and hence $P^3=-I$. It follows that

$$
\begin{aligned}
P^0&=\begin{pmatrix}1&0\\0&1\end{pmatrix},&P&=\begin{pmatrix}1&1\\-1&0\end{pmatrix},&P^2&=\begin{pmatrix}0&1\\-1&-1\end{pmatrix},\\
P^3&=\begin{pmatrix}-1&0\\0&-1\end{pmatrix},&P^4&=\begin{pmatrix}-1&-1\\1&0\end{pmatrix},&P^5&=\begin{pmatrix}0&-1\\1&1\end{pmatrix},
\end{aligned}
$$

and $P^6=I$. These six matrices are distinct; consequently no smaller positive power is the [identity element](../../algebraic-operation.md#identity-element). Thus

$$
\boxed{\langle P\rangle=\{I,P,P^2,P^3,P^4,P^5\}\cong C_6,\qquad\operatorname{ord}(P)=6.}
$$

Products add exponents modulo six and $P^{-1}=P^5$. This verifies the [cyclic group](../../group.md#cyclic-group) structure explicitly.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Observe that $A=-I$, $B^2=I$ and $C=-B$. Thus $A^2=B^2=C^2=I$, while $AB=BA=C$, $AC=CA=B$ and $BC=CB=A$. The [multiplication table](../../arithmetic.md#multiplication-table), with the left factor labeling the row, is

$$
\boxed{\begin{array}{c|cccc}
&I&A&B&C\\\hline
I&I&A&B&C\\
A&A&I&C&B\\
B&B&C&I&A\\
C&C&B&A&I
\end{array}.}
$$

It proves [closure](../../topology.md#closure-topology) of the set. [Associativity](../../algebraic-operation.md#associative-property) is inherited from [matrix multiplication](../../vector-space.md#matrix-multiplication), $I$ is the [identity element](../../algebraic-operation.md#identity-element), and every element is its own [inverse element](../../algebraic-operation.md#inverse-element). Therefore this set is a [group](../../group.md). The table is symmetric, so it is an [Abelian group](../../group.md#abelian-group); its three nonidentity elements have order two, identifying it as the [Klein four-group](../../finite-group-theory.md#klein-four-group) $C_2\times C_2$.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Let $T$ be the set of [torsion elements](../../group-theory.md#torsion-element) of the given [Abelian group](../../group.md#abelian-group). It contains the [identity element](../../algebraic-operation.md#identity-element), which has order one. If $g,h\in T$ have orders $m,n$, set $\ell=\operatorname{lcm}(m,n)$. Commutativity permits powers of the product to split:

$$
(gh^{-1})^\ell=g^\ell h^{-\ell}=e.
$$

Hence $gh^{-1}$ has finite order, dividing $\ell$, and lies in $T$. The nonempty set $T$ therefore satisfies the [subgroup test](../../group.md#subgroup-test) and is a [subgroup](../../group.md#subgroup):

$$
\boxed{T=\{g\in G:\operatorname{ord}(g)<\infty\}\leq G.}
$$

This is the [torsion subgroup](../../group-theory.md#torsion-subgroup). The proof uses commutativity exactly when rearranging the factors in $(gh^{-1})^\ell$; one cannot use that step in an arbitrary noncommutative [group](../../group.md). The subgroup need not itself be a finite set.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Write $A(a,b,c)$ with $a$ in entry $(1,2)$, $b$ in entry $(1,3)$ and $c$ in entry $(2,3)$, and perform all arithmetic in the [finite field](../../algebra.md#finite-field) $\mathbb F_5$. Direct multiplication gives

$$
\boxed{A(a,b,c)A(a',b',c')=A(a+a',\ b+b'+ac',\ c+c').}
$$

Thus the set is closed. [Associativity](../../algebraic-operation.md#associative-property) comes from [matrix multiplication](../../vector-space.md#matrix-multiplication). The [identity element](../../algebraic-operation.md#identity-element) is $A(0,0,0)$, and solving the product formula for it gives

$$
\boxed{A(a,b,c)^{-1}=A(-a,\ ac-b,\ -c).}
$$

Both orders of multiplication with this inverse give the identity. Hence these matrices form a [finite group](../../group.md#finite-group), an instance of the [Heisenberg group over a prime field](../../finite-group-theory.md#heisenberg-group-over-a-prime-field). Each coordinate has five independent possibilities, with distinct triples giving distinct matrices, so

$$
\boxed{|G|=5^3=125.}
$$

The explicit coordinate convention matters because the central coordinate is $b$ here; other descriptions of the [Heisenberg group over a prime field](../../finite-group-theory.md#heisenberg-group-over-a-prime-field) may place the central coordinate last.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

A member of $H$ is $A(t,b,t)$. The multiplication law from part (a) becomes

$$
A(t,b,t)A(s,d,s)=A(t+s,\ b+d+ts,\ t+s).
$$

It stays in $H$ and is unchanged when the two factors are exchanged, since $ts=st$. The identity lies in $H$, and $A(t,b,t)^{-1}=A(-t,t^2-b,-t)$ also lies in $H$. Thus $H$ is an [Abelian subgroup](../../group.md#abelian-subgroup), namely the [Abelian plane subgroup of a finite Heisenberg group](../../finite-group-theory.md#abelian-plane-subgroup-of-a-finite-heisenberg-group) in this coordinate convention.

There are five choices each for $t,b$, so

$$
\boxed{|H|=25,\qquad [G:H]=\frac{125}{25}=5.}
$$

This verifies [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem): the subgroup order divides the group order, and the number of distinct left [cosets](../../group-theory.md#coset) is five.

Explicitly, the map $\varphi(A(a,b,c))=a-c$ is a surjective [group homomorphism](../../group-theory.md#group-homomorphism) to the additive group of $\mathbb F_5$, by the product formula. Its [kernel of a group homomorphism](../../group-theory.md#kernel-of-a-group-homomorphism) is $H$. Thus $H$ is even a [normal subgroup](../../group-theory.md#normal-subgroup); the five left [cosets](../../group-theory.md#coset) are the level sets $a-c=d$ for $d=0,1,2,3,4$, with representatives $A(d,0,0)$. Each contains 25 elements, providing a direct count as well.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

Squaring with the product law gives

$$
A(a,b,c)^2=A(2a,\ 2b+ac,\ 2c).
$$

Equality to the [identity matrix](../../vector-space.md#identity-matrix) requires $2a=2c=0$ in $\mathbb F_5$. Since 2 has a multiplicative inverse modulo 5, this forces $a=c=0$. The middle condition then gives $2b=0$, hence $b=0$. Therefore

$$
\boxed{\{A\in G:A^2=I\}=\{I\}.}
$$

This agrees with [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem): a group of odd order has no element of order two.

The subset specified by $b\ne0$ **is not a subgroup**. It omits the [identity element](../../algebraic-operation.md#identity-element). It also fails [closure](../../topology.md#closure-topology): both $A(0,1,0)$ and $A(0,4,0)$ lie in it, but their product is $A(0,0,0)=I$, whose $b$ coordinate is zero.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

A finite-dimensional [representation](../../representation-theory.md#group-representation) of a [group](../../group.md) $G$ on a vector space $V$ is a [group homomorphism](../../group-theory.md#group-homomorphism) $D:G\to\operatorname{GL}(V)$. Thus each $D(X)$ is invertible and

$$
D(XY)=D(X)D(Y),\qquad D(I)=I_V.
$$

Here the group identity and the identity linear map are different objects, represented by corresponding symbols. Applying the multiplication property to $XX^{-1}=X^{-1}X=I$ gives

$$
D(X)D(X^{-1})=I_V=D(X^{-1})D(X).
$$

By the defining property of a [matrix inverse](../../matrix-inverse.md),

$$
\boxed{D(X^{-1})=D(X)^{-1}.}
$$

If the definition only states the multiplication law together with invertibility, $D(I)^2=D(I)$ already forces $D(I)=I_V$ after multiplication by its inverse.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Use the identity relation as printed in the PDF, $XYZ=I$. Since $Z^2=I$, multiplying on the right by $Z$ gives $XY=Z$. Also

$$
YX=(XY)^{-1}=Z^{-1}=Z=XY,
$$

because $X,Y,Z$ are involutions. Thus $X$ and $Y$ commute, and so does their product $Z$ with either of them. Therefore **the group is Abelian**, and is the [Klein four-group](../../finite-group-theory.md#klein-four-group).

Each [conjugacy class](../../group-action.md#conjugacy-class) is a singleton. Over the complex numbers every [irreducible representation of a finite abelian group](../../representation-theory.md#irreducible-representation-of-a-finite-abelian-group) is one-dimensional. Choose independent signs $\varepsilon=\chi(X)$ and $\eta=\chi(Y)$; the relations force $\varepsilon^2=\eta^2=1$ and $\chi(Z)=\varepsilon\eta$. Hence the complete [character table](../../representation-theory.md#character-table) is

$$
\boxed{\begin{array}{c|rrrr}
&I&X&Y&Z\\\hline
\chi_{++}&1&1&1&1\\
\chi_{+-}&1&1&-1&-1\\
\chi_{-+}&1&-1&1&-1\\
\chi_{--}&1&-1&-1&1
\end{array}.}
$$

These four distinct [one-dimensional representations](../../representation-theory.md#one-dimensional-representation) exhaust the irreducible possibilities: there are four [conjugacy classes](../../group-action.md#conjugacy-class), and their squared dimensions already sum to $|G|=4$. The rows also satisfy [character orthogonality](../../representation-theory.md#character-orthogonality). The local transcription damages the final symbol in the defining relation; the PDF makes the identity $I$ unambiguous.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Put $Y_p=D(Y)$. Direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives

$$
Y_p^2=\begin{pmatrix}1&p-p\\0&1\end{pmatrix}=I_2
$$

for every real $p$. Since $D(X)=-I_2$ commutes with all matrices and $D(Z)=-Y_p$, the remaining relations also hold:

$$
D(X)^2=D(Z)^2=I_2,\qquad D(X)D(Y)=D(Z),\qquad D(X)D(Y)D(Z)=I_2.
$$

All matrices are invertible, and the relations reproduce the [multiplication table](../../arithmetic.md#multiplication-table) of the [Klein four-group](../../finite-group-theory.md#klein-four-group). Therefore

$$
\boxed{p\in\mathbb R\text{ is arbitrary}.}
$$

A [representation](../../representation-theory.md#group-representation) need not be an [orthogonal representation](../../representation-theory.md#orthogonal-representation); imposing orthogonality on the displayed matrices would be an extra condition.

The [characters](../../representation-theory.md#character-of-a-representation) are their traces, independent of $p$:

$$
\boxed{\big(\chi(I),\chi(X),\chi(Y),\chi(Z)\big)=(2,-2,0,0).}
$$

In terms of part (b), $\chi=\chi_{-+}+\chi_{--}$, so the representation is reducible. For an explicit [change of basis](../../linear-algebra.md#change-of-basis), take

$$
S=\begin{pmatrix}1&-p/2\\0&1\end{pmatrix}.
$$

Then $S^{-1}D(Y)S=\operatorname{diag}(-1,1)$ and $S^{-1}D(Z)S=\operatorname{diag}(1,-1)$, while $D(X)$ remains $-I_2$. These are the [equivalent sheared representations of the Klein four-group](../../finite-group-theory.md#equivalent-sheared-representations-of-the-klein-four-group); the parameter changes the basis, not the two irreducible constituents.

## ↑ Ancestors (10)

1. [2017](../2017.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
