# Paper 1

↑ **Parent:** [2025](../2025.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2025/papernst_ib_1_2025.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2025/papernst_ib_1_2025.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
    - [iv](#5/b/iv)
      - [Solution](#5/b/iv/solution)
    - [v](#5/b/v)
      - [Solution](#5/b/v/solution)
    - [vi](#5/b/vi)
      - [Solution](#5/b/vi/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [i](#6/d/i)
      - [Solution](#6/d/i/solution)
    - [ii](#6/d/ii)
      - [Solution](#6/d/ii/solution)
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

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use [Einstein summation convention](../../multilinear-algebra.md#einstein-notation), writing $\partial_j=\partial/\partial x_j$. The [contraction of two Levi-Civita symbols](../../multivariable-calculus.md#contraction-of-two-levi-civita-symbols) gives

$$
\begin{aligned}
[\nabla\times(\mathbf a\times\mathbf b)]_i
&=\epsilon_{ijk}\partial_j(\epsilon_{klm}a_lb_m)\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j(a_lb_m)\\
&=\partial_j(a_ib_j-a_jb_i)\\
&=a_i\partial_jb_j-b_i\partial_ja_j+b_j\partial_ja_i-a_j\partial_jb_i.
\end{aligned}
$$

The last equality is the [product rule](../../calculus.md#product-rule). Recognizing the [divergences](../../multivariable-calculus.md#divergence) and [directional derivatives](../../multivariable-calculus.md#directional-derivative) proves the [curl of a cross product](../../multivariable-calculus.md#curl-of-a-cross-product) identity:

$$
\boxed{\nabla\times(\mathbf a\times\mathbf b)=\mathbf a(\nabla\cdot\mathbf b)-\mathbf b(\nabla\cdot\mathbf a)+(\mathbf b\cdot\nabla)\mathbf a-(\mathbf a\cdot\nabla)\mathbf b.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) states that, for a continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) $\mathbf H$ on a bounded region $V$ with piecewise smooth boundary $S$ and outward [unit normal](../../differential-geometry.md#unit-normal) $\hat{\mathbf n}$,

$$
\int_V\nabla\cdot\mathbf H\,dV=\int_S\mathbf H\cdot\hat{\mathbf n}\,dS.
$$

To apply it, first derive the [divergence of a cross product](../../multivariable-calculus.md#divergence-of-a-cross-product) using the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) and the [product rule](../../calculus.md#product-rule):

$$
\begin{aligned}
\nabla\cdot(\mathbf F\times\mathbf G)
&=\epsilon_{ijk}\partial_i(F_jG_k)\\
&=\epsilon_{ijk}(\partial_iF_j)G_k+\epsilon_{ijk}F_j\partial_iG_k\\
&=\mathbf G\cdot(\nabla\times\mathbf F)-\mathbf F\cdot(\nabla\times\mathbf G).
\end{aligned}
$$

In the second term the minus sign comes from interchanging the first two indices of the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol). The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) with $\mathbf H=\mathbf F\times\mathbf G$ now yields

$$
\boxed{\int_V[\mathbf G\cdot(\nabla\times\mathbf F)-\mathbf F\cdot(\nabla\times\mathbf G)]\,dV=\int_S(\mathbf F\times\mathbf G)\cdot\hat{\mathbf n}\,dS.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Close the [hyperboloid](../../differential-geometry.md#hyperboloid) segment with the two disks at $z=\pm1$, and let $V$ be its interior. The [flux](../../mathematical-physics.md#flux) through either disk is zero because $A_z=0$. Thus the desired [surface integral](../../multivariable-calculus.md#surface-integral) is the total outward [flux](../../mathematical-physics.md#flux) through the closed boundary. Since

$$
\nabla\cdot\mathbf A=3x^2+3y^2,
$$

the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) and [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system) give

$$
\begin{aligned}
\int_{\widetilde S}\mathbf A\cdot\hat{\mathbf n}\,dS
&=\int_{-1}^1\int_0^{2\pi}\int_0^{\sqrt{1+z^2}}3r^2\,r\,dr\,d\theta\,dz\\
&=\frac{3\pi}{2}\int_{-1}^1(1+z^2)^2\,dz\\
&=\frac{3\pi}{2}\left(2+\frac43+\frac25\right)
=\boxed{\frac{28\pi}{5}}.
\end{aligned}
$$

The extra factor $r$ is the [volume integral](../../multivariable-calculus.md#volume-integral) measure in [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system); omitting it would give the wrong [flux](../../mathematical-physics.md#flux).

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For [separation of variables](../../partial-differential-equation.md#separation-of-variables), take $n=T(t)X(x)Y(y)Z(z)$ and divide the [reaction-diffusion equation](../../diffusion-equation.md#reaction-diffusion-system) by this product wherever it is nonzero:

$$
\frac{T'}{\mu T}-\frac\gamma\mu=\frac{X''}{X}+\frac{Y''}{Y}+\frac{Z''}{Z}.
$$

Each spatial term depends on a different variable and must be constant. Write $X''=-k_x^2X$ and similarly for the other two factors. The [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) give $X(0)=X(L)=0$. A zero separation constant permits only a linear function and hence the zero solution; a positive value of $X''/X$ likewise permits no nonzero function vanishing at both endpoints. The nontrivial choices are therefore

$$
\boxed{X_p(x)=\sin\frac{p\pi x}{L},\quad Y_q(y)=\sin\frac{q\pi y}{L},\quad Z_r(z)=\sin\frac{r\pi z}{L},\qquad p,q,r=1,2,\ldots.}
$$

The temporal [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) is

$$
T'_{p,q,r}=\left[\gamma-\frac{\mu\pi^2}{L^2}(p^2+q^2+r^2)\right]T_{p,q,r},
$$

so, absorbing its constant multiplier into $a_{p,q,r}$,

$$
\boxed{T_{p,q,r}(t)=\exp\left\{\left[\gamma-\frac{\mu\pi^2}{L^2}(p^2+q^2+r^2)\right]t\right\}.}
$$

The [superposition principle](../../vector-space.md#superposition-principle) and completeness of the [Fourier sine series](../../fourier-series.md#fourier-sine-series) give the stated threefold expansion with these factors. For an initial density $n_0$, [orthogonality](../../inner-product.md#orthogonal-vectors) also determines the constants:

$$
a_{p,q,r}=\frac8{L^3}\int_0^L\int_0^L\int_0^L n_0(x,y,z)\sin\frac{p\pi x}{L}\sin\frac{q\pi y}{L}\sin\frac{r\pi z}{L}\,dx\,dy\,dz.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The fastest temporal growth occurs for the lowest spatial [eigenvalue](../../linear-operator-theory.md#eigenvalue), with $p=q=r=1$. Its growth rate is

$$
s_{111}=\gamma-\frac{3\mu\pi^2}{L^2}.
$$

For a generic initial condition its coefficient is nonzero, so this term determines the long-time behavior. In fact, every nonzero, nonnegative initial density has $a_{111}>0$, since the product of the three first sine [eigenfunctions](../../linear-operator-theory.md#eigenfunction) is strictly positive in the interior. Consequently

$$
\boxed{L_{\mathrm{crit}}=\pi\sqrt{\frac{3\mu}{\gamma}},\qquad \text{exponential growth precisely when }L>L_{\mathrm{crit}}.}
$$

For $L<L_{\mathrm{crit}}$ every term decays. At equality the first term is stationary and all higher terms decay: equality does not produce exponential growth. This is a [reaction-diffusion equation](../../diffusion-equation.md#reaction-diffusion-system) threshold arising from competition between production and loss through the [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [separation of variables](../../partial-differential-equation.md#separation-of-variables) solution with [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) on the cuboid is

$$
\boxed{n=\sum_{p,q,r\geq1}a_{p,q,r}\sin\frac{p\pi x}{\lambda L}\sin\frac{q\pi\sqrt\lambda\,y}{L}\sin\frac{r\pi\sqrt\lambda\,z}{L}\exp\left\{\left[\gamma-\frac{\mu\pi^2}{L^2}\left(\frac{p^2}{\lambda^2}+\lambda q^2+\lambda r^2\right)\right]t\right\}.}
$$

The constants are fixed by the initial density through [Fourier sine series](../../fourier-series.md#fourier-sine-series). The fastest term again has $p=q=r=1$. When $L=2L_{\mathrm{crit}}$, its growth rate becomes

$$
s_{111}=\gamma\left[1-\frac1{12}(\lambda^{-2}+2\lambda)\right].
$$

Thus the precise condition for no exponentially growing term is

$$
\boxed{\lambda^{-2}+2\lambda\geq12,\qquad\text{equivalently }2\lambda^3-12\lambda^2+1\geq0,\quad\lambda>0.}
$$

For example, $\lambda=1/4$ gives $\lambda^{-2}+2\lambda=33/2>12$, while $\lambda=6$ gives $12+1/36>12$: either a sufficiently flat or a sufficiently elongated cuboid suppresses growth despite its unchanged volume. The function $\lambda^{-2}+2\lambda$ decreases to its minimum $3$ at $\lambda=1$, then increases without bound. Hence there are two positive threshold values, with growth only between them; equality leaves one stationary term and all other terms decaying.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The homogeneous [linear differential equation](../../differential-equation.md#linear-differential-equation) can be written in [divergence form](../../analysis.md#divergence-form):

$$
(x^{n+1}u')'=0.
$$

One integration gives $u'=C x^{-n-1}$. Therefore the two cases are

$$
\boxed{u_h(x)=A+B x^{-n}\quad(n\ne0),\qquad u_h(x)=A+B\log x\quad(n=0).}
$$

In each case the displayed functions have [linear independence](../../vector-space.md#linear-independence) throughout the interval. Imposing both homogeneous [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) forces $A=B=0$: for $n\ne0$, $2^n\ne1$, and for $n=0$, $\log2\ne0$. This also establishes uniqueness for the inhomogeneous [boundary value problem](../../boundary-value-problem.md).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose the convention $L_xG(x,s)=\delta(x-s)$, where $\delta$ is the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function), together with $G(1/2,s)=G(1,s)=0$. The [Green's function](../../green-s-function.md) is continuous at $x=s$ and obeys

$$
\partial_xG(s^+,s)-\partial_xG(s^-,s)=1.
$$

These conditions follow by integrating its [differential equation](../../differential-equation.md) across $s$; continuity prevents a derivative of the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function). If $\ell$ and $r$ are homogeneous solutions satisfying the left and right [boundary conditions](../../differential-equation.md#boundary-condition), respectively, and $W=\ell r'-\ell'r$ is their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian), then

$$
G(x,s)=\frac{\ell(x_<)r(x_>)}{W(s)},\qquad x_<=\min(x,s),\quad x_>=\max(x,s).
$$

For $n\ne0$ take $\ell(x)=x^{-n}-2^n$ and $r(x)=x^{-n}-1$. Their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is $W(s)=n(2^n-1)s^{-n-1}$, and hence

$$
\boxed{G_n(x,s)=\frac{s^{n+1}(x_<^{-n}-2^n)(x_>^{-n}-1)}{n(2^n-1)},\qquad n\ne0.}
$$

For $n=0$ take $\ell(x)=\log(2x)$ and $r(x)=\log x$, giving $W(s)=\log2/s$ and

$$
\boxed{G_0(x,s)=\frac{s}{\log2}\log(2x_<)\log x_>.}
$$

Both formulas satisfy the endpoint conditions, continuity, and the unit jump directly. The unique solution of the [boundary value problem](../../boundary-value-problem.md) is

$$
\boxed{u(x)=\int_{1/2}^1G_n(x,s)f(s)\,ds.}
$$

The factor $s^{n+1}$ in the first formula matters: this [Green's function](../../green-s-function.md) is for the original monic [differential operator](../../analysis.md#differential-operator), with ordinary measure $ds$, rather than for the operator multiplied by $x^{n+1}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $n\ne0$, split the [Green's function](../../green-s-function.md) integral at $s=x$. Writing $\ell(x)=x^{-n}-2^n$ and $r(x)=x^{-n}-1$ gives

$$
u(x)=\frac{r(x)\int_{1/2}^{x}(1-2^ns^n)\,ds+\ell(x)\int_x^1(1-s^n)\,ds}{n(2^n-1)}.
$$

For $n\ne-1$, the two [integrals](../../integral.md) are

$$
I_1=x-\frac12-\frac{2^n}{n+1}\left(x^{n+1}-2^{-n-1}\right),\qquad I_2=1-x-\frac{1-x^{n+1}}{n+1}.
$$

Substitution and simplification yield

$$
\boxed{u(x)=\frac1{n+1}\left[x-1+\frac{x^{-n}-1}{2(2^n-1)}\right],\qquad n\ne0,-1.}
$$

At $x=1$ both contributions vanish. At $x=1/2$ the bracket is $-1/2+(2^n-1)/[2(2^n-1)]=0$. The [differential operator](../../analysis.md#differential-operator) kills $x^{-n}-1$ and sends $x/(n+1)$ to $1/x$, so this also verifies the inhomogeneous equation.

The exceptional integer is $\boxed{n=-1}$, because then the [integrals](../../integral.md) contain $s^{-1}$. In this case

$$
I_1=x-\frac12-\frac12\log(2x),\qquad I_2=1-x+\log x,
$$

and the [Green's function](../../green-s-function.md) integral becomes

$$
\begin{aligned}
u(x)&=2\left[(x-1)\left(x-\frac12-\frac12\log(2x)\right)+\left(x-\frac12\right)(1-x+\log x)\right]\\
&=\boxed{x\log x+(1-x)\log2}.
\end{aligned}
$$

Here $L=d^2/dx^2$, and $u''=1/x$. Explicitly $u(1)=0$ and $u(1/2)=-(\log2)/2+(\log2)/2=0$. Thus both exceptional and nonexceptional formulas satisfy the required [boundary conditions](../../differential-equation.md#boundary-condition).

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Assume first that $f$ and $g$ are [integrable functions](../../measure-theory.md#lebesgue-integrable-function), so that [Fubini's theorem](../../measure-theory.md#fubini-s-theorem) justifies changing the order of the two [integrals](../../integral.md). In the defining [Fourier transform](../../fourier-transform.md) of the [convolution](../../fourier-analysis.md#convolution), put $y=x-x'$:

$$
\begin{aligned}
\widetilde h(k)
&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}f(x-x')g(x')\,dx'\,dx\\
&=\int_{\mathbb R}\int_{\mathbb R}e^{-ik(y+x')}f(y)g(x')\,dy\,dx'\\
&=\left(\int_{\mathbb R}e^{-iky}f(y)\,dy\right)\left(\int_{\mathbb R}e^{-ikx'}g(x')\,dx'\right).
\end{aligned}
$$

This proves the [convolution theorem](../../fourier-analysis.md#convolution-theorem) with the stated normalization:

$$
\boxed{\widetilde h(k)=\widetilde f(k)\widetilde g(k).}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Direct evaluation of the [Fourier transform](../../fourier-transform.md) gives, for $k\ne0$,

$$
\widetilde g(k)=\int_{-1}^1e^{-ikx}\,dx=\frac{e^{ik}-e^{-ik}}{ik}=\boxed{\frac{2\sin k}{k}}.
$$

At $k=0$ the defining [integral](../../integral.md) is the interval length, so $\boxed{\widetilde g(0)=2}$. This also equals the continuous limit of the displayed formula.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [convolution](../../fourier-analysis.md#convolution) $(g*g)(x)$ is the length of the overlap of $(-1,1)$ with $(x-1,x+1)$. This overlap has length $2-|x|$ when $|x|<2$ and zero otherwise, so $u=g*g$. The [convolution theorem](../../fourier-analysis.md#convolution-theorem) now gives

$$
\boxed{\widetilde u(k)=\widetilde g(k)^2=\frac{4\sin^2 k}{k^2},\qquad \widetilde u(0)=4.}
$$

The value at zero is also the area of the [triangular function](../../fourier-analysis.md#triangular-function), providing a normalization check on its [Fourier transform](../../fourier-transform.md).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [Translation property of the Fourier transform](../../fourier-analysis.md#translation-property-of-the-fourier-transform) gives

$$
\begin{aligned}
\widetilde r(k)&=\widetilde u(k)\sum_{n=1}^4e^{ik(4n-10)}\\
&=\frac{4\sin^2k}{k^2}\left(e^{-6ik}+e^{-2ik}+e^{2ik}+e^{6ik}\right)\\
&=\boxed{\frac{16\sin^2k}{k^2}\cos(4k)\cos(2k)},\qquad \boxed{\widetilde r(0)=16}.
\end{aligned}
$$

For the remaining [integral](../../integral.md), the same [Translation property of the Fourier transform](../../fourier-analysis.md#translation-property-of-the-fourier-transform) identifies $e^{20ik'}\widetilde g(k')$ as the [Fourier transform](../../fourier-transform.md) of $g(x+20)$. By the product form of the [convolution theorem](../../fourier-analysis.md#convolution-theorem), with inverse normalization $1/(2\pi)$,

$$
\int_{\mathbb R}e^{20ik'}\widetilde g(k')\widetilde r(k-k')\,dk'=2\pi\,\mathcal F\{g(x+20)r(x)\}(k).
$$

But $g(x+20)$ is supported in $[-21,-19]$, whereas the four translated [triangular functions](../../fourier-analysis.md#triangular-function) making up $r$ are all supported in $[-8,8]$. Their product is identically zero. Therefore the requested [integral](../../integral.md) is $\boxed{0}$ for every real $k$.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [matrix](../../vector-space.md#matrix) sending the standard [basis](../../vector-space.md#basis) vectors to the given columns is

$$
\boxed{U=\frac1{\sqrt6}\begin{pmatrix}\sqrt3&-i\sqrt3&0\\1&i&-2\\1+i&-1+i&1+i\end{pmatrix}.}
$$

With the [Hermitian inner product](../../linear-algebra.md#hermitian-inner-product), the squared column [norms](../../normed-vector-space.md#norm) are $3/6+1/6+2/6=1$, $3/6+1/6+2/6=1$, and $4/6+2/6=1$. The off-diagonal products are

$$
\begin{aligned}
\mathbf u_1^\dagger\mathbf u_2&=\frac{-3i+i+(1-i)(-1+i)}6=0,\\
\mathbf u_1^\dagger\mathbf u_3&=\frac{-2+(1-i)(1+i)}6=0,\\
\mathbf u_2^\dagger\mathbf u_3&=\frac{2i+(-1-i)(1+i)}6=0.
\end{aligned}
$$

Thus the columns form an [orthonormal basis](../../inner-product.md#orthonormal-basis), so $\boxed{U^\dagger U=I}$ and $U$ is a [unitary matrix](../../linear-operator-theory.md#unitary-matrix). Here the operation maps the old [basis](../../vector-space.md#basis) vectors to the new vectors; the inverse coordinate [change of basis](../../linear-algebra.md#change-of-basis) uses $U^\dagger$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

The [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) reverses the order of [matrix multiplication](../../vector-space.md#matrix-multiplication). Since $A$ and $B$ are [Hermitian matrices](../../hilbert-space.md#hermitian-operator),

$$
(AB)^\dagger=B^\dagger A^\dagger=BA.
$$

Consequently $\boxed{AB\text{ is Hermitian}\ \Longleftrightarrow\ AB=BA}$: the condition is exactly that the two [matrices](../../vector-space.md#matrix) [commute](../../algebraic-operation.md#commuting-elements).

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Take $\boxed{c=1}$. Indeed the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) is

$$
(AB+BA)^\dagger=BA+AB=AB+BA,
$$

so the [anticommutator](../../vector-space.md#anticommutator) is a [Hermitian matrix](../../hilbert-space.md#hermitian-operator). The original PDF, p. 6, supplies the factor $BA$ that is corrupted in the local OCR.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

Using the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) and the [Hermitian matrix](../../hilbert-space.md#hermitian-operator) assumptions,

$$
\boxed{(ABA)^\dagger=A^\dagger B^\dagger A^\dagger=ABA.}
$$

Thus $ABA$ is a [Hermitian matrix](../../hilbert-space.md#hermitian-operator), whether or not $A$ and $B$ [commute](../../algebraic-operation.md#commuting-elements).

<h4 id="5/b/iv">iv</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/b/iv)

Put $D=A-iB$, so $D^\dagger=A+iB$. Because the [Hermitian matrices](../../hilbert-space.md#hermitian-operator) $A,B$ [commute](../../algebraic-operation.md#commuting-elements),

$$
D^\dagger D=DD^\dagger=A^2+B^2.
$$

For every nonzero [vector](../../vector-space.md#vector) $v$,

$$
v^\dagger(A^2+B^2)v=\|Av\|^2+\|Bv\|^2>0,
$$

since $A$ is an [invertible matrix](../../linear-algebra.md#invertible-matrix). Thus $D$ and $D^\dagger$ are [invertible matrices](../../linear-algebra.md#invertible-matrix), justifying the inverse in the definition of $U$. The [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) of $U=D^\dagger D^{-1}$ is $(D^\dagger)^{-1}D$. Since $D$ and $D^\dagger$ [commute](../../algebraic-operation.md#commuting-elements), their inverses do too, and

$$
\boxed{U^\dagger U=(D^\dagger)^{-1}DD^\dagger D^{-1}=I.}
$$

Hence $U$ is a [unitary matrix](../../linear-operator-theory.md#unitary-matrix).

<h4 id="5/b/v">v</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/v/solution">Solution</h5>

↑ **Parent:** [V](#5/b/v)

For the [unitary matrix](../../linear-operator-theory.md#unitary-matrix) $C$, $C^{-1}=C^\dagger$. Therefore $D=C^{-1}AC$ is a [Hermitian matrix](../../hilbert-space.md#hermitian-operator):

$$
D^\dagger=(C^\dagger AC)^\dagger=C^\dagger AC=D.
$$

Every positive integer power remains a [Hermitian matrix](../../hilbert-space.md#hermitian-operator), since $(D^p)^\dagger=(D^\dagger)^p=D^p$. Its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are real by the [finite-dimensional spectral theorem](../../linear-operator-theory.md#finite-dimensional-spectral-theorem). Equivalently, [matrix similarity](../../linear-algebra.md#matrix-similarity) gives

$$
D^p=C^{-1}A^pC,
$$

whose [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $\boxed{\lambda_j^p\in\mathbb R}$, where the $\lambda_j$ are the real [eigenvalues](../../linear-operator-theory.md#eigenvalue) of $A$.

<h4 id="5/b/vi">vi</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#5/b/vi)

Complete the square in the [Hermitian matrix](../../hilbert-space.md#hermitian-operator) polynomial:

$$
H=\left(A+\frac\alpha2I\right)^2+\left(\beta-\frac{\alpha^2}4\right)I.
$$

For every nonzero [vector](../../vector-space.md#vector) $v$,

$$
v^\dagger Hv=\left\|\left(A+\frac\alpha2I\right)v\right\|^2+\left(\beta-\frac{\alpha^2}4\right)\|v\|^2>0.
$$

Thus $H$ is a [positive-definite matrix](../../quadratic-form.md#positive-definite-matrix), so $\boxed{0\text{ is not an eigenvalue of }H}$. In [finite-dimensional spectral theorem](../../linear-operator-theory.md#finite-dimensional-spectral-theorem) terms, each [eigenvalue](../../linear-operator-theory.md#eigenvalue) is

$$
h_j=\lambda_j^2+\alpha\lambda_j+\beta=\left(\lambda_j+\frac\alpha2\right)^2+\beta-\frac{\alpha^2}4>0.
$$

If $\alpha^2\geq4\beta$, the scalar [polynomial](../../polynomial.md) has real [roots of a polynomial](../../polynomial.md#root-of-a-polynomial)

$$
r_\pm=\frac{-\alpha\pm\sqrt{\alpha^2-4\beta}}2.
$$

An allowed nonzero root can be an [eigenvalue](../../linear-operator-theory.md#eigenvalue) of $A$, a [Hermitian matrix](../../hilbert-space.md#hermitian-operator) which is also an [invertible matrix](../../linear-algebra.md#invertible-matrix), in which case $H$ has a zero [eigenvalue](../../linear-operator-theory.md#eigenvalue). For example, $\alpha=2$, $\beta=1$, $A=-I$ gives $H=0$. The weaker inequality does not force failure for every $A$; it removes the general positive lower bound. There is also the harmless corner $\alpha=\beta=0$, for which $H=A^2$ stays positive definite because $A$ is invertible, even though the strict discriminant hypothesis is absent.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For every [vector](../../vector-space.md#vector) $v$, the [Hermitian inner product](../../linear-algebra.md#hermitian-inner-product) gives

$$
\|Cv\|^2=v^\dagger C^\dagger Cv=0.
$$

The [norm](../../normed-vector-space.md#norm) vanishes only on the zero [vector](../../vector-space.md#vector), so $Cv=0$ for every $v$ and $\boxed{C=0}$. In contrast,

$$
\boxed{N=\begin{pmatrix}0&1\\0&0\end{pmatrix}\ne0,\qquad N^2=0}
$$

is a nonzero [nilpotent matrix](../../linear-operator-theory.md#nilpotent-matrix). Multiplying a [matrix](../../vector-space.md#matrix) by its [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) detects column [norms](../../normed-vector-space.md#norm); multiplying it by itself has no corresponding positivity property.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [cyclic property of the trace](../../linear-algebra.md#cyclic-property-of-the-trace) implies

$$
\operatorname{Tr}(MN-NM)=\operatorname{Tr}(MN)-\operatorname{Tr}(NM)=0.
$$

Taking the [matrix trace](../../linear-algebra.md#matrix-trace) of the asserted equality therefore gives $nc=0$. For a positive integer $n$ over the complex numbers this requires $\boxed{c=0}$. It is also sufficient: choose $M=N=0$, or any two [commuting](../../algebraic-operation.md#commuting-elements) [matrices](../../vector-space.md#matrix). Thus a finite-dimensional [operator commutator](../../vector-space.md#operator-commutator) cannot be a nonzero scalar multiple of the [identity matrix](../../vector-space.md#identity-matrix).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The [anticommutator](../../vector-space.md#anticommutator) condition and invertibility give the [matrix similarities](../../linear-algebra.md#matrix-similarity)

$$
B^{-1}AB=-A,\qquad A^{-1}BA=-B.
$$

Since [matrix trace](../../linear-algebra.md#matrix-trace) is invariant under [matrix similarity](../../linear-algebra.md#matrix-similarity),

$$
\operatorname{Tr}A=\operatorname{Tr}(-A)=-\operatorname{Tr}A,\qquad\operatorname{Tr}B=-\operatorname{Tr}B.
$$

Hence $\boxed{\operatorname{Tr}A=\operatorname{Tr}B=0}$. Taking [determinants](../../multilinear-algebra.md#determinant) in the first [matrix similarity](../../linear-algebra.md#matrix-similarity) also gives

$$
\det A=\det(-A)=(-1)^n\det A.
$$

Since $A$ is an [invertible matrix](../../linear-algebra.md#invertible-matrix), $\det A\ne0$, and $\boxed{n\text{ is even}}$. In terms of [eigenvalues](../../linear-operator-theory.md#eigenvalue), the same [matrix similarity](../../linear-algebra.md#matrix-similarity) pairs each nonzero [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\lambda$ with $-\lambda$, with the same [algebraic multiplicity](../../linear-operator-theory.md#algebraic-multiplicity), so an odd number of them is impossible.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/i">i</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/i/solution">Solution</h5>

↑ **Parent:** [I](#6/d/i)

Termwise differentiation of the absolutely convergent [matrix exponential](../../linear-operator-theory.md#matrix-exponential) series gives

$$
\frac{d}{dt}e^{tP}=e^{tP}P=Pe^{tP}.
$$

Because $P$ and $Q$ [commute](../../algebraic-operation.md#commuting-elements), $P$ also [commutes](../../algebraic-operation.md#commuting-elements) with every power of $Q$ and hence with $e^{tQ}$. The [product rule](../../calculus.md#product-rule) therefore gives

$$
f_1'(t)=e^{tP}Pe^{tQ}+e^{tP}e^{tQ}Q=f_1(t)(P+Q).
$$

Direct differentiation gives $f_2'(t)=f_2(t)(P+Q)$, and both initial values are $I$. The [uniqueness theorem for ordinary differential equations](../../analysis.md#uniqueness-theorem-for-ordinary-differential-equations), applied to the finitely many [matrix](../../vector-space.md#matrix) entries, implies $f_1=f_2$. One can see uniqueness directly: the difference $D=f_1-f_2$ obeys $D'=D(P+Q)$ and $D(0)=0$, so

$$
\frac{d}{dt}\left(De^{-t(P+Q)}\right)=0
$$

and the product is identically zero. At $t=1$ this yields

$$
\boxed{e^Pe^Q=e^{P+Q}\quad\text{when }PQ=QP.}
$$

<h4 id="6/d/ii">ii</h4>

↑ **Parent:** [D](#6/d)

<h5 id="6/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/d/ii)

Let $K(t)=e^{tR}Se^{-tR}$. The [product rule](../../calculus.md#product-rule) and differentiation of the [matrix exponential](../../linear-operator-theory.md#matrix-exponential) give

$$
K'(t)=RK(t)-K(t)R=[R,K(t)],\qquad K''(t)=[R,[R,K(t)]],
$$

where brackets are the [operator commutator](../../vector-space.md#operator-commutator). Evaluating at zero gives $K(0)=S$, $K'(0)=[R,S]$ and $K''(0)=[R,[R,S]]$. The [Taylor series](../../calculus.md#taylor-series) at zero is consequently

$$
\boxed{e^{tR}Se^{-tR}=S+t[R,S]+\frac{t^2}{2}[R,[R,S]]+O(t^3).}
$$

In particular $[R,[R,S]]=R^2S-2RSR+SR^2$, which also follows by multiplying the two [matrix exponential](../../linear-operator-theory.md#matrix-exponential) series through quadratic order. For fixed finite [matrices](../../vector-space.md#matrix) the remainder has the stated [Big O notation](../../real-analysis.md#big-o-notation) in any [matrix norm](../../vector-space.md#matrix-norm).

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

For a [holomorphic function](../../holomorphic-function.md), the derivative supplied by [complex differentiability](../../holomorphic-function.md#complex-differentiability) must have the same value along real and imaginary increments. Those two computations give

$$
f'(z)=u_x+iv_x=\frac{u_y+iv_y}{i}=v_y-iu_y.
$$

Equating real and imaginary parts proves the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations):

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

Conversely, if the first partial [derivatives](../../calculus.md#derivative) are continuous near a point and obey these equations there, real differentiability gives

$$
f(z+h)-f(z)=(u_x+iv_x)\operatorname{Re}h+(u_y+iv_y)\operatorname{Im}h+o(|h|)=f'(z)h+o(|h|),
$$

which proves complex differentiability under this regularity assumption.

The [gradients](../../multivariable-calculus.md#gradient) of the real and imaginary parts have [dot product](../../inner-product.md#dot-product)

$$
\nabla u\cdot\nabla v=u_xv_x+u_yv_y=v_yv_x-v_xv_y=0,
$$

and $|\nabla u|^2=|\nabla v|^2=|f'(z)|^2$. At every point with $f'(z)\ne0$, the two [level sets](../../topology.md#level-set) are regular curves, their [gradients](../../multivariable-calculus.md#gradient) are nonzero [normal vectors](../../differential-geometry.md#normal-vector), and their tangent directions are therefore perpendicular.

The printed phrase "at every point" needs this regular-point qualification. At a [critical point](../../analysis.md#critical-point) with $f'(z)=0$, the [level sets](../../topology.md#level-set) may cross or fail to have a unique tangent. For example, $f(z)=z^2$ gives $u=x^2-y^2$ and $v=2xy$: at the origin the zero [level sets](../../topology.md#level-set) are respectively the diagonals and the coordinate axes. Thus the valid conclusion is $\boxed{\text{orthogonality at every regular intersection, where }f'(z)\ne0}$.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) determine the [harmonic conjugate](../../partial-differential-equation.md#harmonic-conjugate). First

$$
u_x=e^x[(x+1)\cos y-y\sin y],
$$

so $v_y=u_x$ integrates with respect to $y$ to

$$
v=e^x(x\sin y+y\cos y)+h(x).
$$

Now

$$
u_y=e^x[-(x+1)\sin y-y\cos y],
$$

and the second [Cauchy-Riemann equation](../../analysis.md#cauchy-riemann-equations), $v_x=-u_y$, forces $h'(x)=0$. Hence

$$
f=e^x\{x\cos y-y\sin y+i(x\sin y+y\cos y)\}+iC=ze^z+iC.
$$

The normalization at zero gives $C=0$, so the required [entire function](../../holomorphic-function.md#entire-function) is

$$
\boxed{f(z)=ze^z.}
$$

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

For the first function, the complex exponential has no [zeros](../../polynomial.md#zero-of-a-function), while the denominator has three distinct simple [zeros](../../polynomial.md#zero-of-a-function). Thus there are $\boxed{\text{simple poles at }z=0,\,2i,\,-2i;\ \text{no finite zeros}}$. To examine infinity, substitute $z=1/w$:

$$
\frac{e^{1/w}}{[(1/w)^2+4]/w}=\frac{w^3e^{1/w}}{1+4w^2}.
$$

The factor $e^{1/w}$ has an [essential singularity](../../isolated-singularity.md#essential-singularity) at zero, and multiplication by a nonzero finite-order factor cannot remove it. Therefore $\boxed{\infty\text{ is an isolated essential singularity}}$ of the first function.

For the second function, $\sin z$ has simple [zeros](../../polynomial.md#zero-of-a-function) at $z=n\pi$. At zero, its [Taylor series](../../calculus.md#taylor-series) gives

$$
\frac{z^2}{\sin^2z}=\left(\frac{z}{z-z^3/6+O(z^5)}\right)^2=1+\frac{z^2}{3}+O(z^4),
$$

so $\boxed{z=0\text{ is removable, with extended value }1}$. Every other $z=n\pi$ is a double [pole](../../isolated-singularity.md#pole), since the numerator is nonzero there. There are no finite [zeros](../../polynomial.md#zero-of-a-function), including after removal at zero.

At infinity the double [poles](../../isolated-singularity.md#pole) $n\pi$ accumulate. Equivalently, after $z=1/w$, the function $1/[w^2\sin^2(1/w)]$ has double [poles](../../isolated-singularity.md#pole) at $w=1/(n\pi)$ tending to zero. Hence $\boxed{\infty\text{ is a non-isolated singularity}}$. The removable/pole/essential trichotomy for [isolated singularities](../../isolated-singularity.md) does not apply there; calling this an isolated [essential singularity](../../isolated-singularity.md#essential-singularity) would be incorrect.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

Put $w=z-1$ and $a=1-i$. [Partial fraction decomposition](../../isolated-singularity.md#partial-fraction-decomposition) gives

$$
\frac1{(z-i)(z+3)}=\frac1{3+i}\left(\frac1{w+a}-\frac1{w+4}\right).
$$

Both terms admit a [geometric series](../../sequence-and-series.md#geometric-series) at $w=0$. The local [Laurent series](../../analysis.md#laurent-series) is actually a [Taylor series](../../calculus.md#taylor-series), since the center is regular:

$$
\boxed{\frac1{(z-i)(z+3)}=\frac1{3+i}\sum_{m=0}^{\infty}(-1)^m\left[\frac1{(1-i)^{m+1}}-\frac1{4^{m+1}}\right](z-1)^m,\quad |z-1|<\sqrt2.}
$$

The nearest [pole](../../isolated-singularity.md#pole) is $z=i$, a distance $|1-i|=\sqrt2$ from the center; the other [pole](../../isolated-singularity.md#pole) is at distance $4$. Thus the requested local [radius of convergence](../../sequence-and-series.md#radius-of-convergence) is $\boxed{R=\sqrt2}$.

For completeness, specifying a [Laurent series](../../analysis.md#laurent-series) without a region can also mean either of the other maximal annuli. Expanding the first fraction in inverse powers and the second in positive powers gives

$$
\frac1{3+i}\left[\sum_{m=0}^{\infty}\frac{(-a)^m}{w^{m+1}}-\sum_{m=0}^{\infty}\frac{(-1)^mw^m}{4^{m+1}}\right],\qquad \sqrt2<|w|<4.
$$

Expanding both fractions in inverse powers instead gives

$$
\frac1{3+i}\sum_{m=0}^{\infty}\frac{(-a)^m-(-4)^m}{w^{m+1}},\qquad |w|>4.
$$

These are different [Laurent series](../../analysis.md#laurent-series) on different annuli, rather than extensions of the local [Taylor series](../../calculus.md#taylor-series) beyond its [radius of convergence](../../sequence-and-series.md#radius-of-convergence).

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

Away from $y=\pm1$, divide by the coefficient of $x''$ to obtain the normal form

$$
x''+P(y)x'+Q(y)x=0,\qquad P(y)=Q(y)=\frac1{y^2-1}.
$$

Thus $\boxed{y=1\text{ and }y=-1}$ are the only finite singular points. For a second-order [linear differential equation](../../differential-equation.md#linear-differential-equation), $y_0$ is a [regular singular point](../../complex-analysis.md#regular-singular-point) if $(y-y_0)P(y)$ and $(y-y_0)^2Q(y)$ extend analytically to $y_0$. At $y_0=1$ these functions are

$$
\frac1{y+1},\qquad \frac{y-1}{y+1},
$$

and at $y_0=-1$ they are

$$
\frac1{y-1},\qquad \frac{y+1}{y-1}.
$$

Each pair is analytic at its respective point. Therefore $\boxed{\text{both finite singular points are regular}}$.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Set $t=y-1$. Then $y^2-1=t(t+2)$, and a [Frobenius solution](../../complex-analysis.md#frobenius-solution) has the form

$$
x=t^\sigma\sum_{j=0}^{\infty}a_jt^j,\qquad a_0\ne0.
$$

In the [differential equation](../../differential-equation.md), the lowest power is $t^{\sigma-1}$, whose coefficient is

$$
[2\sigma(\sigma-1)+\sigma]a_0=\sigma(2\sigma-1)a_0.
$$

The [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) and its [indicial roots](../../linear-ordinary-differential-equation.md#indicial-root) are consequently

$$
\boxed{\sigma(2\sigma-1)=0,\qquad \sigma_1=0,\quad\sigma_2=\frac12.}
$$

Their difference is not an integer, so the [Frobenius method](../../complex-analysis.md#frobenius-method) produces two independent series without a logarithmic term:

$$
\boxed{x_1(y)=\sum_{j=0}^{\infty}a_j(y-1)^j,\qquad x_2(y)=(y-1)^{1/2}\sum_{j=0}^{\infty}b_j(y-1)^j,\quad a_0b_0\ne0.}
$$

Choose a branch of $(y-1)^{1/2}$, or take $y>1$ for real solutions. A general local solution is $C_1x_1+C_2x_2$ by [linear independence](../../vector-space.md#linear-independence) and the [superposition principle](../../vector-space.md#superposition-principle). The analytic factors converge at least for $|y-1|<2$, up to the next singular point at $y=-1$.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

In the shifted variable $t=y-1$, substitute the [Frobenius solution](../../complex-analysis.md#frobenius-solution) $x=\sum_{j\geq0}a_jt^{j+\sigma}$ into $t(t+2)x''+x'+x=0$. Equating the coefficient of $t^{j+\sigma}$ gives

$$
(j+1+\sigma)[2(j+\sigma)+1]a_{j+1}+[(j+\sigma)(j+\sigma-1)+1]a_j=0.
$$

Thus the [linear recurrence relation](../../algebra.md#linear-recurrence-relation), valid for $j=0,1,\ldots$, is

$$
\boxed{a_{j+1}=-\frac{(j+\sigma)(j+\sigma-1)+1}{(j+1+\sigma)[2(j+\sigma)+1]}a_j.}
$$

For the [indicial root](../../linear-ordinary-differential-equation.md#indicial-root) $\sigma=0$, this becomes

$$
a_{j+1}=-\frac{j^2-j+1}{(j+1)(2j+1)}a_j,\qquad \boxed{a_1=-a_0}.
$$

For the [indicial root](../../linear-ordinary-differential-equation.md#indicial-root) $\sigma=1/2$, rename the coefficients $b_j$; then

$$
b_{j+1}=-\frac{j^2+3/4}{(j+3/2)(2j+2)}b_j,\qquad \boxed{b_1=-\frac14b_0}.
$$

With $a_0=b_0=1$, the first terms of the two [Frobenius solutions](../../complex-analysis.md#frobenius-solution) are

$$
\boxed{x_1=1-t+\frac16t^2+O(t^3),\qquad x_2=t^{1/2}\left(1-\frac14t+\frac7{160}t^2+O(t^3)\right).}
$$

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

The [generalized momentum](../../lagrangian-mechanics.md#generalized-momentum) of this [Lagrangian](../../calculus-of-variations.md#lagrangian) is

$$
p=\frac{\partial\mathcal L}{\partial\dot x}=\frac{m\dot x}{\sqrt{1-\dot x^2}},\qquad\frac{\partial\mathcal L}{\partial x}=-V'(x).
$$

The [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) therefore gives

$$
\boxed{\frac{d}{dt}\left(\frac{m\dot x}{\sqrt{1-\dot x^2}}\right)+V'(x)=0,\qquad \frac{m\ddot x}{(1-\dot x^2)^{3/2}}=-V'(x).}
$$

Because $\mathcal L$ has no explicit time dependence, the energy form of the [Beltrami identity](../../analysis.md#beltrami-identity) gives a conserved quantity $E=\dot x\,\partial\mathcal L/\partial\dot x-\mathcal L$. Here

$$
E=\frac{m\dot x^2}{\sqrt{1-\dot x^2}}+m\sqrt{1-\dot x^2}+V(x)=\boxed{\frac{m}{\sqrt{1-\dot x^2}}+V(x)}.
$$

For a direct check of [conservation of energy](../../mathematical-physics.md#conservation-of-energy), differentiate:

$$
\frac{dE}{dt}=\dot x\left[\frac{m\ddot x}{(1-\dot x^2)^{3/2}}+V'(x)\right]=0.
$$

This is the rest-plus-kinetic energy of a [relativistic particle](../../special-relativity.md#relativistic-particle), in units with light speed one, plus its [potential energy](../../energy.md#potential-energy).

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

Write $\Delta V=V_2-V_1>0$ and $\gamma_i=(1-v_i^2)^{-1/2}$, the initial [Lorentz factor](../../special-relativity.md#lorentz-factor). The conserved [energy](../../energy.md) from part (a) is $E=m\gamma_i+V_1$. To emerge on the higher plateau with positive speed, the particle needs $E>m+V_2$. Hence

$$
\gamma_i>1+\frac{\Delta V}{m},\qquad\boxed{v_i>v_{\mathrm{th}}=\sqrt{1-\left(1+\frac{\Delta V}{m}\right)^{-2}}.}
$$

Above this threshold, [conservation of energy](../../mathematical-physics.md#conservation-of-energy) gives $\gamma_f=\gamma_i-\Delta V/m>1$. The transmitted [velocity](../../classical-mechanics.md#velocity) is positive, so

$$
\boxed{v_f=+\sqrt{1-\left[\frac1{\sqrt{1-v_i^2}}-\frac{\Delta V}{m}\right]^{-2}},\qquad v_i>v_{\mathrm{th}}.}
$$

Below threshold there is a turning point within the steep transition, where $\dot x=0$ and $V=E-m<V_2$. The particle returns to the lower plateau. Its final [potential energy](../../energy.md#potential-energy) equals its initial value, so its final [Lorentz factor](../../special-relativity.md#lorentz-factor) equals $\gamma_i$ but its direction is reversed:

$$
\boxed{v_f=-v_i,\qquad 0<v_i<v_{\mathrm{th}}.}
$$

At exact threshold the limiting speed on the upper plateau is zero. This is the marginal case, not passage with positive outgoing speed. The ideal discontinuous potential does not specify the detailed trajectory at equality; a smooth transition can make the particle approach the top asymptotically. The final-speed formulas above cover the strictly transmitted and reflected regimes requested.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Take nonzero real trial functions $y$ with $y,y'$ [square-integrable](../../measure-theory.md#square-integrable-function) and sufficient decay for [integration by parts](../../calculus.md#integration-by-parts). For a compactly supported [variation](../../calculus-of-variations.md#variation) $y\mapsto y+\varepsilon\eta$, the [first variations](../../calculus-of-variations.md#first-variation) are

$$
\delta F=2\int_{\mathbb R}(y'\eta'-V_0e^{-x^2}y\eta)\,dx=2\int_{\mathbb R}(-y''-V_0e^{-x^2}y)\eta\,dx,\qquad\delta G=2\int_{\mathbb R}y\eta\,dx.
$$

The [quotient rule](../../calculus.md#quotient-rule) for the [functional](../../calculus-of-variations.md#functional) then yields

$$
\delta\Lambda=\frac2{G[y]}\int_{\mathbb R}\left[-y''-V_0e^{-x^2}y-\Lambda[y]y\right]\eta\,dx.
$$

By the [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations), stationarity for all such $\eta$ is equivalent to

$$
-y''-V_0e^{-x^2}y=\Lambda[y]y.
$$

Conversely, multiplying a decaying [eigenfunction](../../linear-operator-theory.md#eigenfunction) equation by $y$ and using [integration by parts](../../calculus.md#integration-by-parts) gives $F[y]=EG[y]$, so its [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) equals $E$ and its [first variation](../../calculus-of-variations.md#first-variation) vanishes. Thus the stationary values of the [functional](../../calculus-of-variations.md#functional) are the energy [eigenvalues](../../linear-operator-theory.md#eigenvalue). The word "extrema" in the question includes stationary points here: higher [eigenfunctions](../../linear-operator-theory.md#eigenfunction) can be saddle points of the unrestricted [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient).

The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) gives

$$
\boxed{E_0=\inf_{y\ne0}\Lambda[y],\qquad E_0\leq\Lambda[y_T].}
$$

Choose an admissible trial family, calculate its [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient), and minimize over its parameters to obtain the best upper bound within that family. Equality holds for the exact [ground state](../../quantum-mechanics.md#ground-state); a restricted family generally gives only an upper bound.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

For the trial function, $y_T'=-ax\,y_T$. The required [Gaussian integrals](../../integral.md#gaussian-integral) are

$$
G[y_T]=\int_{\mathbb R}e^{-ax^2}\,dx=\sqrt{\frac\pi a},\qquad\int_{\mathbb R}x^2e^{-ax^2}\,dx=\frac{\sqrt\pi}{2a^{3/2}}.
$$

The second formula follows by differentiating the first with respect to $a$. Therefore

$$
F[y_T]=a^2\frac{\sqrt\pi}{2a^{3/2}}-V_0\sqrt{\frac\pi{1+a}},
$$

and division by $G[y_T]$ gives the [Gaussian variational bound for an attractive Gaussian well](../../linear-operator-theory.md#gaussian-variational-bound-for-an-attractive-gaussian-well):

$$
\boxed{E(a)=\frac a2-V_0\sqrt{\frac a{1+a}},\qquad a>0.}
$$

This is a good trial family because it consists of smooth, positive, [square-integrable functions](../../measure-theory.md#square-integrable-function) decaying at both infinities. Each is an [even function](../../calculus.md#even-function), matching the symmetry of the lowest [bound state](../../quantum-system.md#bound-state) in this even potential, and the parameter varies its width. It also permits exact [Gaussian integrals](../../integral.md#gaussian-integral). Its Gaussian tail need not equal the exact exponential tail of a negative-energy [bound state](../../quantum-system.md#bound-state) for the [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) to give a valid bound.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Differentiating the [Gaussian variational bound for an attractive Gaussian well](../../linear-operator-theory.md#gaussian-variational-bound-for-an-attractive-gaussian-well) gives

$$
E'(a)=\frac12-\frac{V_0}{2\sqrt a(1+a)^{3/2}}.
$$

Thus an interior [stationary point](../../calculus-of-variations.md#stationary-point) obeys

$$
\boxed{\sqrt{a_*}(1+a_*)^{3/2}=V_0,\qquad a_*(1+a_*)^3=V_0^2.}
$$

The left side of the first equation increases strictly from zero to infinity, so there is exactly one such point. More explicitly,

$$
E''(a)=\frac{V_0(1+4a)}{4a^{3/2}(1+a)^{5/2}}>0,
$$

so $E$ is a [strictly convex function](../../real-analysis.md#strictly-convex-function) on $a>0$ and $a_*$ is its global minimum. At that minimum the stationarity equation gives

$$
E(a_*)=\frac{a_*}{2}-a_*(1+a_*)=-\frac{a_*}{2}-a_*^2<0.
$$

There is a continuous limiting zero at $a=0$, although $y_T=1$ at exactly $a=0$ is not a [square-integrable function](../../measure-theory.md#square-integrable-function) and hence is not an admissible trial. For a positive zero, division by $\sqrt a$ and squaring gives $a(1+a)=4V_0^2$, so

$$
\boxed{a_z=\frac{\sqrt{1+16V_0^2}-1}{2}}
$$

is the unique positive zero. The other quadratic root is negative and inadmissible. Near zero,

$$
E(a)=-V_0\sqrt a+\frac a2+O(a^{3/2}),
$$

so the graph leaves the origin with slope $-\infty$, falls to its unique negative minimum, rises through $a_z$, and grows as $a/2-V_0+O(a^{-1})$ at infinity.

<a id="10/c/image-the-gaussian-variational-bound-for-an-attractive-gaussian-well-at-v-0-1-showing-its-negative-minimum-and-positive-zero"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1-gaussian-variational-energy.png)

**[Figure 1](#10/c/image-the-gaussian-variational-bound-for-an-attractive-gaussian-well-at-v-0-1-showing-its-negative-minimum-and-positive-zero). The Gaussian variational bound for an attractive Gaussian well at $V_0=1$, showing its negative minimum and positive zero**.

By the [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle),

$$
\boxed{E_0\leq E(a_*)=-\frac{a_*}{2}-a_*^2<0.}
$$

Thus the attractive well supports a negative-energy [bound state](../../quantum-system.md#bound-state) for every $V_0>0$.

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

It is enough to choose an admissible parameter, without solving the minimizing equation. Take $a=V_0^2>0$ in the [Gaussian variational bound for an attractive Gaussian well](../../linear-operator-theory.md#gaussian-variational-bound-for-an-attractive-gaussian-well). The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) gives

$$
E_0\leq\frac{V_0^2}{2}-\frac{V_0^2}{\sqrt{1+V_0^2}}=-\frac{V_0^2}{2}+\varepsilon,
$$

where an explicit remainder is

$$
\varepsilon=V_0^2\left(1-\frac1{\sqrt{1+V_0^2}}\right)=\frac{V_0^4}{\sqrt{1+V_0^2}(\sqrt{1+V_0^2}+1)}.
$$

The denominator tends to $2$ as $V_0\to0$, proving $\varepsilon=O(V_0^4)$ in [Big O notation](../../real-analysis.md#big-o-notation). More precisely the [binomial series](../../sequence-and-series.md#binomial-series) gives

$$
\varepsilon=\frac12V_0^4-\frac38V_0^6+O(V_0^8),
$$

and therefore

$$
\boxed{E_0\leq-\frac12V_0^2+\varepsilon,\qquad\varepsilon=O(V_0^4).}
$$

This is an upper bound on the exact [ground state](../../quantum-mechanics.md#ground-state) energy, rather than an assertion that the leading coefficient of its exact weak-potential expansion is $-1/2$.

## ↑ Ancestors (10)

1. [2025](../2025.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
