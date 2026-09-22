# Paper 1

↑ **Parent:** [2020](../2020.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2020/papernst_ib_1_2020.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2020/papernst_ib_1_2020.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
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
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [Solution](#5/solution)
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
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
  - [d](#7/d)
    - [Solution](#7/d/solution)
- [8](#8)
  - [a](#8/a)
    - [i](#8/a/i)
      - [Solution](#8/a/i/solution)
    - [ii](#8/a/ii)
      - [Solution](#8/a/ii/solution)
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

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Write the position [vector](../../vector-space.md#vector) as $\mathbf r(\rho,\phi,z)=(\rho\cos\phi,\rho\sin\phi,z)$. Its coordinate tangent [vectors](../../vector-space.md#vector) are

$$
\mathbf r_\rho=(\cos\phi,\sin\phi,0),\qquad
\mathbf r_\phi=(-\rho\sin\phi,\rho\cos\phi,0),\qquad
\mathbf r_z=(0,0,1).
$$

Their pairwise [dot products](../../inner-product.md#dot-product) vanish. Their lengths, the [scale factors of orthogonal coordinates](../../multivariable-calculus.md#scale-factors-of-orthogonal-coordinates), are

$$
\boxed{h_\rho=1,\qquad h_\phi=\rho,\qquad h_z=1.}
$$

Thus the [cylindrical coordinate system](../../multivariable-calculus.md#cylindrical-coordinate-system) is orthogonal wherever it is a nonsingular coordinate chart. At $\rho=0$, the angular tangent [vector](../../vector-space.md#vector) vanishes and the azimuth is undefined; this is the usual [coordinate singularity](../../general-relativity.md#coordinate-singularity) on the axis, not a failure of the [Euclidean geometry](../../euclidean-geometry.md).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Dividing the coordinate tangents by their [scale factors of orthogonal coordinates](../../multivariable-calculus.md#scale-factors-of-orthogonal-coordinates) gives an [orthonormal basis](../../inner-product.md#orthonormal-basis)

$$
\mathbf e_\rho=(\cos\phi,\sin\phi,0),\quad
\mathbf e_\phi=(-\sin\phi,\cos\phi,0),\quad
\mathbf e_z=(0,0,1).
$$

Evaluate the Cartesian [cross products](../../vector-space.md#cross-product) componentwise:

$$
\mathbf e_\rho\times\mathbf e_\phi=(0,0,\cos^2\phi+\sin^2\phi)=\mathbf e_z,
$$



$$
\mathbf e_\phi\times\mathbf e_z=(\cos\phi,\sin\phi,0)=\mathbf e_\rho,
\qquad
\mathbf e_z\times\mathbf e_\rho=(-\sin\phi,\cos\phi,0)=\mathbf e_\phi.
$$

Consequently

$$
\boxed{\mathbf e_\rho\times\mathbf e_\phi=\mathbf e_z,\quad
\mathbf e_\phi\times\mathbf e_z=\mathbf e_\rho,\quad
\mathbf e_z\times\mathbf e_\rho=\mathbf e_\phi.}
$$

The ordered cylindrical [basis](../../vector-space.md#basis) is right-handed: its [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) $\mathbf e_\rho\cdot(\mathbf e_\phi\times\mathbf e_z)$ equals $+1$.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Differentiate the position [vector](../../vector-space.md#vector), using the angular factor from the [scale factors of orthogonal coordinates](../../multivariable-calculus.md#scale-factors-of-orthogonal-coordinates):

$$
\boxed{d\mathbf r=\mathbf e_\rho\,d\rho+\rho\mathbf e_\phi\,d\phi+\mathbf e_z\,dz.}
$$

The [basis](../../vector-space.md#basis) is an [orthonormal basis](../../inner-product.md#orthonormal-basis), so all cross terms in its squared length vanish. The Euclidean [line element](../../riemannian-metric.md#line-element) is therefore

$$
\boxed{|d\mathbf r|^2=d\rho^2+\rho^2d\phi^2+dz^2.}
$$

In particular, an angular change $d\phi$ at fixed radius traverses a physical distance $\rho\,|d\phi|$.

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

For a finite separation use the Cartesian distance, rather than substituting finite coordinate differences into the local [line element](../../riemannian-metric.md#line-element). Expanding the two horizontal components gives

$$
(\rho\cos\phi-\rho'\cos\phi')^2+(\rho\sin\phi-\rho'\sin\phi')^2
=\rho^2+\rho'^2-2\rho\rho'\cos(\phi-\phi').
$$

The vertical contribution is $(z-z')^2$, independently. Thus

$$
\boxed{h=\rho^2+\rho'^2-2\rho\rho'\cos(\phi-\phi'),\qquad j=(z-z')^2,}
$$

and

$$
\boxed{R=\sqrt{\rho^2+\rho'^2-2\rho\rho'\cos(\phi-\phi')+(z-z')^2}.}
$$

Equivalently, the horizontal contribution is $(\rho-\rho')^2+4\rho\rho'\sin^2[(\phi-\phi')/2]$, which also makes its nonnegativity explicit.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The radial [unit vector](../../vector-space.md#unit-vector) in the [spherical coordinate system](../../multivariable-calculus.md#spherical-coordinate-system) is

$$
\mathbf e_r=\frac{\mathbf r}{r}=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta).
$$

The coordinate tangent in the polar direction has length $r$, so its corresponding [unit vector](../../vector-space.md#unit-vector) is

$$
\mathbf e_\theta=\frac1r\frac{\partial\mathbf r}{\partial\theta}
=(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta).
$$

Differentiating $\mathbf e_r$ at fixed $\phi$ therefore gives

$$
\boxed{\frac{\partial\mathbf e_r}{\partial\theta}=\mathbf e_\theta,\qquad\alpha=1.}
$$

The factor is not $r$: the corresponding [scale factors of orthogonal coordinates](../../multivariable-calculus.md#scale-factors-of-orthogonal-coordinates) occur in the [derivative](../../calculus.md#derivative) of the position [vector](../../vector-space.md#vector), whereas the question differentiates its unit direction. The formula is understood away from the [coordinate singularities](../../general-relativity.md#coordinate-singularity) where a complete spherical [basis](../../vector-space.md#basis) is not uniquely specified.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Differentiate the [power series](../../sequence-and-series.md#power-series) term by term inside its [radius of convergence](../../sequence-and-series.md#radius-of-convergence), and reindex the second [derivative](../../calculus.md#derivative) so that every coefficient multiplies $x^m$. The [differential equation](../../differential-equation.md) becomes

$$
\sum_{m=0}^\infty\left[(m+2)(m+1)a_{m+2}+
\{n(n+1)-m(m+1)\}a_m\right]x^m=0.
$$

The uniqueness of power-series coefficients gives

$$
\boxed{a_{m+2}=\frac{m(m+1)-n(n+1)}{(m+1)(m+2)}a_m
=\frac{(m-n)(m+n+1)}{(m+1)(m+2)}a_m,\quad m\geq0.}
$$

The even coefficients depend only on $a_0$ and the odd coefficients only on $a_1$. These are the two local solution branches of the [Legendre differential equation](../../linear-ordinary-differential-equation.md#legendre-differential-equation) around its [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) $x=0$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

For an [integer](../../integer.md) $n\geq0$, choose the [series](../../sequence-and-series.md#series-mathematics) whose [integer parity](../../integer.md#parity-mathematics) agrees with $n$ and set the other initial coefficient to zero. At $m=n$, the numerator in the recurrence vanishes, so $a_{n+2}=0$ and every later coefficient in that [integer parity](../../integer.md#parity-mathematics) vanishes. With a nonzero coefficient of $x^n$, this gives a [polynomial](../../polynomial.md) of degree exactly $n$. Normalize it by $P_n(1)=1$.

For $n=0$, the even branch is constant; for $n=1$, the odd branch is proportional to $x$. For $n=2$, the recurrence gives $a_2=-3a_0$, so normalization fixes $a_0=-1/2$. Hence

$$
\boxed{P_0(x)=1,\qquad P_1(x)=x,\qquad P_2(x)=\frac12(3x^2-1).}
$$

The opposite-parity branch generally does not terminate; [polynomial](../../polynomial.md) termination does not mean that both independent solutions become [polynomials](../../polynomial.md).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Substitute $U=R(r)F(\theta)$ into the axisymmetric [Laplace equation](../../partial-differential-equation.md#laplace-equation) and multiply by $r^2/(RF)$. The radial and angular terms must be separate constants:

$$
\frac1R\frac d{dr}(r^2R')=-\frac1{F\sin\theta}\frac d{d\theta}(\sin\theta F')=\lambda.
$$

Thus

$$
r^2R''+2rR'-\lambda R=0,\qquad
\frac1{\sin\theta}(\sin\theta F')'+\lambda F=0.
$$

With $x=\cos\theta$, the angular equation becomes

$$
(1-x^2)F_{xx}-2xF_x+\lambda F=0.
$$

Requiring boundedness on the entire polar interval, and using the supplied characterization of bounded [Legendre polynomial](../../linear-ordinary-differential-equation.md#legendre-polynomial) solutions, gives $\lambda=n(n+1)$ and $F\propto P_n(\cos\theta)$ for $n=0,1,2,\ldots$. Trying $R=r^s$ gives $s(s+1)=n(n+1)$, hence $s=n$ or $s=-n-1$.

The globally angular-regular separated modes and their superposition are therefore

$$
\boxed{U_n=(A_nr^n+B_nr^{-n-1})P_n(\cos\theta),}
$$



$$
\boxed{U(r,\theta)=\sum_{n=0}^\infty(A_nr^n+B_nr^{-n-1})P_n(\cos\theta).}
$$

Coefficients and convergence are determined by the radial domain and boundary data. A domain containing the origin excludes negative radial powers for a regular solution. If the angular domain excludes a polar axis of the [spherical coordinate system](../../multivariable-calculus.md#spherical-coordinate-system) and singular angular behavior is allowed, additional Legendre-function branches are possible; the displayed family is the one regular over the complete sphere, as intended by the hint.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The far field is proportional to $rP_1(\cos\theta)$, since $P_1(\cos\theta)=\cos\theta$. After matching the growing terms, write the exterior solution as

$$
U=v_0rP_1(\cos\theta)+\sum_{n=0}^\infty B_nr^{-n-1}P_n(\cos\theta).
$$

An added constant has here been excluded by interpreting the far-field condition as $U-v_0r\cos\theta\to0$. Differentiate and impose the radial [Neumann boundary condition](../../differential-equation.md#neumann-boundary-condition):

$$
0=v_0P_1(\cos\theta)-\sum_{n=0}^\infty(n+1)B_nr_0^{-n-2}P_n(\cos\theta).
$$

The [Orthogonality of Legendre polynomials](../../linear-ordinary-differential-equation.md#orthogonality-of-legendre-polynomials) makes each coefficient vanish separately. Thus $B_n=0$ for $n\ne1$, and $2B_1/r_0^3=v_0$. Consequently

$$
\boxed{U(r,\theta)=v_0\left(r+\frac{r_0^3}{2r^2}\right)\cos\theta,\qquad r\geq r_0.}
$$

Indeed $\partial_rU=v_0(1-r_0^3/r^3)\cos\theta$, which vanishes at the boundary, while the correction decays at infinity. If the far-field condition is intended to specify only the leading growing term, an arbitrary additive constant is also allowed; its gradient has no effect on the [Neumann boundary condition](../../differential-equation.md#neumann-boundary-condition).

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives

$$
\tau_1^2=\tau_2^2=\tau_3^2=I_2.
$$

For example, the diagonal entries of $\tau_2^2$ are $(-i)i=i(-i)=1$, and its off-diagonal entries vanish. Associativity now reduces every positive [integer](../../integer.md) power to its [integer parity](../../integer.md#parity-mathematics):

$$
\boxed{\tau_j^{2m}=I_2,\qquad\tau_j^{2m+1}=\tau_j.}
$$

These are the standard [Pauli matrices](../../algebra.md#pauli-matrices), each a [Hermitian matrix](../../hilbert-space.md#hermitian-operator) and an [involution](../../group-theory.md#involution).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Separate the defining [matrix exponential](../../linear-operator-theory.md#matrix-exponential) into even and odd powers and use $\tau_j^2=I_2$:

$$
e^{i\alpha_j\tau_j}=I_2\sum_{m=0}^\infty\frac{(-1)^m\alpha_j^{2m}}{(2m)!}
+i\tau_j\sum_{m=0}^\infty\frac{(-1)^m\alpha_j^{2m+1}}{(2m+1)!}
=I_2\cos\alpha_j+i\tau_j\sin\alpha_j.
$$

Therefore

$$
\boxed{A_1=\begin{pmatrix}\cos\alpha_1&i\sin\alpha_1\\i\sin\alpha_1&\cos\alpha_1\end{pmatrix},\qquad
A_2=\begin{pmatrix}\cos\alpha_2&\sin\alpha_2\\-\sin\alpha_2&\cos\alpha_2\end{pmatrix},}
$$



$$
\boxed{A_3=\begin{pmatrix}e^{i\alpha_3}&0\\0&e^{-i\alpha_3}\end{pmatrix}.}
$$

Since each $\tau_j$ is [Hermitian](../../hilbert-space.md#hermitian-operator), $A_j^\dagger=\cos\alpha_j I_2-i\sin\alpha_j\tau_j=A_j^{-1}$; each is a [unitary matrix](../../linear-operator-theory.md#unitary-matrix).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $A_1$, the [determinant](../../multilinear-algebra.md#determinant) is $\cos^2\alpha_1-(i\sin\alpha_1)^2=1$. For $A_2$ it is $\cos^2\alpha_2+\sin^2\alpha_2=1$, and for $A_3$ it is $e^{i\alpha_3}e^{-i\alpha_3}=1$. Multiplicativity of the [determinant](../../multilinear-algebra.md#determinant) gives

$$
\boxed{\det A_1=\det A_2=\det A_3=1,\qquad\det(A_1A_2A_3)=1.}
$$

Together with [unitarity](../../vector-space.md#unitary-operator), this places the [matrices](../../vector-space.md#matrix) and their product in [SU(2)](../../topological-group.md#su-2-group).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Writing the [matrix](../../vector-space.md#matrix) explicitly gives

$$
M=\begin{pmatrix}ix_3&ix_1+x_2\\ix_1-x_2&-ix_3\end{pmatrix}.
$$

Its [determinant](../../multilinear-algebra.md#determinant) is

$$
\det M=x_3^2-(ix_1+x_2)(ix_1-x_2)
=\boxed{x_1^2+x_2^2+x_3^2.}
$$

Since $\det A_1^\dagger=(\det A_1)^*=1$,

$$
\boxed{\det(A_1^\dagger MA_1)=\det M=|\mathbf x|^2.}
$$

The [conjugation](../../group-action.md#conjugation) therefore preserves the squared Euclidean length encoded in $M$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Set $c=\cos(2\alpha_1)$ and $s=\sin(2\alpha_1)$. Multiplying the [matrices](../../vector-space.md#matrix), or using the [Pauli matrix multiplication law](../../algebra.md#pauli-matrix-multiplication-law), gives

$$
A_1^\dagger\tau_1A_1=\tau_1,\qquad
A_1^\dagger\tau_2A_1=c\tau_2+s\tau_3,\qquad
A_1^\dagger\tau_3A_1=c\tau_3-s\tau_2.
$$

Collecting the coefficients of $i\tau_j$ in $M'$ yields

$$
\boxed{\begin{pmatrix}x_1'\\x_2'\\x_3'\end{pmatrix}
=\begin{pmatrix}1&0&0\\0&c&-s\\0&s&c\end{pmatrix}
\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}.}
$$

This is the right-handed active [rotation](../../riemannian-geometry.md#rotation-mathematics) by $2\alpha_1$ about the positive $x_1$ axis. Likewise, with $c_j=\cos(2\alpha_j)$ and $s_j=\sin(2\alpha_j)$,

$$
\boxed{A_2:\ (x_1,x_2,x_3)\mapsto(c_2x_1+s_2x_3,\ x_2,\ -s_2x_1+c_2x_3),}
$$



$$
\boxed{A_3:\ (x_1,x_2,x_3)\mapsto(c_3x_1-s_3x_2,\ s_3x_1+c_3x_2,\ x_3).}
$$

Thus the other axes also have [rotation](../../riemannian-geometry.md#rotation-mathematics) angle $2\alpha_j$. The factor of two is essential: replacing $A_j$ by $-A_j$ leaves the [conjugation](../../group-action.md#conjugation) unchanged, illustrating the two-to-one relation between [SU(2)](../../topological-group.md#su-2-group) and three-dimensional [rotations](../../riemannian-geometry.md#rotation-mathematics).

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Divide by the leading coefficient for $x\ne0,1$:

$$
y''+P(x)y'+Q(x)y=0,\qquad P(x)=\frac1x,\quad Q(x)=\frac1{x(1-x)}.
$$

The [pole](../../isolated-singularity.md#pole) of $P$ makes $x=0$ a [singular point of a differential equation](../../differential-equation.md#singular-point-of-a-differential-equation). However,

$$
xP(x)=1,\qquad x^2Q(x)=\frac{x}{1-x}
$$

are [real analytic](../../analysis.md#real-analytic-function) at zero. Therefore

$$
\boxed{x=0\text{ is a regular singular point}.}
$$

The ordinary-point power-series theorem does not apply there, but the [Frobenius method](../../complex-analysis.md#frobenius-method) does.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a Frobenius exponent $r$, put $p_0=\lim_{x\to0}xP(x)=1$ and $q_0=\lim_{x\to0}x^2Q(x)=0$. The [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) is

$$
r(r-1)+p_0r+q_0=r^2=0,
$$

so

$$
\boxed{r_1=r_2=0.}
$$

A fundamental pair has the repeated-root Frobenius form

$$
y_1=\sum_{n=0}^\infty u_nx^n,\qquad
y_2=y_1\ln x+\sum_{n=0}^\infty v_nx^n,
\qquad y=C_1y_1+C_2y_2
$$

on a positive-$x$ interval. In this case a [real analytic](../../analysis.md#real-analytic-function) solution is particularly simple: $y_1=1-x$ satisfies the equation exactly. A convenient logarithmic companion, obtained below, is $y_2=x+(1-x)\ln[x/(1-x)]$ for $0<x<1$. It is independent of $y_1$ because of its logarithmic divergence at zero.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $A(x)=\sum_{n=1}^\infty a_nx^n$ denote the analytic part of the prescribed ansatz. Its logarithmic part has [derivatives](../../calculus.md#derivative)

$$
\frac d{dx}[(b+cx)\ln x]=c\ln x+\frac bx+c,\qquad
\frac{d^2}{dx^2}[(b+cx)\ln x]=\frac cx-\frac b{x^2}.
$$

After substitution, the full [differential equation](../../differential-equation.md) reduces to

$$
x(1-x)A''+(1-x)A'+A+2c(1-x)+(b+c)\ln x=0.
$$

The first terms are [real analytic](../../analysis.md#real-analytic-function) at zero and cannot cancel a nonzero [logarithm](../../calculus.md#logarithm). Therefore

$$
\boxed{c=-b.}
$$

The cancellation of the apparent $1/x$ terms is already built into this calculation.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

With $c=-b$, equate coefficients in

$$
x(1-x)A''+(1-x)A'+A+2c(1-x)=0.
$$

The constant term is $a_1+2c=0$, and the coefficient of $x$ is $4a_2-2c=0$. Hence

$$
\boxed{a_1=2b,\qquad a_2=-\frac b2.}
$$

For the coefficient of $x^{n-1}$ with $n\geq3$, the first two positive [derivative](../../calculus.md#derivative) terms contribute $n^2a_n$, while the remaining analytic terms contribute $[1-(n-1)^2]a_{n-1}$. Thus

$$
\boxed{a_n=\frac{n-2}{n}a_{n-1},\quad n\geq3.}
$$

Iteration gives $a_n=-b/[n(n-1)]$ for $n\geq2$. Using

$$
\sum_{n=2}^\infty\frac{x^n}{n(n-1)}=x+(1-x)\ln(1-x),\qquad |x|<1,
$$

the prescribed solution sums to

$$
\boxed{y=b\left[x+(1-x)\ln\frac{x}{1-x}\right].}
$$

The ansatz starts its analytic [series](../../sequence-and-series.md#series-mathematics) at $n=1$, so it omits the freedom to add an arbitrary multiple of $1-x$. The complete two-constant real solution on $0<x<1$ is therefore

$$
\boxed{y=C(1-x)+b\left[x+(1-x)\ln\frac{x}{1-x}\right].}
$$

The narrower ansatz in (c) is a convenient choice of the logarithmic solution, not the full [general solution](../../linear-ordinary-differential-equation.md#general-solution) by itself.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For nonzero $b$, the coefficients satisfy $a_n\sim-b/n^2$, so the analytic [power series](../../sequence-and-series.md#power-series) has [radius of convergence](../../sequence-and-series.md#radius-of-convergence) $1$. It converges absolutely also at $x=\pm1$, by comparison with $\sum n^{-2}$.

The real [logarithm](../../calculus.md#logarithm) in the prescribed solution requires $x>0$. Consequently

$$
\boxed{0<x<1\text{ is the interval of the represented classical solution}.}
$$

The [series](../../sequence-and-series.md#series-mathematics) and the function itself have finite limits at $x=1$; in fact the logarithmic companion tends to $1$. Its [derivatives](../../calculus.md#derivative) are singular there, so convergence of its values at the endpoint does not make it a classical solution through that [singular point of a differential equation](../../differential-equation.md#singular-point-of-a-differential-equation). At $x=0$ the logarithmic branch diverges. The independent analytic solution $C(1-x)$ is a [polynomial](../../polynomial.md) and has no such convergence restriction.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The endpoint constraints are $y(-a)=y(a)=0$. The constants in the three costs contribute only $2aK$, $2aK'$ and $2aK''$ respectively, so they do not affect the minimizing shapes. For companies B and C, the fixed [arc length](../../riemannian-geometry.md#arc-length) is

$$
\mathcal L[y]=\int_{-a}^a\sqrt{1+y'^2}\,dx=L.
$$

The original PDF has $(y')^2$ as company A's first variable term. The local TeX transcription has lost that [derivative](../../calculus.md#derivative) dot and incorrectly repeats $y^2$; the calculation below follows the PDF.

**Company A.** The relevant [functional](../../calculus-of-variations.md#functional) is $J_A=\int(y'^2+y^2-2xy)\,dx$. The [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) gives

$$
2(y-x)-2y''=0,\qquad y''-y=-x.
$$

Its [general solution](../../linear-ordinary-differential-equation.md#general-solution) is $y=x+c_1\cosh x+c_2\sinh x$. Adding and subtracting the endpoint equations gives $c_1=0$ and $c_2=-a/\sinh a$. Thus

$$
\boxed{y_A(x)=x-a\frac{\sinh x}{\sinh a}.}
$$

This [curve](../../topology.md#curve) is odd, negative on the left half and positive on the right half; company A has no lower-half-plane restriction. It is the unique global minimum. Indeed, for any endpoint-zero [variation](../../calculus-of-variations.md#variation) $\eta$, [integration by parts](../../calculus.md#integration-by-parts) and the [differential equation](../../differential-equation.md) cancel all linear terms, leaving

$$
J_A[y_A+\eta]-J_A[y_A]=\int_{-a}^a(\eta'^2+\eta^2)\,dx>0
$$

unless $\eta=0$.

**Company B.** Minimize $\int y\,dx$ under the length constraint. Introduce a constant [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) $\lambda$ and apply the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) to $y+\lambda\sqrt{1+y'^2}$:

$$
1-\lambda\frac{y''}{(1+y'^2)^{3/2}}=0.
$$

The [curvature](../../differential-geometry.md#curvature) is constant, so the required lower arc is a [circular arc](../../topology.md#circular-arc). Writing its radius as $R\geq a$ and imposing the endpoints gives

$$
\boxed{y_B(x)=\sqrt{R^2-a^2}-\sqrt{R^2-x^2}.}
$$

Since $\sqrt{1+y_B'^2}=R/\sqrt{R^2-x^2}$, its length determines the radius:

$$
\boxed{L=2R\arcsin(a/R).}
$$

Equivalently, introduce $0<\theta\leq\pi/2$ with $a=R\sin\theta$. Then $L/(2a)=\theta/\sin\theta$, which increases strictly from $1$ to $\pi/2$. The stipulated range of $L$ therefore selects one minor arc. At $L=\pi a$ it becomes the lower [semicircle](../../topology.md#semicircle), with vertical endpoint tangents; it is still a single-valued finite-length graph.

Global minimality follows from the [convexity](../../real-analysis.md#convex-function) of the augmented slope cost with $\lambda=R$. For a competitor $y=y_B+\eta$,

$$
R\left(\sqrt{1+y'^2}-\sqrt{1+y_B'^2}\right)
\geq\frac{Ry_B'}{\sqrt{1+y_B'^2}}\eta'=x\eta'.
$$

Consequently the augmented cost difference is at least $\int(\eta+x\eta')dx=[x\eta]_{-a}^a=0$. Competitors have the same length, so the multiplier contribution cancels and the original cost is minimized. This proves that a [circular arc maximizes area below a fixed chord](../../analysis.md#circular-arc-maximizes-area-below-a-fixed-chord): minimizing negative signed height maximizes the area between the fence and the chord.

**Company C.** The variable cost is $J_C=\int y\,ds=\int y\sqrt{1+y'^2}\,dx$. The augmented integrand is $(y+\lambda)\sqrt{1+y'^2}$. Since it has no explicit $x$ dependence, the [Beltrami identity](../../analysis.md#beltrami-identity) gives

$$
\frac{y+\lambda}{\sqrt{1+y'^2}}=b.
$$

The hanging branch with $b>0$ integrates to $y+\lambda=b\cosh[(x-x_0)/b]$. Equal endpoint heights [force](../../force.md) $x_0=0$, and the endpoint value fixes $\lambda=b\cosh(a/b)$. Thus

$$
\boxed{y_C(x)=b\left[\cosh(x/b)-\cosh(a/b)\right],\qquad b>0.}
$$

Its length is

$$
\boxed{L=\int_{-a}^a\cosh(x/b)\,dx=2b\sinh(a/b).}
$$

Writing $q=a/b$, the equation $L/(2a)=\sinh q/q$ has one positive solution for every $L>2a$: its [derivative](../../calculus.md#derivative) has numerator $q\cosh q-\sinh q>0$. The [curve](../../topology.md#curve) is a [catenary](../../analysis.md#catenary), is even, and lies strictly below the chord except at the endpoints.

A direct argument proves this is a global minimum, rather than merely an extremum of an augmented [functional](../../calculus-of-variations.md#functional). Parametrize any competitor by [arc length](../../riemannian-geometry.md#arc-length) $s\in[-L/2,L/2]$, from its left endpoint to its right endpoint. Then $x'^2+y'^2=1$, $\int x' ds=2a$, and [integration by parts](../../calculus.md#integration-by-parts) gives

$$
J_C=-\int sy'\,ds=2ab-\int(bx'+sy')\,ds
\geq2ab-\int_{-L/2}^{L/2}\sqrt{b^2+s^2}\,ds.
$$

The [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality) gives the last step. Equality requires $x'=b/\sqrt{b^2+s^2}$ and $y'=s/\sqrt{b^2+s^2}$, whose [integrals](../../integral.md) are precisely the displayed [catenary](../../analysis.md#catenary) with the stated length. Thus it attains a lower bound valid for every competitor. This proves that a [catenary minimizes the integral of height along a fixed-length curve](../../analysis.md#catenary-minimizes-the-integral-of-height-along-a-fixed-length-curve).

<a id="5/image-the-three-minimizing-fence-shapes-with-fixed-length-examples-for-companies-b-and-c"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1-q5-fence-minima.png)

**[Figure 1](#5/image-the-three-minimizing-fence-shapes-with-fixed-length-examples-for-companies-b-and-c). The three minimizing fence shapes, with fixed-length examples for companies B and C**.

The sketch uses $a=1$ and $L=2.7$ for the two fixed-length cases. The vertical scale in the company A panel is enlarged to show its small odd deflection. No comparison between the three companies' absolute prices is required or possible from the shapes alone, since their additive cost constants are independent.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

When $r=p'$, write the differential expression in divergence form,

$$
\widetilde L y=(py')'+qy.
$$

Two integrations by parts give the [Lagrange identity for a Sturm-Liouville operator](../../sturm-liouville-theory.md#lagrange-identity-for-a-sturm-liouville-operator):

$$
\langle f,\widetilde Lg\rangle-\langle\widetilde Lf,g\rangle
=\left[p(fg'-f'g)\right]_a^b.
$$

The $q$ terms cancel because $q$ is real. Hence the exact boundary criterion, in the sense of [self-adjointness](../../linear-operator-theory.md#self-adjoint-operator) defined in the question, is

$$
\boxed{\left[p(fg'-f'g)\right]_a^b=0\quad\text{for every admissible pair }f,g.}
$$

At regular endpoints, all separated homogeneous conditions of the following type satisfy it:

$$
\alpha_a y(a)+\beta_a p(a)y'(a)=0,\qquad
\alpha_b y(b)+\beta_b p(b)y'(b)=0,
$$

with real coefficients, not both zero at either endpoint. The allowed value-and-flux pairs at an endpoint are proportional, so their [determinant](../../multilinear-algebra.md#determinant) $p(fg'-f'g)$ vanishes. This includes [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition), [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition), [Robin boundary conditions](../../differential-equation.md#robin-boundary-condition) and arbitrary mixtures of these at the two ends.

Coupled conditions can also work: periodic conditions $y(b)=y(a)$ and $p(b)y'(b)=p(a)y'(a)$ make the two endpoint expressions equal; simultaneous minus signs give the antiperiodic case. Thus requiring each endpoint term separately to vanish is sufficient, but not necessary.

More generally, for regular endpoints set $Y=(y(a),y(b))^{\mathsf T}$ and $N=(-p(a)y'(a),p(b)y'(b))^{\mathsf T}$. All maximal homogeneous self-adjoint [boundary conditions](../../differential-equation.md#boundary-condition) can be written $AY+BN=0$ with real two-by-two [matrices](../../vector-space.md#matrix) satisfying $\operatorname{rank}(A\ B)=2$ and $AB^{\mathsf T}=BA^{\mathsf T}$. If an endpoint is singular, the relevant limiting boundary form and admissible domain must instead be specified; the assumption $p>0$ only in the interior does not itself fix those endpoint limits.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

First move the order parameter term to the right-hand side:

$$
x^2y''+xy'+\beta^2x^2y=n^2y.
$$

Here $p=x^2$, $r=x$, so the [integrating factor](../../linear-ordinary-differential-equation.md#integrating-factor) obeys

$$
\frac{w'}w=\frac{r-p'}p=-\frac1x,
\qquad w(x)=\frac{C}{x}.
$$

Choose the irrelevant positive constant $C=1$. Multiplying the equation by $1/x$ gives

$$
(xy')'+\beta^2xy=\frac{n^2}{x}y.
$$

Thus a [Sturm-Liouville theory](../../sturm-liouville-theory.md) [eigenvalue](../../linear-operator-theory.md#eigenvalue) formulation with the requested [eigenvalue](../../linear-operator-theory.md#eigenvalue) is

$$
\boxed{Ly=\lambda wy,\qquad
L=\frac d{dx}\left(x\frac d{dx}\right)+\beta^2x,\quad
w=\frac1x,\quad\lambda=n^2.}
$$

This is the [Sturm-Liouville formulation with Bessel order as eigenvalue](../../bessel-function.md#sturm-liouville-formulation-with-bessel-order-as-eigenvalue). The spectral parameter is the squared order of the [Bessel function](../../bessel-function.md), with $\beta$ treated as fixed. This differs from the also familiar formulation in which $\beta^2$ is the [eigenvalue](../../linear-operator-theory.md#eigenvalue).

The factor $1/x$ is singular at the origin. Consequently the [integral](../../integral.md) defining $w$ cannot literally use lower limit zero; take a positive reference point $x_*>0$, obtain $w=x_*/x$, and absorb $x_*$ into the normalization. The differential identity holds for $x>0$. [Boundary conditions](../../differential-equation.md#boundary-condition) and admissibility at zero and at the outer endpoint are additional ingredients needed to make a particular self-adjoint spectral problem.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Denote the unshifted differential expression by $L_0y=(py')'+qy$. The supplied [Green's function](../../green-s-function.md) satisfies $L_0G(x,\xi)=\delta(x-\xi)$, whereas the inhomogeneous equation is $L_0y=\lambda wy+wf$.

Multiply the latter equation by $G$ and the Green equation by $y$, subtract and integrate in $x$:

$$
\int_a^b\left[G L_0y-yL_0G\right]dx
=\lambda\int_a^bwGy\,dx+\int_a^bwGf\,dx-y(\xi).
$$

The left-hand side is the boundary term

$$
\left[p(Gy'-yG_x)\right]_a^b.
$$

It vanishes because $G$ and $y$ satisfy the same homogeneous [Robin boundary conditions](../../differential-equation.md#robin-boundary-condition). For example, where $\alpha\ne0$, substituting $y'=-\beta y/\alpha$ and $G_x=-\beta G/\alpha$ cancels the endpoint expression; where $\alpha=0$, both values vanish. The other endpoint works identically. Hence

$$
\boxed{\int_a^b f(x)w(x)G(x,\xi)\,dx
+\lambda\int_a^b w(x)G(x,\xi)y(x)\,dx-y(\xi)=0.}
$$

The [Dirac delta function](../../distribution-theory.md#dirac-delta-function) contribution is valid for an interior evaluation point $\xi$; equivalently, $G$ is continuous there and has flux-derivative jump $[pG_x]_{\xi^-}^{\xi^+}=1$.

This uses the existence of the unshifted [Green's function](../../green-s-function.md) stated in the question. Such a function is not automatic for every choice of $p,q$ and endpoint conditions: a nontrivial [zero mode](../../linear-operator-theory.md#zero-mode) of $L_0$ would obstruct an ordinary inverse and would require a compatibility condition and a modified [Green's function](../../green-s-function.md). Under the stated inverse assumption, the [differential equation](../../differential-equation.md) and the displayed [integral equation](../../analysis.md#integral-equation) are equivalent for functions in the boundary-condition domain.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

The [Cauchy integral formula](../../analysis.md#cauchy-integral-formula) for [derivatives](../../calculus.md#derivative), with $z_0=0$, gives

$$
\oint_C\frac{f(z)}{z^{n+1}}\,dz=\frac{2\pi i}{n!}f^{(n)}(0).
$$

The [derivative](../../calculus.md#derivative) cycles of [sine](../../geometry-and-topology.md#sine) and [cosine](../../geometry-and-topology.md#cosine) give $\sin^{(n)}(0)=\sin(n\pi/2)$ and $\cos^{(n)}(0)=\cos(n\pi/2)$. Therefore

$$
\boxed{\oint_C\frac{\sin z}{z^{n+1}}\,dz=\frac{2\pi i}{n!}\sin\frac{n\pi}{2},\qquad
\oint_C\frac{\cos z}{z^{n+1}}\,dz=\frac{2\pi i}{n!}\cos\frac{n\pi}{2}.}
$$

In particular the [sine](../../geometry-and-topology.md#sine) [integral](../../integral.md) vanishes for even $n$, and the [cosine](../../geometry-and-topology.md#cosine) [integral](../../integral.md) vanishes for odd $n$. For the remaining cases their signs alternate. The radius is irrelevant provided $R>0$, since the numerator is entire and the origin is enclosed once counterclockwise.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Factor the denominator as $(z-z_0)(z+z_0)$. Since $z_0\ne0$, its zeros are distinct, and the potential simple [poles](../../isolated-singularity.md#pole) and their [residues](../../analysis.md#residue) are

$$
\boxed{\operatorname{Res}_{z=z_0}f=\frac{g(z_0)}{2z_0},\qquad
\operatorname{Res}_{z=-z_0}f=-\frac{g(-z_0)}{2z_0}.}
$$

For example, the first follows by taking $\lim_{z\to z_0}(z-z_0)f(z)$. If the numerator vanishes at either denominator zero, the singularity there is removable and the corresponding [residue](../../analysis.md#residue) is zero. Thus the data identify the possible [poles](../../isolated-singularity.md#pole), not an unconditional [pole](../../isolated-singularity.md#pole) at a point canceled by $g$.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

If $f$ is analytic on and inside a positively oriented simple closed contour except for finitely many isolated [poles](../../isolated-singularity.md#pole) $z_j$ strictly inside it, then the [residue theorem](../../analysis.md#residue-theorem) states

$$
\boxed{\oint_Cf(z)\,dz=2\pi i\sum_{z_j\text{ inside }C}\operatorname{Res}_{z=z_j}f.}
$$

There must be no singularity on the contour. More generally each [residue](../../analysis.md#residue) is multiplied by the contour's [winding number](../../complex-analysis.md#winding-number) about its point.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

Let $n\geq2$ be even and integrate $f(z)=1/(1+z^n)$ around an upper-half-plane [semicircle](../../topology.md#semicircle) of radius $R>1$ with the real segment traversed from $-R$ to $R$. There are no real [poles](../../isolated-singularity.md#pole), and the $n/2$ upper-half-plane [poles](../../isolated-singularity.md#pole) are

$$
z_j=e^{i(2j+1)\pi/n},\qquad j=0,\ldots,n/2-1.
$$

Each is simple. Since $z_j^n=-1$,

$$
\operatorname{Res}_{z=z_j}f=\frac1{nz_j^{n-1}}=-\frac{z_j}{n}.
$$

On the [semicircle](../../topology.md#semicircle) the [integral](../../integral.md) magnitude is at most $\pi R/(R^n-1)$, which tends to zero. The real [integral](../../integral.md) is [absolutely convergent](../../sequence-and-series.md#absolute-convergence) because its tail is of order $|x|^{-n}$. Thus

$$
\int_{-\infty}^{\infty}\frac{dx}{1+x^n}
=-\frac{2\pi i}{n}\sum_{j=0}^{n/2-1}e^{i(2j+1)\pi/n}.
$$

Evaluate the finite [geometric series](../../sequence-and-series.md#geometric-series), writing $\theta=\pi/n$:

$$
\sum_{j=0}^{n/2-1}e^{i(2j+1)\theta}
=e^{i\theta}\frac{1-e^{in\theta}}{1-e^{2i\theta}}
=\frac{2e^{i\theta}}{-2ie^{i\theta}\sin\theta}
=\frac{i}{\sin\theta}.
$$

Consequently

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{1+x^n}=\frac{2\pi}{n\sin(\pi/n)},\qquad
A_n=\frac{2\pi}{n},\quad B_n=\frac\pi n.}
$$

For $n=2$ this reduces to $\pi$, as a check on the contour orientation and [residue](../../analysis.md#residue) signs.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/i">i</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8/a/i)

With the stated [Fourier transform](../../fourier-transform.md) convention, [integration by parts](../../calculus.md#integration-by-parts) gives

$$
\widetilde{f'}(\omega)=\int_{-\infty}^\infty f'(t)e^{-i\omega t}\,dt
=\left[f(t)e^{-i\omega t}\right]_{-\infty}^{\infty}
+i\omega\int_{-\infty}^\infty f(t)e^{-i\omega t}\,dt.
$$

The boundary term vanishes, so

$$
\boxed{\widetilde{f'}(\omega)=i\omega\widetilde f(\omega).}
$$

For an [absolutely continuous function](../../sobolev-space.md#absolutely-continuous-function), this calculation requires enough integrability to justify the displayed operations. Under the paper's broader bounded-variation hypothesis, the general identity is the [Fourier transform of a derivative](../../fourier-analysis.md#fourier-transform-of-a-derivative) interpreted distributionally: the [derivative](../../calculus.md#derivative) measure includes [Dirac delta functions](../../distribution-theory.md#dirac-delta-function) at jumps and any singular continuous part. If one instead differentiates only the smooth pieces and discards jumps, the formula needs the corresponding jump corrections. Absolute integrability and [bounded variation](../../real-analysis.md#total-variation-of-a-function) ensure the limits of $f$ at both infinities are zero, but do not by themselves make its ordinary [derivative](../../calculus.md#derivative) capture those singular parts.

<h4 id="8/a/ii">ii</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/a/ii)

For real $f$, [complex conjugation](../../complex-analysis.md#complex-conjugation) commutes with its [absolutely convergent](../../sequence-and-series.md#absolute-convergence) Fourier [integral](../../integral.md):

$$
[\widetilde f(-\omega)]^*
=\left[\int_{-\infty}^\infty f(t)e^{i\omega t}\,dt\right]^*
=\int_{-\infty}^\infty f(t)e^{-i\omega t}\,dt.
$$

Thus

$$
\boxed{[\widetilde f(-\omega)]^*=\widetilde f(\omega).}
$$

This [Hermitian symmetry](../../fourier-transform.md#hermitian-symmetry) pairs the positive- and negative-frequency components of a real signal; its real part is even and its imaginary part is odd.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/i">i</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8/b/i)

Transform in time, leaving $r$ as a parameter. Applying the [derivative](../../calculus.md#derivative) identity twice gives $\widetilde{\partial_t^2\sigma}=-\omega^2\widetilde\sigma$. Therefore

$$
-\omega^2\widetilde\sigma-\partial_r^2\widetilde\sigma+\mu^2\widetilde\sigma=0,
\qquad
\boxed{\partial_r^2\widetilde\sigma=(\mu^2-\omega^2)\widetilde\sigma.}
$$

These manipulations can be justified for sufficiently decaying smooth fields, or with distributional [Fourier transforms](../../fourier-transform.md) when ordinary integrability is unavailable.

<h4 id="8/b/ii">ii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/b/ii)

At fixed [frequency](../../wave.md#frequency), the transformed equation has characteristic roots $\pm ik$, where

$$
\boxed{k^2=\omega^2-\mu^2.}
$$

For a consistent explicit branch choose

$$
k(\omega)=\begin{cases}
\sqrt{\omega^2-\mu^2},&|\omega|>\mu,\\
i\sqrt{\mu^2-\omega^2},&|\omega|<\mu.
\end{cases}
$$

This branch is even in $\omega$. Away from the two thresholds, the spatial solution is $\widetilde\sigma=A(\omega)e^{ikr}+B(\omega)e^{-ikr}$, so [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\boxed{\sigma(t,r)=\frac1{2\pi}\int_{-\infty}^{\infty}
\left[A(\omega)e^{ik(\omega)r}+B(\omega)e^{-ik(\omega)r}\right]e^{i\omega t}\,d\omega.}
$$

At $|\omega|=\mu$, the spatial equation has a double zero characteristic root and its full solution is $C+D r$. The two exponentials at $k=0$ represent only its constant part. This isolated-frequency issue does not change an [integral](../../integral.md) with ordinary integrable amplitudes; threshold-supported distributional modes require separate treatment.

<h4 id="8/b/iii">iii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8/b/iii)

Reality requires $\widetilde\sigma(\omega,r)=\widetilde\sigma(-\omega,r)^*$. The way it constrains the amplitudes depends on whether the spatial [wave number](../../wave-equation.md#wavenumber) is real or imaginary.

For $|\omega|>\mu$, $k$ is real and even. [Complex conjugation](../../complex-analysis.md#complex-conjugation) interchanges the two exponentials, so comparing independent spatial factors gives

$$
\boxed{A(\omega)=B(-\omega)^*\qquad(|\omega|>\mu).}
$$

The companion equation $B(\omega)=A(-\omega)^*$ is the same constraint with [frequency](../../wave.md#frequency) reversed and conjugated. Neither oscillatory spatial branch grows as $r\to\infty$.

For $|\omega|<\mu$, put $k=i\kappa$ with $\kappa>0$. Then

$$
\widetilde\sigma=A(\omega)e^{-\kappa r}+B(\omega)e^{\kappa r}.
$$

Boundedness excludes the growing exponential, and reality then pairs the remaining amplitudes:

$$
\boxed{B(\omega)=0,\qquad A(\omega)=A(-\omega)^*\qquad(|\omega|<\mu).}
$$

These are the two independent low-frequency requirements. At threshold boundedness eliminates the separate linear-in-$r$ solution discussed in (ii). The constraints are understood for a [Fourier transform](../../fourier-transform.md) representation in which spatial mode amplitudes are well defined; sufficient amplitude integrability also ensures the spectral [integral](../../integral.md) itself is bounded.

<h4 id="8/b/iv">iv</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#8/b/iv)

Split the inverse transform into the intervals $|\omega|<\mu$ and $|\omega|>\mu$, and in each case pair the positive-frequency [integral](../../integral.md) with its [complex conjugate](../../complex-analysis.md#complex-conjugate) at negative [frequency](../../wave.md#frequency). The low-frequency pair becomes

$$
\frac1\pi\operatorname{Re}\int_0^\mu A(\omega)e^{ik(\omega)r}e^{i\omega t}\,d\omega,
$$

since $B=0$ and the decaying spatial factor is real. In the high-frequency positive half, replace $A(\omega)$ by $B(-\omega)^*$. The negative half is again its conjugate. Combining the two pieces gives

$$
\boxed{\sigma(t,r)=\frac1\pi\operatorname{Re}\left[
\int_0^\mu A(\omega)e^{ikr}e^{i\omega t}\,d\omega+
\int_\mu^\infty\left\{B(\omega)e^{-ikr}e^{i\omega t}
+B(-\omega)^*e^{ikr}e^{i\omega t}\right\}d\omega\right],\quad\lambda=\frac1\pi.}
$$

Every integrand satisfies the massive [wave equation](../../wave-equation.md) because $\omega^2=k^2+\mu^2$. Linearity, and taking the real part, preserve the equation whenever differentiation under the [integrals](../../integral.md) is justified, or distributionally under the corresponding spectral assumptions. The construction is exactly the [real bounded Fourier modes of the Klein-Gordon equation](../../wave-equation.md#real-bounded-fourier-modes-of-the-klein-gordon-equation) decomposition.

The displayed expression uses ordinary spectral amplitudes. If distributions supported at $\omega=\pm\mu$ are admitted, a further bounded threshold contribution $c_1\cos\mu t+c_2\sin\mu t$, independent of $r$, is possible. It is not a missing propagating or evanescent branch of the open [frequency](../../wave.md#frequency) intervals.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Label the equilibrium vertices in the order $+x,-x,+y,-y,+z,-z$, and write their [displacements](../../classical-mechanics.md#displacement) as $\mathbf u_i(t)\in\mathbb R^3$. Their eighteen Cartesian components are [generalized coordinates](../../lagrangian-mechanics.md#generalized-coordinate). Linearize the axial Hookean [springs](../../elasticity-physics.md#spring) about the unstressed equilibrium. For an edge with unit direction $\mathbf n_{ij}$, its first-order extension is $\mathbf n_{ij}\cdot(\mathbf u_i-\mathbf u_j)$, so the quadratic [potential energy](../../energy.md#potential-energy) is

$$
V=\frac k2\sum_{\langle ij\rangle}[\mathbf n_{ij}\cdot(\mathbf u_i-\mathbf u_j)]^2.
$$

Three [zero modes](../../linear-operator-theory.md#zero-mode) are [translations](../../geometry-and-topology.md#translation-geometry): for each Cartesian [unit vector](../../vector-space.md#unit-vector) $\mathbf e_\alpha$, take $\mathbf u_i=\mathbf e_\alpha$ at every vertex. Three more are infinitesimal [rotations](../../riemannian-geometry.md#rotation-mathematics) $\mathbf u_i=\mathbf e_\alpha\times\mathbf r_i$. Explicitly, in the stated vertex order, their [displacement](../../classical-mechanics.md#displacement) [vectors](../../vector-space.md#vector) are

$$
R_x:\quad (\mathbf0,\mathbf0,\mathbf e_z,-\mathbf e_z,-\mathbf e_y,\mathbf e_y),
$$



$$
R_y:\quad (-\mathbf e_z,\mathbf e_z,\mathbf0,\mathbf0,\mathbf e_x,-\mathbf e_x),
$$



$$
R_z:\quad (\mathbf e_y,-\mathbf e_y,-\mathbf e_x,\mathbf e_x,\mathbf0,\mathbf0).
$$

[Translations](../../geometry-and-topology.md#translation-geometry) leave each [displacement](../../classical-mechanics.md#displacement) difference zero. For [rotations](../../riemannian-geometry.md#rotation-mathematics),

$$
\mathbf n_{ij}\cdot[\boldsymbol\Omega\times(\mathbf r_i-\mathbf r_j)]=0
$$

because the equilibrium edge [vector](../../vector-space.md#vector) is parallel to $\mathbf n_{ij}$. Hence every [spring](../../elasticity-physics.md#spring) has zero first-order extension in all six patterns, and the [stiffness matrix](../../finite-element-method.md#stiffness-matrix) annihilates them.

The [translations](../../geometry-and-topology.md#translation-geometry) have nonzero summed [displacement](../../classical-mechanics.md#displacement), while all the [rotations](../../riemannian-geometry.md#rotation-mathematics) have zero sum. The three rotational patterns are themselves independent because the vertices do not lie on a single line. Thus

$$
\boxed{\text{there are at least six independent zero modes: three translations and three rotations}.}
$$

These are the [rigid-motion zero modes of a spring framework](../../linear-operator-theory.md#rigid-motion-zero-modes-of-a-spring-framework). The rotational [displacements](../../classical-mechanics.md#displacement) describe infinitesimal rigid [rotations](../../riemannian-geometry.md#rotation-mathematics); an arbitrary finite [rotation](../../riemannian-geometry.md#rotation-mathematics) would require its nonlinear [displacement](../../classical-mechanics.md#displacement) field.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

For a breathing [displacement](../../classical-mechanics.md#displacement) take $\mathbf u_i=q(t)\mathbf r_i$. Every [spring](../../elasticity-physics.md#spring) has equilibrium length $\sqrt2$ in the given length units, so its linear extension is $\sqrt2q$. At the vertex $\mathbf r_i$, the four adjacent equilibrium vertices sum to zero. Therefore the [spring](../../elasticity-physics.md#spring) [force](../../force.md) there is

$$
\mathbf F_i=-kq\sum_{j\sim i}(\mathbf r_i-\mathbf r_j)=-4kq\mathbf r_i.
$$

It remains radial and proportional to the original [displacement](../../classical-mechanics.md#displacement) at every vertex, proving that this symmetric [displacement](../../classical-mechanics.md#displacement) is a [normal mode](../../wave-equation.md#normal-mode). [Newton's second law](../../force.md#newton-s-second-law) gives

$$
m\ddot q=-4kq,\qquad
\boxed{\omega_b=2\sqrt{\frac km},\qquad f_b=\frac1\pi\sqrt{\frac km}.}
$$

The first is [angular frequency](../../lagrangian-mechanics.md#angular-frequency) and the second is cycles per unit time. For $k$ in $\mathrm{N\,m^{-1}}$ and $m$ in $\mathrm{kg}$, these have units $\mathrm{rad\,s^{-1}}$ and $\mathrm{Hz}$ respectively. An [energy](../../energy.md) check gives $T=3m\dot q^2$ and $V=12kq^2$, leading to the same ratio $\omega_b^2=24k/(6m)$.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

The initial [displacement](../../classical-mechanics.md#displacement) lies in an [invariant subspace](../../representation-theory.md#invariant-subspace) of axial motions. Let the three opposite vertex pairs have positions

$$
\pm(1+q_x)\mathbf e_x,\qquad \pm(1+q_y)\mathbf e_y,\qquad \pm(1+q_z)\mathbf e_z.
$$

For a vertex on the positive $x$ axis, the two [springs](../../elasticity-physics.md#spring) towards the $y$ vertices contribute $-k(q_x+q_y)$ in the $x$ direction; the two towards the $z$ vertices contribute $-k(q_x+q_z)$. Transverse components cancel in pairs. Cyclically,

$$
m\frac{d^2}{dt^2}\begin{pmatrix}q_x\\q_y\\q_z\end{pmatrix}
=-k\begin{pmatrix}2&1&1\\1&2&1\\1&1&2\end{pmatrix}
\begin{pmatrix}q_x\\q_y\\q_z\end{pmatrix}.
$$

The [matrix](../../vector-space.md#matrix) is $I+\mathbf1\mathbf1^{\mathsf T}$. It has [eigenvalue](../../linear-operator-theory.md#eigenvalue) $4$ on the breathing [vector](../../vector-space.md#vector) $(1,1,1)$, and [eigenvalue](../../linear-operator-theory.md#eigenvalue) $1$ on the orthogonal plane $q_x+q_y+q_z=0$. This identifies the [axial normal modes of an octahedral spring framework](../../wave-equation.md#axial-normal-modes-of-an-octahedral-spring-framework) without a large characteristic [determinant](../../multilinear-algebra.md#determinant).

Put $\omega_0=\sqrt{k/m}$ and decompose the initial [vector](../../vector-space.md#vector) as

$$
(\epsilon_1,\epsilon_2,\epsilon_2)
=A(1,1,1)+D(2,-1,-1),\qquad
A=\frac{\epsilon_1+2\epsilon_2}{3},\quad D=\frac{\epsilon_1-\epsilon_2}{3}.
$$

Since all initial [velocities](../../classical-mechanics.md#velocity) are zero, only [cosine](../../geometry-and-topology.md#cosine) time factors occur. The complete motion to first order in the [displacements](../../classical-mechanics.md#displacement) is

$$
\boxed{q_x(t)=A\cos(2\omega_0t)+2D\cos(\omega_0t),\qquad
q_y(t)=q_z(t)=A\cos(2\omega_0t)-D\cos(\omega_0t),}
$$

with the vertex positions given by the first displayed formula. No [translation](../../geometry-and-topology.md#translation-geometry) or [rotation](../../riemannian-geometry.md#rotation-mathematics) is excited: the initial [displacements](../../classical-mechanics.md#displacement) are orthogonal to those [zero modes](../../linear-operator-theory.md#zero-mode) and their initial [velocities](../../classical-mechanics.md#velocity) vanish. The two checks $\epsilon_1=\epsilon_2$ and $\epsilon_1+2\epsilon_2=0$ respectively isolate pure breathing and pure traceless axial [oscillation](../../wave.md#oscillation). Nonlinear corrections beyond the small-displacement approximation have been omitted.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

The [sign homomorphism](../../finite-group-theory.md#sign-homomorphism) $\operatorname{sgn}:S_n\to\{+1,-1\}$ records [parity of a permutation](../../finite-group-theory.md#parity-of-a-permutation). The [kernel of a group homomorphism](../../group-theory.md#kernel-of-a-group-homomorphism) in this case is the [alternating group](../../finite-group-theory.md#alternating-group) $A_n$, consisting of even [permutations](../../combinatorics.md#permutation). For $n\geq2$ it has index two in the [symmetric group](../../finite-group-theory.md#symmetric-group) and order $n!/2$.

The [cycle type](../../finite-group-theory.md#cycle-type) is the multiset of lengths of the disjoint cycles, including fixed points if desired. For $A_4$ the complete count is

$$
\begin{array}{c|c|c}
\text{cycle type}&\text{kind}&\text{number}\\\hline
1^4&\text{identity}&1\\
(3,1)&\text{three-cycle}&\binom43\,2=8\\
(2,2)&\text{two disjoint transpositions}&3
\end{array}
$$

A single [transposition](../../combinatorics.md#transposition-permutation) and a four-cycle are odd and are excluded. Thus

$$
\boxed{|A_4|=12,\quad\text{with cycle types }1^4,\ (3,1),\ (2,2).}
$$

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

A rigid [rotation](../../riemannian-geometry.md#rotation-mathematics) of a regular [tetrahedron](../../euclidean-geometry.md#tetrahedron) permutes its four vertices, giving an injective [group homomorphism](../../group-theory.md#group-homomorphism) from its [rotation](../../riemannian-geometry.md#rotation-mathematics) [group](../../group.md) to $S_4$: fixing every vertex [forces](../../force.md) the [rotation](../../riemannian-geometry.md#rotation-mathematics) to be the identity. Its seven nontrivial [rotation](../../riemannian-geometry.md#rotation-mathematics) axes are four lines through a vertex and the opposite face centre, and three lines through midpoints of opposite edges.

Each vertex-face axis admits [rotations](../../riemannian-geometry.md#rotation-mathematics) by $\pm2\pi/3$, giving eight three-cycles on the vertices. Each opposite-edge axis admits a half-turn, giving three double [transpositions](../../combinatorics.md#transposition-permutation). Along with the identity there are twelve [rotations](../../riemannian-geometry.md#rotation-mathematics). All their induced [permutations](../../combinatorics.md#permutation) are even, so the injective image is a twelve-element [subgroup](../../group.md#subgroup) of $A_4$, hence the whole [group](../../group.md). Therefore

$$
\boxed{\text{the tetrahedron rotation group is isomorphic to }A_4.}
$$

Its action on $\mathbb R^3$ supplies a three-dimensional [representation](../../representation-theory.md#group-representation). To prove irreducibility even after complexification, choose vertices

$$
(1,1,1),\quad(1,-1,-1),\quad(-1,1,-1),\quad(-1,-1,1).
$$

The [group](../../group.md) contains the half-turns $D_x=\operatorname{diag}(1,-1,-1)$ and their cyclic variants, as well as the coordinate cycle $(x,y,z)\mapsto(y,z,x)$. If a nonzero [invariant subspace](../../representation-theory.md#invariant-subspace) over the complex numbers contains a [vector](../../vector-space.md#vector) with nonzero $x$ component, applying $(I+D_x)/2$ shows it contains the $x$ axis. If another component is nonzero, use the corresponding projection instead. The coordinate cycle then supplies the other two axes. Every nonzero [invariant subspace](../../representation-theory.md#invariant-subspace) is therefore the full space, proving

$$
\boxed{A_4\text{ has an irreducible representation of dimension }3.}
$$

This also gives an elementary proof without presupposing the [character table](../../representation-theory.md#character-table).

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

For a [finite group](../../group.md#finite-group) over the complex numbers, the sum of the squared dimensions of its inequivalent [irreducible representations](../../representation-theory.md#irreducible-representation) equals the [group order](../../group.md#order-of-a-finite-group). There is always a one-dimensional [trivial representation](../../representation-theory.md#trivial-representation), and part (b) supplies an [irreducible representation](../../representation-theory.md#irreducible-representation) of dimension three. Thus the remaining squared dimensions sum to

$$
12-1^2-3^2=2.
$$

They must be two further dimensions equal to one. Hence

$$
\boxed{\text{the irreducible dimensions are }1,1,1,3.}
$$

The number of inequivalent [irreducible representations](../../representation-theory.md#irreducible-representation) equals the number of [conjugacy classes](../../group-action.md#conjugacy-class), so $A_4$ has four classes. There are only three [cycle types](../../finite-group-theory.md#cycle-type) in part (a); consequently [cycle type](../../finite-group-theory.md#cycle-type) cannot classify conjugacy within $A_4$.

More explicitly, the identity is a singleton class, and [conjugation](../../group-action.md#conjugation) by three-cycles permutes the three double [transpositions](../../combinatorics.md#transposition-permutation) transitively. For a three-cycle, the [centralizer](../../group-action.md#centralizer) in $A_4$ consists of its three powers, so its [conjugacy class](../../group-action.md#conjugacy-class) has $12/3=4$ elements. The eight three-cycles therefore split into two classes of four:

$$
\boxed{\text{class sizes }1,3,4,4;\quad\text{the three-cycle type splits into two classes}.}
$$

For example, $(123)$ and $(132)$ have the same [cycle type](../../finite-group-theory.md#cycle-type) but are not conjugate in $A_4$. Any [permutation](../../combinatorics.md#permutation) conjugating the first to its inverse must fix its unique fixed vertex and reverse the orientation of the remaining three labels, so it is odd. They are conjugate in $S_4$, illustrating exactly why restricting the ambient [group](../../group.md) changes the answer.

## ↑ Ancestors (10)

1. [2020](../2020.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
