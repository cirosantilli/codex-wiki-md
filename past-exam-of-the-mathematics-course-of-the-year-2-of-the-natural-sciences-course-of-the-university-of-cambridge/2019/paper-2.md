# Paper 2

↑ **Parent:** [2019](../2019.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2019/papernst_ib_2_2019.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2019/papernst_ib_2_2019.pdf)

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
  - [d](#4/d)
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
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
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
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
  - [d](#10/d)
    - [Solution](#10/d/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A weighted [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator) has the form

$$
\boxed{Ly=\frac1{w(x)}\left[-\frac{d}{dx}\left(p(x)\frac{dy}{dx}\right)+q(x)y\right]},
$$

where $p,q,w$ are real, $p>0$ and $w>0$ in the interval's interior, and the coefficients have the regularity required by the derivatives. The corresponding [eigenvalue equation](../../linear-operator-theory.md#eigenvalue-equation) is $-(py')'+qy=\lambda wy$. Its natural [weighted inner product](../../inner-product.md#weighted-inner-product) is $\langle f,g\rangle_w=\int w f\bar g\,dx$. Suitable endpoint conditions must also annihilate $[p(f\bar g'-f'\bar g)]$ for a [self-adjoint differential operator](../../sturm-liouville-theory.md#self-adjoint-differential-operator); the displayed differential expression alone does not specify those conditions.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Multiplication by a positive weight puts the [differential equation](../../differential-equation.md) into [Sturm-Liouville form](../../sturm-liouville-theory.md#sturm-liouville-form) if $(xw)'=(1-x)w$. Thus $xw'=-xw$, and the constant factor can be chosen so that

$$
\boxed{w(x)=e^{-x}},\qquad -(xe^{-x}y')'=n e^{-x}y.
$$

This fixes the otherwise arbitrary normalization of the weight consistently with the requested unit norms.

Write the [polynomial](../../polynomial.md) as $p_n(x)=\sum_{j=0}^n c_jx^j$. Comparing coefficients gives

$$
(j+1)^2c_{j+1}+(n-j)c_j=0,\qquad c_0=1.
$$

Consequently $c_j=(-1)^j\binom nj/j!$, identifying the solutions as [Laguerre polynomials](../../linear-operator-theory.md#laguerre-polynomial). In particular,

$$
\boxed{p_0=1,\qquad p_1=1-x,\qquad p_2=1-2x+\frac{x^2}{2}}.
$$

Repeated [integration by parts](../../calculus.md#integration-by-parts) gives the moments $\int_0^\infty e^{-x}x^j\,dx=j!$. Therefore

$$
\begin{aligned}
\|p_0\|_w^2&=1,\\
\|p_1\|_w^2&=1-2(1!)+2!=1,\\
\|p_2\|_w^2&=1-4(1!)+5(2!)-2(3!)+\tfrac14(4!)=1.
\end{aligned}
$$

For later use, [integration by parts](../../calculus.md#integration-by-parts) in the weighted [eigenvalue equations](../../linear-operator-theory.md#eigenvalue-equation) also gives

$$
(n-m)\langle p_n,p_m\rangle_w
=\left[xe^{-x}(p_np_m'-p_n'p_m)\right]_0^\infty=0.
$$

The endpoint expression vanishes because of the factor $x$ at zero and exponential decay at infinity. Hence distinct [Laguerre polynomials](../../linear-operator-theory.md#laguerre-polynomial) are orthogonal, an instance of [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The optimal approximation is the [orthogonal projection](../../hilbert-space.md#orthogonal-projection) onto the [linear span](../../vector-space.md#linear-span) of $p_0,\ldots,p_N$. Their [orthogonality](../../inner-product.md#orthogonal-vectors) gives

$$
\left\|f-\sum_{n=0}^N a_np_n\right\|_w^2
=\|f\|_w^2-2\sum_{n=0}^N a_n\langle f,p_n\rangle_w
+\sum_{n=0}^N a_n^2\|p_n\|_w^2.
$$

Completing each square proves both optimality and uniqueness:

$$
\boxed{a_n=\frac{\langle f,p_n\rangle_w}{\|p_n\|_w^2}}.
$$

For real $f$, these are real coefficients. If complex-valued $f$ is allowed while the coefficients remain real, replace the numerator by its real part and use the modulus-squared norm. The question's real formulation corresponds to real $f$.

Here the first three squared norms are one. Using $\int_0^\infty x^j e^{-2x}\,dx=j!/2^{j+1}$,

$$
\begin{aligned}
a_0&=\int_0^\infty e^{-2x}(1+x)\,dx=\frac12+\frac14=\frac34,\\
a_1&=\int_0^\infty e^{-2x}(1-x^2)\,dx=\frac12-\frac14=\frac14,\\
a_2&=\int_0^\infty e^{-2x}\left(1-x-\frac32x^2+\frac12x^3\right)dx
=\frac12-\frac14-\frac38+\frac3{16}=\frac1{16}.
\end{aligned}
$$

Thus

$$
\boxed{(a_0,a_1,a_2)=\left(\frac34,\frac14,\frac1{16}\right),\qquad
f_2(x)=\frac{17}{16}-\frac38x+\frac1{32}x^2}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The coefficient formula from part (b) and the [Leibniz rule](../../calculus.md#leibniz-rule) yield [Rodrigues' formula](../../orthogonal-polynomial.md#rodrigues-formula) directly:

$$
p_n(x)=\sum_{j=0}^n\frac{(-1)^j}{j!}\binom njx^j
=\frac{e^x}{n!}\frac{d^n}{dx^n}(e^{-x}x^n).
$$

The leading coefficient is $(-1)^n/n!$, so $p_n^{(n)}=(-1)^n$. Substitute this differentiated expression into one factor in the squared [weighted norm](../../inner-product.md#weighted-norm) and apply [integration by parts](../../calculus.md#integration-by-parts) $n$ times:

$$
\begin{aligned}
\|p_n\|_w^2
&=\frac1{n!}\int_0^\infty p_n(x)\frac{d^n}{dx^n}(e^{-x}x^n)\,dx\\
&=\frac{(-1)^n}{n!}\int_0^\infty e^{-x}x^n p_n^{(n)}(x)\,dx
=\frac1{n!}\int_0^\infty e^{-x}x^n\,dx
=\boxed{1}.
\end{aligned}
$$

Every endpoint term contains a derivative of $e^{-x}x^n$ of order less than $n$: it vanishes at zero, and its exponential decay beats every [polynomial](../../polynomial.md) at infinity. This proves the [normalization of the ordinary Laguerre polynomials](../../linear-operator-theory.md#normalization-of-the-ordinary-laguerre-polynomials) for all $n$, including $n=0$ without any integrations by parts.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a separated [axisymmetric harmonic function](../../partial-differential-equation.md#axisymmetric-harmonic-function) $\Psi=R(r)\Theta(\theta)$, multiplying the [Laplace equation](../../partial-differential-equation.md#laplace-equation) by $r^2/(R\Theta)$ gives

$$
\frac{(r^2R')'}{R}
=-\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}=\lambda.
$$

The two sides depend on different variables, hence both equal a constant. Put $u=\cos\theta$ in the angular equation. Since $\sin\theta\,\Theta'=-\sin^2\theta\,d\Theta/du$, it becomes the [Legendre differential equation](../../linear-ordinary-differential-equation.md#legendre-differential-equation)

$$
\frac{d}{du}\left[(1-u^2)\frac{d\Theta}{du}\right]+\lambda\Theta=0.
$$

Regularity on both parts of the polar axis restricts $\lambda=\ell(\ell+1)$, with $\ell=0,1,\ldots$, and selects the [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) $P_\ell(u)$. The other angular solution is singular at an endpoint.

The radial [Euler differential equation](../../linear-ordinary-differential-equation.md#cauchy-euler-equation) is

$$
r^2R''+2rR'-\ell(\ell+1)R=0.
$$

Trying $R=r^s$ gives $s(s+1)=\ell(\ell+1)$, so $s=\ell$ or $s=-\ell-1$. [Superposition](../../vector-space.md#superposition-principle) of these separated [harmonic functions](../../partial-differential-equation.md#harmonic-function) gives

$$
\boxed{\Psi(r,\theta)=\sum_{\ell=0}^\infty
\left(A_\ell r^\ell+B_\ell r^{-\ell-1}\right)P_\ell(\cos\theta)}.
$$

The [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial) form the angular expansion for regular data with [rotational symmetry](../../linear-algebra.md#rotational-symmetry) about the polar axis; the radial domain and the [boundary conditions](../../differential-equation.md#boundary-condition) determine which coefficients survive and where the expansion converges.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

With $u=\cos\theta$, the boundary data have the finite [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) expansion

$$
-2+2u+3u^2=-P_0(u)+2P_1(u)+2P_2(u).
$$

Inside the sphere, every $r^{-\ell-1}$ term is singular at the origin and must be absent. Matching at $r=a$ therefore gives

$$
\boxed{\Psi_{\mathrm{in}}(r,\theta)
=-1+2\frac ra\cos\theta+\frac{r^2}{a^2}(3\cos^2\theta-1)}.
$$

In the exterior, decay at infinity excludes all $r^\ell$ terms, including the constant term at $\ell=0$. Thus

$$
\boxed{\Psi_{\mathrm{out}}(r,\theta)
=-\frac ar+2\frac{a^2}{r^2}\cos\theta
+\frac{a^3}{r^3}(3\cos^2\theta-1)}.
$$

Both [harmonic functions](../../partial-differential-equation.md#harmonic-function) have the prescribed [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition), and each is finite throughout its own domain. The interior expression is regular even at the origin because $r\cos\theta=z$ and $r^2(3\cos^2\theta-1)=2z^2-x^2-y^2$. [Uniqueness of the Dirichlet problem](../../analysis.md#uniqueness-of-the-dirichlet-problem) identifies these as the respective solutions. Their normal derivatives need not match: the two [Dirichlet problems](../../analysis.md#dirichlet-problem) do not require a single [harmonic function](../../partial-differential-equation.md#harmonic-function) across the bounding sphere.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the sign convention in which a [fundamental solution of the Laplace equation](../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation) satisfies

$$
\Delta_{\mathbf r}G(\mathbf r,\mathbf r')=\delta^{(2)}(\mathbf r-\mathbf r')
$$

in the sense of [distributions](../../distribution-theory.md#distribution-mathematical-analysis). It is a [harmonic function](../../partial-differential-equation.md#harmonic-function) away from the source. Writing $\rho=|\mathbf r-\mathbf r'|$, the radial equation is $(\rho G')'=0$, so $G=A\log\rho+B$. The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) on a small circle about the source fixes its total flux:

$$
1=\int_{\rho<\varepsilon}\Delta G\,d^2r
=\int_{\rho=\varepsilon}\partial_\rho G\,ds
=\frac A\varepsilon(2\pi\varepsilon)=2\pi A.
$$

Consequently

$$
\boxed{G(\mathbf r,\mathbf r')=\frac1{2\pi}\log|\mathbf r-\mathbf r'|+B}.
$$

The arbitrary constant is a [harmonic function](../../partial-differential-equation.md#harmonic-function). For the alternative convention $-\Delta G=\delta^{(2)}$, the logarithm has the opposite sign; subsequent [Green's function](../../green-s-function.md) formulas must use that convention consistently.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [Dirichlet Green function](../../green-s-function.md#dirichlet-green-function) satisfies $\Delta_{\mathbf x}G_D(\mathbf x,\mathbf y)=\delta^{(2)}(\mathbf x-\mathbf y)$ in the domain and $G_D=0$ when $\mathbf x$ lies on its boundary. For a source $\mathbf y\ne0$ in the [unit disc](../../topology.md#unit-disc), put its opposite image at $\mathbf y^*=\mathbf y/|\mathbf y|^2$. The [method of images](../../mathematics.md#method-of-images) gives

$$
\boxed{G_D(\mathbf x,\mathbf y)
=\frac1{2\pi}\log\frac{|\mathbf x-\mathbf y|}{|\mathbf y|\,|\mathbf x-\mathbf y^*|}}.
$$

The image lies outside the [unit disc](../../topology.md#unit-disc), so its logarithm is a [harmonic function](../../partial-differential-equation.md#harmonic-function) inside. The original logarithm has precisely the unit source strength found in part (a). On $|\mathbf x|=1$,

$$
|\mathbf x-\mathbf y|^2
=1-2\mathbf x\cdot\mathbf y+|\mathbf y|^2
=|\mathbf y|^2|\mathbf x-\mathbf y^*|^2,
$$

so the boundary value is zero. Equivalently, in [complex coordinates](../../complex-analysis.md#complex-coordinate), the [Dirichlet Green function inside the unit disk](../../green-s-function.md#dirichlet-green-function-inside-the-unit-disk) is

$$
G_D(z,\zeta)=\frac1{2\pi}\log\left|\frac{z-\zeta}{1-z\bar\zeta}\right|.
$$

This also covers a source at the origin, where $G_D(z,0)=(2\pi)^{-1}\log|z|$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Fix the observation point $\mathbf x$ and apply [Green's second identity](../../partial-differential-equation.md#green-second-identity) in the source variable $\mathbf y$. Since $\Delta u=0$, $\Delta_{\mathbf y}G_D=\delta_{\mathbf x}$ and $G_D=0$ on the boundary, it gives

$$
u(\mathbf x)=\int_D(u\Delta G_D-G_D\Delta u)\,d^2y
=\int_{\partial D}f(\mathbf y)\partial_{n_{\mathbf y}}G_D(\mathbf x,\mathbf y)\,ds_{\mathbf y}.
$$

The identity can be justified by deleting a small circle about $\mathbf x$ and letting its radius tend to zero; the logarithmic flux contributes $u(\mathbf x)$.

Set $\mathbf x=(r,\phi)$ and $\mathbf y=(\rho,\phi')$, and write $c=\cos(\phi-\phi')$. The symmetric expression for the [Green's function](../../green-s-function.md) is

$$
G_D=\frac1{4\pi}\log\frac{r^2+\rho^2-2r\rho c}{1+r^2\rho^2-2r\rho c}.
$$

At the boundary, the outward [normal derivative](../../differential-geometry.md#normal-derivative) is $\partial_\rho$ at $\rho=1$, and hence

$$
\left.\partial_\rho G_D\right|_{\rho=1}
=\frac1{4\pi}\frac{(2-2rc)-(2r^2-2rc)}{1+r^2-2rc}
=\frac1{2\pi}\frac{1-r^2}{1-2rc+r^2}.
$$

Since $ds=d\phi'$ on the [unit circle](../../complex-analysis.md#complex-unit-circle), the [Poisson integral on the unit disk](../../partial-differential-equation.md#poisson-integral-on-the-unit-disk) follows, with [Poisson kernel](../../partial-differential-equation.md#poisson-kernel)

$$
\boxed{P(r,\vartheta)=\frac{1-r^2}{1-2r\cos\vartheta+r^2}},\qquad
u(r,\phi)=\frac1{2\pi}\int_0^{2\pi}f(\phi')P(r,\phi-\phi')\,d\phi'.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

At the origin, the [Poisson kernel](../../partial-differential-equation.md#poisson-kernel) is one, so the [mean value property for harmonic functions](../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) gives

$$
u(0)=\frac1{2\pi}\int_0^{2\pi}f(\phi')\,d\phi'.
$$

For $0<r<1$, the denominator in the [Poisson kernel](../../partial-differential-equation.md#poisson-kernel) satisfies $1-2r\cos\vartheta+r^2\geq(1-r)^2$. Thus

$$
0<P(r,\vartheta)\leq\frac{1-r^2}{(1-r)^2}=\frac{1+r}{1-r}.
$$

The nonnegativity of $f$ allows this upper bound to be inserted under the [Poisson integral on the unit disk](../../partial-differential-equation.md#poisson-integral-on-the-unit-disk):

$$
\boxed{u(r,\phi)\leq\frac{1+r}{1-r}\,u(0)}.
$$

This is the upper bound in the [Harnack inequality on the unit disk](../../partial-differential-equation.md#harnack-inequality-on-the-unit-disk). The same argument with the minimum of the [Poisson kernel](../../partial-differential-equation.md#poisson-kernel) gives the corresponding lower bound $(1-r)u(0)/(1+r)$.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In the [Laurent series](../../analysis.md#laurent-series)

$$
f(z)=\sum_{j=-m}^{\infty}c_j(z-z_0)^j,\qquad 0<|z-z_0|<R,
$$

about a [pole](../../isolated-singularity.md#pole) of order $m$, the [residue](../../analysis.md#residue) is the coefficient

$$
\boxed{\operatorname{Res}_{z=z_0}f=c_{-1}}
=\frac1{2\pi i}\oint_{|z-z_0|=\rho}f(z)\,dz,\qquad 0<\rho<R,
$$

where the circle is traversed anticlockwise. Equivalently, the [residue](../../analysis.md#residue) is $\frac1{(m-1)!}\left.\frac{d^{m-1}}{dz^{m-1}}[(z-z_0)^mf(z)]\right|_{z=z_0}$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Taylor series](../../calculus.md#taylor-series) of the [entire function](../../holomorphic-function.md#entire-function) $g$ gives

$$
\frac{g(z)}{z-z_0}=\frac{g(z_0)}{z-z_0}+g'(z_0)+O(z-z_0).
$$

The coefficient of $(z-z_0)^{-1}$, and therefore the [residue](../../analysis.md#residue), is

$$
\boxed{\operatorname{Res}_{z=z_0}\frac{g(z)}{z-z_0}=g(z_0)}.
$$

If $g(z_0)=0$, the apparent [pole](../../isolated-singularity.md#pole) is a [removable singularity](../../isolated-singularity.md#removable-singularity) and the [residue](../../analysis.md#residue) is zero.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For the simple-contour form of the [residue theorem](../../analysis.md#residue-theorem), let $C$ be a positively oriented, simple, closed, piecewise smooth [contour](../../complex-analysis.md#complex-integration-contour). Assume $f$ is [holomorphic](../../holomorphic-function.md) on a neighbourhood of $C$ and its interior except at finitely many isolated singularities $z_1,\ldots,z_s$, all strictly inside $C$, with none on $C$. Then

$$
\oint_C f(z)\,dz=2\pi i\sum_{j=1}^s\operatorname{Res}_{z=z_j}f.
$$

The more general version weights each [residue](../../analysis.md#residue) by the contour's [winding number](../../complex-analysis.md#winding-number), with the usual requirement that the contour be homologous to zero in the domain of analyticity containing it and the nonsingular region.

For the requested application, assume $f$ is [holomorphic](../../holomorphic-function.md) on a neighbourhood of the contour and its closed interior, and $z_0$ is strictly inside it. Its [Taylor series](../../calculus.md#taylor-series) shows

$$
\frac{f(z)}{(z-z_0)^2}
=\frac{f(z_0)}{(z-z_0)^2}+\frac{f'(z_0)}{z-z_0}+O(1).
$$

Only the second term contributes a [residue](../../analysis.md#residue). The [residue theorem](../../analysis.md#residue-theorem) therefore proves the derivative form of the [Cauchy integral formula](../../analysis.md#cauchy-integral-formula):

$$
\boxed{\frac1{2\pi i}\oint_C\frac{f(z)}{(z-z_0)^2}\,dz=f'(z_0)}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

Close the real segment $[-R,R]$ by an anticlockwise semicircle in the upper half-plane. For $F(z)=1/[(z^2+1)(z^2+4)]$, the [contour integral](../../complex-analysis.md#contour-integral) over the arc is $O(R^{-3})$: its length is $\pi R$, whereas $|z^2+1|\geq R^2-1$ and $|z^2+4|\geq R^2-4$. The enclosed [simple poles](../../isolated-singularity.md#simple-pole) are $i$ and $2i$, with [residues](../../analysis.md#residue)

$$
\operatorname{Res}_{i}F=\frac1{(2i)(i^2+4)}=\frac1{6i},\qquad
\operatorname{Res}_{2i}F=\frac1{(4i)((2i)^2+1)}=-\frac1{12i}.
$$

Letting $R\to\infty$ in the [residue theorem](../../analysis.md#residue-theorem) yields

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{(x^2+1)(x^2+4)}
=2\pi i\left(\frac1{6i}-\frac1{12i}\right)=\frac\pi6}.
$$

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

Use $z=e^{i\theta}$, so $\sin\theta=(z-z^{-1})/(2i)$ and $d\theta=dz/(iz)$. The [unit circle](../../complex-analysis.md#complex-unit-circle) is traversed anticlockwise, and the integral becomes

$$
\oint_{|z|=1}\frac{2\,dz}{-3z^2+10iz+3}
=\oint_{|z|=1}\frac{2\,dz}{-3(z-i/3)(z-3i)}.
$$

Only the [simple pole](../../isolated-singularity.md#simple-pole) $z=i/3$ lies inside the [contour](../../complex-analysis.md#complex-integration-contour). Its [residue](../../analysis.md#residue) is

$$
\frac{2}{-6(i/3)+10i}=\frac1{4i}.
$$

Hence the [residue theorem](../../analysis.md#residue-theorem) gives

$$
\boxed{\int_0^{2\pi}\frac{d\theta}{5-3\sin\theta}=2\pi i\frac1{4i}=\frac\pi2}.
$$

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $a=s+ib$ with real $s,b$, and first translate the real integration variable by $s$. It remains to integrate $e^{-z^2}$ along the horizontal line $\operatorname{Im}z=b$.

For $b>0$, apply the [Cauchy integral theorem](../../complex-analysis.md#cauchy-s-integral-theorem) to the rectangle with vertices $-R,R,R+ib,-R+ib$. The [integrand](../../integral.md#integrand) is an [entire function](../../holomorphic-function.md#entire-function), so

$$
\int_{-R}^{R}e^{-x^2}\,dx-\int_{-R}^{R}e^{-(x+ib)^2}\,dx
$$

is the negative of the two vertical-edge integrals. On either vertical edge, $z=\pm R+iy$ and

$$
|e^{-z^2}|=e^{-R^2+y^2}\leq e^{-R^2+b^2}.
$$

Their combined absolute value is at most $2b e^{-R^2+b^2}$ and tends to zero. The rectangle below the real axis gives the same estimate with $|b|$ when $b<0$; $b=0$ needs no deformation. Absolute convergence follows from $|e^{-(x+ib)^2}|=e^{b^2}e^{-x^2}$. Taking $R\to\infty$ proves the [Gaussian contour translation](../../complex-analysis.md#gaussian-contour-translation) identity

$$
\boxed{\int_{-\infty}^{\infty}e^{-(u+a)^2}\,du=\sqrt\pi,\qquad a\in\mathbb C}.
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Take $\lambda>0$ and $t>0$, the [positive diffusivity requirement for the forward heat kernel](../../diffusion-equation.md#positive-diffusivity-requirement-for-the-forward-heat-kernel). The PDF does not explicitly specify the sign of $\lambda$; the stated real [Gaussian function](../../calculus.md#gaussian-function) formula requires this assumption. For a direct calculation, initially assume sufficiently smooth and rapidly decreasing data, so that the [Fourier transform](../../fourier-transform.md), its inverse and the following integrations are justified. The resulting [heat-kernel convolution](../../diffusion-equation.md#heat-kernel-convolution) extends to wider classes of initial data.

Using the stated [Fourier transform](../../fourier-transform.md) convention and [integration by parts](../../calculus.md#integration-by-parts),

$$
\widetilde{u_{xx}}(k,t)=-k^2\widetilde u(k,t),\qquad
\partial_t\widetilde u=-\lambda k^2\widetilde u.
$$

The transformed [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) has solution $\widetilde u(k,t)=e^{-\lambda k^2t}\widetilde u_0(k)$. [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) then gives

$$
u(x,t)=\int_{-\infty}^{\infty}u_0(y)K_t(x-y)\,dy,\qquad
K_t(s)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{-\lambda tk^2+iks}\,dk.
$$

Complete the square:

$$
-\lambda tk^2+iks
=-\lambda t\left(k-\frac{is}{2\lambda t}\right)^2-\frac{s^2}{4\lambda t}.
$$

Part (a), after scaling by $\sqrt{\lambda t}$, evaluates the remaining [Gaussian integral](../../integral.md#gaussian-integral) even though its shift is imaginary. Therefore

$$
K_t(s)=\frac{e^{-s^2/(4\lambda t)}}{\sqrt{4\pi\lambda t}},\qquad
\boxed{u(x,t)=\frac1{\sqrt{4\pi\lambda t}}\int_{-\infty}^{\infty}
e^{-(x-y)^2/(4\lambda t)}u(y,0)\,dy}.
$$

The [heat kernel](../../diffusion-equation.md#heat-kernel) has integral one and is an [approximate identity](../../fourier-analysis.md#approximate-identity) as $t\downarrow0$, which recovers the initial condition. Mere decay at spatial infinity does not by itself imply every Fourier integral is absolutely convergent; the regularity assumption above supplies a rigorous setting for the derivation.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Put $s=\lambda t>0$. In the [heat-kernel convolution](../../diffusion-equation.md#heat-kernel-convolution), complete the real square as

$$
\alpha^2y^2+\frac{(x-y)^2}{4s}
=\left(\alpha^2+\frac1{4s}\right)
\left(y-\frac{x}{1+4s\alpha^2}\right)^2
+\frac{\alpha^2x^2}{1+4s\alpha^2}.
$$

The [Gaussian integral](../../integral.md#gaussian-integral) therefore gives

$$
\boxed{\beta=\frac{\alpha}{\sqrt{1+4\lambda t\alpha^2}},\qquad
u(x,t)=\frac{\beta}{\sqrt\pi}e^{-\beta^2x^2}}.
$$

At $t=0$ the same formula gives $\beta=\alpha$. Equivalently, $\beta^{-2}=\alpha^{-2}+4\lambda t$: the [variance](../../variance.md) of this normalized [Gaussian function](../../calculus.md#gaussian-function) grows from $1/(2\alpha^2)$ to $1/(2\alpha^2)+2\lambda t$.

The initial profiles have unit integral and concentrate at zero as $\alpha\to\infty$. Precisely, for every smooth compactly supported [test function](../../distribution-theory.md#test-function) $\varphi$,

$$
\int_{\mathbb R}\frac{\alpha}{\sqrt\pi}e^{-\alpha^2y^2}\varphi(y)\,dy
=\frac1{\sqrt\pi}\int_{\mathbb R}e^{-v^2}\varphi(v/\alpha)\,dv
\longrightarrow\varphi(0).
$$

Thus the limit is the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function), rather than an ordinary function: pointwise the profiles tend to zero away from the origin and diverge at the origin. At every fixed $t>0$,

$$
\boxed{u(\cdot,0)\longrightarrow\delta_0\ \text{in distributions},\qquad
u(x,t)\longrightarrow\frac1{\sqrt{4\pi\lambda t}}e^{-x^2/(4\lambda t)}}.
$$

The limiting evolved profile is the [heat kernel](../../diffusion-equation.md#heat-kernel) for a unit point source.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

An order-$n$ Cartesian [tensor](../../multilinear-algebra.md#tensor) has $3^n$ components whose values in two orthonormal Cartesian frames satisfy

$$
T'_{i_1\ldots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\ldots j_n},\qquad R^TR=I,
$$

with repeated indices summed as in [Einstein notation](../../multilinear-algebra.md#einstein-notation). It is an [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor) when its components are unchanged by every proper [rotation](../../riemannian-geometry.md#rotation-mathematics), $R\in SO(3)$.

For rank two, a half-turn about any coordinate axis changes the sign of each component having exactly one index along that axis. Invariance therefore makes every off-diagonal component zero. Quarter-turns interchanging two coordinate axes then require $T_{11}=T_{22}=T_{33}$. Thus, without assuming symmetry in advance,

$$
\boxed{T_{ij}=a\delta_{ij}}.
$$

Conversely, the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta) is invariant because $R_{ik}R_{jk}=\delta_{ij}$, so every tensor of this form is isotropic.

For rank three the general proper-rotation invariant form is

$$
\boxed{T_{ijk}=b\epsilon_{ijk}},
$$

where $\epsilon_{ijk}$ is the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol). The convention matters: the [isotropic rank-three tensor and reflections](../../multilinear-algebra.md#isotropic-rank-three-tensor-and-reflections) distinction says that invariance of a polar [tensor](../../multilinear-algebra.md#tensor) under all $R\in O(3)$ would force $b=0$. A nonzero $\epsilon_{ijk}$ is invariant under proper [rotations](../../riemannian-geometry.md#rotation-mathematics), and is a [pseudotensor](../../multilinear-algebra.md#pseudotensor) under the full orthogonal group. The shell integrals below are invariant under reflections as well, so their odd moments vanish.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

Introduce the second moment [tensor](../../multilinear-algebra.md#tensor) $M_{ij}=\int_Vx_ix_j\,d^3x$. The [spherical shell](../../euclidean-geometry.md#spherical-shell) is preserved by every [rotation](../../riemannian-geometry.md#rotation-mathematics), so this is an [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor), $M_{ij}=A\delta_{ij}$. Its [trace](../../linear-algebra.md#matrix-trace) determines the constant:

$$
3A=M_{ii}=\int_Vr^2\,d^3x
=4\pi\int_{R_1}^{R_2}r^4\,dr
=\frac{4\pi}{5}(R_2^5-R_1^5).
$$

Contracting with the components of the two unit [vectors](../../vector-space.md#vector) gives

$$
\boxed{\int_V(\mathbf x\cdot\mathbf n_1)(\mathbf x\cdot\mathbf n_2)\,d^3x
=\frac{4\pi}{15}(R_2^5-R_1^5)(\mathbf n_1\cdot\mathbf n_2)}.
$$

This is the second-order case of [radial tensor moments in three dimensions](../../geometry-and-topology.md#radial-tensor-moments-in-three-dimensions).

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Under inversion $\mathbf x\mapsto-\mathbf x$, the [spherical shell](../../euclidean-geometry.md#spherical-shell) and its volume element are unchanged, while the product of three [scalar products](../../inner-product.md#dot-product) changes sign. Its integral is therefore its own negative:

$$
\boxed{\int_V(\mathbf x\cdot\mathbf n_1)(\mathbf x\cdot\mathbf n_2)
(\mathbf x\cdot\mathbf n_3)\,d^3x=0}.
$$

Equivalently, its rank-three moment [tensor](../../multilinear-algebra.md#tensor) is completely symmetric and cannot have a nonzero multiple of the antisymmetric [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol).

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

Let $M_{ijkl}=\int_Vx_ix_jx_kx_l\,d^3x$. It is an [isotropic tensor](../../multilinear-algebra.md#isotropic-tensor) and is invariant under every permutation of its four indices. Thus the three coefficients in the general rank-four isotropic form must coincide:

$$
M_{ijkl}=C(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

A double [tensor contraction](../../multilinear-algebra.md#tensor-contraction) gives

$$
15C=M_{iijj}=\int_Vr^4\,d^3x
=4\pi\int_{R_1}^{R_2}r^6\,dr
=\frac{4\pi}{7}(R_2^7-R_1^7).
$$

Here the three contracted [Kronecker delta](../../multilinear-algebra.md#kronecker-delta) products contribute $9$, $3$ and $3$. Contracting instead with the four unit [vectors](../../vector-space.md#vector) yields

$$
\boxed{\begin{aligned}
&\int_V\prod_{a=1}^4(\mathbf x\cdot\mathbf n_a)\,d^3x\\
&\quad=\frac{4\pi}{105}(R_2^7-R_1^7)
\big[(\mathbf n_1\cdot\mathbf n_2)(\mathbf n_3\cdot\mathbf n_4)
+(\mathbf n_1\cdot\mathbf n_3)(\mathbf n_2\cdot\mathbf n_4)
+(\mathbf n_1\cdot\mathbf n_4)(\mathbf n_2\cdot\mathbf n_3)\big].
\end{aligned}}
$$

This agrees with subtracting two instances of the [isotropic fourth moment of a ball](../../multilinear-algebra.md#isotropic-fourth-moment-of-a-ball).

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

For an ordinary conservative mechanical system, choose [generalized coordinates](../../lagrangian-mechanics.md#generalized-coordinate) $q_i$ measured from a static [equilibrium point](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). Assume the [kinetic energy](../../energy.md#kinetic-energy) is quadratic in velocities and there are no velocity-dependent forces. Expanding about equilibrium, the linear term in the [potential energy](../../energy.md#potential-energy) vanishes. Retaining only terms of total degree two gives the [small oscillation](../../lagrangian-mechanics.md#small-oscillation) [Lagrangian](../../calculus-of-variations.md#lagrangian)

$$
\boxed{L=\frac12\dot{\mathbf q}^{\,T}M\dot{\mathbf q}-\frac12\mathbf q^TK\mathbf q},\qquad
M_{ij}=\left.\frac{\partial^2T}{\partial\dot q_i\partial\dot q_j}\right|_0,\quad
K_{ij}=\left.\frac{\partial^2V}{\partial q_i\partial q_j}\right|_0.
$$

An irrelevant constant has been dropped. Coordinate dependence of $M$ contributes only terms of third or higher total degree. The matrices $M,K$ are symmetric, $M$ is positive definite for independent coordinates, and $K$ is positive semidefinite at a [stable equilibrium](../../dynamical-systems.md#stable-equilibrium). The [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) are

$$
\boxed{M\ddot{\mathbf q}+K\mathbf q=0}.
$$

A [normal mode](../../wave-equation.md#normal-mode) has a fixed [mode shape](../../wave-equation.md#mode-shape) $\mathbf v$ and one time factor: $\mathbf q=\mathbf v Q(t)$. Its [angular frequency](../../lagrangian-mechanics.md#angular-frequency) $\omega$ solves the [generalized eigenvalue problem](../../linear-operator-theory.md#generalized-eigenvalue-problem) $K\mathbf v=\omega^2M\mathbf v$, with $\ddot Q+\omega^2Q=0$. Thus $\omega$ is the normal angular frequency, and the frequency in cycles per unit time is $\omega/(2\pi)$. A [zero mode](../../linear-operator-theory.md#zero-mode) satisfies $K\mathbf v=0$; its time dependence is $Q=A+Bt$, describing an unopposed displacement or uniform drift rather than a restoring oscillation.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Label the equal [masses](../../classical-mechanics.md#mass) $1,2$ and the mass $2m$ by $3$, in cyclic order. Let their equilibrium angles be $0,2\pi/3,4\pi/3$, with angular displacements $q_1,q_2,q_3$. Because the hoop has unit radius, its three arc lengths are

$$
\ell_1=\frac{2\pi}{3}+q_2-q_1,\quad
\ell_2=\frac{2\pi}{3}+q_3-q_2,\quad
\ell_3=\frac{2\pi}{3}+q_1-q_3.
$$

The [springs](../../elasticity-physics.md#spring) themselves are constrained to the hoop, so these are arc lengths. If their common natural length is $\ell_0$, [Hooke's law](../../elasticity-physics.md#hooke-s-law) gives $V=\frac k2\sum_i(\ell_i-\ell_0)^2$. Since the arc lengths have fixed sum $2\pi$, all terms linear in the $q_i$ cancel. Dropping the constant,

$$
\boxed{T=\frac m2(\dot q_1^2+\dot q_2^2+2\dot q_3^2),\qquad
V-V_0=\frac k2\big[(q_2-q_1)^2+(q_3-q_2)^2+(q_1-q_3)^2\big]}.
$$

Thus the unspecified common natural length does not affect the motion. The mass and restoring matrices in the [generalized eigenvalue problem](../../linear-operator-theory.md#generalized-eigenvalue-problem) are

$$
M=m\begin{pmatrix}1&0&0\\0&1&0\\0&0&2\end{pmatrix},\qquad
K=k\begin{pmatrix}2&-1&-1\\-1&2&-1\\-1&-1&2\end{pmatrix}.
$$

Exchange of the two equal [masses](../../classical-mechanics.md#mass) separates symmetric and antisymmetric [normal modes](../../wave-equation.md#normal-mode). Direct multiplication gives the complete set

$$
\boxed{\begin{array}{c|c}
\text{mode shape}&\omega^2\\ \hline
(1,1,1)&0\\
(1,-1,0)&3k/m\\
(1,1,-1)&2k/m
\end{array}}.
$$

The first is rigid [rotation](../../riemannian-geometry.md#rotation-mathematics) of all three beads: every arc length stays fixed, giving a [zero mode](../../linear-operator-theory.md#zero-mode). In the second, the equal [masses](../../classical-mechanics.md#mass) move oppositely while the heavy bead stays fixed; the net force on that bead cancels. In the third, the equal [masses](../../classical-mechanics.md#mass) move together and the heavy bead moves oppositely with equal angular amplitude. Both nonzero [normal modes](../../wave-equation.md#normal-mode) have zero total [angular momentum](../../momentum.md#angular-momentum). These are the [normal modes of three beads connected by springs on a circular hoop](../../lagrangian-mechanics.md#normal-modes-of-three-beads-connected-by-springs-on-a-circular-hoop) with $M=2m$.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Use the [mode shapes](../../wave-equation.md#mode-shape) from part (b), and put $\omega=\sqrt{2k/m}$. The initial [velocity](../../classical-mechanics.md#velocity) decomposes as

$$
(0,0,\Omega)=\frac\Omega2(1,1,1)-\frac\Omega2(1,1,-1).
$$

There is no antisymmetric component because the initial state treats the equal [masses](../../classical-mechanics.md#mass) identically. Initial displacements are zero, so the [zero mode](../../linear-operator-theory.md#zero-mode) contributes a linear drift and the nonzero [normal mode](../../wave-equation.md#normal-mode) contributes a sine:

$$
\mathbf q(t)=\frac{\Omega t}{2}(1,1,1)
-\frac{\Omega}{2\omega}\sin(\omega t)(1,1,-1).
$$

In terms of actual angular positions,

$$
\boxed{\begin{aligned}
\theta_1(t)&=\frac\Omega2\left(t-\frac{\sin\omega t}{\omega}\right),\\
\theta_2(t)&=\frac{2\pi}{3}+\frac\Omega2\left(t-\frac{\sin\omega t}{\omega}\right),\\
\theta_3(t)&=\frac{4\pi}{3}+\frac\Omega2\left(t+\frac{\sin\omega t}{\omega}\right),\qquad
\omega=\sqrt{\frac{2k}{m}}.
\end{aligned}}
$$

The conserved [angular momentum](../../momentum.md#angular-momentum) is initially $2m\Omega$ and the total [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia) is $4m$, so the common [angular velocity](../../rigid-body-dynamics.md#angular-velocity) must be $\Omega/2$, agreeing with the drift. The relative displacements remain of order $\Omega/\omega$, even when the common angle becomes large. Hence small $\Omega/\omega$ preserves the cyclic ordering and small spring extensions at arbitrarily late times. In the ideal arc-spring model the displayed energies are exactly quadratic in the relative angles, so this motion remains exact while that ordering persists.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

A [group](../../group.md) is a set $G$ equipped with a binary operation satisfying the [group axioms](../../group.md#group-axioms): closure; [associativity](../../algebraic-operation.md#associative-property), $(gh)k=g(hk)$; an [identity element](../../algebraic-operation.md#identity-element) $e$ with $eg=ge=g$; and an [inverse element](../../algebraic-operation.md#inverse-element) $g^{-1}$ for every $g$, with $gg^{-1}=g^{-1}g=e$.

A [subgroup](../../group.md#subgroup) $H$ is a subset that is a [group](../../group.md) under the restricted operation. Equivalently, it is nonempty and contains $xy^{-1}$ whenever $x,y\in H$. A [generating set of a group](../../group.md#generating-set-of-a-group) is a set whose elements and inverses can be multiplied in finite words to produce every group element.

The [group order](../../group.md#order-of-a-finite-group) is its number of elements, $|G|$. The [order of a group element](../../group-theory.md#order-of-a-group-element) $g$ is the least positive integer $r$ with $g^r=e$, or infinity if there is none. [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem) states that for a finite [group](../../group.md) and [subgroup](../../group.md#subgroup) $H$, $|H|$ divides $|G|$ and $|G|=[G:H]|H|$. In particular, every finite element order divides the [group order](../../group.md#order-of-a-finite-group).

A [cyclic group](../../group.md#cyclic-group) is generated by one element, so every element is a power of that generator. A [group isomorphism](../../algebra.md#group-isomorphism) is a bijective [group homomorphism](../../group-theory.md#group-homomorphism): a bijection $\phi:G\to G'$ satisfying $\phi(gh)=\phi(g)\phi(h)$ for all $g,h$.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

By [Lagrange's theorem](../../group-theory.md#lagrange-s-theorem), the possible values of the [order of a group element](../../group-theory.md#order-of-a-group-element) are

$$
\boxed{1,2,4,8}.
$$

These are possibilities across groups of order eight; they need not all occur in one group.

If every element has order at most two, every element equals its own inverse. Thus for any $x,y$,

$$
xy=(xy)^{-1}=y^{-1}x^{-1}=yx,
$$

so $G$ is an [abelian group](../../group.md#abelian-group). Choose $a\ne e$, and then $b\notin\langle a\rangle$. The four elements $e,a,b,ab$ are distinct and form a [subgroup](../../group.md#subgroup) $H$: commutativity and $a^2=b^2=e$ prove closure and inverses. Choose $c\notin H$. The elements of $H$ and $Hc$ are disjoint, since $hc\in H$ would imply $c\in H$. These two four-element sets therefore exhaust $G$.

Every element consequently has a unique expression $a^ib^jc^k$, with $i,j,k\in\{0,1\}$. The map from triples to these products is bijective and respects multiplication by addition of exponents modulo two. Hence

$$
\boxed{G\cong C_2\times C_2\times C_2},
$$

a [direct product of groups](../../group-theory.md#direct-product-of-groups) and an [elementary abelian group](../../group.md#elementary-abelian-group).

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

The [cyclic subgroup](../../group.md#cyclic-subgroup) $A=\langle a\rangle$ has order four and index two. Every index-two [subgroup](../../group.md#subgroup) is normal: its complement is both the only nontrivial left [coset](../../group-theory.md#coset) and the only nontrivial right [coset](../../group-theory.md#coset). Thus [conjugation](../../group-action.md#conjugation) by $b$ is an [automorphism](../../algebra.md#automorphism) of $A$. It must send its generator $a$ to another element of order four, namely $a$ or $a^3$. Since $b^{-1}=b$,

$$
bab=a\quad\text{or}\quad bab=a^3,
$$

equivalently $ab=ba$ or $ab=ba^3$, as required. Also $b\notin A$, since otherwise $a,b$ could generate at most four elements.

In the commuting case, every word reduces uniquely to $a^jb^\varepsilon$ with $0\leq j<4$ and $\varepsilon\in\{0,1\}$. The eight expressions are distinct because $A$ and $Ab$ are disjoint. Multiplication is addition of the two exponents modulo four and two, respectively. Therefore

$$
\boxed{G\cong C_4\times C_2}.
$$

This gives the [multiplication table](../../arithmetic.md#multiplication-table) independently of any other properties of $G$, proving uniqueness up to [group isomorphism](../../algebra.md#group-isomorphism).

In the inversion case, the relation $ba=a^{-1}b$ gives the same eight unique normal forms, now with multiplication

$$
(a^ib^\varepsilon)(a^jb^\eta)
=a^{i+(-1)^\varepsilon j}b^{\varepsilon+\eta},
$$

with exponents reduced modulo four and two. Thus this case also has a uniquely determined [group](../../group.md) structure. A faithful geometric realization is the [dihedral group](../../finite-group-theory.md#dihedral-group) of a square, with $a$ a quarter-turn and $b$ a reflection in a line through opposite edge midpoints. For example, on the plane,

$$
a=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
b=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

These preserve the square with vertices $(\pm1,\pm1)$ and satisfy $a^4=b^2=I$, $bab=a^{-1}$. They generate eight distinct transformations, so

$$
\boxed{G\cong D_4\quad\text{(the symmetry group of a square, of order eight)}}.
$$

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

**No.** The [quaternion group](../../finite-group-theory.md#quaternion-group)

$$
Q_8=\{1,-1,i,-i,j,-j,k,-k\},\qquad
i^2=j^2=k^2=ijk=-1,
$$

is another [non-abelian group](../../group.md#non-abelian-group) of order eight: for example $ij=k$ while $ji=-k$. Its multiplication comes from the associative [quaternion](../../algebra-over-a-field.md#quaternion) algebra, so it does define a [group](../../group.md).

It is not [isomorphic](../../algebra.md#isomorphism) to the [dihedral group](../../finite-group-theory.md#dihedral-group) of the square. In $Q_8$, only $-1$ has order two; the six elements $\pm i,\pm j,\pm k$ have order four. The square's [dihedral group](../../finite-group-theory.md#dihedral-group) has five elements of order two: four reflections and the half-turn. [Group isomorphisms](../../algebra.md#group-isomorphism) preserve element orders, so these groups are distinct. The hypothesis in part (c) excludes $Q_8$, since its only element of order two is already in each cyclic subgroup of order four.

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

A [group homomorphism](../../group-theory.md#group-homomorphism) $f:G\to G'$ satisfies $f(gh)=f(g)f(h)$ for all $g,h\in G$. It consequently sends the [identity element](../../algebraic-operation.md#identity-element) to the identity and inverses to inverses. Its [group homomorphism kernel](../../group-theory.md#kernel-of-a-group-homomorphism) is

$$
\boxed{\ker f=\{g\in G:f(g)=e_{G'}\}}.
$$

A [normal subgroup](../../group-theory.md#normal-subgroup) $H$ of $G$ is a [subgroup](../../group.md#subgroup) invariant under [conjugation](../../group-action.md#conjugation):

$$
\boxed{gHg^{-1}=H\quad\text{for every }g\in G}.
$$

Equivalently, $gH=Hg$ for every $g$, so left and right [cosets](../../group-theory.md#coset) coincide.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

Write $M(a,b)=\begin{pmatrix}a&b\\0&1\end{pmatrix}$. Direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives

$$
M(a,b)M(c,d)=M(ac,ad+b).
$$

Since $a,c\ne0$, the product is again in $G$. [Associativity](../../algebraic-operation.md#associative-property) is inherited from [matrix multiplication](../../vector-space.md#matrix-multiplication), the [identity element](../../algebraic-operation.md#identity-element) is $M(1,0)$, and

$$
M(a,b)^{-1}=M(a^{-1},-b/a)
$$

lies in $G$. These verify all [group axioms](../../group.md#group-axioms). This is the [Affine group of the complex line](../../group-theory.md#affine-group-of-the-complex-line), acting by $z\mapsto az+b$.

For the diagonal subset, $M(a,0)M(c,0)=M(ac,0)$, it contains $M(1,0)$, and $M(a,0)^{-1}=M(a^{-1},0)$. Thus $G'$ is a [subgroup](../../group.md#subgroup). Finally,

$$
f(M(a,b)M(c,d))=M(ac,0)
=M(a,0)M(c,0)=f(M(a,b))f(M(c,d)),
$$

so **$f:G\to G'$ is a surjective [group homomorphism](../../group-theory.md#group-homomorphism)**.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

The [kernel of a group homomorphism](../../group-theory.md#kernel-of-a-group-homomorphism) found in part (b) is the translation subgroup

$$
\boxed{N=\ker f=\left\{T_c=\begin{pmatrix}1&c\\0&1\end{pmatrix}:c\in\mathbb C\right\}}.
$$

It is a [subgroup](../../group.md#subgroup) because $T_cT_d=T_{c+d}$, $T_0=I$ and $T_c^{-1}=T_{-c}$. It is nontrivial since $T_1\ne I$, and proper since, for example, $M(2,0)\notin N$.

Every kernel is a [normal subgroup](../../group-theory.md#normal-subgroup): if $n\in\ker f$, then $f(gng^{-1})=f(g)e f(g)^{-1}=e$. Applying the same argument with $g^{-1}$ gives equality of the conjugate subgroup and the kernel. Here one can also check invariance under [conjugation](../../group-action.md#conjugation) directly:

$$
M(a,b)T_cM(a,b)^{-1}=T_{ac}.
$$

Multiplication by nonzero $a$ permutes all $c\in\mathbb C$, so $M(a,b)NM(a,b)^{-1}=N$. Thus $N$ is a nontrivial proper [normal subgroup](../../group-theory.md#normal-subgroup), [isomorphic](../../algebra.md#isomorphism) to the additive [group](../../group.md) $(\mathbb C,+)$.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

The [symmetric group](../../finite-group-theory.md#symmetric-group) $S_n$ consists of all bijections of $\{1,\ldots,n\}$, with composition as its operation; its [group order](../../group.md#order-of-a-finite-group) is $n!$.

An $m$-dimensional complex [group representation](../../representation-theory.md#group-representation) of $G$ is a [group homomorphism](../../group-theory.md#group-homomorphism) $\rho:G\to GL(V)$, where $V$ is an $m$-dimensional complex [vector space](../../vector-space.md). After a choice of [basis](../../vector-space.md#basis), each $\rho(g)$ is an invertible $m\times m$ complex [matrix](../../vector-space.md#matrix), with $\rho(gh)=\rho(g)\rho(h)$.

An [irreducible representation](../../representation-theory.md#irreducible-representation) has $V\ne0$ and no invariant [vector subspace](../../vector-space.md#vector-subspace) other than $\{0\}$ and $V$. Two [group representations](../../representation-theory.md#group-representation) $\rho$ on $V$ and $\sigma$ on $W$ are [isomorphic representations](../../representation-theory.md#isomorphic-representations) if there exists an invertible [linear map](../../vector-space.md#linear-map) $S:V\to W$ such that $S\rho(g)=\sigma(g)S$ for every $g$. They are inequivalent if no such map exists; in equal-dimensional [matrix](../../vector-space.md#matrix) form this says no fixed change of [basis](../../vector-space.md#basis) conjugates every $\rho(g)$ to $\sigma(g)$.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

In a [symmetric group](../../finite-group-theory.md#symmetric-group), two [permutations](../../combinatorics.md#permutation) are in the same [conjugacy class](../../group-action.md#conjugacy-class) exactly when they have the same [cycle type](../../finite-group-theory.md#cycle-type). For $S_4$ the five possibilities and their sizes are

$$
\boxed{\begin{array}{c|c|c}
\text{cycle type}&\text{representative}&\text{class size}\\ \hline
1^4&e&1\\
2\,1^2&(12)&6\\
2^2&(12)(34)&3\\
3\,1&(123)&8\\
4&(1234)&6
\end{array}}.
$$

There are $\binom42=6$ [transpositions](../../combinatorics.md#transposition-permutation), three pairings into two unordered pairs, $\binom43(3-1)!=8$ three-cycles, and $(4-1)!=6$ four-cycles. Together with the identity these counts sum to $24=|S_4|$.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

The two [one-dimensional representations](../../representation-theory.md#one-dimensional-representation) are the [trivial representation](../../representation-theory.md#trivial-representation), $\rho_+(g)=1$, and the [sign representation](../../representation-theory-of-the-symmetric-group.md#sign-representation), $\rho_-(g)=\operatorname{sgn}(g)$. The first respects multiplication immediately. For the second, the [sign of a permutation](../../finite-group-theory.md#sign-of-a-permutation) is the [determinant](../../multilinear-algebra.md#determinant) of its [permutation matrix](../../vector-space.md#permutation-matrix), and multiplicativity of the [determinant](../../multilinear-algebra.md#determinant) proves $\rho_-(gh)=\rho_-(g)\rho_-(h)$. They are inequivalent since a [transposition](../../combinatorics.md#transposition-permutation) has images $1$ and $-1$, and conjugation by a nonzero scalar cannot change a one-dimensional matrix.

Their [group homomorphism kernels](../../group-theory.md#kernel-of-a-group-homomorphism) are

$$
\boxed{\ker\rho_+=S_4,\qquad \ker\rho_-=A_4}.
$$

Both are [subgroups](../../group.md#subgroup), indeed [normal subgroups](../../group-theory.md#normal-subgroup), because they are kernels. In the second case $A_4$ is the [alternating group](../../finite-group-theory.md#alternating-group) of even [permutations](../../combinatorics.md#permutation), with twelve elements.

The [characters](../../representation-theory.md#character-of-a-representation) are their scalar values, since the [trace](../../linear-algebra.md#matrix-trace) of a one-dimensional matrix is its only entry. In the class order from part (b),

$$
\chi_+=(1,1,1,1,1),\qquad \chi_-=(1,-1,1,1,-1).
$$

The [character inner product](../../representation-theory.md#character-inner-product) is the group average of $\chi_+\overline{\chi_-}$, so

$$
\boxed{\langle\chi_+,\chi_-\rangle
=\frac1{24}(1-6+3+8-6)=0}.
$$

Each has squared norm $(1+6+3+8+6)/24=1$, in agreement with [character orthogonality](../../representation-theory.md#character-orthogonality) for distinct [irreducible representations](../../representation-theory.md#irreducible-representation).

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

For a finite [group](../../group.md) over $\mathbb C$, the number of inequivalent [irreducible representations](../../representation-theory.md#irreducible-representation) is its number of [conjugacy classes](../../group-action.md#conjugacy-class), and the [sum of squares of irreducible representation dimensions](../../representation-theory.md#sum-of-squares-of-irreducible-representation-dimensions) equals the [group order](../../group.md#order-of-a-finite-group). There are therefore five irreducibles for $S_4$, with squared dimensions summing to $24$.

First establish that part (c) found every [one-dimensional representation](../../representation-theory.md#one-dimensional-representation). In such a representation, conjugate elements have the same scalar image. All [transpositions](../../combinatorics.md#transposition-permutation) are conjugate and square to the identity, so they all have one common image $s$ with $s^2=1$. [Transpositions](../../combinatorics.md#transposition-permutation) generate $S_4$, hence $s=1$ gives exactly the [trivial representation](../../representation-theory.md#trivial-representation), while $s=-1$ gives exactly the [sign representation](../../representation-theory-of-the-symmetric-group.md#sign-representation). There are precisely two degree-one irreducibles.

The other three dimensions $d_1,d_2,d_3$ are integers at least two and satisfy

$$
d_1^2+d_2^2+d_3^2=24-1-1=22.
$$

No one of them can be at least four, since $4^2+2^2+2^2=24>22$. They are therefore all two or three. Starting from three twos gives sum of squares $12$; each replacement of a two by a three adds $5$. To reach $22$ requires exactly two replacements. Thus the complete list is

$$
\boxed{1,\ 1,\ 2,\ 3,\ 3}.
$$

The count of [conjugacy classes](../../group-action.md#conjugacy-class) guarantees that these are all the inequivalent complex [irreducible representations](../../representation-theory.md#irreducible-representation), not just dimensions of a proposed incomplete list.

## ↑ Ancestors (10)

1. [2019](../2019.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
