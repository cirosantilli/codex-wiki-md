# Paper 1

↑ **Parent:** [2013](../2013.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2013/PaperNST_IB_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2013/PaperNST_IB_1.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
  - [iv](#6/iv)
    - [Solution](#6/iv/solution)
  - [v](#6/v)
    - [Solution](#6/v/solution)
- [7](#7)
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
  - [iii](#7/iii)
    - [Solution](#7/iii/solution)
  - [iv](#7/iv)
    - [Solution](#7/iv/solution)
  - [v](#7/v)
    - [Solution](#7/v/solution)
- [8](#8)
  - [i](#8/i)
    - [Solution](#8/i/solution)
  - [ii](#8/ii)
    - [Solution](#8/ii/solution)
  - [iii](#8/iii)
    - [Solution](#8/iii/solution)
  - [iv](#8/iv)
    - [Solution](#8/iv/solution)
  - [v](#8/v)
    - [Solution](#8/v/solution)
  - [vi](#8/vi)
    - [Solution](#8/vi/solution)
- [9](#9)
  - [i](#9/i)
    - [Solution](#9/i/solution)
  - [ii](#9/ii)
    - [Solution](#9/ii/solution)
    - [a](#9/ii/a)
      - [Solution](#9/ii/a/solution)
    - [b](#9/ii/b)
      - [Solution](#9/ii/b/solution)
  - [iii](#9/iii)
    - [Solution](#9/iii/solution)
  - [iv](#9/iv)
    - [Solution](#9/iv/solution)
  - [v](#9/v)
    - [Solution](#9/v/solution)
- [10](#10)
  - [i](#10/i)
    - [Solution](#10/i/solution)
  - [ii](#10/ii)
    - [Solution](#10/ii/solution)
  - [iii](#10/iii)
    - [Solution](#10/iii/solution)
  - [iv](#10/iv)
    - [Solution](#10/iv/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Using the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) and the [Einstein summation convention](../../multilinear-algebra.md#einstein-notation) in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system), the [product rule](../../calculus.md#product-rule) gives

$$
\begin{aligned}
\nabla\cdot(\mathbf A\times\mathbf B)
&=\partial_i(\epsilon_{ijk}A_jB_k)\\
&=\epsilon_{ijk}(\partial_iA_j)B_k+\epsilon_{ijk}A_j\partial_iB_k\\
&=B_k\epsilon_{kij}\partial_iA_j-A_j\epsilon_{jik}\partial_iB_k.
\end{aligned}
$$

The cyclic permutation in the first term preserves the sign, whereas exchanging the first two indices in the second reverses it. Recognizing the two [curls](../../multivariable-calculus.md#curl) proves

$$
\boxed{\nabla\cdot(\mathbf A\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf A)-\mathbf A\cdot(\nabla\times\mathbf B).}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) states that a continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) $\mathbf F$ on a volume $V$ with piecewise smooth closed boundary $S$ satisfies

$$
\int_V\nabla\cdot\mathbf F\,dV=\int_S\mathbf F\cdot\hat{\mathbf n}\,dS,
$$

where $\hat{\mathbf n}$ is the outward [unit normal](../../differential-geometry.md#unit-normal). Take $\mathbf F=\nabla a\times\mathbf B$. Since the [curl of a gradient](../../multivariable-calculus.md#curl-of-a-gradient) is zero for a twice continuously differentiable [scalar field](../../classical-field-theory.md#scalar-field), part (i) gives

$$
\nabla\cdot(\nabla a\times\mathbf B)=-\nabla a\cdot(\nabla\times\mathbf B).
$$

Integrating this identity and applying the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) proves

$$
\boxed{\int_V\nabla a\cdot(\nabla\times\mathbf B)\,dV=-\int_S(\nabla a\times\mathbf B)\cdot\hat{\mathbf n}\,dS.}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Direct [differentiation](../../calculus.md#differentiation) gives

$$
\nabla a=(y,x,2z),\qquad \nabla\times\mathbf B=(y,-1,-1),\qquad \nabla a\cdot(\nabla\times\mathbf B)=y^2-x-2z.
$$

On the unit disk $D$, [polar coordinates](../../multivariable-calculus.md#polar-coordinates) give $\int_Dy^2\,dA=\pi/4$, $\int_Dx\,dA=0$ and $\int_DdA=\pi$. Consequently the [volume integral](../../multivariable-calculus.md#volume-integral) is

$$
\int_0^h\left(\frac\pi4-2\pi z\right)dz=\boxed{\frac{\pi h}{4}-\pi h^2}.
$$

For an independent [surface integral](../../multivariable-calculus.md#surface-integral) calculation, the relevant [cross product](../../vector-space.md#cross-product) is

$$
\mathbf F=\nabla a\times\mathbf B=(x^2+2yz^2,\ 2yz-xy,\ -y^2z-xy).
$$

The bottom face contributes $\int_Dxy\,dA=0$ and the top contributes $\int_D(-hy^2-xy)\,dA=-\pi h/4$. On the cylindrical side, put $x=\cos\theta$, $y=\sin\theta$, $\hat{\mathbf n}=(x,y,0)$ and $dS=d\theta\,dz$. The [flux](../../mathematical-physics.md#flux) density is $x^3+2xyz^2+2y^2z-xy^2$. All terms except $2y^2z$ integrate to zero because they are [odd functions](../../calculus.md#odd-function) of $x$ or $y$, giving

$$
\int_{\mathrm{side}}\mathbf F\cdot\hat{\mathbf n}\,dS=\int_0^h2\pi z\,dz=\pi h^2.
$$

Thus minus the total outward [flux](../../mathematical-physics.md#flux) is $-(\pi h^2-\pi h/4)$, in agreement with the [volume integral](../../multivariable-calculus.md#volume-integral).

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For [separation of variables](../../partial-differential-equation.md#separation-of-variables), take $u(x,t)=X(x)T(t)$ in the [damped wave equation](../../wave-equation.md#damped-wave-equation). Dividing by $c^2XT$, with $c>0$, gives $X''/X=(T''+\alpha T')/(c^2T)=-k^2$. The separated [ordinary differential equations](../../differential-equation.md#ordinary-differential-equation) are therefore

$$
\boxed{X''+k^2X=0,\qquad T''+\alpha T'+c^2k^2T=0.}
$$

The negative separation constant anticipates the positive spatial [eigenvalues](../../linear-operator-theory.md#eigenvalue) selected by the fixed endpoints.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

An [even function](../../calculus.md#even-function) satisfying the spatial equation has $X=C\cos(kx)$. The [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) require $\cos(kL)=0$, so the allowed [wavenumbers](../../wave-equation.md#wavenumber) are

$$
k_n=\frac{n\pi}{2L},\qquad n=1,3,5,\ldots.
$$

There is no nonzero zero-wavenumber mode. With $T=e^{-\alpha t/2}S$, the time equation becomes $S''+\omega_n^2S=0$, where $\omega_n^2=c^2k_n^2-\alpha^2/4$. Thus [superposition](../../vector-space.md#superposition-principle) of the even [normal modes](../../wave-equation.md#normal-mode) gives

$$
\boxed{u(x,t)=\sum_{\substack{n\geq1\\ n\ {
m odd}}}e^{-\alpha t/2}\cos(k_nx)\operatorname{Re}\left(A_ne^{i\omega_nt}+B_ne^{-i\omega_nt}\right).}
$$

This uses completeness of the even [Fourier series](../../fourier-series.md) modes. Imaginary $\omega_n$ describe [overdamping](../../wave-equation.md#overdamping). At [critical damping](../../wave-equation.md#critical-damping), $\omega_n=0$, the two displayed exponentials coincide: the complete time factor must instead be $e^{-\alpha t/2}(C_n+D_nt)$. This repeated-root exception is necessary for a genuinely general solution.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The [angular frequency](../../lagrangian-mechanics.md#angular-frequency) of an underdamped mode is

$$
\boxed{\omega_n=\sqrt{\frac{c^2n^2\pi^2}{4L^2}-\frac{\alpha^2}{4}}.}
$$

For ordinary [damping](../../wave-equation.md#damping), $\alpha\geq0$, mode $n$ oscillates precisely when $\alpha<cn\pi/L$. In particular, **all modes, including the fundamental, oscillate when $\alpha<c\pi/L$**. There are some oscillatory modes for every finite $\alpha$, since the allowed $n$ are unbounded; no finite damping coefficient overdamps the entire ideal string spectrum.

If $\alpha<0$, the same mode has negative [damping](../../wave-equation.md#damping): oscillatory amplitudes grow as $e^{|\alpha|t/2}$. For modes with real characteristic roots, both roots are positive, since $|\alpha|/2>\sqrt{\alpha^2/4-c^2k_n^2}$. Hence those modes also grow. Negative damping makes the equilibrium unstable.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $d_n$ be the even [Fourier coefficient](../../fourier-series.md#fourier-coefficient) of the initial displacement, with the normalization $\int_{-L}^L\cos^2(k_nx)dx=L$. Writing $s_n=\sin(n\pi/2)=(-1)^{(n-1)/2}$ gives

$$
\begin{aligned}
d_n&=\frac2L\int_0^Le^{-x/l}\cos(k_nx)\,dx\\
&=\boxed{\frac{2l}{L}\frac{1+k_nl\,s_ne^{-L/l}}{1+(k_nl)^2}}\qquad(n\text{ odd}).
\end{aligned}
$$

Zero initial velocity requires the real modal time factor

$$
T_n(t)=d_ne^{-\alpha t/2}\left[\cos(\omega_nt)+\frac{\alpha}{2\omega_n}\sin(\omega_nt)\right].
$$

One consistent choice in the question's complex representation is therefore

$$
\boxed{A_n=\frac{d_n}{2}\left(1-\frac{i\alpha}{2\omega_n}\right),\qquad B_n=\frac{d_n}{2}\left(1+\frac{i\alpha}{2\omega_n}\right).}
$$

For real $\omega_n$, $B_n=\overline{A_n}$; the real-part notation otherwise makes the complex coefficients nonunique. For imaginary $\omega_n$, the same formula is interpreted using [hyperbolic functions](../../calculus.md#hyperbolic-function). Its limit at $\omega_n=0$ is $d_ne^{-\alpha t/2}(1+\alpha t/2)$.

For $l/L\to0$ at fixed mode number,

$$
\boxed{d_n\simeq\frac{2l/L}{1+(n\pi l/2L)^2},}
$$

which can be substituted into $A_n,B_n$ above. The profile specified at $t=0$ is actually nonzero at $x=\pm L$. Thus for finite $l/L$ it cannot be the initial data of a solution continuous at the initial endpoint corners with fixed endpoints. The [Fourier series](../../fourier-series.md) reproduces it in the open interval, with zero endpoint values; it is an [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space) initial-data interpretation. The assumption $l\ll L$ makes this compatibility error exponentially small, rather than exactly zero.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The substitution $y=e^xg$ reduces the [homogeneous linear differential equation](../../differential-equation.md#homogeneous-linear-differential-equation) to

$$
g''+\left(1-\frac1x\right)g'=0.
$$

A first [integration](../../integral.md) gives $g'=Cxe^{-x}$, and a second gives $g=D-C(x+1)e^{-x}$. Hence

$$
\boxed{y=Ae^x+B(1+x).}
$$

The [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) of $1+x,e^x$ is $xe^x$, so they are [linearly independent](../../vector-space.md#linear-independence) on either side of zero. At zero the differential equation has a [regular singular point](../../complex-analysis.md#regular-singular-point). The displayed solutions extend analytically through it; their linear combinations describe the global solutions when two continuous derivatives are required there. If no matching condition is imposed, the two sides have independent constants.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Use the boundary-adapted [homogeneous solutions](../../linear-ordinary-differential-equation.md#homogeneous-solution)

$$
u(x)=1+x,\qquad v(x)=e^x-\frac e2(1+x),\qquad W(x)=uv'-u'v=xe^x.
$$

For a source point $\xi\ne0$, the [Green function](../../green-s-function.md) is

$$
\boxed{G(x,\xi)=\frac1{\xi e^\xi}\begin{cases}u(x)v(\xi),&x\leq\xi,\\u(\xi)v(x),&x\geq\xi.\end{cases}}
$$

It vanishes at both endpoints and is continuous at $x=\xi$. Its first [derivative](../../calculus.md#derivative) has the jump

$$
G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=\frac{u(\xi)v'(\xi)-u'(\xi)v(\xi)}{W(\xi)}=1,
$$

as required for a monic second-order [differential operator](../../analysis.md#differential-operator) with a [Dirac delta](../../distribution-theory.md#dirac-delta-function) source. Away from that source it is a [homogeneous solution](../../linear-ordinary-differential-equation.md#homogeneous-solution) and extends smoothly through $x=0$.

**The interior singular point requires a qualification.** This is a [Green kernel with a vanishing Wronskian at an interior singular point](../../green-s-function.md#green-kernel-with-a-vanishing-wronskian-at-an-interior-singular-point), with a $1/\xi$ singularity in its source variable. It is not an ordinary integral inverse for unrestricted forcing. For smooth forcing $f(\xi)=\xi q(\xi)$, however, the product $Gf$ extends continuously at zero and the integral is well defined. This includes part (iii). We use solutions with two continuous derivatives across zero, interpreting the equation there after multiplication by $x$. For such a solution, expansion at zero forces $f(0)=0$; arbitrary nonzero forcing at zero cannot satisfy this regularity. Merely imposing one continuous derivative would leave a piecewise homogeneous ambiguity, so the original singular coefficients alone do not specify an unrestricted boundary-value inverse.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The source factor cancels the singular denominator of the [Green function](../../green-s-function.md). Splitting the [integral](../../integral.md) at $\xi=x$ gives

$$
y(x)=v(x)\int_{-1}^x(1+\xi)e^{-\xi}d\xi+(1+x)\int_x^1\left[1-\frac e2(1+\xi)e^{-\xi}\right]d\xi.
$$

Using $\int(1+\xi)e^{-\xi}d\xi=-(\xi+2)e^{-\xi}$, these two integrals are $e-(x+2)e^{-x}$ and $5/2-x-e(x+2)e^{-x}/2$, respectively. Simplification gives

$$
\boxed{y(x)=e^{x+1}+\frac{1-e^2}{2}(1+x)-x^2.}
$$

The exponential and linear terms are homogeneous solutions, while direct [differentiation](../../calculus.md#differentiation) gives $L(-x^2)=x$ for $x\ne0$. Also $y(-1)=y(1)=0$, and the expression is analytic through zero. Uniqueness in this regular class follows because any difference is a global [linear combination](../../vector-space.md#linear-combination) $Ae^x+B(1+x)$: the left boundary forces $A=0$, and the right then forces $B=0$.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

First take $f,g\in L^1(\mathbb R)$, so [Fubini's theorem](../../measure-theory.md#fubini-s-theorem) applies to the [cross-correlation](../../fourier-analysis.md#cross-correlation) double integral. With $s=x+y$, the [Fourier transform](../../fourier-transform.md) is

$$
\begin{aligned}
\widehat h(k)&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}\overline{f(y)}g(x+y)\,dy\,dx\\
&=\left[\int_{\mathbb R}\overline{f(y)}e^{iky}\,dy\right]\left[\int_{\mathbb R}g(s)e^{-iks}\,ds\right]\\
&=\boxed{\overline{\widehat f(k)}\,\widehat g(k)}.
\end{aligned}
$$

The [complex conjugation](../../complex-analysis.md#complex-conjugation) and the sign in $x+y$ are both essential to this convention.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Set $g=f$. The [cross-correlation](../../fourier-analysis.md#cross-correlation) at zero is $h(0)=\int_{\mathbb R}|f(x)|^2dx$, while part (i) gives $\widehat h=|\widehat f|^2$. Evaluating the [inverse Fourier transform](../../fourier-transform.md#inverse-fourier-transform) at zero yields the [Parseval identity](../../fourier-analysis.md#parseval-identity)

$$
\boxed{\int_{\mathbb R}|f(x)|^2dx=\frac1{2\pi}\int_{\mathbb R}|\widehat f(k)|^2dk.}
$$

This derivation is immediate for [Schwartz functions](../../fourier-analysis.md#schwartz-function), for which all integrations and [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) are justified. Approximation by such functions and completeness then extend the identity to [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space), defining its [Fourier transform](../../fourier-transform.md) by the corresponding norm limit. This is the [Plancherel theorem](../../fourier-analysis.md#plancherel-theorem) extension; no absolute integrability of an arbitrary square-integrable function is presumed.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The direct squared [L2 norm](../../real-analysis.md#l2-norm) is the length of the interval, namely $2$. The [Fourier transform](../../fourier-transform.md) is

$$
\widehat f(k)=\int_{-1}^1e^{-ikx}dx=\frac{2\sin k}{k},\qquad \widehat f(0)=2.
$$

For the transformed norm, let $I=\int_0^\infty\sin^2k/k^2\,dk$. [Integration by parts](../../calculus.md#integration-by-parts), with vanishing endpoint term $-\sin^2k/k$, gives

$$
I=2\int_0^\infty\frac{\sin k\cos k}{k}\,dk=\frac\pi2.
$$

The supplied oscillatory integral is understood as an [improper integral](../../real-analysis.md#improper-integral). Therefore

$$
\boxed{\frac1{2\pi}\int_{-\infty}^{\infty}\left|\frac{2\sin k}{k}\right|^2dk=\frac4\pi I=2,}
$$

which agrees with the direct norm and verifies the [Parseval identity](../../fourier-analysis.md#parseval-identity) with the specified normalization.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Taking the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) of $MM^{-1}=I$ and $M^{-1}M=I$ reverses the product order and gives

$$
(M^{-1})^\dagger M^\dagger=I,\qquad M^\dagger(M^{-1})^\dagger=I.
$$

Thus $(M^{-1})^\dagger$ is the two-sided [matrix inverse](../../matrix-inverse.md) of $M^\dagger$, proving

$$
\boxed{(M^\dagger)^{-1}=(M^{-1})^\dagger.}
$$

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Since $A$ is [Skew-Hermitian](../../linear-operator-theory.md#skew-hermitian-matrix), $H=iA$ is a [Hermitian matrix](../../hilbert-space.md#hermitian-operator). The [spectral theorem](../../hilbert-space.md#spectral-theorem) gives a [unitary matrix](../../linear-operator-theory.md#unitary-matrix) $Q$ with $Q^\dagger HQ=\operatorname{diag}(\lambda_1,\ldots,\lambda_N)$ and real [eigenvalues](../../linear-operator-theory.md#eigenvalue) $\lambda_j$. Hence $Q^\dagger AQ=\operatorname{diag}(-i\lambda_j)$ and

$$
\boxed{|\det(I+A)|^2=\prod_{j=1}^N|1-i\lambda_j|^2=\prod_{j=1}^N(1+\lambda_j^2)\geq1.}
$$

In particular the [determinant](../../multilinear-algebra.md#determinant) is nonzero, so $I+A$ is invertible. Applying the same argument to $-A$ proves that $I-A$ is also invertible. Equality holds precisely when all $\lambda_j=0$, equivalently $A=0$.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Using part (i) and $A^\dagger=-A$ in the [Cayley transform](../../lie-theory.md#cayley-transform-lie-theory) with argument $-A$ gives

$$
\begin{aligned}
U^\dagger&=[(I+A)^{-1}]^\dagger(I-A)^\dagger\\
&=(I-A)^{-1}(I+A)\\
&=(I+A)(I-A)^{-1}=U^{-1}.
\end{aligned}
$$

The factors commute because $I-A$ and $I+A$ are polynomials in the same [matrix](../../vector-space.md#matrix), and an invertible commuting matrix also commutes with the other factor's [matrix inverse](../../matrix-inverse.md). Both inverses exist by part (ii). Thus **$U$ is unitary**.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

Multiplying the defining equation on the right by $I+A$ gives $(I+U)A=I-U$. Consequently the only possible answer is

$$
\boxed{A=(I+U)^{-1}(I-U)=(I-U)(I+U)^{-1}.}
$$

The factors commute because they are rational functions of $U$. Its [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose), using the [unitarity](../../vector-space.md#unitary-operator) $U^\dagger=U^{-1}$, is

$$
\begin{aligned}
A^\dagger&=(I+U^{-1})^{-1}(I-U^{-1})\\
&=(I+U)^{-1}U\bigl[-U^{-1}(I-U)\bigr]=-A.
\end{aligned}
$$

Thus $A$ is [Skew-Hermitian](../../linear-operator-theory.md#skew-hermitian-matrix). Moreover $I+A=2(I+U)^{-1}$ and $I-A=2U(I+U)^{-1}$, so substitution recovers $U$ and establishes existence as well as uniqueness. The [unitary matrix](../../linear-operator-theory.md#unitary-matrix) $U=-I$ is a counterexample to invertibility of $I+U$; more generally the obstruction is an [eigenvalue](../../linear-operator-theory.md#eigenvalue) $-1$.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

For a [skew-symmetric matrix](../../linear-algebra.md#skew-symmetric-matrix), $M^T=-M$. Invariance of the [determinant](../../multilinear-algebra.md#determinant) under [transpose](../../vector-space.md#transpose) gives

$$
\boxed{\det M=\det M^T=\det(-M)=(-1)^n\det M.}
$$

For odd $n$, $2\det M=0$, so **$\det M=0$** over the real or complex numbers.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Since $M$ is real, $(M^2)^T=(M^T)^2=(-M)^2=M^2$. For every real [vector](../../vector-space.md#vector) $x$,

$$
\boxed{x^TM^2x=-(Mx)^T(Mx)=-\|Mx\|^2\leq0.}
$$

Thus $M^2$ is a real [symmetric matrix](../../linear-algebra.md#symmetric-matrix) and is [negative semidefinite](../../multivariable-calculus.md#negative-semidefinite-matrix). When $n$ is odd, part (i) supplies a nonzero $x$ in the [kernel](../../kernel-of-a-linear-map.md) of $M$, and then $M^2x=0$. Hence zero is an [eigenvalue](../../linear-operator-theory.md#eigenvalue) of $M^2$. In fact $\ker M^2=\ker M$, as the displayed norm identity shows.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

Choose $e_1$ real, as permitted by the [spectral theorem for real symmetric matrices](../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices). Matrix powers commute, so

$$
M^2(Me_1)=M(M^2e_1)=-\mu_1^2Me_1.
$$

The proposed partner $e_2=Me_1$ is nonzero because

$$
\|e_2\|^2=-e_1^TM^2e_1=\mu_1^2\|e_1\|^2>0.
$$

Also the real scalar $e_1^TMe_1$ equals its own transpose $e_1^TM^Te_1=-e_1^TMe_1$, so it vanishes. Therefore **$e_1$ and $e_2$ are orthogonal eigenvectors with the same eigenvalue**. This is the basic pairing in the [paired eigenspaces of the square of a real skew-symmetric matrix](../../linear-algebra.md#paired-eigenspaces-of-the-square-of-a-real-skew-symmetric-matrix).

<h3 id="6/iv">iv</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6/iv)

Normalize $e_1$ and put $f_1=Me_1/\mu_1$. The two vectors are an [orthonormal basis](../../inner-product.md#orthonormal-basis) of a plane $E$ invariant under $M$, since $Me_1=\mu_1f_1$ and $Mf_1=-\mu_1e_1$. Its [orthogonal complement](../../hilbert-space.md#orthogonal-complement) is also invariant: for $w\perp E$ and $z\in E$,

$$
\langle Mw,z\rangle=-\langle w,Mz\rangle=0.
$$

Apply the [spectral theorem for real symmetric matrices](../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) to the restriction of $M^2$ to $E^\perp$. Any remaining negative [eigenvalue](../../linear-operator-theory.md#eigenvalue) supplies another orthonormal pair by the same construction. Induction leaves only the [kernel](../../kernel-of-a-linear-map.md). Thus **every nonzero eigenvalue of $M^2$ has even multiplicity**. The pairs can share an eigenvalue, so this does not assert distinctness of the different $-\mu_j^2$.

<h3 id="6/v">v</h3>

↑ **Parent:** [6](#6)

<h4 id="6/v/solution">Solution</h4>

↑ **Parent:** [V](#6/v)

Collect the paired [orthonormal bases](../../inner-product.md#orthonormal-basis) from part (iv), followed by an orthonormal basis of $\ker M^2=\ker M$. The matrix $Q$ of these columns is an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix), and

$$
\boxed{Q^TMQ=\bigoplus_{j=1}^r\begin{pmatrix}0&-\mu_j\\\mu_j&0\end{pmatrix}\ \oplus\ 0_{n-2r},\qquad \mu_j>0.}
$$

Indeed, each pair obeys $Me_j=\mu_jf_j$, $Mf_j=-\mu_je_j$, and all kernel vectors are annihilated. This proves the real block form of a [skew-symmetric matrix](../../linear-algebra.md#skew-symmetric-matrix) directly, including repeated block parameters. In particular its [rank](../../quadratic-form.md#rank-one-quadratic-form) is $2r$, always even.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

For a [holomorphic function](../../holomorphic-function.md), the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) are $u_x=v_y$ and $u_y=-v_x$. Consequently

$$
\boxed{\nabla u\cdot\nabla v=u_xv_x+u_yv_y=0,\qquad |\nabla u|^2=u_x^2+u_y^2=v_x^2+v_y^2=|\nabla v|^2.}
$$

A [gradient](../../multivariable-calculus.md#gradient) is normal to its [level set](../../topology.md#level-set), so these identities give orthogonal level curves wherever the gradients are nonzero. At a critical point where $f'=0$, both gradients vanish and a regular tangent to a [level set](../../topology.md#level-set) need not exist; the geometric orthogonality statement is restricted to regular intersections.

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

Differentiate the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) and use equality of mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative):

$$
\boxed{\Delta u=u_{xx}+u_{yy}=(v_y)_x-(v_x)_y=0.}
$$

Thus the real part is a [harmonic function](../../partial-differential-equation.md#harmonic-function). The same calculation gives $\Delta v=0$. Every [holomorphic function](../../holomorphic-function.md) has the required smoothness.

<h3 id="7/iii">iii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7/iii)

Inverting $u+iv=\operatorname{arcosh}z$ gives $z=\cosh(u+iv)$, hence the [elliptic coordinates](../../geometry-and-topology.md#elliptic-coordinates)

$$
x=\cosh u\cos v,\qquad y=\sinh u\sin v.
$$

Eliminating $v$ at fixed $u>0$ gives the [ellipse](../../euclidean-geometry.md#ellipse)

$$
\boxed{\frac{x^2}{\cosh^2u}+\frac{y^2}{\sinh^2u}=1.}
$$

Its focal distance is $\sqrt{\cosh^2u-\sinh^2u}=1$. At fixed $v$, eliminating $u$ instead gives the [hyperbola](../../euclidean-geometry.md#hyperbola)

$$
\boxed{\frac{x^2}{\cos^2v}-\frac{y^2}{\sin^2v}=1.}
$$

Its focal distance is also one, so both families have foci $(\pm1,0)$. A fixed $v$ traces an appropriate half of the hyperbola; complementary coordinate values complete it. Degenerate values give the focal segment and portions of the coordinate axes. Away from these degeneracies the curves are orthogonal by part (i), or by $\mathbf r_u\cdot\mathbf r_v=0$ in the displayed parametrization. A branch of the inverse is used locally; its real part with $u\geq0$ is single-valued outside the focal segment.

<a id="7/iii/image-confocal-ellipses-and-hyperbolae-generated-by-the-complex-inverse-hyperbolic-cosine"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1-q7-elliptic-coordinates.png)

**[Figure 1](#7/iii/image-confocal-ellipses-and-hyperbolae-generated-by-the-complex-inverse-hyperbolic-cosine). Confocal ellipses and hyperbolae generated by the complex inverse hyperbolic cosine**.

<h3 id="7/iv">iv</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#7/iv)

On the specified [ellipse](../../euclidean-geometry.md#ellipse), the semiaxes are $\sqrt2$ and $1$, so its elliptic coordinate is $u_0=\operatorname{arcosh}\sqrt2=\log(\sqrt2+1)$. Thus in the exterior,

$$
\boxed{\phi=\operatorname{Re}\log\left(z+\sqrt{z^2-1}\right)-\log(\sqrt2+1)}
$$

is a [harmonic function](../../partial-differential-equation.md#harmonic-function) with a homogeneous [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) on that ellipse. Choose the square root with $\sqrt{z^2-1}\sim z$ at infinity. Although a global complex logarithm requires a cut, its real part $\log|z+\sqrt{z^2-1}|$ is well defined throughout the exterior and gives the same $\phi$.

Expanding at large $|z|$ yields $z+\sqrt{z^2-1}=2z[1-1/(4z^2)+O(|z|^{-4})]$. Therefore

$$
\boxed{\phi=\log\frac{2\sqrt{x^2+y^2}}{\sqrt2+1}+O\bigl((x^2+y^2)^{-1}\bigr).}
$$

In particular the potential grows logarithmically in the distance, in every direction at infinity. It is the exterior solution; no [harmonic](../../partial-differential-equation.md#harmonic-function) continuation through the focal segment in the ellipse's interior is claimed.

<h3 id="7/v">v</h3>

↑ **Parent:** [7](#7)

<h4 id="7/v/solution">Solution</h4>

↑ **Parent:** [V](#7/v)

Use the [Wirtinger derivatives](../../analysis.md#wirtinger-derivatives) $\partial_z=(\partial_x-i\partial_y)/2$ and $\partial_{\bar z}=(\partial_x+i\partial_y)/2$, for which $\Delta=4\partial_z\partial_{\bar z}$. Since $H$ and $G$ are [holomorphic](../../holomorphic-function.md),

$$
\partial_{\bar z}F=H(z),\qquad \Delta F=4H'(z),\qquad \Delta^2F=16\partial_z\partial_{\bar z}H'(z)=0.
$$

The [Laplacian](../../multivariable-calculus.md#laplacian) has real coefficients, so taking real and imaginary parts proves

$$
\boxed{\Delta^2U=0,\qquad\Delta^2V=0.}
$$

This is the [complex analytic representation of biharmonic functions](../../multivariable-calculus.md#complex-analytic-representation-of-biharmonic-functions); $F$ itself is generally not holomorphic because of its $\bar z$ factor.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/i">i</h3>

↑ **Parent:** [8](#8)

<h4 id="8/i/solution">Solution</h4>

↑ **Parent:** [I](#8/i)

Set $y=\sum_{j\geq0}a_jx^j$ and equate coefficients in the [power series](../../sequence-and-series.md#power-series). The constant coefficient gives $a_2=0$. For $m\geq1$, the coefficient of $x^m$ gives

$$
(m+2)(m+1)a_{m+2}-[(m-1)(m-2)+6(m-1)+6]a_{m-1}=0.
$$

The square bracket is $(m+1)(m+2)$, so the [recurrence relation](../../sequence-and-series.md#recurrence-relation) is $a_{j+3}=a_j$ for $j\geq0$. The [initial conditions](../../differential-equation.md#initial-condition) give $a_0=1$, $a_1=0$, $a_2=0$. Hence

$$
\boxed{y(x)=1+x^3+x^6+x^9+\cdots,\qquad |x|<1.}
$$

<h3 id="8/ii">ii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8/ii)

Summing the [geometric series](../../sequence-and-series.md#geometric-series) gives

$$
\boxed{y(x)=\frac1{1-x^3}.}
$$

There is a particularly short verification using the [product rule](../../calculus.md#product-rule):

$$
(1-x^3)y''-6x^2y'-6xy=\bigl[(1-x^3)y\bigr]''=1''=0.
$$

Also $y(0)=1$ and $y'(0)=0$. The [radius of convergence](../../sequence-and-series.md#radius-of-convergence) of the series is one, set by the three complex cube roots of unity; the closed expression continues the solution beyond that disk wherever its denominator is nonzero. The real initial-value solution extends on the interval $(-\infty,1)$.

<h3 id="8/iii">iii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8/iii)

Substitute $y=vP_n$ into the [Legendre differential equation](../../linear-ordinary-differential-equation.md#legendre-differential-equation) and expand using the [product rule](../../calculus.md#product-rule). The terms proportional to $v$ cancel because $P_n$ is itself a solution. What remains is

$$
\boxed{(1-x^2)P_nv''+\left[2(1-x^2)P_n'-2xP_n\right]v'=0.}
$$

Multiplying by $P_n$ identifies an exact [derivative](../../calculus.md#derivative):

$$
\boxed{\frac{d}{dx}\left[(1-x^2)P_n^2v'\right]=0.}
$$

The latter form is convenient for [reduction of order](../../linear-ordinary-differential-equation.md#reduction-of-order) on intervals where $P_n\ne0$ and $x\ne\pm1$.

<h3 id="8/iv">iv</h3>

↑ **Parent:** [8](#8)

<h4 id="8/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#8/iv)

Two integrations give the general [reduction of order](../../linear-ordinary-differential-equation.md#reduction-of-order) formula

$$
\boxed{v(x)=C_1+C_2\int^x\frac{dt}{(1-t^2)P_n(t)^2},\qquad y(x)=P_n(x)\left[C_1+C_2\int^x\frac{dt}{(1-t^2)P_n(t)^2}\right].}
$$

The integral is local on intervals avoiding zeros of $P_n$. A pole of the integral at an interior polynomial zero need not be a singularity of $y$: the product extends by [reduction of order across a zero of the known solution](../../linear-ordinary-differential-equation.md#reduction-of-order-across-a-zero-of-the-known-solution). After a standard normalization the independent second solution is the [Legendre function of the second kind](../../linear-ordinary-differential-equation.md#legendre-function-of-the-second-kind) $Q_n$.

<h3 id="8/v">v</h3>

↑ **Parent:** [8](#8)

<h4 id="8/v/solution">Solution</h4>

↑ **Parent:** [V](#8/v)

For normalized [Legendre polynomials](../../linear-ordinary-differential-equation.md#legendre-polynomial), $P_n(1)=1$ and $P_n(-1)=(-1)^n$. Near the endpoints the integral factor has the asymptotics

$$
\int^x\frac{dt}{(1-t^2)P_n(t)^2}=-\frac12\log|1-x|+O(1)\quad(x\to1),
$$

and

$$
\int^x\frac{dt}{(1-t^2)P_n(t)^2}=\frac12\log|1+x|+O(1)\quad(x\to-1).
$$

Thus an independent solution, for which $C_2\ne0$, has the logarithmic endpoint singularities

$$
\boxed{y=-\frac{C_2}{2}\log|1-x|+O(1)\quad(x\to1),\qquad y=\frac{(-1)^nC_2}{2}\log|1+x|+O(1)\quad(x\to-1).}
$$

The constants are understood for a solution continued consistently across the ordinary interior points. Adding any multiple of $P_n$ cannot cancel these logarithms. This explains why boundedness at an endpoint selects the [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) and excludes the independent [Legendre function of the second kind](../../linear-ordinary-differential-equation.md#legendre-function-of-the-second-kind).

<h3 id="8/vi">vi</h3>

↑ **Parent:** [8](#8)

<h4 id="8/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#8/vi)

Write $P_n(x)\sim c_nx^n$ with $c_n\ne0$. For $n\geq1$, this branch grows. Choosing the other [reduction of order](../../linear-ordinary-differential-equation.md#reduction-of-order) solution by an integral from infinity gives, on $x>1$,

$$
P_n(x)\int_\infty^x\frac{dt}{(1-t^2)P_n(t)^2}\sim\frac{x^{-n-1}}{c_n(2n+1)}.
$$

Thus **for $n\geq1$, every bounded exterior solution decays as $|x|^{-n-1}$**, up to a constant factor, on each exterior interval. Equivalently the dominant-balance exponents in the [Legendre differential equation](../../linear-ordinary-differential-equation.md#legendre-differential-equation) are $n$ and $-n-1$.

There is an important exception at degree zero. Since $P_0=1$,

$$
\boxed{y=C_1+\frac{C_2}{2}\log\left|\frac{x+1}{x-1}\right|=C_1+\frac{C_2}{x}+O(|x|^{-3})\quad(n=0).}
$$

These solutions are bounded even when $C_1\ne0$; boundedness alone does not then imply decay to zero. The constants on $x>1$ and $x<-1$ are independent unless continuation across the singular endpoints is specified.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/i">i</h3>

↑ **Parent:** [9](#9)

<h4 id="9/i/solution">Solution</h4>

↑ **Parent:** [I](#9/i)

For a variation $y+\varepsilon\eta$ with $\eta(a)=\eta(b)=0$, the first variation of the [functional](../../calculus-of-variations.md#functional) is

$$
\delta I=\int_a^b(F_y\eta+F_{y'}\eta')dx=\int_a^b\left(F_y-\frac{d}{dx}F_{y'}\right)\eta\,dx.
$$

The boundary term vanishes by the fixed endpoints. The [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore gives the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation)

$$
\boxed{\frac{d}{dx}F_{y'}-F_y=0.}
$$

<h3 id="9/ii">ii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9/ii)

A missing explicit dependence produces a [first integral](../../differential-equation.md#first-integral) of the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation). The two cases follow by differentiating the candidate conserved quantity, as shown in the child solutions.

<h4 id="9/ii/a">a</h4>

↑ **Parent:** [Ii](#9/ii)

<h5 id="9/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#9/ii/a)

When $F_y=0$, the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) reduces immediately to $dF_{y'}/dx=0$. Therefore

$$
\boxed{F_{y'}=C.}
$$

This is conservation of the generalized momentum associated with a [cyclic coordinate](../../lagrangian-mechanics.md#cyclic-coordinate).

<h4 id="9/ii/b">b</h4>

↑ **Parent:** [Ii](#9/ii)

<h5 id="9/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#9/ii/b)

Along a differentiable curve, the [chain rule](../../calculus.md#chain-rule) gives

$$
\frac{d}{dx}(F-y'F_{y'})=F_x+y'F_y-y'\frac{dF_{y'}}{dx}=F_x
$$

by the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation). Thus when $F_x=0$ the [Beltrami identity](../../analysis.md#beltrami-identity) is

$$
\boxed{F-y'F_{y'}=C.}
$$

<h3 id="9/iii">iii</h3>

↑ **Parent:** [9](#9)

<h4 id="9/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9/iii)

Here $F$ has no explicit $x$ dependence, so use the [Beltrami identity](../../analysis.md#beltrami-identity). With $p=y'$, one has $F_{y'}=yp/\sqrt{1+p^2}$ and therefore

$$
\boxed{\frac{y}{\sqrt{1+(y')^2}}-\lambda y=C.}
$$

This [first integral](../../differential-equation.md#first-integral) reduces the second-order [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) to a first-order relation.

<h3 id="9/iv">iv</h3>

↑ **Parent:** [9](#9)

<h4 id="9/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#9/iv)

Choose the tangent angle $\psi=\arctan y'$ in $(-\pi/2,\pi/2)$, so $1/\sqrt{1+(y')^2}=\cos\psi$. At the maximum, the [first integral](../../differential-equation.md#first-integral) has value $C=y_0(1-\lambda)$. Hence

$$
y\cos\psi-\lambda y=y_0(1-\lambda),\qquad
\boxed{\lambda=\frac{y_0-y\cos\psi}{y_0-y}=1+\frac{y(1-\cos\psi)}{y_0-y}.}
$$

A nonconstant regular branch below its positive maximum has $y>0$ and $\psi\ne0$, giving **$\lambda>1$**. For completeness, strictness follows from the differential equation rather than assuming it at every point: the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) simplifies to

$$
yy''=1+(y')^2-\lambda[1+(y')^2]^{3/2}.
$$

At the maximum, $y_0y''=1-\lambda$ implies $\lambda\geq1$. If $\lambda=1$, the positive-height initial data $y=y_0$, $y'=0$ give the constant solution uniquely, contradicting the existence of the lower-height branch. Thus $\lambda=1$ is only the degenerate horizontal solution. The first integral with $\lambda>1$ also excludes $y=0$ on this regular branch.

<h3 id="9/v">v</h3>

↑ **Parent:** [9](#9)

<h4 id="9/v/solution">Solution</h4>

↑ **Parent:** [V](#9/v)

Rearrange the [first integral](../../differential-equation.md#first-integral) from part (iv) and use the [half-angle identities](../../geometry-and-topology.md#half-angle-identities):

$$
\lambda-1=\frac{2y\sin^2(\psi/2)}{y_0-y}=\frac{2y_1\sin^2(\alpha/2)}{y_0-y_1}.
$$

Eliminating $\lambda$ gives

$$
\boxed{\sin^2\frac\psi2=\frac{y_1}{y}\frac{y_0-y}{y_0-y_1}\sin^2\frac\alpha2,\qquad y_1<y<y_0.}
$$

Squaring removes the sign of the slope; the rising and falling sides of the same profile have opposite tangent angles but obey the same height relation. Heights and angles must remain on the regular branch with $\cos\psi>0$.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/i">i</h3>

↑ **Parent:** [10](#10)

<h4 id="10/i/solution">Solution</h4>

↑ **Parent:** [I](#10/i)

The time dependence gives $u_{tt}=-\omega^2u$, and the angular derivative vanishes for these radial [normal modes](../../wave-equation.md#normal-mode). The [Laplacian](../../multivariable-calculus.md#laplacian) in [polar coordinates](../../multivariable-calculus.md#polar-coordinates) therefore yields

$$
R''+\frac1rR'+\frac{\omega^2}{c^2}R=0.
$$

Multiplication by $r$ puts the [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) in the form

$$
\boxed{-(rR')'=\lambda rR,\qquad p(r)=r,\quad q(r)=0,\quad w(r)=r,\quad\lambda=\omega^2/c^2.}
$$

The relevant [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) is $\mathcal A R=-r^{-1}(rR')'$ in the [weighted inner product](../../inner-product.md#weighted-inner-product) with weight $r$. A physical displacement is regular at the origin, excluding the logarithmic singular solution. In particular $R$ is bounded and $rR'\to0$ there; regular eigenfunctions also have $R'(0)=0$. This origin condition is needed in addition to the fixed outer boundary.

<h3 id="10/ii">ii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10/ii)

The conditions of regularity at $r=0$ and $R(a)=0$ select the [radial vibrations of a circular membrane](../../wave-equation.md#radial-vibrations-of-a-circular-membrane) as an [eigenvalue problem](../../linear-operator-theory.md#eigenvalue-problem). Multiply $-(rR')'=\lambda rR$ by $\overline R$ and integrate. [Integration by parts](../../calculus.md#integration-by-parts) gives

$$
\lambda\int_0^ar|R|^2dr=\int_0^ar|R'|^2dr-[r\overline RR']_0^a=\int_0^ar|R'|^2dr.
$$

The boundary term vanishes by regularity and $R(a)=0$. For a nonzero eigenfunction the denominator is positive; the numerator could vanish only for a constant function, and the outer condition would then make that function zero. Consequently

$$
\boxed{\lambda=\frac{\int_0^ar|R'|^2dr}{\int_0^ar|R|^2dr}>0,\qquad \nu=\frac{c\sqrt\lambda}{2\pi}\in\mathbb R.}
$$

This also proves reality without presuming real-valued eigenfunctions. Explicitly, regular solutions are [Bessel functions of the first kind](../../bessel-function.md#bessel-function-of-the-first-kind) $R=J_0(\sqrt\lambda r)$, and the positive zeros of $J_0(\sqrt\lambda a)$ give the discrete spectrum.

<h3 id="10/iii">iii</h3>

↑ **Parent:** [10](#10)

<h4 id="10/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10/iii)

Use the [weighted inner product](../../inner-product.md#weighted-inner-product)

$$
\boxed{\langle R_m,R_n\rangle_r=\int_0^ar\overline{R_m(r)}R_n(r)\,dr.}
$$

Multiply the equation for $R_n$ by $\overline R_m$, subtract the complex conjugate equation for $R_m$ times $R_n$, and integrate. Since the [eigenvalues](../../linear-operator-theory.md#eigenvalue) are real,

$$
(\lambda_n-\lambda_m)\langle R_m,R_n\rangle_r=\left[r\left(\overline{R_m'}R_n-\overline R_mR_n'\right)\right]_0^a=0.
$$

The boundary term vanishes as before. Thus **eigenfunctions with distinct eigenvalues are orthogonal**. The full disk [inner product](../../inner-product.md) differs only by the angular factor $2\pi$.

<h3 id="10/iv">iv</h3>

↑ **Parent:** [10](#10)

<h4 id="10/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#10/iv)

The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) bounds the lowest [eigenvalue](../../linear-operator-theory.md#eigenvalue) by the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) of any nonzero admissible trial function. For $f=1-(r/a)^p$, take $p>0$, which ensures boundedness, the outer [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition), and finite radial Dirichlet energy. Direct [integration](../../integral.md) gives

$$
\int_0^ar(f')^2dr=\frac p2,\qquad\int_0^arf^2dr=a^2\left[\frac12-\frac2{p+2}+\frac1{2p+2}\right]=\frac{a^2p^2}{2(p+1)(p+2)}.
$$

Therefore

$$
\lambda_1\leq\frac{(p+1)(p+2)}{a^2p}=\frac1{a^2}\left(p+3+\frac2p\right).
$$

The derivative is $1-2/p^2$, so the unique minimizing positive exponent is $p=\sqrt2$. This yields the [power-law variational bound for a circular membrane](../../wave-equation.md#power-law-variational-bound-for-a-circular-membrane)

$$
\boxed{\lambda_1\leq\frac{3+2\sqrt2}{a^2},\qquad \nu_1\leq\frac{c(1+\sqrt2)}{2\pi a}\simeq0.384234\,\frac ca.}
$$

The optimizing function has zero derivative at the origin and is admissible for the energy principle despite its unbounded second derivative there. For comparison, the exact radial fundamental has $\sqrt{\lambda_1}a\simeq2.404826$, giving $\nu_1\simeq0.382740\,c/a$. The bound is about $0.39\%$ above this value.

## ↑ Ancestors (10)

1. [2013](../2013.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
