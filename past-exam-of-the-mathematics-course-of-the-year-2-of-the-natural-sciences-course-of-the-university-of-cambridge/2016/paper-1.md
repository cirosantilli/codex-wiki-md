# Paper 1

↑ **Parent:** [2016](../2016.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2016/papernst_ib_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2016/papernst_ib_1.pdf)

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
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
    - [iii](#5/c/iii)
      - [Solution](#5/c/iii/solution)
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
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)
    - [iii](#7/b/iii)
      - [Solution](#7/b/iii/solution)
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
    - [i](#9/b/i)
      - [Solution](#9/b/i/solution)
    - [ii](#9/b/ii)
      - [Solution](#9/b/ii/solution)
- [10](#10)
  - [a](#10/a)
    - [i](#10/a/i)
      - [Solution](#10/a/i/solution)
    - [ii](#10/a/ii)
      - [Solution](#10/a/ii/solution)
    - [iii](#10/a/iii)
      - [Solution](#10/a/iii/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a bounded volume $V$ with piecewise smooth closed boundary $S=\partial V$, and a continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) $\mathbf F$ on a neighbourhood of $\overline V$, the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) states

$$
\boxed{\iint_S\mathbf F\cdot\hat{\mathbf n}\,dS=\iiint_V\nabla\cdot\mathbf F\,dV.}
$$

Here $\hat{\mathbf n}$ is the outward [unit normal vector](../../differential-geometry.md#unit-normal). The left side is the outward [flux](../../mathematical-physics.md#flux); the right side integrates the [divergence](../../multivariable-calculus.md#divergence) over the enclosed volume.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The upper piece is a downward-opening circular [elliptic paraboloid](../../euclidean-geometry.md#elliptic-paraboloid) cap, running from the circle $r=1,z=1$ to the apex $r=0,z=2$. The middle piece is the side of a circular [cylinder](../../geometry-and-topology.md#cylinder-geometry) of radius one and height one. The lower piece is the unit [disk](../../topology.md#disk-mathematics) in the horizontal plane. Their union is the closed boundary of

$$
V=\{(x,y,z):0\leq z\leq1,\ x^2+y^2\leq1\}\ \cup\ \{(x,y,z):1\leq z\leq2,\ x^2+y^2\leq2-z\}.
$$

The four panels show the three separate pieces and their union; there is no additional fourth component. In a meridional section, the boundary consists of the base segment, two vertical sides, and the parabolic cap. The outward normals point downward on the base, radially outward on the cylindrical side, and upward/outward on the cap.

<a id="1/b/image-three-boundary-pieces-and-their-closed-union-shown-as-original-surfaces-of-revolution"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-q1-closed-surface.png)

**[Figure 1](#1/b/image-three-boundary-pieces-and-their-closed-union-shown-as-original-surfaces-of-revolution). Three boundary pieces and their closed union, shown as original surfaces of revolution**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [polynomial](../../polynomial.md) [vector field](../../multivariable-calculus.md#vector-field) is smooth throughout the solid, so the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) applies. Differentiation gives

$$
\nabla\cdot\mathbf F=(2y+6x^5)+(-2y+4y^3)+1=6x^5+4y^3+1.
$$

The volume is invariant under both $x\mapsto-x$ and $y\mapsto-y$. Hence the [integrals](../../integral.md) of the two odd terms vanish, and the [flux](../../mathematical-physics.md#flux) is simply the volume. Using the circular cross-sections,

$$
\iint_S\mathbf F\cdot d\mathbf S=\pi\int_0^1 dz+\pi\int_1^2(2-z)\,dz=\boxed{\frac{3\pi}{2}}.
$$

The seams between the surface pieces have zero surface measure and contribute no extra term.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Set $y(x,t)=X(x)T(t)$ in the [wave equation](../../wave-equation.md). A nonzero product obtained by [separation of variables](../../partial-differential-equation.md#separation-of-variables) obeys

$$
\frac{X''}{X}=\frac{T''}{c^2T}=-k^2.
$$

The fixed-end [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) require $X(0)=X(L)=0$. The zero and negative spatial [eigenvalue](../../linear-operator-theory.md#eigenvalue) cases produce only the trivial solution; the nontrivial [eigenfunctions](../../linear-operator-theory.md#eigenfunction) are

$$
X_n(x)=\sin\frac{n\pi x}{L},\qquad k_n=\frac{n\pi}{L},\qquad\omega_n=ck_n,\qquad n=1,2,\ldots.
$$

For each [normal mode](../../wave-equation.md#normal-mode), $T_n''+\omega_n^2T_n=0$. By [superposition](../../vector-space.md#superposition-principle) and completeness of the [Fourier sine basis](../../fourier-series.md#fourier-sine-basis), the general finite-energy solution has the expansion

$$
\boxed{y(x,t)=\sum_{n=1}^{\infty}\left[A_n\cos\omega_nt+B_n\sin\omega_nt\right]\sin\frac{n\pi x}{L}.}
$$

If $f(x)=y(x,0)$ and $g(x)=y_t(x,0)$, [orthogonality](../../inner-product.md#orthogonal-vectors) gives $A_n=(2/L)\int_0^Lf(x)\sin(k_nx)\,dx$ and $B_n=2\int_0^Lg(x)\sin(k_nx)\,dx/(L\omega_n)$. Individual products are separable; their sum is the general solution.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Assume the struck interval lies within the string, so $0\leq\ell-a/2<\ell+a/2\leq L$. The initially stationary straight string has $A_n=0$. Write its initial velocity as a [Fourier sine series](../../fourier-series.md#fourier-sine-series) $g(x)=\sum_ng_n\sin(k_nx)$. Then

$$
g_n=\frac{2v}{L}\int_{\ell-a/2}^{\ell+a/2}\sin\frac{n\pi x}{L}\,dx=\frac{4v}{n\pi}\sin\frac{n\pi\ell}{L}\sin\frac{n\pi a}{2L}.
$$

Thus $y(x,t)=\sum_n(g_n/\omega_n)\sin(\omega_nt)\sin(k_nx)$. Immediately after the strike all the [energy](../../energy.md) is [kinetic energy](../../energy.md#kinetic-energy):

$$
E=\frac\rho2\int_0^L g(x)^2\,dx=\frac{\rho av^2}{2}.
$$

The [orthogonality](../../inner-product.md#orthogonal-vectors) [integral](../../integral.md) $\int_0^L\sin(k_nx)\sin(k_mx)\,dx=(L/2)\delta_{nm}$ assigns [energy](../../energy.md) $E_n=\rho Lg_n^2/4$ to mode $n$. Since the ideal modes evolve independently, their total kinetic-plus-elastic energies remain constant. Therefore the [modal energy of a localized velocity impulse on a string](../../wave-equation.md#modal-energy-of-a-localized-velocity-impulse-on-a-string) gives

$$
\boxed{\frac{E_n}{E}=\frac{8L}{a\pi^2n^2}\sin^2\frac{n\pi\ell}{L}\sin^2\frac{n\pi a}{2L}.}
$$

The centre factor selects modes having significant motion at the impact location; the width factor accounts for cancellation across the finite hammer footprint. [Parseval's identity](../../fourier-analysis.md#parseval-identity) ensures $\sum_{n\geq1}E_n/E=1$. The velocity discontinuities are understood in the mean-square sense and do not alter the [energy](../../energy.md) [integrals](../../integral.md).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

With the specified ratios, the two factors in the modal amplitude become $\sin(n\pi/5)$ and $\sin(n\pi/14)$. Hence a [normal mode](../../wave-equation.md#normal-mode) is unexcited precisely when one of these factors is zero:

$$
\boxed{n\in5\mathbb N\ \cup\ 14\mathbb N.}
$$

That includes all multiples of five or fourteen, with multiples of seventy counted once. The mode $n=0$ is not a fixed-end string mode.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Away from $x=\xi$, the homogeneous equation has solutions $e^x,e^{-x}$. A basis adapted to the two [boundary conditions](../../differential-equation.md#boundary-condition) is $u(x)=\sinh x$ at the origin and $v(x)=e^{-x}$ at infinity. Their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is $uv'-u'v=-1$. The [Green function](../../green-s-function.md) must be continuous at $\xi$, while [integration](../../integral.md) of $-G_{xx}+G=\delta(x-\xi)$ across the source gives

$$
G_x(\xi+,\xi)-G_x(\xi-,\xi)=-1.
$$

These conditions give the [Dirichlet half-line Green function for minus d2 plus 1](../../green-s-function.md#dirichlet-half-line-green-function-for-minus-d2-plus-1):

$$
\boxed{G(x,\xi)=\sinh(x_<)e^{-x_>}=\frac12\left(e^{-|x-\xi|}-e^{-(x+\xi)}\right),}
$$

where $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. The second term is the image that enforces $G(0,\xi)=0$; both terms decay as $x\to\infty$.

For the finite forcing interval, $y(x)=\int_0^\mu G(x,\xi)\,d\xi$. When $x\leq\mu$, split the [integral](../../integral.md) at $\xi=x$:

$$
y(x)=e^{-x}\int_0^x\sinh\xi\,d\xi+\sinh x\int_x^\mu e^{-\xi}\,d\xi=1-e^{-x}-e^{-\mu}\sinh x.
$$

When $x\geq\mu$, the entire source interval lies to the left, giving the [Dirichlet half-line response to uniform interval forcing](../../green-s-function.md#dirichlet-half-line-response-to-uniform-interval-forcing)

$$
\boxed{y(x)=\begin{cases}1-e^{-x}-e^{-\mu}\sinh x,&0\leq x\leq\mu,\\(\cosh\mu-1)e^{-x},&x\geq\mu.\end{cases}}
$$

This solution is unique: a homogeneous difference satisfying the origin condition is proportional to $\sinh x$, which cannot decay at infinity unless its coefficient is zero.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The left-hand value at the junction is

$$
y(\mu-)=1-e^{-\mu}-e^{-\mu}\sinh\mu=\frac12-e^{-\mu}+\frac12e^{-2\mu}.
$$

The right-hand value is

$$
y(\mu+)=(\cosh\mu-1)e^{-\mu}=\frac12+\frac12e^{-2\mu}-e^{-\mu}.
$$

Thus the piecewise [Green function](../../green-s-function.md) solution is [continuous](../../calculus.md#continuous-function), with

$$
\boxed{y(\mu)=\frac12(1+e^{-2\mu}-2e^{-\mu})=\frac12(1-e^{-\mu})^2.}
$$

Its [derivative](../../calculus.md#derivative) is continuous as well: both one-sided values equal $-\tfrac12(1-e^{-\mu})^2$. Only the second [derivative](../../calculus.md#derivative) jumps, consistently with the step in the forcing and the absence of a [Dirac delta](../../distribution-theory.md#dirac-delta-function) source.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the [Fourier transform](../../fourier-transform.md) convention

$$
\widetilde f(\omega)=\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt,\qquad f(t)=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde f(\omega)e^{i\omega t}\,d\omega.
$$

Since $\mathcal F[e^{i\Omega t}]=2\pi\delta(\omega-\Omega)$ in [distribution theory](../../distribution-theory.md), the carrier has transform

$$
\boxed{\widetilde c(\omega)=\pi[\delta(\omega-\Omega)+\delta(\omega+\Omega)].}
$$

The [modulation property of the Fourier transform](../../fourier-transform.md#modulation-property-of-the-fourier-transform) translates the message spectrum to the two carrier frequencies. Therefore

$$
\boxed{\widetilde\phi(\omega)=\pi[\delta(\omega-\Omega)+\delta(\omega+\Omega)]+\frac12[\widetilde s(\omega-\Omega)+\widetilde s(\omega+\Omega)].}
$$

The first term represents the unmodulated [carrier wave](../../dispersion-relation.md#carrier-wave); the other terms are the [amplitude modulation sidebands](../../electrical-engineering.md#amplitude-modulation-sidebands).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A direct way to avoid the singular transform of $1/t^2$ is to invert a [triangular function](../../fourier-analysis.md#triangular-function). Evenness gives

$$
\frac1{2\pi}\int_{-1}^1\pi(1-|\omega|)e^{i\omega t}\,d\omega=\int_0^1(1-\omega)\cos(\omega t)\,d\omega=\frac{1-\cos t}{t^2}.
$$

At $t=0$ the limit is $1/2$, so there is no singularity in the original signal. Thus

$$
\boxed{\widetilde s(\omega)=\pi(1-|\omega|)_+,\qquad (r)_+=\max(r,0).}
$$

Alternatively, the hint uses the [Hadamard finite-part reciprocal-power distribution](../../distribution-theory.md#hadamard-finite-part-reciprocal-power-distribution), whose [distributional Fourier transform](../../fourier-analysis.md#fourier-transform-of-a-tempered-distribution) is $\mathcal F[\operatorname{fp}(1/t^2)]=-\pi|\omega|$; combining its three translates gives $\pi(|\omega-1|+|\omega+1|-2|\omega|)/2$, the same triangle. Treating $1/t^2$ as an ordinary integrable function would be invalid.

The message spectrum has height $\pi$ at zero, vanishing at $\omega=\pm1$. For $\Omega>1$, the modulated continuous spectrum consists of disjoint triangles of height $\pi/2$, centred at $\pm\Omega$, each with half-width one. In addition there is a [Dirac delta](../../distribution-theory.md#dirac-delta-function) carrier line of weight $\pi$ at each centre. These lines have specified area, not a finite height; arrows mark them schematically.

<a id="4/b/image-triangular-message-spectrum-separated-sidebands-and-overlapping-sidebands-with-the-prescribed-carrier-rejecting-filter"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-q4-modulation-spectra.png)

**[Figure 2](#4/b/image-triangular-message-spectrum-separated-sidebands-and-overlapping-sidebands-with-the-prescribed-carrier-rejecting-filter). Triangular message spectrum, separated sidebands, and overlapping sidebands with the prescribed carrier-rejecting filter**.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

At $\Omega=3/4$, the two continuous triangles overlap near zero. Their amplitudes add, giving a central plateau. Explicitly, write $C(\omega)$ for the continuous part of $\widetilde\phi$:

$$
C(\omega)=\begin{cases}\pi/4,&|\omega|\leq1/4,\\\dfrac\pi2(1/4+|\omega|),&1/4<|\omega|\leq3/4,\\\dfrac\pi2(7/4-|\omega|),&3/4<|\omega|<7/4,\\0,&|\omega|\geq7/4.\end{cases}
$$

There are also the two carrier [Dirac delta](../../distribution-theory.md#dirac-delta-function) lines $\pi\delta(\omega\mp3/4)$. The last panel of the preceding figure shows this spectrum and the retained central portion. The prescribed strict cutoff removes the carriers and keeps

$$
\boxed{\widetilde\rho(\omega)=\begin{cases}\pi/4,&|\omega|\leq1/4,\\\dfrac\pi2(1/4+|\omega|),&1/4<|\omega|<3/4,\\0,&|\omega|\geq3/4.\end{cases}}
$$

The values of the ordinary function at individual endpoints do not affect its inverse transform. To handle the carrier lines, one must additionally assign zero filter gain to those lines, as the carrier-rejecting prescription indicates. A discontinuous mask has no canonical product with a [Dirac delta](../../distribution-theory.md#dirac-delta-function) at its discontinuity; a different physical boundary gain would leave a corresponding multiple of $\cos(3t/4)$.

The retained spectrum is real and even. Its inverse [Fourier transform](../../fourier-transform.md) is

$$
\rho(t)=\frac14\int_0^{1/4}\cos(\omega t)\,d\omega+\frac12\int_{1/4}^{3/4}(1/4+\omega)\cos(\omega t)\,d\omega.
$$

Integrating the linear factors yields

$$
\boxed{\rho(t)=\frac{\sin(3t/4)}{2t}+\frac{\cos(3t/4)-\cos(t/4)}{2t^2},\qquad t\neq0.}
$$

The removable value is $\boxed{\rho(0)=1/4}$, obtained either by expansion or by integrating $\widetilde\rho/(2\pi)$. Because the carrier [frequency](../../wave.md#frequency) is below the message bandwidth, this is [Fourier filtering of overlapping amplitude-modulation sidebands](../../electrical-engineering.md#fourier-filtering-of-overlapping-amplitude-modulation-sidebands); the usual picture of two isolated bands in [single-sideband modulation](../../electrical-engineering.md#single-sideband-modulation) does not apply without that qualification.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The inverse is assumed to exist. First,

$$
(I+M)(I-M)=I-M^2=(I-M)(I+M).
$$

By [matrix commutation with an inverse](../../matrix-inverse.md#matrix-commutation-with-an-inverse), multiplying on both sides by $(I-M)^{-1}$ gives

$$
\boxed{(I+M)(I-M)^{-1}=(I-M)^{-1}(I+M).}
$$

An equivalent calculation writes $I+M=2I-(I-M)$, so both products equal $2(I-M)^{-1}-I$. No convergent infinite [matrix](../../vector-space.md#matrix) series is needed.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $Q$ be the real [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix). If $Qv=\lambda v$ for a nonzero complex [eigenvector](../../linear-operator-theory.md#eigenvector), then preservation of the complex Euclidean [norm](../../normed-vector-space.md#norm) gives

$$
\|v\|^2=\|Qv\|^2=|\lambda|^2\|v\|^2,
$$

so $|\lambda|=1$. Its [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) has real coefficients, hence nonreal [eigenvalues](../../linear-operator-theory.md#eigenvalue) occur in conjugate pairs. Such a pair is $e^{i\alpha},e^{-i\alpha}$, and the remaining real [eigenvalue](../../linear-operator-theory.md#eigenvalue) is $+1$ or $-1$.

If all three [eigenvalues](../../linear-operator-theory.md#eigenvalue) are real, each is $\pm1$; two have the same sign and can be paired as $e^{\pm i\alpha}$ with $\alpha=0$ or $\pi$. Thus in every case the spectrum has the form

$$
\boxed{\{e^{i\alpha},e^{-i\alpha},\varepsilon\},\quad\alpha\in\mathbb R,\quad\varepsilon=\pm1.}
$$

Their product shows that $\varepsilon=\det Q$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

First, $I-A$ is invertible. If $(I-A)x=0$ for a real [vector](../../vector-space.md#vector), then $Ax=x$, whereas the [skew-symmetric matrix](../../linear-algebra.md#skew-symmetric-matrix) identity gives $x^TAx=0$; hence $x^Tx=0$ and $x=0$. Thus its real [kernel](../../kernel-of-a-linear-map.md) is trivial, which suffices for invertibility. The same argument applies to $I+A$.

Using $A^T=-A$ and the rule for the [transpose](../../vector-space.md#transpose) of a product,

$$
N^T=[(I-A)^{-1}]^T(I+A)^T=(I+A)^{-1}(I-A).
$$

The factors $I+A$ and $I-A$ commute, as do the required inverses. Consequently

$$
N^TN=(I+A)^{-1}(I-A)(I+A)(I-A)^{-1}=I.
$$

Thus $\boxed{N\text{ is orthogonal}}$. This is the [Cayley transform of a real skew-symmetric matrix](../../lie-theory.md#cayley-transform-of-a-real-skew-symmetric-matrix).

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

For a possibly complex [eigenvector](../../linear-operator-theory.md#eigenvector) $v\neq0$ with $Av=\lambda v$, invertibility of $I-A$ gives $(I-A)^{-1}v=(1-\lambda)^{-1}v$. Therefore

$$
\boxed{Nv=\frac{1+\lambda}{1-\lambda}v,\qquad\nu=\frac{1+\lambda}{1-\lambda}.}
$$

Thus every [eigenvector](../../linear-operator-theory.md#eigenvector) of $A$ remains an [eigenvector](../../linear-operator-theory.md#eigenvector) of $N$. For a real [skew-symmetric matrix](../../linear-algebra.md#skew-symmetric-matrix), its [eigenvalues](../../linear-operator-theory.md#eigenvalue) have the form $\lambda=it$ with $t$ real, so $\nu=e^{2i\arctan t}$ lies on the [unit circle](../../complex-analysis.md#complex-unit-circle), consistently with [orthogonality](../../inner-product.md#orthogonal-vectors).

<h4 id="5/c/iii">iii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/c/iii)

Taking [determinants](../../multilinear-algebra.md#determinant) and using invariance under [transpose](../../vector-space.md#transpose),

$$
\det(I+A)=\det((I+A)^T)=\det(I-A),\qquad\boxed{\det N=1.}
$$

This [determinant](../../multilinear-algebra.md#determinant) identity actually holds in every dimension. In dimension three, skew symmetry additionally gives

$$
\det A=\det A^T=\det(-A)=(-1)^3\det A=-\det A,
$$

so $\det A=0$. Hence there is a real nonzero [vector](../../vector-space.md#vector) $x$ in the [kernel](../../kernel-of-a-linear-map.md):

$$
\boxed{Ax=0,\qquad x\neq0.}
$$

The [eigenvalue](../../linear-operator-theory.md#eigenvalue) relation then gives $Nx=x$. Thus the [Cayley transform](../../lie-theory.md#cayley-transform-lie-theory) fixes an axis and is a proper three-dimensional rotation, including the identity as a degenerate case.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A square [matrix](../../vector-space.md#matrix) $A$ is [diagonalizable](../../linear-operator-theory.md#diagonalizable-matrix) over a specified scalar field if an invertible [matrix](../../vector-space.md#matrix) $P$ exists such that

$$
\boxed{P^{-1}AP=D\quad\text{with }D\text{ diagonal}.}
$$

Equivalently, the underlying [vector space](../../vector-space.md) has a basis of [eigenvectors](../../linear-operator-theory.md#eigenvector) of $A$: those basis [vectors](../../vector-space.md#vector) are the columns of $P$, and their [eigenvalues](../../linear-operator-theory.md#eigenvalue) are the diagonal entries of $D$. Here the field is $\mathbb C$ unless specified otherwise.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Taking [determinants](../../multilinear-algebra.md#determinant) of $A^p=0$ gives $(\det A)^p=0$, so $A$ is singular and has the [eigenvalue](../../linear-operator-theory.md#eigenvalue) zero. More strongly, if $Av=\lambda v$ with $v\neq0$, then $0=A^pv=\lambda^pv$, so **every [eigenvalue](../../linear-operator-theory.md#eigenvalue) is zero**.

If the [nilpotent matrix](../../linear-operator-theory.md#nilpotent-matrix) were [diagonalizable](../../linear-operator-theory.md#diagonalizable-matrix), write $A=PDP^{-1}$. Then $0=A^p=PD^pP^{-1}$, hence each diagonal entry of $D$ has zero $p$th power and is zero. Thus $D=0$ and $A=0$. Conversely the zero [matrix](../../vector-space.md#matrix) is diagonal. Therefore

$$
\boxed{A^p=0:\quad A\text{ diagonalizable}\iff A=0.}
$$

The conclusion is valid over $\mathbb C$ and also over $\mathbb R$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Use the full $3\times3$ [matrix](../../vector-space.md#matrix) $B$ in the original PDF; the transcription has dropped its middle column. For either [matrix](../../vector-space.md#matrix), the three-dimensional [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $\chi_M(t)=t^3-(\operatorname{tr}M)t^2+[(\operatorname{tr}M)^2-\operatorname{tr}(M^2)]t/2-\det M$. Both have zero [trace](../../linear-algebra.md#matrix-trace) and zero [determinant](../../multilinear-algebra.md#determinant), while $\operatorname{tr}(B^2)=0$ and $\operatorname{tr}(C^2)=72$. Consequently

$$
\boxed{\chi_B(t)=t^3,\qquad\chi_C(t)=t(t-6)(t+6).}
$$

For $B$, a useful check is

$$
B^2=\begin{pmatrix}12&0&-24\\18&0&-36\\6&0&-12\end{pmatrix},\qquad B^3=0,
$$

for every value of $\alpha$. Thus $B$ is a nonzero [nilpotent matrix](../../linear-operator-theory.md#nilpotent-matrix) for all $\alpha$; for example its second column never vanishes. By the preceding result, $\boxed{B\text{ is not diagonalizable for any }\alpha}$.

For $C$, the three [eigenvalues](../../linear-operator-theory.md#eigenvalue) $-6,0,6$ are distinct and real, so their [eigenvectors](../../linear-operator-theory.md#eigenvector) are linearly independent. An explicit eigenbasis is

$$
v_- =\begin{pmatrix}-1\\0\\1\end{pmatrix},\qquad v_0=\begin{pmatrix}2\\-3\\1\end{pmatrix},\qquad v_+=\begin{pmatrix}2\\3\\1\end{pmatrix}.
$$

With $P=(v_-,v_0,v_+)$, $\det P=18\neq0$ and $P^{-1}CP=\operatorname{diag}(-6,0,6)$. Hence $\boxed{C\text{ is diagonalizable over }\mathbb R\text{ and }\mathbb C}$.

A repeated root of the [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) alone would not settle diagonalizability; for $B$ it is the nonzero nilpotence that completes the argument.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

A complex function is [holomorphic](../../holomorphic-function.md) at a point if it is complex differentiable throughout some open neighbourhood of that point. Writing $\zeta=\xi+i\eta$ and $\psi=P+iQ$, a convenient sufficient and necessary criterion under continuously differentiable real components is the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations)

$$
\boxed{P_\xi=Q_\eta,\qquad P_\eta=-Q_\xi.}
$$

They must hold throughout an open neighbourhood, rather than at an isolated point. Merely having partial [derivatives](../../calculus.md#derivative) that satisfy these equalities at one point is not enough without an appropriate differentiability hypothesis. For the composition $\psi=G\circ f$, [holomorphy](../../holomorphic-function.md) of $f$ and $G$ on the relevant open sets suffices; the additional condition $f'\neq0$ is needed when using a local inverse [conformal map](../../geometry-and-topology.md#conformal-map), not for [holomorphy](../../holomorphic-function.md) of the composition itself.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

Choose the branch of $\sqrt{(\zeta+1)(\zeta-1)}$ [holomorphic](../../holomorphic-function.md) in the [upper half-plane](../../complex-analysis.md#upper-half-plane-complex-analysis) whose boundary value at zero is $+i$. Then

$$
f'(\zeta)=\frac1{\sqrt{1-\zeta^2}},\qquad f(0)=0,
$$

and [integration](../../integral.md) gives $\boxed{z=\arcsin\zeta,\quad\zeta=\sin z}$ on this branch. The normalization and intended upper-half-plane image fix the otherwise ambiguous square-root sign.

To see the image, put $z=x+iy$. For $-\pi/2<x<\pi/2$ and $y>0$,

$$
\operatorname{Im}\sin z=\cos x\sinh y>0.
$$

The bottom edge maps monotonically onto $[-1,1]$. The right wall maps by $\sin(\pi/2+iy)=\cosh y$ onto $[1,\infty)$, and the left by $\sin(-\pi/2+iy)=-\cosh y$ onto $(-\infty,-1]$. These boundaries describe the [conformal map of a vertical half-strip by sine](../../geometry-and-topology.md#conformal-map-of-a-vertical-half-strip-by-sine).

For completeness, the map is one-to-one in the interior: equality of two sine values forces arguments differing by $2\pi m$ or summing to $(2m+1)\pi$, and neither alternative yields two distinct points in this half-strip. It is onto the [upper half-plane](../../complex-analysis.md#upper-half-plane-complex-analysis) as well. Setting $w=e^{iz}$ gives $w^2-2i\zeta w-1=0$; the root product is $-1$, and no root lies on $|w|=1$ because that would make $\zeta$ real. Thus exactly one root has $|w|<1$. The identity $\operatorname{Im}\zeta=(\operatorname{Re}w)(|w|^{-2}-1)/2$ then gives $\operatorname{Re}w>0$, so $z=-i\log w$ belongs to the half-strip. The closure gives the stated boundary-inclusive region; [holomorphy](../../holomorphic-function.md) is understood in its open interior.

In this region the transformed function is $G(z)=\log(2+\sin z)$. Its only finite intrinsic [branch point](../../complex-analysis.md#branch-point) in the closure occurs where $2+\sin z=0$:

$$
\boxed{z_*=-\frac\pi2+i\operatorname{arcosh}2=-\frac\pi2+i\log(2+\sqrt3),\qquad\zeta_*=-2.}
$$

It lies on the left boundary. There are no singularities in the open half-strip. The points $\zeta=\pm1$, where $f'$ diverges, map to the bottom corners; $G$ is [holomorphic](../../holomorphic-function.md) through those corners since $2+\sin z\neq0$ there.

For the principal logarithm, the boundary segment $z=-\pi/2+iy$, $y\geq\operatorname{arcosh}2$, is the preimage of its cut $\zeta\leq-2$. Points on that cut above $z_*$ admit local [analytic continuation](../../holomorphic-function.md#analytic-continuation) after changing branch; $z_*$ itself is the genuine logarithmic [branch point](../../complex-analysis.md#branch-point).

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

Writing $\zeta=\xi+i\eta$,

$$
u-iv=\frac1{\zeta+2}=\frac{\xi+2-i\eta}{(\xi+2)^2+\eta^2}.
$$

Therefore

$$
\boxed{\mathbf u=\frac{(\xi+2,\eta)}{(\xi+2)^2+\eta^2},\qquad |\mathbf u|=\frac1{\sqrt{(\xi+2)^2+\eta^2}}.}
$$

The [vector field](../../multivariable-calculus.md#vector-field) points radially **away from $(-2,0)$**, with magnitude inversely proportional to distance from that point. It diverges on approach to that boundary point and tends to zero far away. This is the radial [potential flow](../../fluid-mechanics.md#potential-flow) described by the logarithmic [complex potential of a two-dimensional potential flow](../../fluid-mechanics.md#complex-potential-of-a-two-dimensional-potential-flow).

<h4 id="7/b/iii">iii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/b/iii)

The [chain rule](../../calculus.md#chain-rule) gives

$$
\boxed{U-iV=\frac{dG}{dz}=\frac{d\psi/d\zeta}{df/d\zeta}=\frac{\cos z}{2+\sin z}.}
$$

To make the directions explicit, set $z=x+iy$ and $D=(2+\sin x\cosh y)^2+\cos^2x\sinh^2y$. Multiplying by the [complex conjugate](../../complex-analysis.md#complex-conjugate) of the denominator gives the [logarithmic flow in a sine-mapped half-strip](../../fluid-mechanics.md#logarithmic-flow-in-a-sine-mapped-half-strip):

$$
\boxed{U=\frac{\cos x(2\cosh y+\sin x)}D,\qquad V=\frac{\sinh y(\cosh y+2\sin x)}D.}
$$

In the open strip $U>0$. The vertical component is negative near the lower left wall where $\cosh y+2\sin x<0$, and positive above that curve. On the bottom the flow is rightward. On the right wall it is upward, whereas on the left wall it points downward below $z_*$ and upward above $z_*$. The field is tangent to the boundaries except at the source and vanishes at the two bottom corners. At large $y$, $U-iV\to-i$, so it tends to a uniform upward field $(0,1)$.

Near $z_*$, $G'(z)\sim1/(z-z_*)$, showing a radial boundary source. The [streamlines](../../fluid-mechanics.md#streamline) are the curves $\operatorname{Im}G=\arg(2+\sin z)=\text{constant}$; the figure shows their orientation without reusing the exam's graphics.

<a id="7/b/iii/image-radial-flow-in-the-upper-half-plane-and-its-image-in-a-vertical-half-strip"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-q7-sine-map-flow.png)

**[Figure 3](#7/b/iii/image-radial-flow-in-the-upper-half-plane-and-its-image-in-a-vertical-half-strip). Radial flow in the upper half-plane and its image in a vertical half-strip**.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

For the normalized second-order equation, $x_0$ is an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) if both coefficient functions $p$ and $q$ are [holomorphic](../../holomorphic-function.md) near $x_0$. If it is singular but $(x-x_0)p(x)$ and $(x-x_0)^2q(x)$ are [holomorphic](../../holomorphic-function.md) there, it is a [regular singular point](../../complex-analysis.md#regular-singular-point). Thus $p$ may have at most a simple pole and $q$ at most a double pole.

The distinction tells us which local series method is justified. At an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation), two independent solutions are represented by ordinary [Taylor series](../../calculus.md#taylor-series). At a [regular singular point](../../complex-analysis.md#regular-singular-point), the [Frobenius method](../../complex-analysis.md#frobenius-method) uses $(x-x_0)^r\sum_{n\geq0}a_n(x-x_0)^n$; the [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) determines the exponents, and logarithmic terms may appear in a second solution. Singularities worse than these are irregular and need not have this Frobenius form.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

The [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is

$$
\boxed{W(f,g)(x)=\begin{vmatrix}f(x)&g(x)\\f'(x)&g'(x)\end{vmatrix}=f(x)g'(x)-f'(x)g(x).}
$$

Suppose constants $A,B$ satisfy $Af+Bg=0$ throughout the interval. Differentiating gives $Af'+Bg'=0$. At $x_0$, these form the homogeneous linear system

$$
\begin{pmatrix}f(x_0)&g(x_0)\\f'(x_0)&g'(x_0)\end{pmatrix}\begin{pmatrix}A\\B\end{pmatrix}=0.
$$

Its [determinant](../../multilinear-algebra.md#determinant) is nonzero by hypothesis, so $A=B=0$. This is exactly [linear independence](../../vector-space.md#linear-independence) of the two functions on the interval. No differential equation is needed for this implication; the converse for arbitrary differentiable functions would require additional hypotheses.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

The origin is an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation). Substitute $y=\sum_{n\geq0}a_nx^n$ into the equation and collect the coefficient of $x^n$:

$$
(n+2)(n+1)a_{n+2}+(k^2-n^2)a_n=0.
$$

Hence the [recurrence relation](../../sequence-and-series.md#recurrence-relation) is

$$
\boxed{a_{n+2}=\frac{n^2-k^2}{(n+2)(n+1)}a_n,\qquad n\geq0.}
$$

There are two free initial coefficients. The independent even and odd [power series](../../sequence-and-series.md#power-series) begin

$$
\begin{aligned}
y_{\rm e}(x)&=1-\frac{k^2}{2!}x^2+\frac{k^2(k^2-4)}{4!}x^4-\frac{k^2(k^2-4)(k^2-16)}{6!}x^6+\cdots,\\
y_{\rm o}(x)&=x+\frac{1-k^2}{3!}x^3+\frac{(1-k^2)(9-k^2)}{5!}x^5+\cdots.
\end{aligned}
$$

The general solution is $\boxed{y=a_0y_{\rm e}+a_1y_{\rm o}}$. As a useful independent check, the substitution $x=\sin t$ reduces the equation to $d^2y/dt^2+k^2y=0$. Thus

$$
y_{\rm e}=\cos(k\arcsin x),\qquad y_{\rm o}=\begin{cases}\sin(k\arcsin x)/k,&k\neq0,\\\arcsin x,&k=0.\end{cases}
$$

For a nonterminating parity series, $|a_{n+2}/a_n|\to1$, so the [ratio test](../../sequence-and-series.md#ratio-test) in $x^2$ gives $\boxed{R=1}$. The [regular singular points](../../complex-analysis.md#regular-singular-point) at $\pm1$ explain the natural obstruction.

There is an important exception to an unconditional radius-one answer. If $k^2=m^2$ for an integer $m\geq0$, the series of parity $m$ terminates at degree $m$ and is a multiple of a [Chebyshev polynomial](../../numerical-analysis.md#chebyshev-polynomial). Its [radius of convergence](../../sequence-and-series.md#radius-of-convergence) is $\boxed{R=\infty}$; the other independent parity solution still has radius one. For $m=0$ the even solution is constant. Any nonzero combination containing the nonterminating solution has radius one. These are the full [power series of the Chebyshev differential equation](../../numerical-analysis.md#power-series-of-the-chebyshev-differential-equation), including the terminating cases.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Assume $c(y)>0$ is differentiable along the ray, with sufficient regularity for the following variation, and fix the endpoints. [Fermat principle](../../mathematical-physics.md#fermat-principle) makes the travel time stationary:

$$
T[y]=\int\frac{\sqrt{1+y'^2}}{c(y)}\,dx.
$$

For the variational [integrand](../../integral.md#integrand) $f=\sqrt{1+y'^2}/c$, the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is

$$
\frac{d}{dx}\left[\frac{y'}{c\sqrt{1+y'^2}}\right]+\frac{c'}{c^2}\sqrt{1+y'^2}=0.
$$

Expanding the [derivative](../../calculus.md#derivative) and multiplying by $c^2(1+y'^2)^{3/2}$ gives

$$
c y''-c'y'^2(1+y'^2)+c'(1+y'^2)^2=0,
$$

and therefore

$$
\boxed{c(y)y''+c'(y)(1+y'^2)=0.}
$$

Equivalently, the [Beltrami identity](../../analysis.md#beltrami-identity) gives $1/[c(y)\sqrt{1+y'^2}]=\text{constant}$. Mere continuity of $c$, as stated in the wording, does not by itself justify the appearance of $c'$; the displayed classical ray equation requires this additional differentiability.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/i">i</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9/b/i)

Introduce a constant [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) $\lambda$ for the fixed [arc length](../../riemannian-geometry.md#arc-length). Up to an irrelevant constant term, the augmented [functional](../../calculus-of-variations.md#functional) is

$$
J[y]=\int_{-a}^a(y+\lambda)\sqrt{1+y'^2}\,dx.
$$

It has no explicit $x$ dependence, so the [Beltrami identity](../../analysis.md#beltrami-identity) gives

$$
(y+\lambda)\sqrt{1+y'^2}-\frac{(y+\lambda)y'^2}{\sqrt{1+y'^2}}=\frac{y+\lambda}{\sqrt{1+y'^2}}=k.
$$

For the hanging minimum choose $k>0$. Writing $y_0=-\lambda$, this becomes $1+y'^2=(y-y_0)^2/k^2$. Its nonconstant smooth solution is

$$
\boxed{y(x)-y_0=k\cosh\left(\frac{x-x_0}{k}\right).}
$$

One may verify it without dividing by $y'$ at the lowest point: the full [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) gives $(y+\lambda)y''=1+y'^2$, which the expression satisfies everywhere. The branch with negative $k$ is the inverted stationary chain rather than the hanging minimum. The [catenary minimizes the integral of height along a fixed-length curve](../../analysis.md#catenary-minimizes-the-integral-of-height-along-a-fixed-length-curve), so the positive branch is also the global minimum, not merely a stationary candidate.

<h4 id="9/b/ii">ii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/b/ii)

Equal endpoint heights imply

$$
\cosh\frac{a-x_0}{k}=\cosh\frac{a+x_0}{k},
$$

so $x_0=0$. The height condition then gives $y_0=b-k\cosh(a/k)$ and the hanging [catenary](../../analysis.md#catenary) is

$$
y(x)=b+k\left[\cosh(x/k)-\cosh(a/k)\right].
$$

Since $\sqrt{1+y'^2}=\cosh(x/k)$, its length fixes $k$ through

$$
2L=\int_{-a}^a\cosh(x/k)\,dx=2k\sinh(a/k),\qquad\boxed{L=k\sinh(a/k).}
$$

For the requested graphical argument, put $u=a/k>0$ and $q=L/a>1$. Intersections of $Y=\sinh u$ with $Y=qu$ determine the solution. Near zero the line has larger slope, while the hyperbolic sine eventually grows faster. Its slope $\cosh u$ increases strictly, so after turning upwards relative to the line it can cross it only once. The intersection at $u=0$ is excluded: it corresponds to infinite $k$ and the limiting length $L=a$.

<a id="9/b/ii/image-unique-positive-catenary-parameter-from-a-hyperbolic-sine-intersection-with-an-example-hanging-chain"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-q9-catenary-uniqueness.png)

**[Figure 4](#9/b/ii/image-unique-positive-catenary-parameter-from-a-hyperbolic-sine-intersection-with-an-example-hanging-chain). Unique positive catenary parameter from a hyperbolic-sine intersection, with an example hanging chain**.

More explicitly, $h(u)=\sinh u/u$ has [derivative](../../calculus.md#derivative) $(u\cosh u-\sinh u)/u^2>0$, because the numerator vanishes at zero and has [derivative](../../calculus.md#derivative) $u\sinh u>0$. Since $h(0+)=1$ and $h(u)\to\infty$, every $q>1$ yields **exactly one positive $u$, hence exactly one positive $k$**.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/i">i</h4>

↑ **Parent:** [A](#10/a)

<h5 id="10/a/i/solution">Solution</h5>

↑ **Parent:** [I](#10/a/i)

For an [eigenfunction](../../linear-operator-theory.md#eigenfunction) in the [operator domain](../../vector-space.md#operator-domain), $H\psi_n=E_n\psi_n$. Substitution into the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) gives

$$
\boxed{F[\psi_n]=\frac{E_n\langle\psi_n,\psi_n\rangle}{\langle\psi_n,\psi_n\rangle}=E_n.}
$$

The cancellation only needs a finite nonzero [norm](../../normed-vector-space.md#norm); orthonormalization makes both denominator and [norm](../../normed-vector-space.md#norm) equal to one.

<h4 id="10/a/ii">ii</h4>

↑ **Parent:** [A](#10/a)

<h5 id="10/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10/a/ii)

Assume $H$ is [self-adjoint](../../linear-operator-theory.md#self-adjoint-operator) on its specified [operator domain](../../vector-space.md#operator-domain), and the admissible variations preserve that domain and any [boundary conditions](../../differential-equation.md#boundary-condition), so no boundary terms spoil self-adjointness. Let $N=\langle\phi,\phi\rangle>0$. The first variation of the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) is

$$
\delta F=\frac{\langle\delta\phi,(H-F[\phi])\phi\rangle+\langle(H-F[\phi])\phi,\delta\phi\rangle}{N}=\frac{2\operatorname{Re}\langle\delta\phi,(H-F[\phi])\phi\rangle}{N}.
$$

At $\phi=\psi_n$, the residual vanishes, so $\boxed{\delta F[\psi_n]=0}$. More explicitly, for a normalized $\psi_n$ and $\phi=\psi_n+\eta$,

$$
F[\psi_n+\eta]-E_n=\frac{\langle\eta,(H-E_n)\eta\rangle}{1+2\operatorname{Re}\langle\psi_n,\eta\rangle+\|\eta\|^2}.
$$

For a fixed admissible direction scaled by a small parameter, the change is second order. This is stationarity, and is not necessarily a minimum for an excited state.

Conversely, vanishing first variation for every admissible complex direction yields the stationary equation

$$
\boxed{(H-F[\phi])\phi=0\quad\text{at a stationary }\phi.}
$$

At the original stationary point, this is $(H-F[\psi_n])\psi_n=0$. **The printed equation with an arbitrary perturbed $\phi$ in the final factor is not generally true.** Taking $\phi=\psi_n+\epsilon\psi_m$ with $E_m\neq E_n$ gives $(H-E_n)\phi=\epsilon(E_m-E_n)\psi_m\neq0$, even though the first-order change in $F$ is zero. Thus the valid claim is the stationary equation at the extremal state, not an exact [eigenvalue](../../linear-operator-theory.md#eigenvalue) equation for every variation.

<h4 id="10/a/iii">iii</h4>

↑ **Parent:** [A](#10/a)

<h5 id="10/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10/a/iii)

Assume a complete [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis) and a [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) bounded below, with the trial state in its [operator domain](../../vector-space.md#operator-domain) or associated energy-form domain. The expansion and [orthogonality](../../inner-product.md#orthogonal-vectors) give

$$
\langle\phi,\phi\rangle=\sum_n|a_n|^2,\qquad\langle\phi,H\phi\rangle=\sum_nE_n|a_n|^2.
$$

Consequently

$$
\boxed{F[\phi]=\frac{\sum_nE_n|a_n|^2}{\sum_n|a_n|^2}\geq E_0.}
$$

It is a weighted average of [eigenvalues](../../linear-operator-theory.md#eigenvalue), all at least $E_0$. This is the [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle); equality holds precisely when the trial state lies in the [ground-state subspace](../../quantum-mechanics.md#ground-state-subspace). A continuous part of the spectrum would require the corresponding spectral [integral](../../integral.md) in place of part of the sum.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Use the intended [infinite square well](../../quantum-mechanics.md#infinite-square-well) interpretation: the kinetic-energy operator on $(-a,a)$ with zero [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition). The variational [energy](../../energy.md) is most safely evaluated through its [quadratic form](../../quadratic-form.md),

$$
F[\phi]=\frac{\hbar^2}{2m}\frac{\int_{-a}^a|\phi'(x)|^2\,dx}{\int_{-a}^a|\phi(x)|^2\,dx}.
$$

The boundary term vanishes because the trial function vanishes at both walls. Its zero extension has [derivative](../../calculus.md#derivative) jumps there, so the form interpretation avoids assigning an unrestricted full-line second [derivative](../../calculus.md#derivative) to it.

Set $u=x/a$ and $b=\lambda a^2$. Apart from an irrelevant factor $a^2$, the trial function is $q_b(u)=(1-u^2)(1+bu^2)$. [Polynomial](../../polynomial.md) [integration](../../integral.md) gives

$$
\begin{aligned}
D(b)&=\int_{-1}^1q_b^2\,du=\frac{16}{315}(b^2+6b+21),\\
N(b)&=\int_{-1}^1(q_b')^2\,du=\frac8{105}(11b^2+14b+35).
\end{aligned}
$$

Hence the [polynomial Rayleigh-Ritz trial space for a one-dimensional box](../../linear-operator-theory.md#polynomial-rayleigh-ritz-trial-space-for-a-one-dimensional-box) has [energy](../../energy.md)

$$
F(b)=\frac{\hbar^2}{ma^2}\frac{3(11b^2+14b+35)}{4(b^2+6b+21)}.
$$

The denominator is strictly positive, since $b^2+6b+21=(b+3)^2+12$. Differentiation gives

$$
\frac{ma^2}{\hbar^2}\frac{dF}{db}=\frac{3(13b^2+98b+21)}{(b^2+6b+21)^2}.
$$

The two stationary parameters are $b_\pm=(-49\pm4\sqrt{133})/13$. The smaller is a local maximum; the larger is a local minimum. Since the [energy](../../energy.md) tends to $33\hbar^2/(4ma^2)$ as $|b|\to\infty$, the latter is the global minimum:

$$
\boxed{\lambda_* =\frac{-49+4\sqrt{133}}{13a^2}\simeq-\frac{0.220750}{a^2},\qquad E_{\rm upper}=\left(7-\frac{\sqrt{133}}2\right)\frac{\hbar^2}{ma^2}\simeq1.233718703\frac{\hbar^2}{ma^2}.}
$$

The upper stationary value is $(7+\sqrt{133}/2)\hbar^2/(ma^2)$. Exact roots give a slightly tighter bound than substituting the rounded hints.

**There are two qualifications to the printed operator and comparison [energy](../../energy.md).** For the box with [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) and width $2a$, the actual [ground-state energy](../../quantum-mechanics.md#ground-state-energy) is

$$
\boxed{E_0^{\rm box}=\frac{\pi^2\hbar^2}{8ma^2}\simeq1.233700550\frac{\hbar^2}{ma^2},}
$$

which lies just below the variational result. The coefficient $6/5$ printed as an exact [eigenvalue](../../linear-operator-theory.md#eigenvalue) is inconsistent with this box problem. Also, merely declaring the differential expression to be zero outside the interval does not impose hard-wall confinement or specify a self-adjoint domain. Read literally on a space admitting exterior-supported states, it has zero-energy states outside and does not have the claimed positive ground [energy](../../energy.md). The boxed variational result is the well-defined answer for the intended confined particle; a different full-line operator would need its domain and matching conditions supplied.

## ↑ Ancestors (10)

1. [2016](../2016.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
