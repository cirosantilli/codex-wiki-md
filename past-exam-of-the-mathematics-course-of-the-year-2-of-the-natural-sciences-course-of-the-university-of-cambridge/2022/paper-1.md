# Paper 1

↑ **Parent:** [2022](../2022.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2022/papernst_ib_1_2022.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2022/papernst_ib_1_2022.pdf)

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
    - [i](#7/c/i)
      - [Solution](#7/c/i/solution)
    - [ii](#7/c/ii)
      - [Solution](#7/c/ii/solution)
    - [iii](#7/c/iii)
      - [Solution](#7/c/iii/solution)
  - [d](#7/d)
    - [Solution](#7/d/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [i](#8/b/i)
      - [Solution](#8/b/i/solution)
    - [ii](#8/b/ii)
      - [Solution](#8/b/ii/solution)
    - [iii](#8/b/iii)
      - [Solution](#8/b/iii/solution)
    - [iv](#8/b/iv)
      - [Solution](#8/b/iv/solution)
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

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\rho=\sqrt{x^2+y^2}=uv$. The condition $u\leq v$ gives $z\leq0$. On the outer coordinate surface $v=1$, elimination of $u$ gives $z=(\rho^2-1)/2$. On $u=v$, the surface is the plane $z=0$, with $\rho=u^2\leq1$. Thus the closure of the body is

$$
\boxed{0\leq\rho\leq1,\qquad\frac{\rho^2-1}{2}\leq z\leq0.}
$$

It is a solid circular cap bounded below by an [elliptic paraboloid](../../euclidean-geometry.md#elliptic-paraboloid) of revolution and above by the unit disk in $z=0$. Its vertex is $\boxed{(0,0,-1/2)}$, its height is $\boxed{1/2}$, and its rim is the [circle](../../topology.md#circle) $\boxed{x^2+y^2=1,\ z=0}$. The symmetry axis is the $z$ axis. The coordinate surface $u=0$ maps to that axis rather than to an additional two-dimensional boundary. These are [parabolic coordinates](../../multivariable-calculus.md#parabolic-coordinates).

<a id="1/a/image-the-solid-cap-bounded-by-an-elliptic-paraboloid-and-the-disk-z-0-with-a-filled-meridian-cross-section"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1-paraboloidal-cap.png)

**[Figure 1](#1/a/image-the-solid-cap-bounded-by-an-elliptic-paraboloid-and-the-disk-z-0-with-a-filled-meridian-cross-section). The solid cap bounded by an elliptic paraboloid and the disk $z=0$, with a filled meridian cross-section**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Differentiate the position [vector](../../vector-space.md#vector) with respect to the three coordinates to obtain the [coordinate basis](../../tangent-vector.md#coordinate-basis) vectors:

$$
\boxed{\mathbf h_u=\begin{pmatrix}v\cos\phi\\v\sin\phi\\u\end{pmatrix},\qquad\mathbf h_v=\begin{pmatrix}u\cos\phi\\u\sin\phi\\-v\end{pmatrix},\qquad\mathbf h_\phi=\begin{pmatrix}-uv\sin\phi\\uv\cos\phi\\0\end{pmatrix}.}
$$

The [chain rule](../../calculus.md#chain-rule) gives $d\mathbf x=\mathbf h_u du+\mathbf h_v dv+\mathbf h_\phi d\phi$. The [scale factors of orthogonal coordinates](../../multivariable-calculus.md#scale-factors-of-orthogonal-coordinates) are the corresponding [norms](../../normed-vector-space.md#norm):

$$
\boxed{h_u=h_v=\sqrt{u^2+v^2},\qquad h_\phi=uv.}
$$

Direct [dot products](../../inner-product.md#dot-product) give $\mathbf h_u\cdot\mathbf h_v=uv-uv=0$, $\mathbf h_u\cdot\mathbf h_\phi=0$, and $\mathbf h_v\cdot\mathbf h_\phi=0$. Thus the [parabolic coordinates](../../multivariable-calculus.md#parabolic-coordinates) are orthogonal wherever the coordinate vectors are nondegenerate. Their degeneracy on $uv=0$ is the usual axis degeneracy of the azimuthal coordinate.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Jacobian determinant](../../multivariable-calculus.md#jacobian-determinant) is the oriented [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) of the three [coordinate basis](../../tangent-vector.md#coordinate-basis) vectors:

$$
J=\det\frac{\partial(x,y,z)}{\partial(u,v,\phi)}=(\mathbf h_u\times\mathbf h_v)\cdot\mathbf h_\phi.
$$

Here $\mathbf h_u\times\mathbf h_v=(u^2+v^2)(-\sin\phi,\cos\phi,0)$, so

$$
\boxed{J=uv(u^2+v^2),\qquad dV=uv(u^2+v^2)\,du\,dv\,d\phi.}
$$

The sign is nonnegative on the stated range, and the absolute [Jacobian determinant](../../multivariable-calculus.md#jacobian-determinant) also equals $h_uh_vh_\phi$ as expected for [orthogonal coordinates](../../multivariable-calculus.md#orthogonal-coordinates).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Since $\mathbf F=\nabla\Omega$, its [divergence](../../multivariable-calculus.md#divergence) is the [Laplacian](../../multivariable-calculus.md#laplacian) of $\Omega$:

$$
\nabla\cdot\mathbf F=\nabla^2\Omega=6x+4z.
$$

The [divergence theorem](../../multivariable-calculus.md#divergence-theorem) changes the outward [flux](../../mathematical-physics.md#flux) through the whole closed boundary into $I=\int_V(6x+4z)dV$. Rotational symmetry makes the $x$ term vanish. With $z=(u^2-v^2)/2$ and the [Jacobian determinant](../../multivariable-calculus.md#jacobian-determinant) from part (c),

$$
\begin{aligned}
I&=2\int_{-\pi}^{\pi}\int_0^1\int_0^v(u^2-v^2)uv(u^2+v^2)\,du\,dv\,d\phi\\
&=4\pi\int_0^1v\left[\frac{u^6}{6}-\frac{v^4u^2}{2}\right]_{u=0}^{u=v}dv\\
&=-\frac{4\pi}{3}\int_0^1v^7\,dv
=\boxed{-\frac\pi6}.
\end{aligned}
$$

Both the curved face and the top disk are included in this [surface integral](../../multivariable-calculus.md#surface-integral) through the [divergence theorem](../../multivariable-calculus.md#divergence-theorem).

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Remove the common nonzero factor $e^{-i\omega t}$ and expand in the small parameter $\epsilon$. To first order, the modified [Laplacian](../../multivariable-calculus.md#laplacian) contributes only its $y$ derivatives: its $x$ derivative term has the extra factor $\epsilon^2$. The [regular perturbation](../../asymptotic-expansion.md#regular-perturbation) expansion therefore gives

$$
\boxed{P=-i\omega b_0+\omega\psi_{0,y},\qquad Q=-i\omega b_1+\omega\psi_{1,y}+\psi_{0,x}-b_{0,yy},}
$$



$$
\boxed{R=-i\omega\psi_{0,yy}-\omega b_{0,y},\qquad S=-i\omega\psi_{1,yy}-\omega b_{1,y}-b_{0,x}.}
$$

Thus the two residuals are $P+\epsilon Q+O(\epsilon^2)$ and $R+\epsilon S+O(\epsilon^2)$, respectively. Subscripts after a comma denote [partial derivatives](../../multivariable-calculus.md#partial-derivative). We retain $\omega\ne0$, as appropriate to the oscillatory wave and the elimination below.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Insert the proposed leading relation into the two zeroth-order residuals. It gives

$$
P=-i\omega(-i\psi_{0,y})+\omega\psi_{0,y}=0,
$$

and, since $b_{0,y}=-i\psi_{0,yy}$,

$$
R=-i\omega\psi_{0,yy}-\omega(-i\psi_{0,yy})=0.
$$

Hence $\boxed{b_0=-i\psi_{0,y}\ \Longrightarrow\ P=R=0}$. The same relation is forced by $P=0$ when $\omega\ne0$; its $y$ derivative then automatically gives $R=0$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The first-order condition $Q=0$, combined with $b_0=-i\psi_{0,y}$, gives

$$
b_1=-i\psi_{1,y}-\frac i\omega\psi_{0,x}+\frac1\omega\psi_{0,yyy}.
$$

Differentiate this expression with respect to $y$ and insert it into $S=0$. The $\psi_1$ terms cancel, leaving

$$
\begin{aligned}
0&=-i\omega\psi_{1,yy}-\omega\left[-i\psi_{1,yy}-\frac i\omega\psi_{0,xy}+\frac1\omega\psi_{0,yyyy}\right]+i\psi_{0,xy}\\
&=2i\psi_{0,xy}-\psi_{0,yyyy}.
\end{aligned}
$$

Thus the compatibility [partial differential equation](../../partial-differential-equation.md) is

$$
\boxed{2\psi_{0,xy}+i\psi_{0,yyyy}=0.}
$$

It is exactly $\partial_y(2\psi_{0,x}+i\psi_{0,yyy})=0$. Integrating with respect to $y$ therefore gives

$$
\boxed{2\psi_{0,x}+i\psi_{0,yyy}=f(x),}
$$

where the integration constant may be any function of $x$. Conversely, differentiating this last equation with respect to $y$ recovers the compatibility equation.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For [separation of variables](../../partial-differential-equation.md#separation-of-variables) matching the boundary [Fourier mode](../../fourier-analysis.md#fourier-mode), take $\psi_0=X(x)e^{iky}$ with $X(0)=1$. Because $\partial_y^3e^{iky}=-ik^3e^{iky}$, the reduced [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) is

$$
2X'+k^3X=0.
$$

Therefore

$$
\boxed{\psi_0(x,y)=e^{-k^3x/2}e^{iky}.}
$$

The [decay of a Fourier mode in a third-order spatial evolution equation](../../partial-differential-equation.md#decay-of-a-fourier-mode-in-a-third-order-spatial-evolution-equation) requires a sign check: this satisfies the requested limit at positive infinity precisely when $\boxed{k>0}$. For $k=0$ it remains identically one, while for $k<0$ its amplitude grows exponentially. Hence for those nonpositive values there is no separated solution meeting both prescribed [boundary conditions](../../differential-equation.md#boundary-condition); the printed assumption that $k$ is merely real needs this additional restriction for decay.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The homogeneous equation is a [Cauchy-Euler equation](../../linear-ordinary-differential-equation.md#cauchy-euler-equation). With the [power-law ansatz](../../linear-ordinary-differential-equation.md#power-law-ansatz) $y=x^r$ on $x>0$, its [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) is

$$
r(r-1)+\alpha r+\frac{(\alpha-1)^2}{4}=\left(r+\frac{\alpha-1}{2}\right)^2=0.
$$

Thus $r=(1-\alpha)/2$ is a repeated [indicial root](../../linear-ordinary-differential-equation.md#indicial-root). The two independent solutions are $x^r$ and $x^r\log x$, giving

$$
\boxed{y_h(x)=x^{(1-\alpha)/2}(C_1+C_2\log x),\qquad x>0.}
$$

Their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian), with $W=y_1y_2'-y_1'y_2$, is $x^{2r-1}=x^{-\alpha}\ne0$, verifying [linear independence](../../vector-space.md#linear-independence).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose the [causal Green function](../../green-s-function.md#causal-green-function) convention $L_xG(x,\xi)=\delta(x-\xi)$ for each source point $\xi>0$, with $G(x,\xi)=0$ when $x<\xi$. This automatically gives the two zero-origin limits. The kernel is continuous at $x=\xi$, and integrating its equation across the source requires the unit [derivative](../../calculus.md#derivative) jump $\partial_xG(\xi^+,\xi)-\partial_xG(\xi^-,\xi)=1$.

For $x>\xi$, the homogeneous basis from part (a) gives a continuous kernel proportional to $x^r\log(x/\xi)$. Its derivative at $x=\xi$ is $\xi^{r-1}$, so the normalization is $\xi^{1-r}$. Hence the [causal Green function for a repeated-root Euler operator](../../green-s-function.md#causal-green-function-for-a-repeated-root-euler-operator) is

$$
\boxed{G(x,\xi)=\begin{cases}x^r\xi^{1-r}\log(x/\xi),&x\geq\xi,\\0,&0\leq x<\xi,\end{cases}\qquad r=\frac{1-\alpha}{2},\quad\xi>0.}
$$

The same formula follows from $[y_1(\xi)y_2(x)-y_2(\xi)y_1(x)]/W(\xi)$ on the right of the source, with $W(\xi)=\xi^{-\alpha}$.

The singular endpoint matters for uniqueness. If $\alpha<-1$, then $r>1$, and both $x^r$ and $x^r\log x$, together with their first [derivatives](../../calculus.md#derivative), vanish at zero. Adding any source-dependent linear combination of these homogeneous solutions to $G$ preserves the two stated origin conditions. Thus those conditions alone do not determine a unique [Green's function](../../green-s-function.md) in that parameter range. The causal requirement used here selects the displayed kernel. For $\alpha\geq-1$ no nonzero homogeneous solution satisfies both zero-origin limits, so this ambiguity is absent.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Using the causal [Green's function](../../green-s-function.md),

$$
y_p(x)=\int_0^xG(x,\xi)\xi\,d\xi=x^r\int_0^x\xi^{2-r}\log(x/\xi)\,d\xi.
$$

Put $\xi=xs$. Since $\alpha>-5$ is equivalent to $r<3$, the [improper integral](../../real-analysis.md#improper-integral) converges and gives

$$
y_p(x)=x^3\int_0^1s^{2-r}(-\log s)\,ds=\frac{x^3}{(3-r)^2}=\boxed{\frac{4x^3}{(\alpha+5)^2}.}
$$

The elementary identity $\int_0^1s^{p-1}(-\log s)ds=1/p^2$ follows by differentiating $\int_0^1s^{p-1}ds=1/p$ for $p>0$. Direct substitution checks $L(x^3)=(\alpha+5)^2x/4$, and the displayed solution and its first [derivative](../../calculus.md#derivative) vanish at zero.

To give all solutions allowed by the printed [boundary conditions](../../differential-equation.md#boundary-condition), retain the singular-endpoint qualification from part (b):

$$
\boxed{y(x)=\begin{cases}\dfrac{4x^3}{(\alpha+5)^2}+x^{(1-\alpha)/2}(C_1+C_2\log x),&-5<\alpha<-1,\\\dfrac{4x^3}{(\alpha+5)^2},&\alpha\geq-1.\end{cases}}
$$

Thus the causal integral gives a particular member of a two-parameter family in the first range and the unique solution in the second.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For [integrable functions](../../measure-theory.md#lebesgue-integrable-function) $f,g$, [Fubini's theorem](../../measure-theory.md#fubini-s-theorem) justifies exchanging the two [integrals](../../integral.md) in the [Fourier transform](../../fourier-transform.md) of the [convolution](../../fourier-analysis.md#convolution). Set $s=x-t$ to obtain

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\int_{\mathbb R}f(t)g(x-t)e^{-ikx}\,dt\,dx\\
&=\int_{\mathbb R}\int_{\mathbb R}f(t)g(s)e^{-ik(s+t)}\,ds\,dt\\
&=\left[\int_{\mathbb R}f(t)e^{-ikt}dt\right]\left[\int_{\mathbb R}g(s)e^{-iks}ds\right].
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

Direct evaluation gives the first [Fourier transform](../../fourier-transform.md):

$$
\widetilde f(k)=\int_{-1/2}^{1/2}e^{-ikx}\,dx=\boxed{\frac{2\sin(k/2)}{k}},\qquad\boxed{\widetilde f(0)=1}.
$$

For the even [triangular function](../../fourier-analysis.md#triangular-function), the odd sine part integrates to zero. Two elementary [integrations by parts](../../calculus.md#integration-by-parts) or one evaluation of the cosine integral give

$$
\widetilde g(k)=2\int_0^1(1-x)\cos(kx)\,dx=\frac{2(1-\cos k)}{k^2}=\boxed{\frac{4\sin^2(k/2)}{k^2}},\qquad\boxed{\widetilde g(0)=1}.
$$

The values at zero are the respective areas, agreeing with the removable limits. Therefore $\widetilde g=\widetilde f^{\,2}$. By the [convolution theorem](../../fourier-analysis.md#convolution-theorem) and uniqueness of the [Fourier transform](../../fourier-transform.md),

$$
\boxed{(f*f)(x)=g(x)=\begin{cases}1-|x|,&|x|<1,\\0,&|x|\geq1.\end{cases}}
$$

There is also a direct interpretation: the [convolution](../../fourier-analysis.md#convolution) is the length of overlap of the intervals $(-1/2,1/2)$ and $(x-1/2,x+1/2)$, giving exactly that triangular profile.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Parseval identity](../../fourier-analysis.md#parseval-identity) for this [Fourier transform](../../fourier-transform.md) convention is

$$
\boxed{\int_{\mathbb R}|h(x)|^2dx=\frac1{2\pi}\int_{\mathbb R}|\widetilde h(k)|^2dk.}
$$

Apply it to $h=g$. Its squared [norm](../../normed-vector-space.md#norm) is $2\int_0^1(1-x)^2dx=2/3$, so

$$
\frac23=\frac1{2\pi}\int_{\mathbb R}\frac{16\sin^4(k/2)}{k^4}\,dk.
$$

Under $k=2x$, the last integrand times $dk$ becomes $2\sin^4x\,dx/x^4$. Consequently

$$
\boxed{\int_{-\infty}^{\infty}\frac{\sin^4x}{x^4}dx=\frac{2\pi}{3}.}
$$

The integrand has continuous value $1$ at zero and decays integrably at infinity, so this is an ordinary convergent [improper integral](../../real-analysis.md#improper-integral).

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A square [matrix](../../vector-space.md#matrix) is a [diagonalizable matrix](../../linear-operator-theory.md#diagonalizable-matrix) over the chosen field when there are an [invertible matrix](../../linear-algebra.md#invertible-matrix) $P$ and a [diagonal matrix](../../linear-algebra.md#diagonal-matrix) $D$ such that $A=PDP^{-1}$. If $v_j$ is column $j$ of $P$ and $D_{jj}=\lambda_j$, the identity $AP=PD$ gives $Av_j=\lambda_jv_j$. Invertibility makes these $n$ columns [linearly independent](../../vector-space.md#linear-independence) [eigenvectors](../../linear-operator-theory.md#eigenvector).

Conversely, put $n$ [linearly independent](../../vector-space.md#linear-independence) [eigenvectors](../../linear-operator-theory.md#eigenvector) in the columns of $P$ and their [eigenvalues](../../linear-operator-theory.md#eigenvalue) in $D$. Then $P$ is invertible and $AP=PD$, giving

$$
\boxed{A\text{ is diagonalizable}\ \Longleftrightarrow\ A\text{ has an eigenbasis of }n\text{ vectors}.}
$$

Repeated [eigenvalues](../../linear-operator-theory.md#eigenvalue) are allowed; the requirement is a complete [eigenbasis](../../linear-operator-theory.md#eigenbasis), not distinctness of the eigenvalues.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

A single [eigenbasis](../../linear-operator-theory.md#eigenbasis) works for every choice of the parameters. The columns $v_1=(1,0,0)^T$, $v_2=(1,1,0)^T$, $v_3=(1,1,1)^T$ satisfy

$$
Mv_1=av_1,\qquad Mv_2=bv_2,\qquad Mv_3=cv_3.
$$

They are [linearly independent](../../vector-space.md#linear-independence) because their column [matrix](../../vector-space.md#matrix) has determinant one. Thus the [diagonalization](../../linear-operator-theory.md#diagonalization-of-a-matrix) is

$$
\boxed{P=\begin{pmatrix}1&1&1\\0&1&1\\0&0&1\end{pmatrix},\qquad P^{-1}=\begin{pmatrix}1&-1&0\\0&1&-1\\0&0&1\end{pmatrix},\qquad M=P\operatorname{diag}(a,b,c)P^{-1}.}
$$

This formula includes all coincidences among $a,b,c$, so no special repeated-[eigenvalue](../../linear-operator-theory.md#eigenvalue) cases need separate bases.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [diagonalization](../../linear-operator-theory.md#diagonalization-of-a-matrix) in part (b) gives $M^k=P\operatorname{diag}(a^k,b^k,c^k)P^{-1}$. Hence

$$
\boxed{M^k\to0\ \Longleftrightarrow\ |a|<1,\ |b|<1,\ |c|<1.}
$$

Sufficiency follows from the scalar powers tending to zero; necessity also follows immediately from the diagonal entries of $M^k$. Under these conditions the [matrix geometric series](../../linear-algebra.md#matrix-geometric-series) converges, and its sum is

$$
(I-M)^{-1}=P\operatorname{diag}\left(\frac1{1-a},\frac1{1-b},\frac1{1-c}\right)P^{-1}.
$$

Writing $A_0=1/(1-a)$, $B_0=1/(1-b)$ and $C_0=1/(1-c)$, all entries are explicitly

$$
\boxed{(I-M)^{-1}=\begin{pmatrix}A_0&B_0-A_0&C_0-B_0\\0&B_0&C_0-B_0\\0&0&C_0\end{pmatrix}.}
$$

For example, $B_0-A_0=(b-a)/[(1-a)(1-b)]$ and $C_0-B_0=(c-b)/[(1-b)(1-c)]$. These expressions remain valid when parameter values coincide.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Expand the [quadratic form](../../quadratic-form.md) of this [Gram matrix](../../inner-product.md#gram-matrix):

$$
\begin{aligned}
Q(\mathbf c)&=\sum_{i,j}c_ic_j\mathbf x_i^T\mathbf x_j\\
&=\left(\sum_i c_i\mathbf x_i\right)^T\left(\sum_jc_j\mathbf x_j\right)
=\left\|\sum_i c_i\mathbf x_i\right\|^2.
\end{aligned}
$$

For $\mathbf c\ne0$, [linear independence](../../vector-space.md#linear-independence) of the real vectors implies $\sum_i c_i\mathbf x_i\ne0$, so its squared [Euclidean norm](../../normed-vector-space.md#euclidean-norm) is strictly positive. Thus

$$
\boxed{Q(\mathbf c)>0\text{ for every }\mathbf c\ne0,}
$$

proving the [positive definiteness of a Gram matrix](../../inner-product.md#positive-definiteness-of-a-gram-matrix) in the independent-vector case.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [skew-Hermitian matrix](../../linear-operator-theory.md#skew-hermitian-matrix) satisfies $A^\dagger=-A$, where $\dagger$ denotes the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose). If $Av=\lambda v$ with $v\ne0$, then

$$
\overline\lambda\,v^\dagger v=v^\dagger A^\dagger v=-v^\dagger Av=-\lambda\,v^\dagger v.
$$

Since $v^\dagger v>0$, this gives $\boxed{\overline\lambda=-\lambda,\text{ so }\lambda\in i\mathbb R}$.

A [unitary matrix](../../linear-operator-theory.md#unitary-matrix) satisfies $U^\dagger U=UU^\dagger=I$. It preserves the [Hermitian inner product](../../linear-algebra.md#hermitian-inner-product) and [norm](../../normed-vector-space.md#norm). Thus if $Uv=\mu v$,

$$
\|v\|^2=\|Uv\|^2=|\mu|^2\|v\|^2,
$$

and therefore $\boxed{|\mu|=1}$. Zero is allowed among the purely imaginary [eigenvalues](../../linear-operator-theory.md#eigenvalue) in the first statement, but not among the unitary [eigenvalues](../../linear-operator-theory.md#eigenvalue).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Let $Av_i=\lambda_i v_i$ and $Av_j=\lambda_jv_j$. The [skew-Hermitian matrix](../../linear-operator-theory.md#skew-hermitian-matrix) property gives

$$
\lambda_jv_i^\dagger v_j=v_i^\dagger Av_j=-(Av_i)^\dagger v_j=-\overline\lambda_i\,v_i^\dagger v_j=\lambda_i v_i^\dagger v_j,
$$

where the last equality uses part (a). Distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue) therefore imply $\boxed{v_i^\dagger v_j=0\text{ for }i\ne j}$. Normalize each [eigenvector](../../linear-operator-theory.md#eigenvector) to length one. Since there are $n$ distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue), these vectors form an [orthonormal basis](../../inner-product.md#orthonormal-basis).

Put them in the columns of $U$. Then $U$ is a [unitary matrix](../../linear-operator-theory.md#unitary-matrix) and $AU=UD$, so

$$
\boxed{A=UDU^\dagger,\qquad D=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

To avoid confusing the diagonalizing [matrix](../../vector-space.md#matrix) with the exponential, write $A=WDW^\dagger$ from part (b). The convergent [matrix exponential](../../linear-operator-theory.md#matrix-exponential) series gives

$$
E=e^A=W e^D W^\dagger=W\operatorname{diag}(e^{\lambda_1},\ldots,e^{\lambda_n})W^\dagger.
$$

Each $\lambda_j$ is purely imaginary, so $|e^{\lambda_j}|=1$. The diagonal exponential is therefore a [unitary matrix](../../linear-operator-theory.md#unitary-matrix), and

$$
\boxed{E^\dagger E=W\operatorname{diag}(|e^{\lambda_j}|^2)W^\dagger=I.}
$$

Hence the matrix called $U=\exp(A)$ in this part is unitary. The series identity $(e^A)^\dagger=e^{A^\dagger}=e^{-A}$ gives the same conclusion directly and also covers repeated [eigenvalues](../../linear-operator-theory.md#eigenvalue).

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Since both real [matrices](../../vector-space.md#matrix) are antisymmetric, $A^\dagger=-A$ and $B^\dagger=-B$. Thus $U^\dagger=-A+iB$. Expand the two unitary identities:

$$
UU^\dagger=-A^2-B^2+i(AB-BA)=I,\qquad U^\dagger U=-A^2-B^2-i(AB-BA)=I.
$$

Subtracting and adding give $\boxed{AB=BA,\qquad A^2+B^2=-I}$. Because $A$ has simple [eigenvalues](../../linear-operator-theory.md#eigenvalue), each of its complex [eigenspaces](../../linear-operator-theory.md#eigenspace) is one-dimensional. Commutation makes each one invariant under $B$: if $Av=av$, then $A(Bv)=a(Bv)$. Hence $Bv=bv$ for some scalar $b$. The complete [eigenbasis](../../linear-operator-theory.md#eigenbasis) of $A$ is therefore a common [eigenbasis](../../linear-operator-theory.md#eigenbasis), which also diagonalizes $U$.

The [skew-Hermitian decomposition of a unitary matrix](../../linear-operator-theory.md#skew-hermitian-decomposition-of-a-unitary-matrix) is explicit:

$$
A=\frac{U-U^\dagger}{2},\qquad B=\frac{U+U^\dagger}{2i}.
$$

If $Uv=uv$, unitarity gives $U^\dagger v=u^{-1}v=\overline u\,v$. Consequently

$$
\boxed{a=\frac{u-\overline u}{2}=i\operatorname{Im}u,\qquad b=\frac{u+\overline u}{2i}=-i\operatorname{Re}u.}
$$

Equivalently, for $u=e^{i\theta}$ the paired [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $\boxed{a=i\sin\theta,\ b=-i\cos\theta}$. The hypotheses can only occur in even dimension: $U^T=-U$ and $U$ is invertible, whereas an odd-dimensional [skew-symmetric matrix](../../linear-algebra.md#skew-symmetric-matrix) has zero [determinant](../../multilinear-algebra.md#determinant).

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) are $\boxed{u_x=v_y,\quad u_y=-v_x}$. They give the [gradient](../../multivariable-calculus.md#gradient) identity

$$
\nabla u\cdot\nabla v=u_xv_x+u_yv_y=v_yv_x-v_xv_y=0.
$$

At a regular intersection, where $f'(z)\ne0$, the two nonzero [gradients](../../multivariable-calculus.md#gradient) are [normal vectors](../../differential-geometry.md#normal-vector) to the two [level sets](../../topology.md#level-set), so their tangent directions are perpendicular. This is the [orthogonality of regular real and imaginary level curves](../../analysis.md#orthogonality-of-regular-real-and-imaginary-level-curves).

The regularity qualification is necessary: $|\nabla u|=|\nabla v|=|f'|$, so at a [critical point](../../analysis.md#critical-point) both normals vanish and the curves need not have unique tangents. For example $f=z^2$ gives diagonal lines for $u=0$ and coordinate axes for $v=0$, all meeting at the origin. Thus the conclusion is $\boxed{\text{right-angle intersection wherever }f'(z)\ne0}$, rather than an unrestricted claim at critical points.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Write $g=u+iv$ and let its constant [modulus](../../complex-analysis.md#modulus) be $C$. If $C=0$, then $g=0$. For $C>0$, differentiating $u^2+v^2=C^2$ with respect to $x$ and $y$, then applying the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations), gives

$$
u u_x+v v_x=0,\qquad u u_y+v v_y=-u v_x+v u_x=0.
$$

Thus

$$
\begin{pmatrix}u&v\\v&-u\end{pmatrix}\begin{pmatrix}u_x\\v_x\end{pmatrix}=0.
$$

The coefficient [matrix](../../vector-space.md#matrix) has [determinant](../../multilinear-algebra.md#determinant) $-(u^2+v^2)=-C^2\ne0$, forcing $u_x=v_x=0$. The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) then also give $u_y=v_y=0$. Therefore $u,v$ are constant on a connected domain and

$$
\boxed{g\text{ is constant}.}
$$

This proves the [constant-modulus holomorphic function](../../holomorphic-function.md#constant-modulus-holomorphic-function) result. If a domain is disconnected, the conclusion applies separately to each connected component.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/i">i</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/i/solution">Solution</h5>

↑ **Parent:** [I](#7/c/i)

The zeros of $\sin z$ are $z=n\pi$ for $n\in\mathbb Z$, all simple, and $\cos(n\pi)=(-1)^n\ne0$. Hence the finite singularities of $\cot z$ are exactly

$$
\boxed{z=n\pi,\quad n\in\mathbb Z,\quad\text{all simple poles}.}
$$

Locally $\cot z\sim1/(z-n\pi)$, so each [pole](../../isolated-singularity.md#pole) has [residue](../../analysis.md#residue) $1$.

<h4 id="7/c/ii">ii</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/c/ii)

For $z\ne0$, singularities occur when $1/z=n\pi$, with $n\ne0$. Each is a [simple pole](../../isolated-singularity.md#simple-pole), since the substitution has nonzero [derivative](../../calculus.md#derivative) there:

$$
\boxed{z_n=\frac1{n\pi},\qquad n\in\mathbb Z\setminus\{0\}.}
$$

More explicitly, $1/z-n\pi\sim-(z-z_n)/z_n^2$, so $\cot(1/z)\sim-z_n^2/(z-z_n)$ and its [residue](../../analysis.md#residue) is $-1/(n^2\pi^2)$.

These [poles](../../isolated-singularity.md#pole) accumulate at zero. Consequently $\boxed{z=0\text{ is a non-isolated singularity}}$. The removable/pole/essential classification for [isolated singularities](../../isolated-singularity.md) cannot be applied at that accumulation point; it is not an isolated [essential singularity](../../isolated-singularity.md#essential-singularity).

<h4 id="7/c/iii">iii</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/c/iii)

At every $z=n\pi$, the inner function has a [simple pole](../../isolated-singularity.md#simple-pole), with $\cot z=1/(z-n\pi)+h(z)$ for analytic $h$. Thus

$$
e^{\cot z}=e^{h(z)}\exp\left(\frac1{z-n\pi}\right).
$$

The first factor is analytic and nonzero, while the second has infinitely many negative powers in its [Laurent series](../../analysis.md#laurent-series). Therefore, by the [exponential of a pole is an essential singularity](../../isolated-singularity.md#exponential-of-a-pole-is-an-essential-singularity) result,

$$
\boxed{z=n\pi,\quad n\in\mathbb Z,\quad\text{all essential singularities}.}
$$

At all other finite points the composition is analytic, so there are no additional finite singularities.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

Set $w=z-1$. [Partial fraction decomposition](../../isolated-singularity.md#partial-fraction-decomposition) gives

$$
\frac{2z}{z^2+1}=\frac1{z-i}+\frac1{z+i}=\frac1{1-i+w}+\frac1{1+i+w}.
$$

Expand both terms as [geometric series](../../sequence-and-series.md#geometric-series):

$$
f(z)=\sum_{n=0}^{\infty}(-1)^n\left[(1-i)^{-n-1}+(1+i)^{-n-1}\right]w^n.
$$

The two bracketed terms are complex conjugates. Using $1\pm i=\sqrt2e^{\pm i\pi/4}$ produces the required real coefficients:

$$
\boxed{f(z)=\sum_{n=0}^{\infty}(-1)^n2^{(1-n)/2}\cos\left(\frac{(n+1)\pi}{4}\right)(z-1)^n.}
$$

The initial terms are $1-\tfrac12w^2+\tfrac12w^3-\tfrac14w^4+\cdots$. The nearest singularities are the [simple poles](../../isolated-singularity.md#simple-pole) $z=\pm i$, both at distance $\sqrt2$ from the center. Hence the [Taylor series](../../calculus.md#taylor-series) has

$$
\boxed{R=\sqrt2,\qquad|z-1|<\sqrt2.}
$$

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

A finite point $x_0$ is an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) when the normal-form coefficients $p,q$ are analytic at $x_0$. Then arbitrary values $y(x_0),y'(x_0)$ determine a convergent [Taylor series](../../calculus.md#taylor-series), and two independent choices give two [linearly independent](../../vector-space.md#linear-independence) local analytic solutions.

A singular point is a [regular singular point](../../complex-analysis.md#regular-singular-point) when $(x-x_0)p(x)$ and $(x-x_0)^2q(x)$ extend analytically to $x_0$. The [Frobenius method](../../complex-analysis.md#frobenius-method) then provides at least one solution

$$
\boxed{y=(x-x_0)^\sigma\sum_{n=0}^{\infty}a_n(x-x_0)^n,\qquad a_0\ne0,}
$$

with a locally convergent analytic factor and an exponent fixed by the [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation). If its two [indicial roots](../../linear-ordinary-differential-equation.md#indicial-root) differ by a noninteger, there are two independent [Frobenius solutions](../../complex-analysis.md#frobenius-solution). For integer-separated roots a second solution may include a logarithm; a repeated root gives a [Logarithmic Frobenius solution](../../complex-analysis.md#logarithmic-solution-from-a-repeated-frobenius-exponent) accompanying the single pure series. Such solutions need not be finite or ordinary [Taylor series](../../calculus.md#taylor-series) at the singular point.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/i">i</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8/b/i)

Expanding the derivative and dividing by $1-x$ gives

$$
y''-\frac1{1-x}y'+\left(c^2+\frac\lambda{1-x}\right)y=0.
$$

The only finite singular point is $\boxed{x=1}$. There $(x-1)p(x)=1$ and $(x-1)^2q(x)=c^2(x-1)^2-\lambda(x-1)$ are analytic, so it is a [regular singular point](../../complex-analysis.md#regular-singular-point). At infinity the coefficient of $y$ tends to $c^2\ne0$, giving an [irregular singular point](../../complex-analysis.md#irregular-singular-point) after reciprocal substitution; the finite classification is independent of $\lambda$.

<h4 id="8/b/ii">ii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/b/ii)

Put $t=1-x$ and $Y(t)=y(x)$. The [differential equation](../../differential-equation.md) becomes

$$
tY''+Y'+(c^2t+\lambda)Y=0.
$$

Substitute the [Frobenius solution](../../complex-analysis.md#frobenius-solution) $Y=t^\sigma\sum_{n\geq0}a_nt^n$. The lowest power has coefficient $\sigma^2a_0$, so

$$
\boxed{\sigma=0\quad\text{is the repeated indicial root}.}
$$

Equating successive coefficients gives, with $a_{-1}=0$,

$$
\boxed{n^2a_n+\lambda a_{n-1}+c^2a_{n-2}=0\quad(n\geq1),\qquad a_n=-\frac{\lambda a_{n-1}+c^2a_{n-2}}{n^2}.}
$$

Thus $a_0\ne0$ is the only free coefficient: $a_1=-\lambda a_0$, $a_2=(\lambda^2-c^2)a_0/4$, and so on. Since every denominator is nonzero, there is exactly one independent pure [Frobenius solution](../../complex-analysis.md#frobenius-solution) of this form. The repeated root supplies no second free coefficient; the other solution is logarithmic, as parts (iii) and (iv) demonstrate.

<h4 id="8/b/iii">iii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8/b/iii)

For the normal-form coefficient $p(x)=-1/(1-x)$, [Abel's identity](../../linear-ordinary-differential-equation.md#abel-s-identity) gives the [Wronskian](../../linear-ordinary-differential-equation.md#wronskian)

$$
\boxed{W(x)=C\exp\left[-\int^xp(s)ds\right]=\frac{C}{1-x}.}
$$

Use [reduction of order](../../linear-ordinary-differential-equation.md#reduction-of-order): if $y_2=y_1v$, then $W=y_1^2v'$. Absorbing a nonzero Wronskian constant into the second integration constant, the general solution is

$$
\boxed{y(x)=C_1y_1(x)+C_2y_1(x)\int^x\frac{ds}{(1-s)y_1(s)^2}.}
$$

This local representation applies on intervals where $y_1\ne0$, in particular sufficiently near $x=1$ because $y_1(1)=a_0\ne0$.

<h4 id="8/b/iv">iv</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#8/b/iv)

Write $t=1-x$. The analytic solution has $y_1=a_0+O(t)$ with $a_0\ne0$, so the integrand in the [reduction of order](../../linear-ordinary-differential-equation.md#reduction-of-order) formula satisfies

$$
\frac1{(1-x)y_1(x)^2}=\frac1{a_0^2(1-x)}+O(1).
$$

Integrating with respect to $x$ gives $-a_0^{-2}\log(1-x)+O(1)$. Multiplication by $y_1$ therefore gives

$$
y_2(x)=-\frac1{a_0}\log(1-x)+O(1).
$$

Any solution independent of $y_1$ has a nonzero coefficient of this second solution. Hence

$$
\boxed{y(x)=K\log(1-x)+O(1),\qquad K\ne0,\quad x\to1^-.}
$$

An added multiple of $y_1$ stays bounded and cannot cancel this logarithm. On the real side $x>1$, the corresponding statement uses $\log|1-x|$.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

The [Fermat principle](../../mathematical-physics.md#fermat-principle) makes the [optical path length](../../physical-optics.md#optical-path-length) stationary. For a graph $y=\xi(x)$ the variational integrand is

$$
\mathcal L(x,\xi,\xi')=n(x,\xi)\sqrt{1+\xi'^2}.
$$

The [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is

$$
\frac d{dx}\left[\frac{n(x,\xi)\xi'}{\sqrt{1+\xi'^2}}\right]-n_y(x,\xi)\sqrt{1+\xi'^2}=0.
$$

Use the [chain rule](../../calculus.md#chain-rule) $d n(x,\xi(x))/dx=n_x+n_y\xi'$ and differentiate $\xi'/\sqrt{1+\xi'^2}$ to obtain

$$
\frac{(n_x+n_y\xi')\xi'}{\sqrt{1+\xi'^2}}+\frac{n\xi''}{(1+\xi'^2)^{3/2}}-n_y\sqrt{1+\xi'^2}=0.
$$

Multiplying through and combining the $n_y$ terms gives the required second-order [ordinary differential equation](../../differential-equation.md#ordinary-differential-equation) with no derivatives in denominators:

$$
\boxed{n(x,\xi)\xi''=(1+\xi'^2)[n_y(x,\xi)-\xi'n_x(x,\xi)].}
$$

All partial [derivatives](../../calculus.md#derivative) of the [refractive index](../../electromagnetic-wave.md#refractive-index) are evaluated along the ray.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

Introduce a constant [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) $\mu$ for this [isoperimetric constraint](../../analysis.md#isoperimetric-constraint) and make $A-\mu(C-B)$ stationary. Its integrand is $(1-\mu)y-\mu y'^2$, so the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) gives

$$
1-\mu+2\mu y''=0.
$$

The endpoint conditions therefore force a parabola $y=Kx(1-x)$. Its area and budget are

$$
A=\frac K6,\qquad C=\frac K6+\frac{K^2}{3}=B.
$$

Solving the quadratic and choosing positive area gives

$$
\boxed{K=\frac{\sqrt{1+48B}-1}{4},\qquad y_{\mathrm{opt}}(x)=\frac{\sqrt{1+48B}-1}{4}x(1-x),\qquad A_{\max}=\frac{\sqrt{1+48B}-1}{24}.}
$$

This requires $B>0$; no positive-area barrier is possible for a nonpositive budget. The corresponding multiplier is $\mu=1/(1+4K)>0$.

To verify a global maximum rather than just stationarity, use the [sharp area-cost bound for a barrier with fixed endpoints](../../analysis.md#sharp-area-cost-bound-for-a-barrier-with-fixed-endpoints). For $w=x(1-x)$, [integration by parts](../../calculus.md#integration-by-parts) gives $2A=\int_0^1y'w'dx$, and $\int_0^1w'^2dx=1/3$. The [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality) implies

$$
\int_0^1y'^2dx\geq12A^2,\qquad B\geq A+12A^2.
$$

For $A>0$ the last expression increases strictly, yielding exactly the boxed upper bound. Equality requires $y'$ proportional to $w'$, hence $y=Kw$ after imposing the endpoints. Thus the displayed optimum is unique and lies above the baseline throughout the interior.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Choose homogeneous [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) $\psi(a)=\psi(b)=0$, and take a nonzero real admissible trial $\psi$. Write the numerator as $F[\psi]$ and denominator as $G[\psi]>0$. For an endpoint-zero [variation](../../calculus-of-variations.md#variation) $\eta$, [integration by parts](../../calculus.md#integration-by-parts) gives

$$
\delta F=2\int_a^b[p\psi'\eta'+q\psi\eta]dx=2\int_a^b[-(p\psi')'+q\psi]\eta\,dx,\qquad\delta G=2\int_a^bw\psi\eta\,dx.
$$

Thus the [first variation](../../calculus-of-variations.md#first-variation) of the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient) is

$$
\delta\Lambda=\frac2G\int_a^b[-(p\psi')'+q\psi-\Lambda[\psi]w\psi]\eta\,dx.
$$

By the [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations), stationarity is equivalent to

$$
\boxed{-(p\psi')'+q\psi=\lambda w\psi,\qquad\lambda=\Lambda[\psi],\qquad\psi(a)=\psi(b)=0.}
$$

Conversely, multiplying an [eigenfunction](../../linear-operator-theory.md#eigenfunction) equation by $\psi$ and integrating gives $F=\lambda G$, so its [first variation](../../calculus-of-variations.md#first-variation) vanishes. This establishes the equivalence for the chosen [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem). Homogeneous [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition), or a mixed Dirichlet-Neumann pair, also cancel the boundary term; general [Robin boundary conditions](../../differential-equation.md#robin-boundary-condition) require adding the corresponding boundary contribution to the numerator.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Use the normalized [eigenfunctions](../../linear-operator-theory.md#eigenfunction) and their [weighted inner product](../../inner-product.md#weighted-inner-product) $\int_a^bw\overline{\psi_m}\psi_n dx=\delta_{mn}$. [Orthogonality](../../inner-product.md#orthogonal-vectors) gives

$$
G[\widetilde\psi]=\sum_{n\geq0}|a_n|^2,\qquad F[\widetilde\psi]=\int_a^b\overline{\widetilde\psi}\,\mathcal L\widetilde\psi\,dx=\sum_{n\geq0}\lambda_n|a_n|^2.
$$

For complex trials, $F$ means the corresponding Hermitian [quadratic form](../../quadratic-form.md) with $|\psi'|^2,|\psi|^2$; it agrees with the displayed functional on real trials. If $a_0\ne0$, division by $|a_0|^2$ yields

$$
\boxed{\Lambda[\widetilde\psi]=\frac{\lambda_0+\sum_{n\geq1}|b_n|^2\lambda_n}{1+\sum_{n\geq1}|b_n|^2},\qquad b_n=\frac{a_n}{a_0}.}
$$

Since $\lambda_n\geq\lambda_0$, this is at least $\lambda_0$. The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) therefore gives an upper bound from any admissible trial, improved by minimizing over trial parameters or enlarging the trial space. Equality holds when the trial is entirely in the lowest [eigenspace](../../linear-operator-theory.md#eigenspace).

The displayed ratio using $b_n$ presupposes $a_0\ne0$. If $a_0=0$, use the undivided quotient $\sum\lambda_n|a_n|^2/\sum|a_n|^2$ instead; the same upper-bound argument still applies. No ground-state coefficient can be divided out in that case.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

For the two sine modes, [orthogonality](../../inner-product.md#orthogonal-vectors) gives

$$
\int_0^1\widetilde\psi^2dx=\frac{1+\alpha^2}{2},\qquad\int_0^1\widetilde\psi'^2dx=\frac{\pi^2}{2}(1+4\alpha^2).
$$

The diagonal potential integrals vanish, while the mixed one is

$$
\int_0^1\sin(\pi x)\sin(2\pi x)\cos(\pi x)dx=\frac14.
$$

Thus $\int_0^1\cos(\pi x)\widetilde\psi^2dx=\alpha/2$, giving the [two-sine variational bound for a Dirichlet Mathieu equation](../../linear-operator-theory.md#two-sine-variational-bound-for-a-dirichlet-mathieu-equation):

$$
\boxed{R(\alpha)=\frac{\pi^2+\alpha+4\pi^2\alpha^2}{1+\alpha^2}.}
$$

Its [derivative](../../calculus.md#derivative) vanishes when $1+6\pi^2\alpha-\alpha^2=0$. Hence the two stationary parameters are $3\pi^2\pm\sqrt{9\pi^4+1}$. To identify the minimum, use the normalized sine basis: the restricted [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) has real [symmetric matrix](../../linear-algebra.md#symmetric-matrix)

$$
H_{\mathrm{trial}}=\begin{pmatrix}\pi^2&1/2\\1/2&4\pi^2\end{pmatrix}.
$$

Its smaller [eigenvalue](../../linear-operator-theory.md#eigenvalue) is the minimum of the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient), attained at the negative stationary parameter. Therefore

$$
\boxed{\alpha_{\mathrm{opt}}=3\pi^2-\sqrt{9\pi^4+1},\qquad\lambda_0\leq\frac{5\pi^2-\sqrt{9\pi^4+1}}2\approx9.86116.}
$$

The estimate improves on the single-sine value $\pi^2$. The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) remains valid here even though $q(x)=\cos(\pi x)$ changes sign: on this finite interval the [Sturm-Liouville operator](../../sturm-liouville-theory.md#sturm-liouville-operator) is self-adjoint and bounded below, which is sufficient for the upper bound.

## ↑ Ancestors (10)

1. [2022](../2022.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
