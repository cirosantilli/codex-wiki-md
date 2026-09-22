# Paper 1

↑ **Parent:** [2006](../2006.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2006/PaperNST_IA_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2006/PaperNST_IA_1.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
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
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
  - [f](#5/f)
    - [Solution](#5/f/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [a](#7/a)
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
    - [iii](#7/a/iii)
      - [Solution](#7/a/iii/solution)
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
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [i](#9/b/i)
      - [Solution](#9/b/i/solution)
    - [ii](#9/b/ii)
      - [Solution](#9/b/ii/solution)
    - [iii](#9/b/iii)
      - [Solution](#9/b/iii/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)
- [11](#11)
  - [a](#11/a)
    - [Solution](#11/a/solution)
  - [b](#11/b)
    - [Solution](#11/b/solution)
  - [c](#11/c)
    - [Solution](#11/c/solution)
- [12](#12)
  - [a](#12/a)
    - [Solution](#12/a/solution)
  - [b](#12/b)
    - [Solution](#12/b/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [matrix proportional to its transpose](../../vector-space.md#matrix-proportional-to-its-transpose), applying the [transpose](../../vector-space.md#transpose) twice gives $A^T=5A$ and therefore $A=25A$. Over the [real numbers](../../arithmetic.md#real-number) or [complex numbers](../../complex-analysis.md#complex-number), $24A=0$ implies

$$
\boxed{A=0.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $P=I-B$, $Q=I+B$, so $P^T=Q$ and $Q^T=P$. The factors commute because both are [polynomials](../../polynomial.md) in $B$. Also $P$ has a [matrix inverse](../../matrix-inverse.md) since it is the [transpose](../../vector-space.md#transpose) of the invertible $Q$. Thus the [Cayley transform of a real skew-symmetric matrix](../../lie-theory.md#cayley-transform-of-a-real-skew-symmetric-matrix), with its parameter replaced by $-B$, satisfies

$$
C^TC=P^{-1}QQ^{-1}P=I.
$$

Hence $C$ is an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix). Its inverse is $Q P^{-1}$; this lets us distinguish the [symmetric and skew-symmetric Cayley transforms](../../lie-theory.md#symmetric-and-skew-symmetric-cayley-transforms) below.

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

A [symmetric matrix](../../linear-algebra.md#symmetric-matrix) that is also an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix) satisfies $C=C^{-1}$. Multiplying by the commuting invertible factors gives $(I-B)^2=(I+B)^2$, hence $4B=0$. Thus **there is no nonzero choice of $B$**. The only symmetric case is $B=0$, giving $C=I$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

**Yes, in even dimension.** For example, choose the [skew-symmetric matrix](../../linear-algebra.md#skew-symmetric-matrix)

$$
\boxed{B=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad C=\begin{pmatrix}0&1\\-1&0\end{pmatrix}=-B.}
$$

Here $B^2=-I$, so $(I+B)^{-1}=(I-B)/2$ and $C=(I-B)^2/2=-B$. It is an [orthogonal skew-symmetric matrix](../../linear-algebra.md#orthogonal-skew-symmetric-matrix). More generally the skew-symmetry condition $C=-C^{-1}$ gives $(I-B)^2=-(I+B)^2$, or $B^2=-I$; no real odd-dimensional matrix can satisfy that condition.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $S_m=I+D+\cdots+D^m$. The finite [matrix geometric series](../../linear-algebra.md#matrix-geometric-series) telescopes to $(I-D)S_m=I-D^{m+1}$. By the assumed convergence, its terms $D^{m+1}$ tend to zero, so the [limit](../../calculus.md#limit-of-a-function) $S$ satisfies $(I-D)S=I$. Consequently $S=(I-D)^{-1}$. This is the finite-dimensional [Neumann series](../../banach-algebra.md#neumann-series) argument; invertibility by itself would not imply convergence.

For the stated [nilpotent matrix](../../linear-operator-theory.md#nilpotent-matrix), $D^3=0$ and only the first three terms remain:

$$
\boxed{(I-D)^{-1}=I+D+D^2=\begin{pmatrix}1&1&1\\0&1&1\\0&0&1\end{pmatrix}.}
$$

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $\det(\lambda I-M)=\lambda(\lambda^2-2)$. Solving the three [eigenvector](../../linear-operator-theory.md#eigenvector) equations gives

$$
\boxed{\lambda=\sqrt2,\ 0,\ -\sqrt2;\qquad v_+=(1,\sqrt2,1)^T,\quad v_0=(1,0,-1)^T,\quad v_-=(1,-\sqrt2,1)^T.}
$$

Each [eigenspace](../../linear-operator-theory.md#eigenspace) consists of the [scalar multiples](../../vector-space.md#scalar-multiple) of its displayed nonzero [vector](../../vector-space.md#vector). Their pairwise [dot products](../../inner-product.md#dot-product) vanish: $v_+\cdot v_-=1-2+1=0$ and $v_\pm\cdot v_0=1-1=0$. This also agrees with the [orthogonal diagonalization of a real symmetric matrix](../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The [Euclidean norms](../../normed-vector-space.md#euclidean-norm) are $\|v_\pm\|=2$ and $\|v_0\|=\sqrt2$. With normalized [eigenvectors](../../linear-operator-theory.md#eigenvector) as rows,

$$
\boxed{R=\begin{pmatrix}1/2&1/\sqrt2&1/2\\1/\sqrt2&0&-1/\sqrt2\\1/2&-1/\sqrt2&1/2\end{pmatrix},\qquad RMR^T=\operatorname{diag}(\sqrt2,0,-\sqrt2).}
$$

The rows form an [orthonormal basis](../../inner-product.md#orthonormal-basis), so $RR^T=I$ and $R$ is an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix). The zero [eigenvalue](../../linear-operator-theory.md#eigenvalue) means $Mv_0=0$ for a nonzero [vector](../../vector-space.md#vector); thus **$M$ is singular** and has no [matrix inverse](../../matrix-inverse.md).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The upper-left block is a planar [rotation matrix](../../linear-algebra.md#rotation-matrix). Its real [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $(\lambda-\cos\theta)^2+\sin^2\theta$, which is strictly positive for real $\lambda$ because the angle excludes integer multiples of $\pi$. Hence any real [eigenvector](../../linear-operator-theory.md#eigenvector) has $x=y=0$. The remaining equation is $5z=\lambda z$, giving

$$
\boxed{\lambda=5,\qquad (x,y,z)=(0,0,z),\quad z\in\mathbb R\setminus\{0\}.}
$$

There are infinitely many nonzero solutions, spanning **one independent eigenvector direction**.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Since $(1-i)^2=-2i$, division in the [complex numbers](../../complex-analysis.md#complex-number) gives

$$
\boxed{\frac{2+i}{(1-i)^2}=\frac{i(2+i)}2=-\frac12+i.}
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Multiplying by the [complex conjugate](../../complex-analysis.md#complex-conjugate) of the denominator gives $(1+i)/(i-1)=-i$. Cubing yields

$$
\boxed{\left(\frac{i+1}{i-1}\right)^3=i.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Write $-8i=8e^{-i\pi/2}$. The three distinct [complex roots](../../polynomial.md#complex-root) are $z=2e^{i(-\pi/6+2k\pi/3)}$, $k=0,1,2$. In Cartesian form,

$$
\boxed{z=\sqrt3-i,\quad 2i,\quad-\sqrt3-i.}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The right-hand side has [modulus](../../complex-analysis.md#modulus) $4$ and [argument](../../complex-analysis.md#argument-complex-analysis) $\pi/3$. Its [square roots](../../algebra.md#square-root) have modulus $2$ and arguments $\pi/6$ and $7\pi/6$, giving

$$
\boxed{z=\sqrt3+i\quad\text{or}\quad z=-\sqrt3-i.}
$$

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

[Complex exponentiation](../../analysis.md#complex-exponentiation) uses a branch of the [complex logarithm](../../analysis.md#complex-logarithm). All logarithms of $i$ are $i(\pi/2+2\pi k)$ with $k\in\mathbb Z$, so

$$
i^{1-i}=\exp\bigl[(1+i)(\pi/2+2\pi k)\bigr].
$$

Since the trigonometric factor is always $i$, all values in Cartesian form are

$$
\boxed{z=0+i\,e^{\pi/2+2\pi k},\qquad k\in\mathbb Z.}
$$

The [principal logarithm](../../analysis.md#principal-complex-logarithm) selects $k=0$ and gives the principal value $ie^{\pi/2}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [complex exponential](../../calculus.md#complex-exponential-function) forms of the [sine](../../geometry-and-topology.md#sine) and [cosine](../../geometry-and-topology.md#cosine), and put $w=e^{2iz}$. Multiplying the equation by $2e^{iz}$ gives $(2-i)(w-1)/i+(w+1)=0$, which simplifies to $w=1-i$. Taking all branches of the [complex logarithm](../../analysis.md#complex-logarithm),

$$
2iz=\frac12\ln2+i\left(-\frac\pi4+2\pi n\right).
$$

Thus every solution is

$$
\boxed{z=n\pi-\frac\pi8-\frac{i}{4}\ln2,\qquad n\in\mathbb Z.}
$$

The exponential factor used to multiply the equation is nonzero, so no solutions were introduced or lost.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a sufficiently smooth [vector field](../../multivariable-calculus.md#vector-field) on an oriented piecewise-smooth [surface](../../topological-surface.md) $S$ with boundary $\partial S$, [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) states

$$
\oint_{\partial S}\mathbf F\cdot d\mathbf r=\iint_S(\nabla\times\mathbf F)\cdot\mathbf n\,dS.
$$

Here $\mathbf n$ is the chosen [unit normal](../../differential-geometry.md#unit-normal), $dS$ is the scalar surface-area element, and $d\mathbf r$ follows the positively oriented boundary. The [boundary orientation](../../differential-geometry.md#boundary-orientation) is fixed by the right-hand rule: the fingers curl along $\partial S$ when the thumb points along $\mathbf n$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The Cartesian [curl](../../multivariable-calculus.md#curl) is obtained by cross-differentiating the components:

$$
\boxed{\nabla\times\mathbf F=(\partial_yF_z-\partial_zF_y,\ \partial_zF_x-\partial_xF_z,\ \partial_xF_y-\partial_yF_x)=(-2yz,4xz^2,0).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

**No scalar potential exists on the full three-dimensional domain.** A sufficiently smooth [gradient field](../../multivariable-calculus.md#gradient-field) has zero [curl](../../multivariable-calculus.md#curl), since mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative) commute. The calculated [curl](../../multivariable-calculus.md#curl) is not identically zero. The fact that it vanishes at some individual points does not make the whole field a [gradient field](../../multivariable-calculus.md#gradient-field).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Orient the triangle by the path $A\to B\to C\to A$. The [cross product](../../vector-space.md#cross-product) $(B-A)\times(C-A)=(0,1,0)$ gives the positive [normal vector](../../differential-geometry.md#normal-vector). In the plane $y=1$, the triangular region is $x,z\geq0$, $x+z\leq1$. The surface integral in [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) is therefore

$$
\int_0^1\int_0^{1-z}4xz^2\,dx\,dz=2\int_0^1z^2(1-z)^2\,dz=\frac1{15}.
$$

For the boundary [line integral](../../multivariable-calculus.md#line-integral), $AB$ has $z=0$, so contributes zero. On $BC$, $x=0$ and only $dz$ is nonzero, so its contribution is also zero. Parametrize $CA$ by $(x,y,z)=(t,1,1-t)$, $0\leq t\leq1$. Its contribution is

$$
\int_0^1[2t(1-t)^3-t^2(1-t)^2]dt=\frac1{15}.
$$

Thus **both oriented integrals equal $1/15$**. Reversing the orientation would reverse both signs.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The coordinate intercepts suggest the [normal vector](../../differential-geometry.md#normal-vector)

$$
\boxed{\mathbf n=(1/a,1/b,1/c).}
$$

Indeed $\mathbf n\cdot\mathbf a=\mathbf n\cdot\mathbf b=\mathbf n\cdot\mathbf c=1$, so the two independent edge [vectors](../../vector-space.md#vector) in the plane are both [orthogonal](../../inner-product.md#orthogonal-vectors) to $\mathbf n$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [plane equation](../../geometry-and-topology.md#cartesian-equation-of-a-plane) in normal form is

$$
\boxed{\mathbf n\cdot\mathbf r=1,\qquad\text{equivalently}\qquad \frac xa+\frac yb+\frac zc=1.}
$$

An equivalent vector parametrization is $\mathbf r=\mathbf a+s(\mathbf b-\mathbf a)+t(\mathbf c-\mathbf a)$, with $s,t\in\mathbb R$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [distance from a point to a plane](../../geometry-and-topology.md#distance-from-a-point-to-a-plane), applied at the origin, is the plane constant divided by the [Euclidean norm](../../normed-vector-space.md#euclidean-norm) of its [normal vector](../../differential-geometry.md#normal-vector). Therefore

$$
\boxed{|OD|=\frac1{\sqrt{a^{-2}+b^{-2}+c^{-2}}}.}
$$

The [closest point on a plane](../../geometry-and-topology.md#closest-point-on-a-plane) lies on the normal through the origin; this is an [orthogonal projection onto an intercept plane](../../geometry-and-topology.md#orthogonal-projection-onto-an-intercept-plane).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Taking the [dot product](../../inner-product.md#dot-product) with $\mathbf n$ gives $\mathbf n\cdot\mathbf r=\lambda+\mu+\nu$. The necessary and sufficient condition is therefore

$$
\boxed{\lambda+\mu+\nu=1.}
$$

These coefficients describe an [affine combination](../../geometry-and-topology.md#affine-combination) of the three vertices, or their [barycentric coordinate system](../../algebraic-topology.md#barycentric-coordinate-system). Nonnegativity would additionally restrict the point to the triangle; it is not required for the whole plane.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Put $S=a^{-2}+b^{-2}+c^{-2}$. The [orthogonal projection onto an intercept plane](../../geometry-and-topology.md#orthogonal-projection-onto-an-intercept-plane) is $\mathbf d=\mathbf n/S$. Comparing its coordinates with $(\lambda a,\mu b,\nu c)$ gives

$$
\boxed{\lambda=\frac{a^{-2}}S,\qquad\mu=\frac{b^{-2}}S,\qquad\nu=\frac{c^{-2}}S.}
$$

Their sum is one, as the [plane equation](../../geometry-and-topology.md#cartesian-equation-of-a-plane) requires.

<h3 id="5/f">f</h3>

↑ **Parent:** [5](#5)

<h4 id="5/f/solution">Solution</h4>

↑ **Parent:** [F](#5/f)

The [vector](../../vector-space.md#vector) $\mathbf a$ is [orthogonal](../../inner-product.md#orthogonal-vectors) to both $\mathbf b$ and $\mathbf c$, so $\mathbf a\cdot(\mathbf b-\mathbf c)=0$. Also $\mathbf d\cdot\mathbf b=\mathbf d\cdot\mathbf c=1/S$, hence $\mathbf d\cdot(\mathbf b-\mathbf c)=0$. Subtraction gives $(\mathbf a-\mathbf d)\cdot(\mathbf b-\mathbf c)=0$. Both vectors are nonzero, so

$$
\boxed{\text{the angle is }\pi/2.}
$$

This is the altitude property of the [orthogonal projection onto an intercept plane](../../geometry-and-topology.md#orthogonal-projection-onto-an-intercept-plane): the projection point is the triangle's [orthocenter](../../euclidean-geometry.md#orthocenter).

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

The [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) is a [determinant](../../multilinear-algebra.md#determinant):

$$
(\mathbf a\times\mathbf b)\cdot\mathbf c=\det(\mathbf a,\mathbf b,\mathbf c).
$$

A cyclic permutation of its three columns is an [even permutation](../../finite-group-theory.md#even-permutation), so it leaves the determinant unchanged. Thus $\det(\mathbf a,\mathbf b,\mathbf c)=\det(\mathbf b,\mathbf c,\mathbf a)=\mathbf a\cdot(\mathbf b\times\mathbf c)$, proving the identity.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

Use the [vector triple product identity](../../multivariable-calculus.md#vector-triple-product) twice:

$$
(\mathbf a\times\mathbf b)\times\mathbf c=\mathbf b(\mathbf a\cdot\mathbf c)-\mathbf a(\mathbf b\cdot\mathbf c),\qquad \mathbf a\times(\mathbf b\times\mathbf c)=\mathbf b(\mathbf a\cdot\mathbf c)-\mathbf c(\mathbf a\cdot\mathbf b).
$$

Subtracting cancels the common term, yielding

$$
\boxed{(\mathbf a\times\mathbf b)\times\mathbf c-\mathbf a\times(\mathbf b\times\mathbf c)=\mathbf c(\mathbf a\cdot\mathbf b)-\mathbf a(\mathbf b\cdot\mathbf c).}
$$

It is generally nonzero: the [cross product](../../vector-space.md#cross-product) does not satisfy the [associative property](../../algebraic-operation.md#associative-property).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

With $s=\sin\theta_0$ and $c=\cos\theta_0$, conversion from [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system) gives $\mathbf a=r_0(s,0,c)$, $\mathbf b=r_0(-s/2,\sqrt3s/2,c)$ and $\mathbf c=r_0(-s/2,-\sqrt3s/2,c)$. The [volume](../../geometry-and-topology.md#volume) of the [parallelepiped](../../euclidean-geometry.md#parallelepiped) is the [absolute value](../../real-analysis.md#absolute-value) of their [scalar triple product](../../multilinear-algebra.md#scalar-triple-product):

$$
\boxed{V=|\det(\mathbf a,\mathbf b,\mathbf c)|=\frac{3\sqrt3}{2}r_0^3\sin^2\theta_0\,|\cos\theta_0|.}
$$

The absolute value matters when the polar angle is in the lower hemisphere. At the poles or equator the three edge vectors are linearly dependent and the volume vanishes.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

Let $G$ denote carrying the [gene](../../genetics.md#gene) and $+$ a positive result. The [law of total probability](../../probability-space.md#law-of-total-probability) gives

$$
\boxed{P(+)=P(+\mid G)P(G)+P(+\mid G^c)P(G^c)=0.99(0.001)+0.05(0.999)=0.05094\simeq0.0509.}
$$

The last value is to three significant figures. The much larger non-carrier population contributes most of the positive tests in this mathematical model.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

By [Bayes' theorem](../../probability-theory.md#bayes-theorem), the required [conditional probability](../../probability-theory.md#conditional-probability) is

$$
\boxed{P(G\mid+)=\frac{P(+\mid G)P(G)}{P(+)}=\frac{0.00099}{0.05094}=0.0194\quad\text{(3 s.f.)}.}
$$

This is about $1.94\%$; it is a different conditioning direction from the test's $99\%$ positive probability among carriers.

<h4 id="7/a/iii">iii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/a/iii)

The negative-test [probability](../../probability-theory.md#probability) is $P(-)=1-0.05094=0.94906$. Applying [Bayes' theorem](../../probability-theory.md#bayes-theorem) again,

$$
\boxed{P(G\mid-)=\frac{P(-\mid G)P(G)}{P(-)}=\frac{0.01(0.001)}{0.94906}=1.05\times10^{-5}\quad\text{(3 s.f.)}.}
$$

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

For $B$ to make a first throw, $A$ must first pass, with [probability](../../probability-theory.md#probability) $1/2$. For $B$ then to win on that throw, $B$ must roll one of two winning faces, with probability $1/3$. The throws are [independent](../../random-variable.md#independent-random-variables), giving

$$
\boxed{P=\frac12\frac13=\frac16.}
$$

A first throw of $3$ by $A$ would make $B$ win without throwing, and is excluded by the requested event.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

Before $A$'s second throw, $A$ can win either immediately, with [probability](../../probability-theory.md#probability) $1/3$, or by passing to $B$ and having $B$ throw $3$, with probability $(1/2)(1/6)$. These are disjoint events, so

$$
\boxed{P=\frac13+\frac1{12}=\frac5{12}.}
$$

<h4 id="7/b/iii">iii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/b/iii)

This is a [two-turn renewal game](../../analysis.md#two-turn-renewal-game). A full pair of throws has probability $(1/2)^2=1/4$ of passing twice and returning to the original state. The probability that $A$ wins before that restart is $5/12$. Thus [first-step analysis](../../analysis.md#first-step-analysis) gives $p=5/12+p/4$, or

$$
\boxed{P(A\text{ wins})=\frac59.}
$$

Equivalently sum the [geometric series](../../sequence-and-series.md#geometric-series) $(5/12)\sum_{j\geq0}(1/4)^j$. The probability of surviving infinitely many pairs is zero, so the eventual winner is well defined with probability one.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

For the [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) equations, use $\mathcal L=x^2y+2y-\lambda(x^2+y^2-1)$. They give $2x(y-\lambda)=0$, $x^2+2=2\lambda y$, and $x^2+y^2=1$. If $x\ne0$, then $\lambda=y$, implying $x^2+2=2y^2$ and therefore $y^2=1$, contradicting $x\ne0$. Thus only $x=0$, $y=\pm1$ remain.

The circle is [compact](../../topology.md#compact-space) and the function is [continuous](../../calculus.md#continuous-function), so global extrema exist. On it, eliminating $x^2$ gives $f=3y-y^3$, which is increasing for $-1<y<1$ since its [derivative](../../calculus.md#derivative) is $3(1-y^2)>0$. Therefore

$$
\boxed{f_{\max}=2\text{ at }(0,1),\qquad f_{\min}=-2\text{ at }(0,-1).}
$$

These constrained extrema are flat to quadratic order along the circle, so a vanishing second derivative alone would not classify them.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

Minimize $\frac12\|\mathbf r\|^2$ subject to $\mathbf n_1\cdot\mathbf r=1$, $\mathbf n_2\cdot\mathbf r=2$, where $\mathbf n_1=(2,1,-1)$ and $\mathbf n_2=(1,-1,1)$. The [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) equation gives $\mathbf r=\lambda\mathbf n_1+\mu\mathbf n_2$. Since $\mathbf n_1\cdot\mathbf n_2=0$, $\|\mathbf n_1\|^2=6$, and $\|\mathbf n_2\|^2=3$, the constraints imply $\lambda=1/6$, $\mu=2/3$. Hence

$$
\boxed{\mathbf r_*=(1,-1/2,1/2).}
$$

No explicit parametrization of the line was needed. For any other feasible point, $\mathbf h=\mathbf r-\mathbf r_*$ is [orthogonal](../../inner-product.md#orthogonal-vectors) to both normals and therefore to $\mathbf r_*$. The [Pythagorean theorem](../../euclidean-geometry.md#pythagorean-theorem) gives $\|\mathbf r\|^2=\|\mathbf r_*\|^2+\|\mathbf h\|^2$, proving the unique global minimum. This is the geometric principle behind the [minimum-norm least-squares solution](../../inverse-problem.md#minimum-norm-least-squares-solution).

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

[Taylor's theorem](../../calculus.md#taylor-s-theorem) expands about $a$ in powers of $h=x-a$. With the usual differentiability assumptions, its finite form with [Lagrange remainder](../../calculus.md#lagrange-remainder) is

$$
f(x)=\sum_{k=0}^n\frac{f^{(k)}(a)}{k!}(x-a)^k+\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-a)^{n+1},
$$

where $\xi$ lies between $a$ and $x$. If the remainder tends to zero as $n\to\infty$, this yields the [Taylor series](../../calculus.md#taylor-series) $f(x)=\sum_{k\geq0}f^{(k)}(a)(x-a)^k/k!$. Smoothness alone does not guarantee that infinite-series equality.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/i">i</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9/b/i)

Put $h=x-1$. The [Taylor series](../../calculus.md#taylor-series) of the [natural logarithm](../../calculus.md#natural-logarithm) gives the first four nonzero terms:

$$
\boxed{\ln x=h-\frac{h^2}{2}+\frac{h^3}{3}-\frac{h^4}{4}+O(h^5).}
$$

The corresponding infinite series converges for $|h|<1$.

<h4 id="9/b/ii">ii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/b/ii)

For the [arctangent](../../geometry-and-topology.md#inverse-tangent), put $h=x-1$. Its [derivative](../../calculus.md#derivative) is $(d/dh)\arctan(1+h)=1/(2+2h+h^2)=\frac12-\frac h2+\frac{h^2}4+O(h^4)$. Integrating and using $\arctan1=\pi/4$ gives

$$
\boxed{\arctan x=\frac\pi4+\frac h2-\frac{h^2}4+\frac{h^3}{12}+O(h^5).}
$$

The constant counts as the first nonzero term. The quartic coefficient vanishes; the next nonzero term is $-h^5/40$.

<h4 id="9/b/iii">iii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9/b/iii)

The removable value at zero is one. Expand the denominator as $e^x-1=x(1+x/2+x^2/6+\cdots)$ and determine the reciprocal coefficients by multiplication. The first four nonzero terms are

$$
\boxed{\frac{x}{e^x-1}=1-\frac x2+\frac{x^2}{12}-\frac{x^4}{720}+O(x^6).}
$$

This is the [exponential generating function](../../sequence-and-series.md#exponential-generating-function) of the [Bernoulli numbers](../../bernoulli-number.md), with convention $B_1=-1/2$. The coefficients of $x^3$ and $x^5$ are zero.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

The [homogeneous solution](../../linear-ordinary-differential-equation.md#homogeneous-solution) is $A\cos2x+B\sin2x$. A trial $C\cos x$ gives the [particular solution](../../linear-ordinary-differential-equation.md#particular-solution) $\cos x/3$. The two initial conditions set $A=-1/3$, $B=0$, giving

$$
\boxed{y(x)=\frac{\cos x-\cos2x}{3}.}
$$

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Use $\cos^2x=(1+\cos2x)/2$. The constant forcing has [particular solution](../../linear-ordinary-differential-equation.md#particular-solution) $1/8$, while the $\cos2x$ term satisfies the [resonance condition](../../linear-ordinary-differential-equation.md#resonance-condition) and needs the trial $Cx\sin2x$. Since $(d^2/dx^2+4)(x\sin2x)=4\cos2x$, the forced term is $x\sin2x/8$. Adding the [homogeneous solution](../../linear-ordinary-differential-equation.md#homogeneous-solution) and imposing the initial conditions gives

$$
\boxed{y(x)=\frac{1-\cos2x+x\sin2x}{8}.}
$$

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

The differential operator is $(D-1)^2$, where $D=d/dx$. Set $y=e^xv$; the [product rule](../../calculus.md#product-rule) reduces the equation to $v''=1+x$. Twice integrating gives $v=x^2/2+x^3/6+Ax+B$. The initial conditions yield $B=A=0$, so

$$
\boxed{y(x)=e^x\left(\frac{x^2}{2}+\frac{x^3}{6}\right).}
$$

This substitution removes the repeated characteristic root before finding a [particular solution](../../linear-ordinary-differential-equation.md#particular-solution).

## 11

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/solution">Solution</h4>

↑ **Parent:** [A](#11/a)

The function is [even](../../calculus.md#even-function) and continuous, with period $2\pi$. On $0<x<\pi$ it is $\sin2x$, so it rises from zero to one at $\pi/4$, crosses zero at $\pi/2$, reaches minus one at $3\pi/4$, and returns to zero at $\pi$. Reflect this curve about the vertical axis and repeat periodically. The joins at integer multiples of $\pi$ have corners, but no jumps.

<a id="11/a/image-even-periodic-extension-of-a-sine-mode-and-its-fourier-approximation"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1-even-sine-extension.png)

**[Figure 1](#11/a/image-even-periodic-extension-of-a-sine-mode-and-its-fourier-approximation). Even periodic extension of a sine mode and its Fourier approximation**. Original plot over two periods. The dashed approximation uses the first twelve nonzero cosine coefficients; the exact function is continuous with corners at integer multiples of $\pi$.

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/solution">Solution</h4>

↑ **Parent:** [B](#11/b)

Because the function is [even](../../calculus.md#even-function), all sine [Fourier coefficients](../../fourier-series.md#fourier-coefficient) vanish. Its average is zero, so $a_0=0$. The [Fourier cosine coefficients of a sine mode](../../fourier-series.md#fourier-cosine-coefficients-of-a-sine-mode) follow from the product-to-sum identity:

$$
a_n=\frac2\pi\int_0^\pi\sin2x\cos nx\,dx=\begin{cases}\displaystyle\frac8{\pi(4-n^2)},&n\text{ odd},\\0,&n\text{ even}.\end{cases}
$$

For $n=2$, the integral is directly zero rather than an undefined substitution into a denominator. Thus

$$
\boxed{f(x)=\frac8\pi\sum_{m=0}^\infty\frac{\cos((2m+1)x)}{4-(2m+1)^2}.}
$$

The [Fourier series](../../fourier-series.md) equals the continuous function at every point, including the corners. Its coefficients decay quadratically, so the series is also [absolutely convergent](../../sequence-and-series.md#absolute-convergence).

<h3 id="11/c">c</h3>

↑ **Parent:** [11](#11)

<h4 id="11/c/solution">Solution</h4>

↑ **Parent:** [C](#11/c)

At $x=0$, the [Fourier series](../../fourier-series.md) equals $f(0)=0$. Isolating the first term gives

$$
0=\frac13+\sum_{m=1}^\infty\frac1{4-(2m+1)^2}.
$$

Changing the sign of the remaining denominators proves

$$
\boxed{\sum_{m=1}^\infty\frac1{(2m+1)^2-4}=\frac13.}
$$

The [absolute convergence](../../sequence-and-series.md#absolute-convergence) justifies the evaluation and rearrangement.

## 12

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12/a">a</h3>

↑ **Parent:** [12](#12)

<h4 id="12/a/solution">Solution</h4>

↑ **Parent:** [A](#12/a)

For [Laplace's equation](../../partial-differential-equation.md#laplace-equation), seek a nonzero separated product $f=X(x)Y(y)$. Dividing by $XY$ gives $X''/X=-Y''/Y$, so both sides are a [separation constant](../../partial-differential-equation.md#separation-constant). Choosing it as $-k^2$ gives $X''+k^2X=0$, $Y''-k^2Y=0$, with trigonometric and [hyperbolic functions](../../calculus.md#hyperbolic-function), respectively. A zero constant gives linear factors; a positive constant interchanges the two types. [Boundary conditions](../../differential-equation.md#boundary-condition) determine which modes are allowed, and [linearity](../../vector-space.md#linearity) permits their superposition to match the remaining boundary data.

<h3 id="12/b">b</h3>

↑ **Parent:** [12](#12)

<h4 id="12/b/solution">Solution</h4>

↑ **Parent:** [B](#12/b)

The zero values at $x=0,a$ select $X_n=\sin(n\pi x/a)$, and the zero value at $y=0$ selects $Y_n=\sinh(n\pi y/a)$. Expanding the constant upper-edge value as a [Fourier sine series](../../fourier-series.md#fourier-sine-series) gives coefficients $b_n=2F[1-(-1)^n]/(n\pi)$. The resulting [harmonic function in a rectangle with one constant boundary value](../../partial-differential-equation.md#harmonic-function-in-a-rectangle-with-one-constant-boundary-value) is

$$
\boxed{f(x,y)=\frac{4F}{\pi}\sum_{m=0}^\infty\frac{\sin((2m+1)\pi x/a)}{2m+1}\frac{\sinh((2m+1)\pi y/a)}{\sinh((2m+1)\pi)},\qquad0<x,y<a.}
$$

Each term satisfies [Laplace's equation](../../partial-differential-equation.md#laplace-equation) and the three zero boundary values. At $y=a$, the series equals $F$ for $0<x<a$. On compact subsets of the interior it and its derivatives converge exponentially, which justifies the termwise equation.

For $F\ne0$, the top-corner boundary prescriptions conflict: a corner cannot be both zero on a vertical edge and $F$ on the upper edge. The bounded interior solution has the specified limits along the open sides; it has no single continuous extension at those two corners. Values assigned only at the isolated corners do not change the interior solution.

<a id="12/b/image-harmonic-extension-from-one-heated-edge-of-a-square"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1-square-harmonic-extension.png)

**[Figure 2](#12/b/image-harmonic-extension-from-one-heated-edge-of-a-square). Harmonic extension from one heated edge of a square**. Original normalized solution $f/F$, with the upper open edge fixed at one and the other three open edges at zero. The top corner circles mark incompatible side limits, not prescribed continuous corner temperatures.

## ↑ Ancestors (10)

1. [2006](../2006.md)
2. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
