# Paper 2

↑ **Parent:** [2015](../2015.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2015/PaperNST_IB_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2015/PaperNST_IB_2.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
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
  - [d](#7/d)
    - [Solution](#7/d/solution)
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
  - [d](#9/d)
    - [Solution](#9/d/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)
  - [d](#10/d)
    - [Solution](#10/d/solution)
  - [e](#10/e)
    - [Solution](#10/e/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

On its specified domain of admissible functions, a [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) equals its adjoint, including the adjoint domain. Its integration identity on the interval is

$$
\boxed{\langle u,Lv\rangle=\langle Lu,v\rangle,\qquad\langle u,v\rangle=\int_a^b u^*(x)v(x)\,dx.}
$$

For a differential operator, the boundary conditions must make the boundary form from [integration by parts](../../calculus.md#integration-by-parts) vanish. Formal symmetry of the differential expression alone does not specify a self-adjoint boundary-value problem.

Apply this identity to two [eigenfunctions](../../linear-operator-theory.md#eigenfunction). Since the weight is real,

$$
\lambda_n\int_a^b wy_m^*y_n\,dx=\int_a^b y_m^*Ly_n\,dx=\int_a^b(Ly_m)^*y_n\,dx=\lambda_m^*\int_a^b wy_m^*y_n\,dx.
$$

First take $m=n$: positivity of $\int_a^b w|y_n|^2dx$ shows $\lambda_n=\lambda_n^*$, so the [eigenvalues](../../linear-operator-theory.md#eigenvalue) are real. For distinct eigenvalues, subtraction therefore gives

$$
\boxed{\int_a^b w(x)y_m^*(x)y_n(x)\,dx=0\quad(\lambda_m\ne\lambda_n).}
$$

This is [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions) in the [weighted inner product](../../inner-product.md#weighted-inner-product), rather than necessarily in the unweighted inner product.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

To obtain [Sturm-Liouville form](../../sturm-liouville-theory.md#sturm-liouville-form), multiply the equation by $(1-x^2)^{-1/2}$. The derivative identity

$$
\frac d{dx}\big[\sqrt{1-x^2}\,y_n'\big]=\sqrt{1-x^2}\,y_n''-\frac{x}{\sqrt{1-x^2}}y_n'
$$

gives

$$
\boxed{-\frac d{dx}\left[\sqrt{1-x^2}\,y_n'\right]=n^2\frac{y_n}{\sqrt{1-x^2}},\qquad p(x)=\sqrt{1-x^2},\quad q(x)=0,\quad w(x)=\frac1{\sqrt{1-x^2}}.}
$$

The weight determines the [weighted inner product](../../inner-product.md#weighted-inner-product) on $(-1,1)$. It is integrable but singular at the endpoints, where $p$ also vanishes. Thus this is a singular-endpoint [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem), not a regular problem with strictly positive endpoint values of $p$. The transformation in part (ii) specifies its admissible Dirichlet realization; these are the [Dirichlet eigenfunctions of the Chebyshev differential operator](../../numerical-analysis.md#dirichlet-eigenfunctions-of-the-chebyshev-differential-operator).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Let $Y(\theta)=y(\cos\theta)$ for $0\leq\theta\leq\pi$. The [chain rule](../../calculus.md#chain-rule) gives

$$
y'=-\frac{Y'}{\sin\theta},\qquad y''=\frac{Y''}{\sin^2\theta}-\frac{\cos\theta}{\sin^3\theta}Y'.
$$

Substitution cancels the first-derivative terms and leaves $-Y''=n^2Y$. The endpoint conditions become $Y(0)=Y(\pi)=0$. For $n\ne0$, the first condition selects $Y=A\sin(n\theta)$, and the second requires $\sin(n\pi)=0$. Thus a nonzero solution requires an integer $n$. The case $n=0$ gives $Y=A+B\theta$ and both conditions force it to vanish. Negative integers give the same eigenvalues and eigenfunctions up to sign, so take $n=1,2,\ldots$.

For [vector normalization](../../vector-space.md#vector-normalization), use $w(x)dx=-d\theta$:

$$
1=\int_{-1}^1w(x)|y_n(x)|^2dx=|A|^2\int_0^\pi\sin^2(n\theta)d\theta=|A|^2\frac\pi2.
$$

Choosing a positive real normalization constant gives

$$
\boxed{y_n(x)=\sqrt{\frac2\pi}\sin(n\arccos x)=\sqrt{\frac2\pi}\sqrt{1-x^2}\,U_{n-1}(x),\qquad\lambda_n=n^2.}
$$

Here $U_{n-1}$ is the [Chebyshev polynomial of the second kind](../../numerical-analysis.md#chebyshev-polynomial-of-the-second-kind). The factors $\sqrt{1-x^2}$ make both endpoint values zero. The derivatives need not stay finite there; instead $py_n'=-n\sqrt{2/\pi}\cos(n\theta)$ has finite endpoint limits, ensuring that the relevant boundary form vanishes.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Using the normalized [eigenfunctions](../../linear-operator-theory.md#eigenfunction) and the same change of variables, their [weighted inner product](../../inner-product.md#weighted-inner-product) is

$$
\int_{-1}^1\frac{y_m(x)y_n(x)}{\sqrt{1-x^2}}\,dx=\frac2\pi\int_0^\pi\sin(m\theta)\sin(n\theta)\,d\theta.
$$

For distinct positive integers $m,n$, the product-to-sum identity gives

$$
\frac1\pi\int_0^\pi[\cos((m-n)\theta)-\cos((m+n)\theta)]d\theta=0,
$$

because each integrated sine has integer-multiple-of-$\pi$ endpoints. For $m=n$, the integral is one by the normalization already calculated. Hence

$$
\boxed{\int_{-1}^1w(x)y_m(x)y_n(x)\,dx=\delta_{mn}.}
$$

This verifies [orthonormality](../../inner-product.md#orthonormal-set) explicitly, with $\delta_{mn}$ the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta).

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $\Phi(r,\theta)=R(r)\Theta(\theta)$ for [separation of variables](../../partial-differential-equation.md#separation-of-variables). Multiplication by $r^2/(R\Theta)$ gives

$$
\frac{r^2R''+rR'}R=-\frac{\Theta''}{\Theta}=\lambda.
$$

Single-valuedness requires a $2\pi$-periodic angular function. The nonzero possibilities are $\lambda=n^2$ for integers $n\geq0$. For $n\geq1$, $\Theta$ is a combination of $\cos n\theta$ and $\sin n\theta$, while the radial [Euler-Cauchy equation](../../linear-ordinary-differential-equation.md#euler-cauchy-equation) has solutions $r^n,r^{-n}$. At $n=0$, periodicity excludes an angular term proportional to $\theta$, and $(rR')'=0$ gives $R=A_0+B_0\ln r$.

Superposing the separated [harmonic functions](../../partial-differential-equation.md#harmonic-function) yields

$$
\boxed{\begin{aligned}
\Phi(r,\theta)={}&A_0+B_0\ln r\\
&+\sum_{n=1}^\infty\big[(A_nr^n+B_nr^{-n})\cos n\theta+(C_nr^n+D_nr^{-n})\sin n\theta\big].
\end{aligned}}
$$

To obtain the general solution, expand any sufficiently regular harmonic function in a [Fourier series](../../fourier-series.md) on circles; each [Fourier coefficient](../../fourier-series.md#fourier-coefficient) satisfies the corresponding radial equation. The coefficients must give the required convergence on compact annuli. Because no condition at zero or infinity is imposed in this part, neither radial branch is discarded.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Boundedness at the origin allows only $r^n$ for nonconstant interior modes; decay at infinity allows only $r^{-n}$ outside. Write the common surface potential in its [Fourier series](../../fourier-series.md) as $\sum_{n\geq1}v_n(\theta)$, where $v_n=A_n\cos n\theta+B_n\sin n\theta$. Continuity then makes the corresponding interior and exterior factors $(r/R)^n$ and $(R/r)^n$.

Their outward radial derivatives at the surface are $nv_n/R$ inside and $-nv_n/R$ outside. Thus the jump is $-2nv_n/R$. Equating it to minus the prescribed surface-charge mode gives

$$
v_n(\theta)=\frac{R}{2n}(a_n\cos n\theta+b_n\sin n\theta).
$$

Therefore the [potential of a charged cylindrical shell with angular Fourier data](../../electric-field.md#potential-of-a-charged-cylindrical-shell-with-angular-fourier-data) is

$$
\boxed{\Phi(r,\theta)=\sum_{n=1}^\infty\frac{R}{2n}\begin{cases}(r/R)^n,&0\leq r\leq R,\\(R/r)^n,&r\geq R\end{cases}(a_n\cos n\theta+b_n\sin n\theta).}
$$

Either branch gives the same value at $R$. The mean angular mode is zero: outside, neither a constant nor a logarithm can survive the condition at infinity; continuity then forces the interior constant to zero. Consequently $\Phi(0)=0$.

The absence of a mean term in the [surface charge density](../../electrostatics.md#surface-charge-density) is essential. A nonzero mean would require a logarithmic exterior potential and would be incompatible with decay at infinity in this two-dimensional reduction. The normalization follows the stated derivative jump, with no additional permittivity factor introduced.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the [product rule](../../calculus.md#product-rule) for the [vector field](../../multivariable-calculus.md#vector-field) $F=\phi\nabla\psi-\psi\nabla\phi$:

$$
\nabla\cdot F=\nabla\phi\cdot\nabla\psi+\phi\nabla^2\psi-\nabla\psi\cdot\nabla\phi-\psi\nabla^2\phi=\phi\nabla^2\psi-\psi\nabla^2\phi.
$$

The mixed [dot products](../../inner-product.md#dot-product) cancel. Applying the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) with the outward [unit normal](../../differential-geometry.md#unit-normal) gives [Green's second identity](../../partial-differential-equation.md#green-second-identity),

$$
\boxed{\int_V(\phi\nabla^2\psi-\psi\nabla^2\phi)dV=\int_S(\phi\,n\cdot\nabla\psi-\psi\,n\cdot\nabla\phi)dS.}
$$

The fields and boundary are assumed sufficiently regular; a Green-function singularity is handled by excising a small ball or by using [distributions](../../distribution-theory.md#distribution-mathematical-analysis).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Fix $\mathbf x'$ inside $V$ and put $\psi(\mathbf x)=G(\mathbf x,\mathbf x')$ in [Green's second identity](../../partial-differential-equation.md#green-second-identity). The volume integral becomes

$$
\int_V\big[\phi(\mathbf x)(-\delta^{(3)}(\mathbf x-\mathbf x'))-G(\mathbf x,\mathbf x')\cdot0\big]dV=-\phi(\mathbf x').
$$

Here [Laplace's equation](../../partial-differential-equation.md#laplace-equation) eliminates the second term, and the [Dirac delta](../../distribution-theory.md#dirac-delta-function) evaluates the first. Reversing the signs in the boundary integral gives

$$
\boxed{\phi(\mathbf x')=\int_S\left[G(\mathbf x,\mathbf x')\,n\cdot\nabla_{\mathbf x}\phi(\mathbf x)-\phi(\mathbf x)\,n\cdot\nabla_{\mathbf x}G(\mathbf x,\mathbf x')\right]dS.}
$$

All boundary derivatives act on the integration variable $\mathbf x$, not on the fixed evaluation point $\mathbf x'$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Impose the homogeneous [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) on the boundary variable:

$$
\boxed{G(\mathbf x,\mathbf x')=0\quad\text{for }\mathbf x\in S,\ \mathbf x'\in V.}
$$

This removes the term containing the unknown normal derivative of $\phi$. The prescribed boundary values alone then determine the solution through

$$
\phi(\mathbf x')=-\int_S f(\mathbf x)\,\partial_{n_{\mathbf x}}G(\mathbf x,\mathbf x')\,dS.
$$

For an unbounded domain one also imposes the appropriate decay condition at infinity. This defines the required [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let the evaluation point be $\mathbf r_0=(x,y,z)$, $z>0$, and reflect it to $\mathbf r_0^*=(x,y,-z)$. The [method of images](../../mathematics.md#method-of-images) constructs

$$
\boxed{G(\mathbf r,\mathbf r_0)=\frac1{4\pi}\left[\frac1{|\mathbf r-\mathbf r_0|}-\frac1{|\mathbf r-\mathbf r_0^*|}\right].}
$$

The two [Euclidean distances](../../topological-analysis.md#euclidean-distance) coincide on the plane, so $G=0$ there. The negative image source lies outside the domain; inside, only the real source contributes to $-\nabla_{\mathbf r}^2G=\delta^{(3)}(\mathbf r-\mathbf r_0)$. The difference also decays at infinity.

On the plane write $\mathbf r=(\xi,\eta,s)$ and set $s=0$. The outward [unit normal](../../differential-geometry.md#unit-normal) of the upper half-space is $n=-e_z$. Direct differentiation gives

$$
\left.\partial_sG\right|_{s=0}=\frac{z}{2\pi[(x-\xi)^2+(y-\eta)^2+z^2]^{3/2}},\qquad\partial_nG=-\partial_sG.
$$

Substituting into the boundary representation from part (c) yields the [Poisson kernel for the upper half-space](../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-space):

$$
\boxed{\phi(x,y,z)=\frac{z}{2\pi}\int_{\mathbb R^2}\frac{f(\xi,\eta)}{[(x-\xi)^2+(y-\eta)^2+z^2]^{3/2}}\,d\xi\,d\eta.}
$$

Its sign is positive, as expected from the [maximum principle](../../partial-differential-equation.md#maximum-principle) for nonnegative boundary data. Its normalization can be checked in [polar coordinates](../../multivariable-calculus.md#polar-coordinates):

$$
\int_{\mathbb R^2}P_z\,d\xi\,d\eta=z\int_0^\infty\frac{r\,dr}{(r^2+z^2)^{3/2}}=1.
$$

As $z\downarrow0$ the kernel is an [approximate identity](../../fourier-analysis.md#approximate-identity), recovering $f$ at its continuity points. Boundary data must have the decay and regularity compatible with the stated condition at infinity.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

On the axis, the [Poisson kernel for the upper half-space](../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-space) depends only on the radial boundary coordinate. Integrating over the disk gives

$$
\phi(0,0,z)=\frac z{2\pi}\int_0^{2\pi}d\theta\int_0^a\frac{r\,dr}{(r^2+z^2)^{3/2}}=z\left[-\frac1{\sqrt{r^2+z^2}}\right]_0^a.
$$

Therefore the [axial Poisson extension of a circular boundary patch](../../partial-differential-equation.md#axial-poisson-extension-of-a-circular-boundary-patch) is

$$
\boxed{\phi(0,0,z)=1-\frac{z}{\sqrt{a^2+z^2}},\qquad z>0.}
$$

It tends to one as the axis approaches the boundary inside the patch, and tends to zero as $a^2/(2z^2)$ far above it.

The boundary values jump at the circular rim. They are understood almost everywhere, or as limits at continuity points; changing the assigned value on that measure-zero circle does not change the integral. At a rim point the vertical limit is one-half, rather than a continuous extension with the specified value on both sides of the jump.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Let $f$ be [meromorphic](../../isolated-singularity.md#meromorphic-function) on and inside a positively oriented simple closed [contour](../../complex-analysis.md#complex-integration-contour) $C$, with finitely many isolated poles $z_k$ inside and none on $C$. The [residue theorem](../../analysis.md#residue-theorem) states

$$
\boxed{\oint_C f(z)\,dz=2\pi i\sum_{z_k\text{ inside }C}\operatorname{Res}_{z=z_k}f(z).}
$$

The positive orientation is counterclockwise. A clockwise contour reverses the sign, and the [residue](../../analysis.md#residue) is the coefficient of $(z-z_k)^{-1}$ in the local [Laurent series](../../analysis.md#laurent-series).

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The denominator vanishes at the four roots of $z^4=-1$, namely $z_k=e^{i(2k+1)\pi/4}$ for $k=0,1,2,3$. They are [simple poles](../../isolated-singularity.md#simple-pole), since $(1+z^4)'=4z^3$ is nonzero at each root and the numerator does not vanish there. The simple-pole [residue](../../analysis.md#residue) formula gives

$$
\boxed{\operatorname{Res}_{z=z_k}\frac{z^2}{1+z^4}=\frac{z_k^2}{4z_k^3}=\frac1{4z_k}.}
$$

Explicitly,

$$
\begin{array}{c|c}
\text{pole}&\text{residue}\\\hline
(1+i)/\sqrt2&(1-i)/(4\sqrt2)\\
(-1+i)/\sqrt2&(-1-i)/(4\sqrt2)\\
(-1-i)/\sqrt2&(-1+i)/(4\sqrt2)\\
(1-i)/\sqrt2&(1+i)/(4\sqrt2)
\end{array}.
$$

There are no branch points or other finite singularities. At infinity the function is $O(z^{-2})$, so infinity is removable rather than a pole.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

Close the interval $[-R,R]$ with an upper [semicircle](../../topology.md#semicircle), traversed counterclockwise. On its large arc,

$$
\left|\frac{z^2}{1+z^4}\right|\leq\frac{R^2}{R^4-1},
$$

so the [estimation lemma](../../complex-analysis.md#estimation-lemma) bounds the arc integral by $\pi R^3/(R^4-1)\to0$. The enclosed [residues](../../analysis.md#residue) are those at $(1+i)/\sqrt2$ and $(-1+i)/\sqrt2$, whose sum is $-i/(2\sqrt2)$. The [residue theorem](../../analysis.md#residue-theorem) therefore gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{x^2}{1+x^4}\,dx=2\pi i\left(-\frac{i}{2\sqrt2}\right)=\frac\pi{\sqrt2}.}
$$

The positive sign agrees with the nonnegative real integrand.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose a branch of the [complex logarithm](../../analysis.md#complex-logarithm) with $-\pi/2<\arg z<3\pi/2$, placing its [branch cut](../../analysis.md#branch-cut) down the negative imaginary axis. Thus $\operatorname{Log} x=\ln x$ for $x>0$, while $\operatorname{Log}(-x)=\ln x+i\pi$ on the negative real axis for $x>0$.

Integrate $\operatorname{Log} z/(z^2+a^2)$ around an upper [semicircle](../../topology.md#semicircle), with a small clockwise semicircular indentation above zero. The large arc contributes $O(\ln R/R)\to0$, and the small arc contributes $O(\varepsilon|\ln\varepsilon|)\to0$. The only enclosed [pole](../../isolated-singularity.md#pole) is $ia$, with

$$
\operatorname{Res}_{z=ia}\frac{\operatorname{Log} z}{z^2+a^2}=\frac{\ln a+i\pi/2}{2ia}.
$$

Writing $I(a)$ for the required integral, the negative real segment contributes $I(a)+i\pi\int_0^\infty dx/(x^2+a^2)$. Hence the [residue theorem](../../analysis.md#residue-theorem) gives

$$
2I(a)+\frac{i\pi^2}{2a}=\frac\pi a\left(\ln a+\frac{i\pi}{2}\right).
$$

The imaginary terms cancel, leaving

$$
\boxed{\int_0^\infty\frac{\ln x}{x^2+a^2}\,dx=\frac{\pi\ln a}{2a}.}
$$

The integral converges at both endpoints because $|\ln x|$ is integrable near zero and $\ln x/x^2$ is integrable at infinity. As a real-variable check, scaling $x=au$ reduces the result to the vanishing first logarithmic moment at $a=1$, one of the [logarithmic moments of the Cauchy kernel](../../complex-analysis.md#logarithmic-moments-of-the-cauchy-kernel).

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use the [Fourier transform](../../fourier-transform.md) convention $\widetilde y(\omega)=\int_{\mathbb R}y(t)e^{-i\omega t}dt$. For a transformable response with the necessary boundary terms vanishing, [integration by parts](../../calculus.md#integration-by-parts) gives

$$
\widetilde{\dot y}=i\omega\widetilde y,\qquad\widetilde{\ddot y}=-\omega^2\widetilde y.
$$

Transforming the differential equation therefore gives $(5-\omega^2+2i\omega)\widetilde y=\widetilde f$, so

$$
\boxed{\widetilde y(\omega)=\frac{-\widetilde f(\omega)}{\omega^2-2i\omega-5}.}
$$

The identities also hold for [tempered distributions](../../fourier-analysis.md#tempered-distribution). The denominator factors as $(\omega-i-2)(\omega-i+2)$; its two poles are in the upper half-plane, corresponding under inverse factor $e^{i\omega t}$ to the [causal Green function of a damped oscillator](../../analysis.md#causal-green-function-of-a-damped-oscillator).

The frequency-domain formula selects the Fourier-transformable response. Decay of the force alone would not remove arbitrary homogeneous solutions, which grow towards negative time and do not have an ordinary bilateral Fourier transform.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Substitution gives

$$
\widetilde y(\omega)=\frac{-i}{(\omega-2i)(\omega-i-2)(\omega-i+2)}.
$$

The inverse [Fourier transform](../../fourier-transform.md) is $(2\pi)^{-1}\int_{\mathbb R}\widetilde y(\omega)e^{i\omega t}d\omega$. For $t<0$, close clockwise in the lower half-plane, where there are no poles; hence $y(t)=0$.

For $t>0$, close counterclockwise in the upper half-plane. The three simple-pole [residues](../../analysis.md#residue) of the full inversion integrand are

$$
\begin{array}{c|c}
\omega&\operatorname{Res}(\widetilde y e^{i\omega t})\\\hline
2i&ie^{-2t}/5\\
2+i&(1-2i)e^{(-1+2i)t}/20\\
-2+i&(-1-2i)e^{(-1-2i)t}/20
\end{array}.
$$

Multiplying their sum by $i$ and combining the conjugate exponential contributions yields

$$
\boxed{y(t)=\begin{cases}0,&t\leq0,\\[2pt]\dfrac1{10}\left[e^{-t}(2\cos2t-\sin2t)-2e^{-2t}\right],&t>0.\end{cases}}
$$

The large arcs vanish because the rational factor is $O(\omega^{-3})$ and the exponential is bounded on the chosen half-plane. At zero, the right-hand value and first derivative are both zero, matching the negative-time branch, so no unwanted delta or delta derivative appears in the second-order equation.

For an independent dynamical check, this is the [exponential forcing of an underdamped oscillator](../../analysis.md#exponential-forcing-of-an-underdamped-oscillator) with damping $\gamma=1$, natural frequency $\sqrt5$, damped frequency $2$, exponent $\beta=2$ and force amplitude $-1$. For positive time its substitution gives $y''+2y'+5y=-e^{-2t}$.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

The result of part (i) vanishes identically on the open interval $t<0$, so its first and second derivatives also vanish there. Substituting into the equation of motion immediately gives

$$
\boxed{f(t)=0\quad(t<0).}
$$

Thus the force has no negative-time prehistory, consistent with the [causal Green function of a damped oscillator](../../analysis.md#causal-green-function-of-a-damped-oscillator). In fact, direct inversion or the positive-time substitution above identifies $f(t)=-e^{-2t}H(t)$; the given numerator $+i$ corresponds to a negative exponential force with this Fourier convention. Here $H$ is the [Heaviside step function](../../integral-transform.md#heaviside-step-function); its value exactly at the jump does not affect the transform.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Preserving Cartesian lengths and [Euclidean inner products](../../inner-product.md#dot-product) requires an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix):

$$
\boxed{M^TM=MM^T=I,\qquad M_{ik}M_{jk}=\delta_{ij}.}
$$

Its determinant is $\pm1$. Relative to an originally right-handed frame, $\det M=+1$ gives a right-handed frame and $\det M=-1$ a left-handed frame. More generally, this sign determines whether the two frames have the same or opposite orientation.

The [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law) is

$$
\boxed{T'_{ij}=M_{ik}M_{j\ell}T_{k\ell},\qquad T'=MTM^T.}
$$

For a [tensor field](../../vector-bundle.md#tensor-field), the components are compared at the same physical point, whose coordinates satisfy $x=M^Tx'$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Define the [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor) and [antisymmetric tensor](../../multilinear-algebra.md#antisymmetric-tensor) parts by $S=(T+T^T)/2$ and $A=(T-T^T)/2$. The transformed transpose satisfies $(T')^T=(MTM^T)^T=MT^TM^T$. Therefore

$$
S'=\frac12(T'+(T')^T)=M\frac12(T+T^T)M^T=MSM^T,
$$

and similarly

$$
A'=\frac12(T'-(T')^T)=M\frac12(T-T^T)M^T=MAM^T.
$$

Both obey the [tensor component transformation law](../../general-relativity.md#tensor-component-transformation-law). Thus **the symmetric and antisymmetric parts are themselves second-order tensors**. Taking a transpose and forming linear combinations commute with this orthogonal change of frame.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $r=\sqrt{x_1^2+x_2^2}$. Averaging each pair of transposed entries gives the [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor)

$$
\boxed{S=\frac12(F+F^T)=\begin{pmatrix}x_1^2&x_1x_2&0\\x_1x_2&x_2^2&0\\0&0&3r^2\end{pmatrix}.}
$$

For $r>0$, the upper block is the [outer product](../../vector-space.md#outer-product) of $(x_1,x_2)$ with itself. It sends that vector to $r^2$ times itself and annihilates its perpendicular. Thus its orthonormal [principal axes](../../rigid-body-dynamics.md#principal-axis) and corresponding [eigenvalues](../../linear-operator-theory.md#eigenvalue) are

$$
\boxed{\begin{array}{c|c|l}
\text{axis}&\text{principal value}&\text{geometric direction}\\\hline
 e_r=(x_1,x_2,0)/r&r^2&\text{radially outward from the }x_3\text{-axis}\\
 e_\theta=(-x_2,x_1,0)/r&0&\text{tangent to a circle about the }x_3\text{-axis}\\
 e_3=(0,0,1)&3r^2&\text{parallel to the }x_3\text{-axis}
\end{array}.}
$$

Taking these vectors as the rows of the change-of-components matrix gives

$$
\boxed{M(x)=\begin{pmatrix}x_1/r&x_2/r&0\\-x_2/r&x_1/r&0\\0&0&1\end{pmatrix},\qquad MSM^T=\operatorname{diag}(r^2,0,3r^2).}
$$

This matrix is orthogonal with determinant one. These are the [principal axes of a planar rank-one tensor block](../../multilinear-algebra.md#principal-axes-of-a-planar-rank-one-tensor-block).

<a id="6/c/image-the-radial-and-tangential-principal-directions-rotate-with-position-the-third-principal-axis-is-perpendicular-to-this-plane"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2-2015-ib-principal-axes.png)

**[Figure 1](#6/c/image-the-radial-and-tangential-principal-directions-rotate-with-position-the-third-principal-axis-is-perpendicular-to-this-plane). The radial and tangential principal directions rotate with position; the third principal axis is perpendicular to this plane**.

The matrix is a pointwise frame transformation: because its angle varies with position, it does not represent one fixed Cartesian rotation diagonalizing the entire field everywhere. On the axis $r=0$, the symmetric tensor is zero; all principal values coincide and any orthonormal axes may be chosen. The displayed formula for $M$ is therefore used only off that axis.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The [scalar, symmetric-traceless and axial tensor decomposition](../../multilinear-algebra.md#scalar-symmetric-traceless-and-axial-tensor-decomposition) fixes the scalar part by the trace:

$$
\boxed{P=\frac13\operatorname{tr}F=\frac43r^2.}
$$

Subtracting this isotropic part from the [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor) in part (c) gives

$$
\boxed{\widehat S=\frac13\begin{pmatrix}-x_1^2-4x_2^2&3x_1x_2&0\\3x_1x_2&-4x_1^2-x_2^2&0\\0&0&5r^2\end{pmatrix}.}
$$

Its trace is zero. The [antisymmetric tensor](../../multilinear-algebra.md#antisymmetric-tensor) part is

$$
\boxed{\widehat A=\frac12(F-F^T)=\begin{pmatrix}0&-r^2&x_1-x_2\\r^2&0&-x_1-x_2\\-x_1+x_2&x_1+x_2&0\end{pmatrix}.}
$$

Adding $PI+\widehat S+\widehat A$ reconstructs every entry of $F$.

Subtracting a scalar multiple of the identity preserves every [eigenvector](../../linear-operator-theory.md#eigenvector): if $Sv=\lambda v$, then $(S-PI)v=(\lambda-P)v$. Thus the [principal axes](../../rigid-body-dynamics.md#principal-axis) are **the same as in part (c)**, with shifted principal values

$$
\boxed{-r^2/3\text{ along }e_r,\qquad-4r^2/3\text{ along }e_\theta,\qquad5r^2/3\text{ along }e_3.}
$$

The two tensors are [coaxial symmetric tensors](../../linear-algebra.md#coaxial-symmetric-tensors). At $r=0$ both vanish, so neither specifies unique axes.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Take downward vertical distances from the support. The climber positions are $q_1=L_1$, $q_2=L_1+L_2$ and $q_3=L_1+L_3$. Their [kinetic energy](../../energy.md#kinetic-energy) is therefore

$$
\boxed{T=\frac12m_1\dot L_1^2+\frac12m_2(\dot L_1+\dot L_2)^2+\frac12m_3(\dot L_1+\dot L_3)^2.}
$$

Integrating the tension-extension relation gives the [elastic potential energy](../../elasticity-physics.md#elastic-energy) $k(L_i-L_0)^2/2$ for each taut rope. Because downward displacement lowers gravitational potential,

$$
\boxed{U=\frac k2\sum_{i=1}^3(L_i-L_0)^2-g\big[(m_1+m_2+m_3)L_1+m_2L_2+m_3L_3\big],\qquad L=T-U.}
$$

An arbitrary additive constant in $U$ is immaterial. This is the vertical-motion model implicit in using only rope lengths as generalized coordinates; swinging angles are not additional degrees of freedom in this model.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

The [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) give

$$
\boxed{\begin{aligned}
(m_1+m_2+m_3)\ddot L_1+m_2\ddot L_2+m_3\ddot L_3+k(L_1-L_0)&=(m_1+m_2+m_3)g,\\
m_2(\ddot L_1+\ddot L_2)+k(L_2-L_0)&=m_2g,\\
m_3(\ddot L_1+\ddot L_3)+k(L_3-L_0)&=m_3g.
\end{aligned}}
$$

For example, differentiating $T$ with respect to $\dot L_1$ collects contributions from all three climbers, because changing $L_1$ moves all of them. At [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), all accelerations vanish, so

$$
\boxed{\widehat L_1=L_0+\frac{(m_1+m_2+m_3)g}{k},\qquad\widehat L_2=L_0+\frac{m_2g}{k},\qquad\widehat L_3=L_0+\frac{m_3g}{k}.}
$$

The top rope supports the total weight, while each lower rope supports only its own climber. These extensions are positive, consistent with the taut-rope tension law.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Set $L_i=\widehat L_i+y_i$. The equilibrium equations cancel the constant gravitational and elastic terms, leaving the [small-oscillation mass and stiffness matrices](../../lagrangian-mechanics.md#small-oscillation-mass-and-stiffness-matrices)

$$
\boxed{M\ddot y+Ky=0,\qquad M=\begin{pmatrix}m_1+m_2+m_3&m_2&m_3\\m_2&m_2&0\\m_3&0&m_3\end{pmatrix},\qquad K=kI_3.}
$$

The off-diagonal mass terms arise because rope-length coordinates are not absolute climber displacements. For any nonzero velocity vector, $\dot y^TM\dot y=m_1\dot y_1^2+m_2(\dot y_1+\dot y_2)^2+m_3(\dot y_1+\dot y_3)^2>0$, so $M$ is a [positive-definite matrix](../../quadratic-form.md#positive-definite-matrix).

Within the vertical Hookean model, the displacement equations are exactly linear while all ropes stay taut. Small amplitudes ensure that none reaches the slack regime $L_i\leq L_0$.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

For equal masses, write $M=mB$ with $B=\left(\begin{smallmatrix}3&1&1\\1&1&0\\1&0&1\end{smallmatrix}\right)$. The [generalized eigenvalue problem for small oscillations](../../lagrangian-mechanics.md#generalized-eigenvalue-problem-for-small-oscillations) is $kv=\omega^2mBv$.

Exchange symmetry of climbers 2 and 3 gives $v_a=(0,1,-1)^T$, for which $Bv_a=v_a$. Hence

$$
\boxed{\omega_a=\sqrt{k/m},\qquad y(t)=A(t)(0,1,-1)^T.}
$$

The physical displacements are $(y_1,y_1+y_2,y_1+y_3)$, so climber 1 is stationary and the other two move vertically with equal amplitudes in opposite directions. Their changes in force on climber 1 cancel.

For the remaining symmetric modes, put $v=(a,b,b)^T$ and let $\mu=k/(m\omega^2)$. The eigenproblem becomes $3a+2b=\mu a$, $a+b=\mu b$. Eliminating $a,b$ gives $(3-\mu)(1-\mu)-2=\mu^2-4\mu+1=0$. Therefore $\mu=2\pm\sqrt3$. Since $(2+\sqrt3)(2-\sqrt3)=1$,

$$
\boxed{\omega_-^2=\frac km(2-\sqrt3),\qquad\omega_+^2=\frac km(2+\sqrt3).}
$$

For clarity, their relative physical climber displacements, rather than rope-length amplitudes, are

$$
q_-\propto\left(1,\frac{1+\sqrt3}{2},\frac{1+\sqrt3}{2}\right),\qquad q_+\propto\left(1,\frac{1-\sqrt3}{2},\frac{1-\sqrt3}{2}\right).
$$

The lower mode moves all climbers in phase; the higher mode moves the lower pair against the top climber. These are the [normal modes of three vertically suspended masses with a branched spring connection](../../lagrangian-mechanics.md#normal-modes-of-three-vertically-suspended-masses-with-a-branched-spring-connection).

<a id="7/d/image-relative-physical-climber-displacements-in-the-three-vertical-normal-modes-branch-spacing-is-schematic"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2-2015-ib-climber-modes.png)

**[Figure 2](#7/d/image-relative-physical-climber-displacements-in-the-three-vertical-normal-modes-branch-spacing-is-schematic). Relative physical climber displacements in the three vertical normal modes; branch spacing is schematic**.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

The left [coset](../../group-theory.md#coset) is

$$
\boxed{gH=\{gh:h\in H\}.}
$$

Every $g\in G$ belongs to $gH$, because $e\in H$, so the cosets cover $G$. If $gH$ and $kH$ intersect, choose $gh_1=kh_2$ in the intersection. Then $k^{-1}g=h_2h_1^{-1}\in H$, so $g=kh$ for some $h\in H$. Thus $gH=khH=kH$.

Hence two left cosets are either identical or disjoint, and the distinct left cosets form a [partition of a set](../../set.md#partition-of-a-set) whose union is $G$. Finiteness is unnecessary for this partition argument. In the finite case each coset has $|H|$ members, since multiplication by $g$ is a [bijection](../../function.md#bijection), giving [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem).

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Denote a matrix by $A(x,y,z)$, with $y$ the upper-right entry. Direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives

$$
\boxed{A(x,y,z)A(x',y',z')=A(x+x',\ y+y'+xz',\ z+z').}
$$

This proves closure. Associativity is inherited from matrix multiplication. The identity is $A(0,0,0)$, and the inverse is

$$
\boxed{A(x,y,z)^{-1}=A(-x,xz-y,-z).}
$$

Both products with this matrix are the identity. Thus these real matrices form the [Heisenberg group](../../lie-algebra.md#heisenberg-group), in the coordinate convention with central coordinate $y$.

Let $N=\{A(0,b,0):b\in\mathbb R\}$. Its multiplication adds $b$, its identity is $b=0$ and its inverse negates $b$, so it is a [subgroup](../../group.md#subgroup). Moreover

$$
A(x,y,z)A(0,b,0)=A(x,y+b,z)=A(0,b,0)A(x,y,z).
$$

Thus every element of $N$ is central, and $gNg^{-1}=N$. Therefore **$N$ is a normal subgroup**. In fact it is the full [center of a group](../../group-theory.md#center-of-a-group), as described by the [center quotient of the real Heisenberg group](../../lie-algebra.md#center-quotient-of-the-real-heisenberg-group).

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Perform the product and inverse formulas from part (b) in the commutative ring $\mathbb Z/4\mathbb Z$. They involve only addition, multiplication and negatives, so closure and inverses remain valid; no division by a nonunit is needed. Associativity again comes from matrix multiplication, and $A(0,0,0)$ remains the identity. The [Heisenberg group over a commutative ring](../../lie-algebra.md#heisenberg-group-over-a-commutative-ring) therefore has

$$
\boxed{|G|=4^3=64.}
$$

These are residues modulo four, not arithmetic in the [finite field](../../algebra.md#finite-field) of four elements.

For the additional subgroup task, write an element of $H$ as $A(t,y,t)$. Its product and inverse are

$$
A(t,y,t)A(s,v,s)=A(t+s,y+v+ts,t+s),\qquad A(t,y,t)^{-1}=A(-t,t^2-y,-t).
$$

Both remain in $H$, and the product is unchanged on exchanging the factors because $ts=st$. The identity is included, so $H$ is an [Abelian subgroup](../../group.md#abelian-subgroup). There are four independent choices each for $t,y$, giving

$$
\boxed{|H|=16,\qquad[G:H]=\frac{64}{16}=4.}
$$

Thus there are four distinct left [cosets](../../group-theory.md#coset). Explicitly the surjective [group homomorphism](../../group-theory.md#group-homomorphism) $A(x,y,z)\mapsto x-z\pmod4$ has kernel $H$; the four cosets are the level sets of that difference, with representatives $A(d,0,0)$, $d=0,1,2,3$. This is the [Abelian plane subgroup of the Heisenberg group modulo four](../../lie-algebra.md#abelian-plane-subgroup-of-the-heisenberg-group-modulo-four).

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

The [kernel of a group homomorphism](../../group-theory.md#kernel-of-a-group-homomorphism) is

$$
\boxed{K=\{g\in G:\Phi(g)=e_{G'}\}.}
$$

The homomorphism sends identity to identity and inverses to inverses. Thus $e_G\in K$, and if $k_1,k_2\in K$, then $\Phi(k_1k_2^{-1})=e_{G'}$, so $K$ is a subgroup by the [subgroup test](../../group.md#subgroup-test).

For any $g\in G$ and $k\in K$,

$$
\Phi(gkg^{-1})=\Phi(g)\Phi(k)\Phi(g)^{-1}=\Phi(g)e_{G'}\Phi(g)^{-1}=e_{G'}.
$$

Hence $gKg^{-1}\subseteq K$. Applying the same inclusion with $g^{-1}$ gives equality, proving

$$
\boxed{K\trianglelefteq G.}
$$

This normality argument does not require either group to be finite.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

The [conjugacy class](../../group-action.md#conjugacy-class) of $g$ is

$$
\boxed{\operatorname{Cl}_G(g)=\{hgh^{-1}:h\in G\}.}
$$

If $N$ is a [normal subgroup](../../group-theory.md#normal-subgroup) and $g\in N$, then normality gives $hgh^{-1}\in N$ for every $h$. Thus the whole conjugacy class of each member of $N$ is contained in $N$, and

$$
\boxed{N=\bigcup_{g\in N}\operatorname{Cl}_G(g).}
$$

Conjugacy classes partition the group, so this is a union of complete disjoint classes, never selected fractions of classes.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

The [cycle type](../../finite-group-theory.md#cycle-type) records the lengths of the disjoint cycles in a [permutation](../../combinatorics.md#permutation), including fixed points as length-one cycles. The possibilities for three objects are

$$
\boxed{\begin{array}{c|c|c}
\text{cycle structure}&\text{elements}&\text{number}\\\hline
1+1+1&e&1\\
2+1&(12),(13),(23)&3\\
3&(123),(132)&2
\end{array}.}
$$

These exhaust the six elements of the [symmetric group](../../finite-group-theory.md#symmetric-group) $S_3$, denoted $\Sigma_3$ in the source. They are also the [conjugacy classes of the symmetric group on three letters](../../group-action.md#conjugacy-classes-of-the-symmetric-group-on-three-letters).

<h3 id="9/d">d</h3>

↑ **Parent:** [9](#9)

<h4 id="9/d/solution">Solution</h4>

↑ **Parent:** [D](#9/d)

The kernel is a [normal subgroup](../../group-theory.md#normal-subgroup), so it contains the identity class and is a union of the classes listed in part (c). Its candidate orders are therefore $1$, $1+3=4$, $1+2=3$ and $1+3+2=6$. [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) excludes four, since it does not divide six. The remaining possibilities are

$$
\boxed{K=\{e\},\qquad K=A_3=\{e,(123),(132)\},\qquad K=S_3.}
$$

All three are normal: the first and last trivially, while $A_3$ is the kernel of the map giving the [sign of a permutation](../../finite-group-theory.md#sign-of-a-permutation), or the index-two subgroup generated by a 3-cycle.

Because $\Phi$ is onto, the [first isomorphism theorem](../../group-theory.md#first-isomorphism-theorem) gives $G'\cong S_3/K$. Explicitly, the map $gK\mapsto\Phi(g)$ is well defined, multiplicative and surjective; equality of its values means $h^{-1}g\in K$, so it is also injective. Thus

$$
\boxed{G'\cong S_3\quad\text{or}\quad C_2\quad\text{or}\quad\{e\}.}
$$

Each is realized by the identity map, the sign map and the trivial map, respectively. This completes the classification of [normal subgroups and quotients of the symmetric group on three letters](../../finite-group-theory.md#normal-subgroups-and-quotients-of-the-symmetric-group-on-three-letters).

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

The table describes the [symmetry group](../../group-action.md#symmetry-group) of a regular [hexagon](../../euclidean-geometry.md#hexagon). Choose $R$ as a counterclockwise rotation through $\pi/3$ and $m_1$ as reflection in one symmetry axis. With $s=m_1$, the relations are

$$
R^6=I,\qquad s^2=I,\qquad sRs=R^{-1}.
$$

The rotation entries already are $I,R,\ldots,R^5$, and the table gives $Rm_j=m_{j+1}$ with indices modulo six. Therefore

$$
\boxed{m_j=R^{j-1}s\quad(j=1,\ldots,6),\qquad G=\{R^k,R^ks:0\leq k<6\}.}
$$

The source writes $D_6$ with the subscript counting polygon vertices; this [dihedral group](../../finite-group-theory.md#dihedral-group) has order 12.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

All six reflections square to the identity, and the rotation $R^3$ is the half-turn. These exhaust the nonidentity involutions: $R^k$ has square one only when $2k\equiv0\pmod6$, giving $k=3$ apart from the identity. Thus the order-two [subgroups](../../group.md#subgroup) are

$$
\boxed{\{I,R^3\},\qquad\{I,m_j\}\quad(j=1,\ldots,6).}
$$

A reflection cannot have order three. The rotations of order three are $R^2$ and $R^4$, and they generate the same subgroup:

$$
\boxed{\{I,R^2,R^4\}=\langle R^2\rangle.}
$$

**All these subgroups are cyclic**, because a group of prime order is cyclic; the displayed nonidentity elements supply their generators. This gives seven subgroups of order two and one of order three, consistently with [involutions in an even dihedral group](../../finite-group-theory.md#involutions-in-an-even-dihedral-group) and the [classification of subgroups of a dihedral group](../../finite-group-theory.md#classification-of-subgroups-of-a-dihedral-group).

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Act on vectors in the plane of the regular hexagon using its actual [rotations](../../riemannian-geometry.md#rotation-mathematics) and [reflections](../../linear-algebra.md#reflection-mathematics). Choose the first reflection axis as the horizontal axis. A [faithful representation](../../representation-theory.md#faithful-representation) is generated by

$$
\boxed{D_2(R)=\begin{pmatrix}1/2&-\sqrt3/2\\\sqrt3/2&1/2\end{pmatrix},\qquad D_2(m_1)=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.}
$$

They are real [orthogonal matrices](../../linear-algebra.md#orthogonal-matrix) obeying $D_2(R)^6=I$, $D_2(m_1)^2=I$ and $D_2(m_1)D_2(R)D_2(m_1)=D_2(R)^{-1}$. Hence they reproduce the group relations. Since $m_2=Rm_1$,

$$
\boxed{D_2(m_2)=\begin{pmatrix}1/2&\sqrt3/2\\\sqrt3/2&-1/2\end{pmatrix}.}
$$

This is reflection in the line at angle $\pi/6$. More generally $D_2(m_j)=D_2(R)^{j-1}D_2(m_1)$. The six rotation matrices are distinct, as are the six reflection matrices; their determinant signs distinguish the two sets. Thus no two group elements have the same matrix, proving faithfulness rather than merely the representation property.

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

Use the left [regular representation](../../representation-theory.md#regular-representation), defined on the ordered basis $(e_I,e_R,\ldots,e_{R^5},e_{m_1},\ldots,e_{m_6})$ by $D_{\rm reg}(g)e_h=e_{gh}$. Reading the $m_4$ row of the original PDF table gives the permutation

$$
(I\ m_4)(R\ m_3)(R^2\ m_2)(R^3\ m_1)(R^4\ m_6)(R^5\ m_5).
$$

Thus an explicit $12\times12$ [permutation matrix](../../vector-space.md#permutation-matrix), in six-by-six blocks, is

$$
\boxed{D_{\rm reg}(m_4)=\begin{pmatrix}0&P\\P&0\end{pmatrix},\qquad P=\begin{pmatrix}0&0&0&1&0&0\\0&0&1&0&0&0\\0&1&0&0&0&0\\1&0&0&0&0&0\\0&0&0&0&0&1\\0&0&0&0&1&0\end{pmatrix}.}
$$

Each column has its one in the row labelled by the left product; this specifies the convention completely. Since $P^2=I_6$, the full matrix squares to $I_{12}$ and is its own inverse. Therefore for every integer, including negative integers,

$$
\boxed{[D_{\rm reg}(m_4)]^n=\begin{cases}I_{12},&n\text{ even},\\D_{\rm reg}(m_4),&n\text{ odd}.\end{cases}}
$$

This is also immediate from $m_4^2=I$ and the multiplication law for a representation.

<h3 id="10/e">e</h3>

↑ **Parent:** [10](#10)

<h4 id="10/e/solution">Solution</h4>

↑ **Parent:** [E](#10/e)

The [character](../../representation-theory.md#character-of-a-representation) is the trace. For the planar representation, the rotation trace and reflection trace give

$$
\boxed{\chi_2(R^k)=2\cos\frac{k\pi}{3},\qquad\chi_2(m_j)=0.}
$$

In the source’s order $(I,R,R^2,R^3,R^4,R^5,m_1,\ldots,m_6)$, these values are $(2,1,-1,-2,-1,1,0,0,0,0,0,0)$.

In the [regular representation](../../representation-theory.md#regular-representation), the trace counts basis vectors fixed by left multiplication. The equation $gh=h$ forces $g=I$, so a nonidentity element fixes none, while the identity fixes all 12. Consequently

$$
\boxed{\chi_{\rm reg}(I)=12,\qquad\chi_{\rm reg}(g)=0\quad(g\ne I).}
$$

In particular $\chi_{\rm reg}(m_4)=0$, consistently with the zero diagonal in part (d). The two characters have different identity values because the representation dimensions are two and twelve.

## ↑ Ancestors (10)

1. [2015](../2015.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
