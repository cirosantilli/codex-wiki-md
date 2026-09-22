# Paper 1

↑ **Parent:** [2024](../2024.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2024/papernst_ib_1_2024.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2024/papernst_ib_1_2024.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
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
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
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
  - [e](#5/e)
    - [Solution](#5/e/solution)
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
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
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
  - [d](#8/d)
    - [Solution](#8/d/solution)
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
  - [c](#9/c)
    - [Solution](#9/c/solution)
  - [d](#9/d)
    - [Solution](#9/d/solution)
  - [e](#9/e)
    - [Solution](#9/e/solution)
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

For a continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) $\mathbf u$ on a bounded region $V\subset\mathbb R^3$ with piecewise smooth closed boundary $S=\partial V$, the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) states

$$
\boxed{\int_V\nabla\cdot\mathbf u\,dV=\int_S\mathbf u\cdot\hat{\mathbf n}\,dS=\int_S\mathbf u\cdot d\mathbf S.}
$$

Here $\nabla\cdot\mathbf u$ is its [divergence](../../multivariable-calculus.md#divergence), $dV$ is the volume element, $dS$ is the surface area element, $\hat{\mathbf n}$ is the outward [unit normal](../../differential-geometry.md#unit-normal), and $d\mathbf S=\hat{\mathbf n}\,dS$. Thus a [volume integral](../../multivariable-calculus.md#volume-integral) of the [divergence](../../multivariable-calculus.md#divergence) equals the outward [flux](../../mathematical-physics.md#flux) through the boundary.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Since $\mathbf a$ is constant, the [product rule](../../calculus.md#product-rule) gives $\nabla\cdot(\mathbf a\psi)=\mathbf a\cdot\nabla\psi$. Applying the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) therefore gives

$$
\mathbf a\cdot\int_V\nabla\psi\,dV=\int_S\psi\,\mathbf a\cdot d\mathbf S=\mathbf a\cdot\int_S\psi\,d\mathbf S.
$$

This holds for every constant [vector](../../vector-space.md#vector) $\mathbf a$, so each component of the difference vanishes. Consequently the [gradient](../../multivariable-calculus.md#gradient) has the boundary representation

$$
\boxed{\int_V\nabla\psi\,dV=\int_S\psi\,d\mathbf S.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [divergence of a cross product](../../multivariable-calculus.md#divergence-of-a-cross-product) and $\nabla\times\mathbf a=0$ give $\nabla\cdot(\mathbf a\times\mathbf A)=-\mathbf a\cdot(\nabla\times\mathbf A)$. On the boundary the [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) gives $(\mathbf a\times\mathbf A)\cdot\hat{\mathbf n}=-\mathbf a\cdot(\hat{\mathbf n}\times\mathbf A)$. Thus the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives

$$
-\mathbf a\cdot\int_V\nabla\times\mathbf A\,dV=-\mathbf a\cdot\int_S\hat{\mathbf n}\times\mathbf A\,dS.
$$

Because $\mathbf a$ is arbitrary, the [curl](../../multivariable-calculus.md#curl) identity follows:

$$
\boxed{\int_V\nabla\times\mathbf A\,dV=\int_S\hat{\mathbf n}\times\mathbf A\,dS.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use [Einstein summation convention](../../multilinear-algebra.md#einstein-notation) and write $\partial_j=\nabla_j$. Since $\partial_jr_i=\delta_{ij}$, where $\delta_{ij}$ is the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta), the [product rule](../../calculus.md#product-rule) gives

$$
\partial_j(r_iw_j)=\delta_{ij}w_j+r_i\partial_jw_j=w_i+P_i.
$$

This proves $\boxed{P_i=\partial_j(r_iw_j)-w_i}$. Now take $w_j=\partial_j\psi$. Integrating this identity and applying the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) to the first term gives

$$
\int_Vr_i\nabla^2\psi\,dV=\int_Sr_i\partial_j\psi\,dS_j-\int_V\partial_i\psi\,dV.
$$

Part (b) changes the last [volume integral](../../multivariable-calculus.md#volume-integral) of the [gradient](../../multivariable-calculus.md#gradient) into a [surface integral](../../multivariable-calculus.md#surface-integral), yielding

$$
\boxed{\int_Vr_i\nabla^2\psi\,dV=\int_Sr_i\partial_j\psi\,dS_j-\int_S\psi\,dS_i.}
$$

Here $dS_i=\hat n_i\,dS$; the [Laplacian](../../multivariable-calculus.md#laplacian) is $\nabla^2\psi=\partial_j\partial_j\psi$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Apply the [product rule](../../calculus.md#product-rule) to the [tensor field](../../vector-bundle.md#tensor-field), without assuming any symmetry of $\Sigma$:

$$
\partial_j(r_i\partial_k\Sigma_{kj})=\delta_{ij}\partial_k\Sigma_{kj}+r_i\partial_j\partial_k\Sigma_{kj}=\partial_k\Sigma_{ki}+r_i\partial_j\partial_k\Sigma_{kj}.
$$

Integrating, the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) converts each of the two [divergences](../../multivariable-calculus.md#divergence) into a boundary term:

$$
\boxed{\int_Vr_i\partial_j\partial_k\Sigma_{kj}\,dV=\int_Sr_i\partial_k\Sigma_{kj}\,dS_j-\int_S\Sigma_{ki}\,dS_k.}
$$

The repeated indices are summed according to [Einstein summation convention](../../multilinear-algebra.md#einstein-notation), while $i$ labels the component of the resulting [vector](../../vector-space.md#vector) identity.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Choose the symmetric [tensor field](../../vector-bundle.md#tensor-field)

$$
\Sigma_{kj}=(\partial_k\psi)(\partial_j\psi)-\frac12\delta_{kj}|\nabla\psi|^2.
$$

The [product rule](../../calculus.md#product-rule) and equality of mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative) give

$$
\begin{aligned}
\partial_k\Sigma_{kj}
&=(\nabla^2\psi)\partial_j\psi+(\partial_k\psi)\partial_k\partial_j\psi-\frac12\partial_j|\nabla\psi|^2\\
&=(\nabla^2\psi)\partial_j\psi.
\end{aligned}
$$

This is the [Euclidean scalar-gradient stress identity](../../multivariable-calculus.md#euclidean-scalar-gradient-stress-identity). Substitute it into part (e), and use $\Sigma_{ki}\hat n_k=(\partial_n\psi)\partial_i\psi-\tfrac12|\nabla\psi|^2\hat n_i$, where $\partial_n\psi=\hat{\mathbf n}\cdot\nabla\psi$. Reassembling the components gives the required pure [surface integral](../../multivariable-calculus.md#surface-integral):

$$
\boxed{\int_V\mathbf r\,\nabla\cdot[(\nabla^2\psi)\nabla\psi]\,dV=\int_S\left[\mathbf r(\nabla^2\psi)\partial_n\psi-(\partial_n\psi)\nabla\psi+\frac12|\nabla\psi|^2\hat{\mathbf n}\right]dS.}
$$

Sufficient smoothness of $\psi$ is understood for the displayed [derivatives](../../calculus.md#derivative) and applications of the [divergence theorem](../../multivariable-calculus.md#divergence-theorem).

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Apply [separation of variables](../../partial-differential-equation.md#separation-of-variables) with $\rho(x,t)=X(x)T(t)$ and temporal factor $T=e^{-\lambda t}$. The spatial [eigenvalue](../../linear-operator-theory.md#eigenvalue) equation is

$$
-DX''-\gamma X=\lambda X,\qquad X(0)=X(L)=0.
$$

The nontrivial solutions of these [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) are sine [eigenfunctions](../../linear-operator-theory.md#eigenfunction). Normalizing in the usual [inner product](../../inner-product.md) on $(0,L)$ gives

$$
\boxed{\psi_n(x)=\sqrt{\frac2L}\sin\frac{n\pi x}{L},\qquad\lambda_n=D\left(\frac{n\pi}{L}\right)^2-\gamma,\qquad n=1,2,\ldots,}
$$

with $\int_0^L\psi_n\psi_m\,dx=\delta_{nm}$. The [superposition principle](../../vector-space.md#superposition-principle) and the [Fourier sine series](../../fourier-series.md#fourier-sine-series) then give

$$
\boxed{\rho(x,t)=\sum_{n=1}^{\infty}a_n\sqrt{\frac2L}\sin\frac{n\pi x}{L}\exp\left[\left(\gamma-\frac{Dn^2\pi^2}{L^2}\right)t\right].}
$$

The constants are the initial-data coefficients $a_n=\int_0^L\rho(x,0)\psi_n(x)\,dx$. Here physical diffusion means $D>0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

By [orthogonality](../../inner-product.md#orthogonal-vectors) and the sampling property of the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function),

$$
a_n=\rho_0\int_0^L\delta(x-x_0)\psi_n(x)\,dx=\boxed{\rho_0\sqrt{\frac2L}\sin\frac{n\pi x_0}{L}}.
$$

Consequently the [reaction-diffusion equation](../../diffusion-equation.md#reaction-diffusion-system) solution is

$$
\boxed{\rho(x,t)=\frac{2\rho_0}{L}\sum_{n=1}^{\infty}\sin\frac{n\pi x_0}{L}\sin\frac{n\pi x}{L}\exp\left[\left(\gamma-\frac{Dn^2\pi^2}{L^2}\right)t\right].}
$$

For every $t>0$ this [eigenfunction expansion](../../algebra.md#eigenfunction-expansion) is smoothed by the Gaussian decay in $n$. As $t\downarrow0$, it recovers the specified initial condition in the sense of [distributions](../../distribution-theory.md#distribution-mathematical-analysis).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The smallest decay-rate [eigenvalue](../../linear-operator-theory.md#eigenvalue) is $\lambda_1=D\pi^2/L^2-\gamma$, so the threshold is

$$
\boxed{\gamma_c(D,L)=\frac{D\pi^2}{L^2}.}
$$

Because $0<x_0<L$, $a_1>0$. For every fixed interior point $0<x<L$, the first sine [eigenfunction](../../linear-operator-theory.md#eigenfunction) is positive and the remaining terms have strictly faster decay relative to it. Hence

$$
\rho(x,t)\sim\frac{2\rho_0}{L}\sin\frac{\pi x_0}{L}\sin\frac{\pi x}{L}\,e^{(\gamma-\gamma_c)t}.
$$

One can justify the relative-error limit directly: after factoring out the first exponential, the absolute remainder is bounded by $(2\rho_0/L)\sum_{n\geq2}e^{-D\pi^2(n^2-1)t/L^2}$, which tends to zero. Thus $\boxed{\rho\to0\text{ if }\gamma<\gamma_c}$, and $\boxed{\rho(x,t)\to+\infty\text{ for each interior }x\text{ if }\gamma>\gamma_c}$. The boundary values stay zero. At equality the first term is stationary and the density approaches its positive sine profile.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $f(x)=\rho(x,0)$. The first normalized [Fourier sine series](../../fourier-series.md#fourier-sine-series) coefficient is

$$
a_1=\sqrt{\frac2L}\int_0^Lf(x)\sin\frac{\pi x}{L}\,dx>0.
$$

Strict positivity follows because $f\geq0$, has positive total mass, and $\sin(\pi x/L)>0$ everywhere inside the interval. In particular, there is no cancellation that could remove the slowest term. This is the [positivity of the first Dirichlet reaction-diffusion coefficient](../../diffusion-equation.md#positivity-of-the-first-dirichlet-reaction-diffusion-coefficient).

For finite initial mass $M=\int_0^Lf(x)\,dx$, all coefficients satisfy $|a_n|\leq\sqrt{2/L}\,M$. The [eigenfunction expansion](../../algebra.md#eigenfunction-expansion) therefore gives the uniform bound

$$
\left|e^{\lambda_1t}\rho(x,t)-a_1\psi_1(x)\right|\leq\frac{2M}{L}\sum_{n=2}^{\infty}e^{-D\pi^2(n^2-1)t/L^2}\longrightarrow0.
$$

The positive first profile thus controls the long-time behavior. We recover exactly the threshold $\boxed{\gamma_c=D\pi^2/L^2}$, with decay below it and unbounded positive growth at every interior point above it. The finite-mass condition is the usual meaning of an initial density profile here; standard positive-time smoothing gives the same conclusion in the usual broader admissible data classes.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For an exponential trial $y=e^{rx}$, the [characteristic equation](../../linear-ordinary-differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) is

$$
r^2+2ar+a^2+b^2=(r+a)^2+b^2=0.
$$

Its distinct complex [roots](../../semisimple-lie-algebra.md#root-of-a-root-system) are $r=-a\pm ib$. Thus the general real solution of the homogeneous [second-order linear differential equation](../../linear-ordinary-differential-equation.md#second-order-linear-differential-equation) is

$$
\boxed{y_h(x)=e^{-ax}[C_1\cos(bx)+C_2\sin(bx)].}
$$

The two displayed solutions have nonzero [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) $be^{-2ax}$ and hence [linear independence](../../vector-space.md#linear-independence). The same formula permits complex solutions when $C_1,C_2$ are complex.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For the zero-data [initial value problem](../../differential-equation.md#initial-value-problem), choose a [causal Green function](../../green-s-function.md#causal-green-function) satisfying $L_xG(x,\xi)=\delta(x-\xi)$ and $G=0$ for $x<\xi$. Continuity at $x=\xi$ prevents a derivative of the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function), while integration across the source gives

$$
G(\xi^+,\xi)=0,\qquad\partial_xG(\xi^+,\xi)-\partial_xG(\xi^-,\xi)=1.
$$

For $x>\xi$, part (i) gives the shifted homogeneous solutions. The zero value at the join removes the cosine term, and the unit [derivative](../../calculus.md#derivative) jump fixes the sine coefficient. Therefore the [causal Green function of a damped oscillator](../../analysis.md#causal-green-function-of-a-damped-oscillator) is

$$
\boxed{G(x,\xi)=\begin{cases}\dfrac1b e^{-a(x-\xi)}\sin[b(x-\xi)],&x\geq\xi,\\0,&x<\xi.\end{cases}}
$$

Equivalently, multiply the first expression by the [Heaviside step function](../../integral-transform.md#heaviside-step-function) $H(x-\xi)$. The required solution is

$$
\boxed{y(x)=\int_0^{\infty}G(x,\xi)g(\xi)\,d\xi=\frac1b\int_0^xe^{-a(x-\xi)}\sin[b(x-\xi)]g(\xi)\,d\xi.}
$$

Its initial value and first [derivative](../../calculus.md#derivative) vanish: the interval has zero length at $x=0$ and the kernel vanishes at its upper limit. Differentiating twice shows that the upper-limit contribution to $y''$ is precisely $g(x)$, while the remaining homogeneous kernel terms cancel in $Ly$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The original PDF has the absolute-value hypothesis $|g(\xi)|<Ce^{-s\xi}$, which is missing from the local OCR. From the [Green's function](../../green-s-function.md) formula and $|\sin|\leq1$,

$$
\begin{aligned}
|y(x)|&\leq\frac{C}{b}\int_0^xe^{-a(x-\xi)}e^{-s\xi}\,d\xi\\
&=\frac{C}{b}e^{-ax}\int_0^xe^{-(s-a)\xi}\,d\xi\\
&=\frac{C}{b(s-a)}e^{-ax}[1-e^{-(s-a)x}]\leq\frac{C}{b(s-a)}e^{-ax}.
\end{aligned}
$$

Because $s>a>0$, the upper bound tends to zero. The [squeeze theorem](../../calculus.md#squeeze-theorem) proves $\boxed{y(x)\to0\text{ as }x\to\infty}$.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

With the paper's [Fourier transform](../../fourier-transform.md) convention, the [Fourier inversion theorem](../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\boxed{f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{ikx}\widetilde f(k)\,dk.}
$$

This holds at continuity points under the usual inversion hypotheses; at a jump with one-sided limits it gives their mean. The factor $1/(2\pi)$ and the sign change in the exponential are part of this normalization.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Insert the inverse [Fourier transforms](../../fourier-transform.md) of $f$ and its complex conjugate, initially under enough decay to justify interchanging [integrals](../../integral.md):

$$
\begin{aligned}
\int_{\mathbb R}|f(x)|^2\,dx
&=\frac1{(2\pi)^2}\int_{\mathbb R}\int_{\mathbb R}\widetilde f(k)\overline{\widetilde f(\ell)}\left[\int_{\mathbb R}e^{i(k-\ell)x}\,dx\right]dk\,d\ell\\
&=\frac1{2\pi}\int_{\mathbb R}\int_{\mathbb R}\widetilde f(k)\overline{\widetilde f(\ell)}\delta(k-\ell)\,dk\,d\ell\\
&=\boxed{\frac1{2\pi}\int_{\mathbb R}|\widetilde f(k)|^2\,dk}.
\end{aligned}
$$

The middle step uses the stated [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function) identity, and the last uses its sampling property. This is the [Parseval identity](../../fourier-analysis.md#parseval-identity) for the chosen normalization. Approximation extends the result to [square-integrable functions](../../measure-theory.md#square-integrable-function), including the function used below.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The real [odd function](../../calculus.md#odd-function) has a purely imaginary odd [Fourier transform](../../fourier-transform.md). Setting $A=\pi/2$ and using a product-to-sum identity,

$$
\begin{aligned}
\widetilde f(k)&=-2i\int_0^A\sin x\sin(kx)\,dx\\
&=-i\left[\frac{\sin[(k-1)A]}{k-1}-\frac{\sin[(k+1)A]}{k+1}\right]\\
&=\boxed{\frac{2ik\cos(\pi k/2)}{k^2-1}},\qquad k\ne\pm1.
\end{aligned}
$$

The apparent singularities are removable. Direct evaluation or limits give

$$
\boxed{\widetilde f(1)=-\frac{i\pi}{2},\qquad\widetilde f(-1)=\frac{i\pi}{2},\qquad\widetilde f(0)=0.}
$$

In particular, the transform stays finite where its numerator and denominator both vanish.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The squared [norm](../../normed-vector-space.md#norm) of the original function is

$$
\int_{\mathbb R}|f(x)|^2\,dx=\int_{-\pi/2}^{\pi/2}\sin^2x\,dx=\frac\pi2.
$$

Applying the [Parseval identity](../../fourier-analysis.md#parseval-identity) to part (c), using the evenness of the squared transform, gives

$$
\frac\pi2=\frac1{2\pi}\int_{\mathbb R}\frac{4k^2\cos^2(\pi k/2)}{(k^2-1)^2}\,dk=\frac4\pi\int_0^{\infty}\frac{k^2\cos^2(\pi k/2)}{(k^2-1)^2}\,dk.
$$

Thus the last [integral](../../integral.md) equals $\pi^2/8$. Now set $u=\pi k/2$. Since

$$
\frac{k^2\,dk}{(k^2-1)^2}=\frac\pi2\frac{u^2\,du}{(u^2-\pi^2/4)^2},
$$

we obtain

$$
\boxed{\int_0^{\infty}\frac{u^2\cos^2u}{(u^2-\pi^2/4)^2}\,du=\frac2\pi\frac{\pi^2}{8}=\frac\pi4.}
$$

The apparent singularity at $u=\pi/2$ is removable: the continuous value of the integrand there is $1/4$. No principal-value interpretation is needed.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $Av=\lambda v$ with $v\ne0$. Taking the [Hermitian inner product](../../linear-algebra.md#hermitian-inner-product) with $v$ gives $v^\dagger Av=\lambda\|v\|^2$. For an [anti-Hermitian matrix](../../linear-operator-theory.md#skew-hermitian-matrix),

$$
\overline{v^\dagger Av}=v^\dagger A^\dagger v=-v^\dagger Av.
$$

Consequently $\overline\lambda\|v\|^2=-\lambda\|v\|^2$. As $\|v\|^2>0$, the [eigenvalue](../../linear-operator-theory.md#eigenvalue) satisfies $\boxed{\overline\lambda=-\lambda}$, or $\boxed{\lambda=i\theta\text{ with }\theta\in\mathbb R}$. Zero is included as a purely imaginary [eigenvalue](../../linear-operator-theory.md#eigenvalue).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

If $I+A$ were a [singular matrix](../../linear-algebra.md#singular-matrix), a nonzero [vector](../../vector-space.md#vector) $v$ would satisfy $(I+A)v=0$, so $Av=-v$. This would make $-1$ an [eigenvalue](../../linear-operator-theory.md#eigenvalue) of the [anti-Hermitian matrix](../../linear-operator-theory.md#skew-hermitian-matrix), contrary to part (a). Thus $\boxed{I+A\text{ is invertible}}$. The same argument shows $I-A$ is an [invertible matrix](../../linear-algebra.md#invertible-matrix), which will also be used below.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Taking the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) term by term in the convergent [matrix exponential](../../linear-operator-theory.md#matrix-exponential) gives

$$
U^\dagger=e^{A^\dagger}=e^{-A}.
$$

The [matrices](../../vector-space.md#matrix) $A$ and $-A$ [commute](../../algebraic-operation.md#commuting-elements), so the [matrix exponential](../../linear-operator-theory.md#matrix-exponential) product law gives $U^\dagger U=e^{-A}e^A=I$ and likewise $UU^\dagger=I$. Hence $\boxed{U\text{ is unitary}}$.

For $V$, use the inverse and product rules for the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose):

$$
V^\dagger=[(I+A)^{-1}]^\dagger(I-A)^\dagger=(I-A)^{-1}(I+A).
$$

The factors $I\pm A$ [commute](../../algebraic-operation.md#commuting-elements), as do their inverses, since they are expressions in the same [matrix](../../vector-space.md#matrix). Consequently

$$
V^\dagger V=(I-A)^{-1}(I+A)(I-A)(I+A)^{-1}=I,
$$

and similarly $VV^\dagger=I$. Therefore $\boxed{V\text{ is unitary}}$. This rational construction is the skew-Hermitian form of the [Cayley transform of a Hermitian matrix](../../linear-operator-theory.md#cayley-transform-of-a-hermitian-matrix), obtained by writing $A=iH$ with $H$ a [Hermitian matrix](../../hilbert-space.md#hermitian-operator).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

If $Av=\lambda v$, then $A^nv=\lambda^nv$, and the [matrix exponential](../../linear-operator-theory.md#matrix-exponential) series gives $Uv=e^\lambda v$. Also $(I+A)^{-1}v=(1+\lambda)^{-1}v$, since $1+\lambda\ne0$. Thus

$$
\boxed{\lambda_U=e^\lambda,\qquad\lambda_V=\frac{1-\lambda}{1+\lambda}.}
$$

The assumed diagonalization ensures that these account for all [eigenvalues](../../linear-operator-theory.md#eigenvalue), including multiplicities. In particular, for $\lambda=i\theta$,

$$
\boxed{\lambda_U=e^{i\theta},\qquad\lambda_V=\frac{1-i\theta}{1+i\theta}=e^{-2i\arctan\theta},}
$$

both of [modulus](../../complex-analysis.md#modulus) one, in agreement with the [unitary matrix](../../linear-operator-theory.md#unitary-matrix) property.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Here $A^2=-I$. Splitting the [matrix exponential](../../linear-operator-theory.md#matrix-exponential) into even and odd powers therefore gives

$$
U=I\cos1+A\sin1=\boxed{\begin{pmatrix}\cos1&\sin1\\-\sin1&\cos1\end{pmatrix}}.
$$

For the second [matrix](../../vector-space.md#matrix), $(I+A)(I-A)=I-A^2=2I$, so $(I+A)^{-1}=(I-A)/2$. Hence

$$
V=\frac12(I-A)^2=\frac12(I-2A+A^2)=-A=\boxed{\begin{pmatrix}0&-1\\1&0\end{pmatrix}}.
$$

Both are real [orthogonal matrices](../../linear-algebra.md#orthogonal-matrix), and hence also [unitary matrices](../../linear-operator-theory.md#unitary-matrix).

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Choose a real unit [eigenvector](../../linear-operator-theory.md#eigenvector) $e_1$ of the real [symmetric matrix](../../linear-algebra.md#symmetric-matrix) $Q$, with [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\lambda_1$. Its [orthogonal complement](../../hilbert-space.md#orthogonal-complement) is an [invariant subspace](../../representation-theory.md#invariant-subspace): for any $v$ with $e_1^Tv=0$,

$$
e_1^TQv=(Qe_1)^Tv=\lambda_1e_1^Tv=0.
$$

The restriction of $Q$ to this $(n-1)$-dimensional space is again real and symmetric. Applying the same argument inductively produces an [orthonormal basis](../../inner-product.md#orthonormal-basis) $e_1,\ldots,e_n$ of real [eigenvectors](../../linear-operator-theory.md#eigenvector). The base case $n=1$ is immediate. This proves the [spectral theorem for real symmetric matrices](../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) without assuming that distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue) are available.

One can also check that [eigenvectors](../../linear-operator-theory.md#eigenvector) with different [eigenvalues](../../linear-operator-theory.md#eigenvalue) are automatically orthogonal: $\lambda_i e_i^Te_j=(Qe_i)^Te_j=e_i^TQe_j=\lambda_j e_i^Te_j$. Within a repeated [eigenspace](../../linear-operator-theory.md#eigenspace), the [Gram-Schmidt process](../../inner-product.md#gram-schmidt-process) preserves the eigenvector property. Thus repeated [eigenvalues](../../linear-operator-theory.md#eigenvalue) cause no obstruction, and $\boxed{Q=ODO^T\text{ for an orthogonal }O\text{ and real diagonal }D}$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [quadratic form](../../quadratic-form.md) is $\mathbf x^TQ\mathbf x$ for the real [symmetric matrix](../../linear-algebra.md#symmetric-matrix)

$$
Q=\begin{pmatrix}5&0&3\\0&-3&0\\3&0&-3\end{pmatrix}.
$$

The $y$ axis has [eigenvalue](../../linear-operator-theory.md#eigenvalue) $-3$. On the $xz$ plane, the [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is

$$
\det\begin{pmatrix}5-\ell&3\\3&-3-\ell\end{pmatrix}=(5-\ell)(-3-\ell)-9=\ell^2-2\ell-24=(\ell-6)(\ell+4).
$$

Thus the [orthogonal diagonalization](../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix) from part (a) yields

$$
\boxed{\lambda=6,\qquad\mu=-3,\qquad\nu=-4,\qquad6u^2-3v^2-4w^2=\alpha.}
$$

For later use, one possible [orthonormal basis](../../inner-product.md#orthonormal-basis) is

$$
e_u=\frac{(3,0,1)}{\sqrt{10}},\qquad e_v=(0,1,0),\qquad e_w=\frac{(1,0,-3)}{\sqrt{10}}.
$$

Then $u=(3x+z)/\sqrt{10}$, $v=y$, $w=(x-3z)/\sqrt{10}$. This explicit choice also confirms that the [Euclidean norm](../../normed-vector-space.md#euclidean-norm) is preserved: $x^2+y^2+z^2=u^2+v^2+w^2$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

In the [orthonormal basis](../../inner-product.md#orthonormal-basis) of part (b), the three [quadric surfaces](../../euclidean-geometry.md#quadric-surface) have the following forms. For $\alpha=1$,

$$
\frac{u^2}{1/6}-\frac{v^2}{1/3}-\frac{w^2}{1/4}=1,
$$

a [two-sheeted hyperboloid](../../differential-geometry.md#two-sheeted-hyperboloid) with axis $u$, vertices $(\pm1/\sqrt6,0,0)$, and one sheet on each side of the plane $u=0$. For $\alpha=0$,

$$
6u^2=3v^2+4w^2,
$$

an [elliptic cone](../../euclidean-geometry.md#elliptic-cone) with vertex at the origin and the same axis. For $\alpha=-1$,

$$
\frac{v^2}{1/3}+\frac{w^2}{1/4}-\frac{u^2}{1/6}=1,
$$

a [one-sheet hyperboloid](../../differential-geometry.md#one-sheet-hyperboloid) with axis $u$ and a waist [ellipse](../../euclidean-geometry.md#ellipse) at $u=0$, whose semiaxes are $1/\sqrt3$ along $v$ and $1/2$ along $w$. The sections at fixed $u$ enlarge away from the waist.

<a id="6/c/image-the-two-sheeted-hyperboloid-elliptic-cone-and-one-sheet-hyperboloid-in-separate-orthonormal-coordinate-frames"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1-quadrics.png)

**[Figure 1](#6/c/image-the-two-sheeted-hyperboloid-elliptic-cone-and-one-sheet-hyperboloid-in-separate-orthonormal-coordinate-frames). The two-sheeted hyperboloid, elliptic cone and one-sheet hyperboloid in separate orthonormal coordinate frames**.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The [orthogonal change of coordinates](../../linear-algebra.md#orthogonal-change-of-coordinates) preserves distance to the origin. On the required [quadric surface](../../euclidean-geometry.md#quadric-surface),

$$
1=-6u^2+3v^2+4w^2\leq4(u^2+v^2+w^2).
$$

Thus the squared distance is at least $1/4$. Equality holds precisely when $u=v=0$, and the constraint then gives $w=\pm1/2$. Using $e_w=(1,0,-3)/\sqrt{10}$ from part (b), the nearest points in the original coordinates are

$$
\boxed{(x,y,z)=\pm\frac{(1,0,-3)}{2\sqrt{10}},\qquad\text{minimum distance }=\frac12.}
$$

Substitution checks the constraint directly: $5x^2-3z^2+6xz=(5-27-18)/40=-1$. The inequality proves these are global nearest points, rather than merely stationary candidates.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

Write $z=x+iy$ and square the [modulus](../../complex-analysis.md#modulus) equation. It becomes

$$
x^2+(y+b)^2=P^2[x^2+(y-b)^2].
$$

For $P\ne1$, completing the square gives the [Apollonius circle](../../euclidean-geometry.md#circles-of-apollonius)

$$
x^2+\left(y-\frac{b(P^2+1)}{P^2-1}\right)^2=\frac{4b^2P^2}{(P^2-1)^2}.
$$

Hence

$$
\boxed{\text{center }\left(0,\frac{b(P^2+1)}{P^2-1}\right),\qquad\text{radius }\frac{2bP}{|P^2-1|}.}
$$

The printed statement needs the exception $\boxed{P=1\ \Longrightarrow\ y=0}$: equal distances from $ib$ and $-ib$ give their perpendicular bisector, a straight line rather than a finite-radius [circle](../../topology.md#circle). For $P>1$ the center lies in the upper half-plane; this is the case needed in part (ii). The original PDF confirms the numerator $z+ib$, correcting the duplicated, corrupted OCR formula.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

For the upper [Apollonius circle](../../euclidean-geometry.md#circles-of-apollonius), let its constant ratio be $P>1$. Matching the center and radius from part (i) gives

$$
y_0=\frac{b(P^2+1)}{P^2-1},\qquad R=\frac{2bP}{P^2-1}.
$$

Subtracting their squares yields $\boxed{b=\sqrt{y_0^2-R^2}}$. Also

$$
\frac{y_0}{R}=\frac{P+P^{-1}}2=\cosh(\log P),\qquad\log P=\operatorname{arcosh}(y_0/R).
$$

The relevant [inverse hyperbolic cosine](../../calculus.md#inverse-hyperbolic-cosine) is positive. Now $\log|(z+ib)/(z-ib)|$ is the [real part](../../complex-analysis.md#real-part) of a local [holomorphic logarithm](../../complex-analysis.md#holomorphic-logarithm), hence a [harmonic function](../../partial-differential-equation.md#harmonic-function) away from $z=\pm ib$. The point $ib$ is inside the excluded disk, because $0<y_0-b<R$, while $-ib$ is below the real axis. Thus neither singularity lies in the physical domain.

On $y=0$ the numerator and denominator have equal [modulus](../../complex-analysis.md#modulus), so the logarithm is zero. On the circular boundary its value is $\log P=\operatorname{arcosh}(y_0/R)$. Therefore the [harmonic potential between a grounded line and a circular boundary](../../partial-differential-equation.md#harmonic-potential-between-a-grounded-line-and-a-circular-boundary) is

$$
\boxed{V(x,y)=\frac{V_0}{\operatorname{arcosh}(y_0/R)}\log\left|\frac{x+iy+i\sqrt{y_0^2-R^2}}{x+iy-i\sqrt{y_0^2-R^2}}\right|.}
$$

This verifies [Laplace's equation](../../partial-differential-equation.md#laplace-equation) and both prescribed [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition). It also tends to zero at infinity. A uniqueness assertion on this unbounded domain would require an additional boundedness or infinity condition; the displayed function is the natural decaying solution requested.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

Substituting $z=1$ into the defining [gamma integral](../../complex-analysis.md#gamma-integral) gives

$$
\boxed{\Gamma(1)=\int_0^{\infty}e^{-t}\,dt=[-e^{-t}]_0^{\infty}=1.}
$$

Both endpoints are convergent, so no continuation of the [Gamma function](../../complex-analysis.md#gamma-function) is needed here.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

For real $z>0$, apply [integration by parts](../../calculus.md#integration-by-parts) to the [gamma integral](../../complex-analysis.md#gamma-integral) with $u=t^z$ and $dv=e^{-t}dt$:

$$
\Gamma(z+1)=\int_0^{\infty}t^ze^{-t}\,dt=[-t^ze^{-t}]_0^{\infty}+z\int_0^{\infty}t^{z-1}e^{-t}\,dt.
$$

The boundary term vanishes: $t^z\to0$ at zero, and exponential decay dominates the power at infinity. This proves the [Gamma function recurrence](../../complex-analysis.md#gamma-function-recurrence)

$$
\boxed{\Gamma(z+1)=z\Gamma(z).}
$$

<h4 id="7/b/iii">iii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/b/iii)

Iterating the [Gamma function recurrence](../../complex-analysis.md#gamma-function-recurrence) gives a [meromorphic continuation](../../holomorphic-function.md#meromorphic-continuation)

$$
\Gamma(z)=\frac{\Gamma(z+m+1)}{z(z+1)\cdots(z+m)},\qquad m=0,1,2,\ldots.
$$

Near $z=-m$, the numerator is analytic and tends to $\Gamma(1)=1$. Exactly one denominator factor, $z+m$, vanishes, while all other factors tend to the nonzero product $(-1)^m m!$. Therefore

$$
\Gamma(z)\sim\frac{(-1)^m}{m!}\frac1{z+m}.
$$

Thus $\boxed{z=0,-1,-2,\ldots\text{ are all simple poles}}$. More precisely, the [Gamma function residue at a nonpositive integer](../../complex-analysis.md#gamma-function-residue-at-a-nonpositive-integer) is $\boxed{\operatorname{Res}_{z=-m}\Gamma(z)=(-1)^m/m!}$. Taking $m$ large enough to put $z+m+1$ in the original right half-plane also shows that this continuation introduces no other finite [poles](../../isolated-singularity.md#pole).

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

First simplify the coefficient of $y$ using

$$
\frac{m^3}{x-m}+x^2+mx+m^2=\frac{x^3}{x-m}.
$$

After dividing by $x(x-m)$, the [second-order linear differential equation](../../linear-ordinary-differential-equation.md#second-order-linear-differential-equation) is

$$
y''+P(x)y'+Q(x)y=0,\qquad P(x)=\frac1x+\frac1{x-m},\qquad Q(x)=\frac{\omega^2x^2}{(x-m)^2}.
$$

At zero, $xP\to1$ and $x^2Q\to0$, and both products are analytic there. At $m$, $(x-m)P\to1$ and $(x-m)^2Q\to m^2\omega^2$, again with analytic extensions. Thus $\boxed{x=0\text{ and }x=m\text{ are regular singular points}}$, and there are no other finite singular points.

Infinity must also be considered because the question asks for all singular points. Put $t=1/x$ and $Y(t)=y(1/t)$. The coefficient of $Y$ in its normal-form equation is $Q(1/t)/t^4\sim\omega^2/t^4$. Multiplication by $t^2$ does not make it analytic at zero. Hence $\boxed{x=\infty\text{ is an irregular singular point}}$.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Set $t=x-m$ and use the [Frobenius solution](../../complex-analysis.md#frobenius-solution) $y=t^\nu(a_0+a_1t+\cdots)$ with $a_0\ne0$. From part (a), the leading coefficients are $P\sim1/t$ and $Q\sim m^2\omega^2/t^2$. The coefficient of the lowest power $t^{\nu-2}$ is therefore

$$
[\nu(\nu-1)+\nu+m^2\omega^2]a_0.
$$

The [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) reduces to $\nu^2+m^2\omega^2=0$, giving

$$
\boxed{\nu_+=im\omega,\qquad\nu_-=-im\omega.}
$$

Since $m\omega>0$, the two [indicial roots](../../linear-ordinary-differential-equation.md#indicial-root) differ by a nonzero imaginary number, not an integer. Thus the two local [Frobenius solutions](../../complex-analysis.md#frobenius-solution) exist independently on a chosen branch of $\log(x-m)$.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Define the [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) by $W=y_1y_2'-y_1'y_2$. Differentiating and using the normal-form [differential equation](../../differential-equation.md) gives

$$
W'=y_1y_2''-y_1''y_2=-P(x)(y_1y_2'-y_1'y_2)=-P(x)W.
$$

Integrating this first-order [linear differential equation](../../differential-equation.md#linear-differential-equation) proves [Abel's identity](../../linear-ordinary-differential-equation.md#abel-s-identity):

$$
\boxed{W(x)=C\exp\left[-\int^x p(u)\,du\right],\qquad p(u)=\frac1u+\frac1{u-m}.}
$$

Thus, on any interval avoiding zero and $m$,

$$
\boxed{W(x)=\frac{C}{x(x-m)}}.
$$

Absolute-value signs from real logarithms can be absorbed into the constant on each such interval. For [linearly independent](../../vector-space.md#linear-independence) solutions, $C\ne0$.

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

At zero the [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) is $\nu(\nu-1)+\nu=\nu^2=0$, with repeated [indicial root](../../linear-ordinary-differential-equation.md#indicial-root) zero. To exhibit the analytic solution rather than only its candidate exponent, clear the denominator in the normal form:

$$
x(x-m)^2y''+(2x-m)(x-m)y'+\omega^2x^3y=0.
$$

Substitute $y_1=\sum_{n\geq0}b_nx^n$ and equate coefficients. With $b_j=0$ for negative indices, the [linear recurrence relation](../../algebra.md#linear-recurrence-relation) is

$$
\boxed{m^2(n+1)^2b_{n+1}=mn(2n+1)b_n-n(n-1)b_{n-1}-\omega^2b_{n-3},\qquad n\geq0.}
$$

Every leading coefficient on the left is nonzero. Hence $b_0\ne0$ is free and all later coefficients are determined; the [Frobenius method](../../complex-analysis.md#frobenius-method) guarantees local convergence up to the next singularity. In particular,

$$
b_1=b_2=b_3=0,\qquad b_4=-\frac{\omega^2b_0}{16m^2},\qquad y_1=b_0\left[1-\frac{\omega^2x^4}{16m^2}+O(x^5)\right].
$$

For a second solution, use [reduction of order](../../linear-ordinary-differential-equation.md#reduction-of-order). Writing $y_2=y_1v$ gives $W=y_1^2v'$, so part (c) yields

$$
\boxed{y_2(x)=y_1(x)\int^x\frac{C\,ds}{s(s-m)y_1(s)^2},\qquad C\ne0.}
$$

The additive constant in the [integral](../../integral.md) only adds a multiple of $y_1$. As $x\downarrow0$ within $(0,m)$, its integrand is

$$
\frac{C}{x(x-m)y_1(x)^2}=-\frac{C}{mb_0^2}\frac1x+O(1).
$$

Therefore

$$
\boxed{y_2(x)=c_0\log x+O(1),\qquad c_0=-\frac{C}{mb_0}\ne0.}
$$

The nonzero [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) proves [linear independence](../../vector-space.md#linear-independence), and the logarithm is unavoidable for this second local solution.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

For fixed initial and final coordinates, the two [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) are

$$
\boxed{\frac d{dt}\left(\frac{\partial f}{\partial\dot x}\right)-\frac{\partial f}{\partial x}=0,\qquad\frac d{dt}\left(\frac{\partial f}{\partial\dot y}\right)-\frac{\partial f}{\partial y}=0.}
$$

Indeed the [first variation](../../calculus-of-variations.md#first-variation) of the [functional](../../calculus-of-variations.md#functional) is

$$
\delta F=\int_0^T(f_x\delta x+f_y\delta y+f_{\dot x}\delta\dot x+f_{\dot y}\delta\dot y)\,dt.
$$

[Integration by parts](../../calculus.md#integration-by-parts) moves the time [derivatives](../../calculus.md#derivative) from the [variations](../../calculus-of-variations.md#variation); their endpoint values are zero. The [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) then gives the two equations above.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

The [total derivative](../../calculus.md#total-derivative) contributes only the [boundary term](../../calculus.md#boundary-term)

$$
\int_0^T\frac d{dt}g(x,y)\,dt=g(x(T),y(T))-g(x(0),y(0)).
$$

This is fixed by the endpoint data, so its [first variation](../../calculus-of-variations.md#first-variation) vanishes. It cannot change the [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) or which path minimizes $F$.

For a direct check, let $h=g_x\dot x+g_y\dot y$. Then

$$
\frac d{dt}h_{\dot x}=g_{xx}\dot x+g_{xy}\dot y=h_x,\qquad\frac d{dt}h_{\dot y}=g_{yx}\dot x+g_{yy}\dot y=h_y.
$$

The equality uses commuting mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative). Thus $\boxed{d g/dt\text{ contributes zero to both Euler-Lagrange equations}}$, as in [total time derivatives preserve fixed-endpoint Euler-Lagrange equations](../../analysis.md#total-time-derivatives-preserve-fixed-endpoint-euler-lagrange-equations).

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

This is an [isoperimetric constraint](../../analysis.md#isoperimetric-constraint), imposed on the whole path rather than separately at each time. Introduce a constant [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) $\lambda$ and replace the variational integrand by $\widetilde f=f+\lambda u$. The modified [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) are

$$
\boxed{\frac d{dt}f_{\dot x}-f_x-\lambda u_x=0,\qquad\frac d{dt}f_{\dot y}-f_y-\lambda u_y=0.}
$$

Solve these together with the fixed endpoint conditions, treating $\lambda$ as an unknown constant, then choose its value so that

$$
\boxed{\int_0^Tu(x(t),y(t))\,dt=0.}
$$

The multiplier is constant because there is one scalar [integral](../../integral.md) constraint. A condition imposed at every time would instead call for a time-dependent multiplier. As usual, this multiplier procedure assumes the constraint is regular, so its [first variation](../../calculus-of-variations.md#first-variation) does not vanish identically on all admissible [variations](../../calculus-of-variations.md#variation).

<h3 id="9/d">d</h3>

↑ **Parent:** [9](#9)

<h4 id="9/d/solution">Solution</h4>

↑ **Parent:** [D](#9/d)

The needed partial [derivatives](../../calculus.md#derivative) are

$$
\begin{aligned}
f_x&=\alpha\beta(1+\gamma_1\dot x+\gamma_2\dot y),&f_y&=0,\\
f_{\dot x}&=\alpha\gamma_1(1+\beta x)+\delta_1\dot x,&f_{\dot y}&=\alpha\gamma_2(1+\beta x)+\delta_2\dot y.
\end{aligned}
$$

Substitution into the [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) gives

$$
\alpha\beta\gamma_1\dot x+\delta_1\ddot x=\alpha\beta(1+\gamma_1\dot x+\gamma_2\dot y),\qquad\alpha\beta\gamma_2\dot x+\delta_2\ddot y=0.
$$

The $\gamma_1$ terms cancel in the first equation, leaving

$$
\boxed{\delta_1\ddot x=\alpha\beta(1+\gamma_2\dot y),\qquad\delta_2\ddot y=-\alpha\beta\gamma_2\dot x.}
$$

These are accompanied by $x(0)=y(0)=0$ and $x(T)=y(T)=S$. The cancellation is consistent with part (b): the term proportional to $\gamma_1$ is the [total derivative](../../calculus.md#total-derivative) of $\alpha\gamma_1(x+\beta x^2/2)$.

<h3 id="9/e">e</h3>

↑ **Parent:** [9](#9)

<h4 id="9/e/solution">Solution</h4>

↑ **Parent:** [E](#9/e)

Impose $y=x$ before varying. Writing $\delta=\delta_1+\delta_2$, the restricted integrand is

$$
f_{\mathrm{line}}=\alpha(1+\beta x)+\alpha(\gamma_1+\gamma_2)(1+\beta x)\dot x+\frac\delta2\dot x^2.
$$

Its middle term is the [total derivative](../../calculus.md#total-derivative) of $\alpha(\gamma_1+\gamma_2)(x+\beta x^2/2)$, so it can be dropped for fixed endpoints by part (b). The remaining [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is $\delta\ddot x=\alpha\beta$. Integrating twice and imposing $x(0)=0$, $x(T)=S$ gives

$$
\boxed{x(t)=y(t)=\frac STt-\frac{\alpha\beta}{2(\delta_1+\delta_2)}t(T-t),\qquad0\leq t\leq T.}
$$

This is the unique [global minimizer](../../analysis.md#global-minimizer) among paths on the specified line. To prove it, add any admissible [variation](../../calculus-of-variations.md#variation) $\eta$ with $\eta(0)=\eta(T)=0$. The change in fuel, after dropping the fixed [boundary term](../../calculus.md#boundary-term), is

$$
F[x+\eta]-F[x]=\int_0^T[\alpha\beta\eta+\delta\dot x\dot\eta]dt+\frac\delta2\int_0^T\dot\eta^2dt=\frac\delta2\int_0^T\dot\eta^2dt\geq0.
$$

The first [integral](../../integral.md) vanishes by [integration by parts](../../calculus.md#integration-by-parts) and the equation for $x$. Equality forces $\eta=0$. No monotonicity or restriction to the segment between endpoints was imposed in the question; the minimizing coordinate can initially decrease for sufficiently large $T$.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Use the standard regular [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) hypotheses: positive weight $w$, real coefficients, and real [self-adjoint](../../linear-operator-theory.md#self-adjoint-operator) [boundary conditions](../../differential-equation.md#boundary-condition). The positive weight and boundary-domain assumptions are implicit in the requested real [orthonormal basis](../../inner-product.md#orthonormal-basis); real differential coefficients alone would not guarantee them for arbitrary complex boundary conditions.

Multiply the [eigenfunction](../../linear-operator-theory.md#eigenfunction) equation by $\overline{y_n}$ and integrate. By [self-adjointness](../../linear-operator-theory.md#self-adjoint-operator), the number $\int_a^b\overline{y_n}\mathcal Ly_n\,dx$ is real, whereas

$$
\int_a^b\overline{y_n}\mathcal Ly_n\,dx=\lambda_n\int_a^bw|y_n|^2dx.
$$

The second [integral](../../integral.md) is strictly positive, so $\boxed{\lambda_n\in\mathbb R}$. Because the coefficients and [boundary conditions](../../differential-equation.md#boundary-condition) are real, the real and imaginary parts of any complex [eigenfunction](../../linear-operator-theory.md#eigenfunction) separately obey the same equation and conditions. At least one is nonzero, so a real [eigenfunction](../../linear-operator-theory.md#eigenfunction) can be chosen. More generally, each [eigenspace](../../linear-operator-theory.md#eigenspace) has a real basis, which can be orthonormalized using the [weighted inner product](../../inner-product.md#weighted-inner-product).

The [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions), with normalization chosen to one, is

$$
\boxed{\int_a^bw(x)\overline{y_m(x)}y_n(x)\,dx=\delta_{mn}.}
$$

For the real choice, omit the complex conjugate.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

The [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) of a suitable real function $f$ is

$$
f(x)=\sum_ny_n(x)\int_a^bw(\xi)y_n(\xi)f(\xi)\,d\xi=\int_a^b\left[w(\xi)\sum_ny_n(\xi)y_n(x)\right]f(\xi)\,d\xi.
$$

Comparing this identity with the sampling property of the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function) gives the completeness kernel

$$
\boxed{w(\xi)\sum_ny_n(\xi)y_n(x)=\delta(x-\xi).}
$$

This is an identity of [distributions](../../distribution-theory.md#distribution-mathematical-analysis), rather than a pointwise-convergent series of ordinary functions.

Assuming zero is not an [eigenvalue](../../linear-operator-theory.md#eigenvalue), define the [spectral Green function of a regular Sturm-Liouville problem](../../sturm-liouville-theory.md#spectral-green-function-of-a-regular-sturm-liouville-problem) by

$$
\boxed{G(x;\xi)=\sum_n\frac{y_n(x)y_n(\xi)}{\lambda_n}.}
$$

Applying $\mathcal L_x$ gives $w(x)\sum_ny_n(x)y_n(\xi)=\delta(x-\xi)$: multiplying the preceding completeness kernel by $w(x)/w(\xi)$ leaves the [Dirac delta distribution](../../distribution-theory.md#dirac-delta-function) unchanged. Each term also obeys the same homogeneous [boundary conditions](../../differential-equation.md#boundary-condition). There is no extra weight factor in $G$ for the ordinary source measure $d\xi$.

If zero is an [eigenvalue](../../linear-operator-theory.md#eigenvalue), the inverse [Green's function](../../green-s-function.md) does not exist on all forcing functions: the forcing must obey the [solvability condition at a Sturm-Liouville eigenvalue](../../sturm-liouville-theory.md#solvability-condition-at-a-sturm-liouville-eigenvalue). Omitting the zero mode instead constructs a reduced inverse, with its projection removed from the right-hand side. This exception occurs in part (c) at $\alpha=1$.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Write the endpoint condition in its linear [Robin boundary condition](../../differential-equation.md#robin-boundary-condition) form $y'(1)=y(1)/\alpha$. For a positive [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\lambda=q^2$, the left [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) gives $y=C\sin(qx)$, and the right condition gives

$$
q\cos q=\frac1\alpha\sin q,\qquad\boxed{\tan q=\alpha q.}
$$

For each positive root $q_n$, the squared [norm](../../normed-vector-space.md#norm) is

$$
N_n=\int_0^1\sin^2(q_nx)\,dx=\frac12-\frac{\sin(2q_n)}{4q_n}.
$$

Consequently the sine coefficients in any complete expansion are

$$
\boxed{a_n=\frac{\int_0^1f(x)\sin(q_nx)\,dx}{N_n}=\frac{2\int_0^1f(x)\sin(q_nx)\,dx}{1-\sin(2q_n)/(2q_n)}.}
$$

When $\alpha>1$, these are all modes and the [Sturm-Liouville eigenfunction expansion](../../sturm-liouville-theory.md#sturm-liouville-eigenfunction-expansion) gives exactly the stated sine series, with the usual convergence interpretation. Positivity of all [eigenvalues](../../linear-operator-theory.md#eigenvalue) follows from [integration by parts](../../calculus.md#integration-by-parts) and the [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
\int_0^1y(-y'')dx=\int_0^1(y')^2dx-\frac{y(1)^2}{\alpha}\geq\left(1-\frac1\alpha\right)\int_0^1(y')^2dx>0
$$

for a nonzero admissible $y$, since $y(1)=\int_0^1y'\,dx$.

However, the original PDF states only $\alpha>0$, and with that range its sine-only completeness claim is false. The missing modes are as follows. At $\alpha=1$, $\lambda=0$ admits $y=x$, so the correct expansion is

$$
\boxed{f(x)=3x\int_0^1t f(t)\,dt+\sum_{n\geq1}a_n\sin(q_nx),\qquad\alpha=1.}
$$

For $0<\alpha<1$, a negative [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\lambda=-\kappa^2$ admits $y=\sinh(\kappa x)$, with

$$
\boxed{\tanh\kappa=\alpha\kappa,\qquad\kappa>0.}
$$

There is exactly one positive root: $\tanh\kappa/\kappa$ decreases strictly from $1$ to zero. For example, its [derivative](../../calculus.md#derivative) has the sign of $\kappa\operatorname{sech}^2\kappa-\tanh\kappa<0$, because $\sinh\kappa\cosh\kappa>\kappa$. Thus the corrected expansion is

$$
\boxed{f(x)=a_-\sinh(\kappa x)+\sum_{n\geq1}a_n\sin(q_nx),\quad a_-=\frac{\int_0^1f(t)\sinh(\kappa t)\,dt}{\sinh(2\kappa)/(4\kappa)-1/2},\quad0<\alpha<1.}
$$

These are the [nonpositive modes in a Dirichlet-Robin interval expansion](../../sturm-liouville-theory.md#nonpositive-modes-in-a-dirichlet-robin-interval-expansion). As an explicit counterexample to the printed claim, at $\alpha=1$ take $f(x)=x$: it satisfies both [boundary conditions](../../differential-equation.md#boundary-condition), and each positive root obeys

$$
\int_0^1x\sin(q_nx)\,dx=-\frac{\cos q_n}{q_n}+\frac{\sin q_n}{q_n^2}=0
$$

because $\tan q_n=q_n$. Thus all $a_n$ vanish despite $f\ne0$. Likewise $f=\sinh(\kappa x)$ is a counterexample for $\alpha<1$, by [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions) with distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue). The formulas above give the full solution without silently assuming away the omitted modes.

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

Put $s_n(x)=\sin(q_nx)$ and $s_m(x)=\sin(q_mx)$. Their [differential equations](../../differential-equation.md) are $-s_n''=q_n^2s_n$ and $-s_m''=q_m^2s_m$. Subtract the two cross-multiplied equations and use [integration by parts](../../calculus.md#integration-by-parts):

$$
(q_n^2-q_m^2)\int_0^1s_ns_m\,dx=[s_ns_m'-s_ms_n']_0^1.
$$

The lower boundary term is zero because both functions vanish there. At the upper endpoint, the [Robin boundary condition](../../differential-equation.md#robin-boundary-condition) gives $s_j'(1)=s_j(1)/\alpha$, so

$$
s_n(1)s_m'(1)-s_m(1)s_n'(1)=\frac{s_n(1)s_m(1)}\alpha-\frac{s_m(1)s_n(1)}\alpha=0.
$$

Since distinct positive roots have $q_n^2\ne q_m^2$, we conclude

$$
\boxed{\int_0^1\sin(q_nx)\sin(q_mx)\,dx=0,\qquad n\ne m.}
$$

This [orthogonality](../../inner-product.md#orthogonal-vectors) holds for every $\alpha>0$, even when the sine family requires the additional nonpositive mode for completeness as explained in part (c).

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
