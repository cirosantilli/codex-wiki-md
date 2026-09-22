# Paper 1

↑ **Parent:** [2010](../2010.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2010/PaperNST_IB_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2010/PaperNST_IB_1.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
- [7](#7)
  - [Solution](#7/solution)
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
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system), use the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) and the [Einstein summation convention](../../multilinear-algebra.md#einstein-notation) to expand

$$
\begin{aligned}
[\mathbf u\times(\nabla\times\mathbf u)]_i
&=\epsilon_{ijk}\epsilon_{klm}u_j\partial_lu_m\\
&=u_j\partial_i u_j-u_j\partial_j u_i\\
&=\frac12\partial_i(u_ju_j)-[(\mathbf u\cdot\nabla)\mathbf u]_i.
\end{aligned}
$$

The contraction of the two symbols uses the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta), and the final step is the [product rule](../../calculus.md#product-rule). Thus the [convective acceleration](../../continuum-mechanics.md#convective-acceleration) identity is

$$
\boxed{(\mathbf u\cdot\nabla)\mathbf u=\frac12\nabla|\mathbf u|^2-\mathbf u\times(\nabla\times\mathbf u).}
$$

Put $\boldsymbol\omega=\nabla\times\mathbf u$. The [curl of a gradient](../../multivariable-calculus.md#curl-of-a-gradient) vanishes, and the [curl of a cross product](../../multivariable-calculus.md#curl-of-a-cross-product) identity gives

$$
\nabla\times(\mathbf u\times\boldsymbol\omega)=\mathbf u\,\nabla\cdot\boldsymbol\omega-\boldsymbol\omega\,\nabla\cdot\mathbf u+(\boldsymbol\omega\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\boldsymbol\omega.
$$

Since the [divergence of a curl is zero](../../multivariable-calculus.md#divergence-of-a-curl-is-zero), taking the [curl](../../multivariable-calculus.md#curl) of the first identity yields

$$
\boxed{\nabla\times[(\mathbf u\cdot\nabla)\mathbf u]=(\nabla\cdot\mathbf u)\boldsymbol\omega+(\mathbf u\cdot\nabla)\boldsymbol\omega-(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

Twice continuous differentiability suffices for the mixed-derivative identities used here.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Away from the axis, [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system) put the field in the [line vortex](../../vorticity.md#line-vortex) form

$$
\mathbf v=\frac{\kappa}{2\pi\rho}\mathbf e_\phi.
$$

The only potentially nonzero component of its [curl](../../multivariable-calculus.md#curl) is

$$
(\nabla\times\mathbf v)_z=\frac1\rho\frac{\partial}{\partial\rho}(\rho v_\phi)=\frac1\rho\frac{\partial}{\partial\rho}\frac\kappa{2\pi}=0.
$$

The other components vanish because there is no axial dependence and no radial or axial velocity. Thus **the [curl](../../multivariable-calculus.md#curl) is zero for $\rho>0$**; the field is singular on the axis, so a classical [curl](../../multivariable-calculus.md#curl) there is not defined.

For a spanning surface avoiding that axis, the smoothness hypotheses of [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) hold and give $\oint_C\mathbf v\cdot d\mathbf r=0$. If the enclosed planar region contains the axis, the singularity prevents applying that theorem directly. Excise a small disk about the origin. The resulting annulus has zero [curl](../../multivariable-calculus.md#curl), so its outer [circulation](../../vorticity.md#circulation-physics) equals the counterclockwise circulation on the small circle:

$$
\boxed{\oint_C\mathbf v\cdot d\mathbf r=\int_0^{2\pi}\frac{\kappa}{2\pi\rho}\rho\,d\phi=\kappa.}
$$

This sign assumes positive, counterclockwise orientation. Clockwise orientation gives $-\kappa$; more generally the value is $\kappa$ times the [winding number](../../complex-analysis.md#winding-number) about the origin. A curve through the origin is excluded because its integral is singular. In the [distribution](../../distribution-theory.md#distribution-mathematical-analysis) interpretation the missing [vorticity](../../vorticity.md) is concentrated on the axis as $\kappa\delta(x)\delta(y)\mathbf e_z$, explaining the nonzero circulation despite zero classical [curl](../../multivariable-calculus.md#curl) away from it.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Since the endpoints represent the same point of the tube, both density and diffusive flux must match. For a positive [diffusion](../../thermodynamics.md#diffusion) coefficient $\lambda$, the [periodic boundary conditions](../../differential-equation.md#periodic-boundary-conditions) are

$$
\boxed{u(-\pi,t)=u(\pi,t),\qquad u_x(-\pi,t)=u_x(\pi,t).}
$$

For [separation of variables](../../partial-differential-equation.md#separation-of-variables), periodic spatial modes solve $X''+n^2X=0$ and have time factors $e^{-\lambda n^2t}$. The constant mode has no decay. The [periodic diffusion on a circle](../../diffusion-equation.md#periodic-diffusion-on-a-circle) solution is therefore

$$
u(x,t)=\frac{a_0}{2}+\sum_{n=1}^\infty[a_n\cos(nx)+b_n\sin(nx)]e^{-\lambda n^2t},
$$

where the [Fourier coefficients](../../fourier-series.md#fourier-coefficient) are

$$
a_n=\frac1\pi\int_{-\pi}^\pi f(x)\cos(nx)dx,\qquad b_n=\frac1\pi\int_{-\pi}^\pi f(x)\sin(nx)dx.
$$

The expression for $a_n$ includes $n=0$.

The specified profile is even, so $b_n=0$. Its mean follows from $\int_0^\pi(\pi-x)^2dx=\pi^3/3$, giving $a_0=2\pi^2/3$. For $n\geq1$, two [integrations by parts](../../calculus.md#integration-by-parts) give

$$
\int_0^\pi(\pi-x)^2\cos(nx)dx=\frac{2\pi}{n^2},\qquad a_n=\frac4{n^2}.
$$

Consequently

$$
\boxed{u(x,t)=\frac{\pi^2}{3}+4\sum_{n=1}^\infty\frac{\cos(nx)}{n^2}e^{-\lambda n^2t}.}
$$

All nonconstant [normal modes](../../wave-equation.md#normal-mode) decay for $\lambda>0$, so the density becomes uniform:

$$
\boxed{u(x,t)\longrightarrow\frac{\pi^2}{3}\quad(t\to\infty).}
$$

The conserved total amount is $\int_{-\pi}^\pi u\,dx=2\pi^3/3$. The initial cusp at zero is compatible with an [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space) solution and is immediately smoothed by [diffusion](../../thermodynamics.md#diffusion). At $\lambda=0$ there would be no relaxation, so positivity is needed for this long-time conclusion.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Expand the [radial modified Helmholtz equation](../../partial-differential-equation.md#radial-modified-helmholtz-equation) as $Ly=-y''-2y'/x+y$. Setting $y=z/x$ gives $Ly=(-z''+z)/x$, so

$$
y(x)=\frac{Ae^x+Be^{-x}}x.
$$

Boundedness at zero requires $A+B=0$, whereas boundedness at infinity requires $A=0$. The respective adapted [homogeneous solutions](../../linear-ordinary-differential-equation.md#homogeneous-solution) are therefore

$$
\boxed{u(x)=\frac{\sinh x}{x}\quad\text{at zero},\qquad v(x)=\frac{e^{-x}}x\quad\text{at infinity}.}
$$

The first has limit one at zero. Their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is $uv'-u'v=-x^{-2}$. Since the highest-derivative coefficient of $L$ is $-1$, the [Green function](../../green-s-function.md) must have first-derivative jump $-1$. The [radial modified Helmholtz Green function on the half-line](../../green-s-function.md#radial-modified-helmholtz-green-function-on-the-half-line) is

$$
\boxed{G(x,\xi)=\frac\xi x\sinh(\min(x,\xi))e^{-\max(x,\xi)},\qquad x,\xi>0.}
$$

It is continuous at the source, and its [derivative](../../calculus.md#derivative) jump is $-1$, giving $L_xG=\delta(x-\xi)$. For fixed source it tends to $\xi e^{-\xi}$ as $x\downarrow0$ and decays at infinity. This kernel is for the original operator and ordinary measure $d\xi$; multiplying the equation by $x^2$ would change the source normalization.

For the compact source, split the [integral](../../integral.md) at $\xi=x$ when $x<R$. The needed antiderivatives are

$$
\int\xi\sinh\xi\,d\xi=\xi\cosh\xi-\sinh\xi,\qquad\int\xi e^{-\xi}d\xi=-(\xi+1)e^{-\xi}.
$$

Thus

$$
y(x)=\frac{e^{-x}}x\int_0^x\xi\sinh\xi\,d\xi+\frac{\sinh x}{x}\int_x^R\xi e^{-\xi}d\xi\quad(x<R),
$$

while for $x>R$ the result is $e^{-x}x^{-1}\int_0^R\xi\sinh\xi\,d\xi$. Simplifying gives

$$
\boxed{y(x)=\begin{cases}\displaystyle1-(R+1)e^{-R}\frac{\sinh x}{x},&0\leq x\leq R,\\\displaystyle(R\cosh R-\sinh R)\frac{e^{-x}}x,&x\geq R.\end{cases}}
$$

The continuous value at zero is $1-(R+1)e^{-R}$, and $y'(0)=0$. Both $y$ and $y'$ match at $R$, so no extra [Dirac delta](../../distribution-theory.md#dirac-delta-function) appears there. The only [homogeneous solution](../../linear-ordinary-differential-equation.md#homogeneous-solution) bounded at both ends is zero, establishing uniqueness.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Split the [Fourier transform](../../fourier-transform.md) integral at zero:

$$
\boxed{\widehat g(k)=\int_0^\infty e^{-(\lambda+ik)x}dx+\int_0^\infty e^{-(\lambda-ik)x}dx=\frac{2\lambda}{\lambda^2+k^2}.}
$$

By [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem) applied to this pair, or by the [residue theorem](../../analysis.md#residue-theorem), the other transform is

$$
\boxed{\widehat h(k)=\frac\pi\mu e^{-\mu|k|}.}
$$

For example, inversion with $\lambda=\mu$ gives $\int e^{ikx}(k^2+\mu^2)^{-1}dk=(\pi/\mu)e^{-\mu|x|}$; evenness supplies the desired sign convention.

Take the spatial [Fourier transform](../../fourier-transform.md) of the [Laplace equation](../../partial-differential-equation.md#laplace-equation). For $y>0$ it gives $\widehat\psi_{yy}-k^2\widehat\psi=0$. Removing the exponentially growing solution and matching the boundary gives

$$
\widehat\psi(k,y)=\widehat f(k)e^{-|k|y}.
$$

At $k=0$ this formula is interpreted by continuity; a single transform value does not alter the inverse integral. The previous transform pair identifies

$$
\mathcal F^{-1}[e^{-|k|y}](x)=\frac1\pi\frac{y}{x^2+y^2}=P_y(x),
$$

the [Poisson kernel for the upper half-plane](../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane). The [convolution theorem](../../fourier-analysis.md#convolution-theorem) therefore gives the [Poisson integral](../../partial-differential-equation.md#poisson-integral)

$$
\boxed{\psi(x,y)=\frac y\pi\int_{\mathbb R}\frac{f(u)}{(x-u)^2+y^2}du.}
$$

This is the bounded harmonic solution for bounded decaying data, or the corresponding solution in an appropriate Fourier class. Such a growth condition matters if vertical decay is interpreted only pointwise: the nonzero [harmonic function](../../partial-differential-equation.md#harmonic-function) $e^{x^2-y^2}\sin(2xy)=\operatorname{Im}e^{(x+iy)^2}$ vanishes on the real axis and tends to zero for fixed $x$ as $y\to\infty$, but grows rapidly in $x$ and has no ordinary spatial [Fourier transform](../../fourier-transform.md). It can be excluded by requiring boundedness; the stated pointwise limits alone would not establish uniqueness.

For the interval data, direct integration gives the [Poisson extension of interval boundary data](../../partial-differential-equation.md#poisson-extension-of-interval-boundary-data)

$$
\boxed{\psi(x,y)=\frac c\pi\left[\arctan\frac{a-x}{y}+\arctan\frac{a+x}{y}\right],\qquad y>0.}
$$

As $y\downarrow0$ it approaches $c$ for $|x|<a$, zero for $|x|>a$, and $c/2$ at $x=\pm a$. At those jump points the prescribed isolated values cannot be attained by a continuous extension; they do not affect the integral. The solution decays vertically, with $\psi\sim2ac/(\pi y)$ for fixed $x$ and large $y$.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

An [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\lambda$ and associated [eigenvector](../../linear-operator-theory.md#eigenvector) $e\ne0$ satisfy $Ae=\lambda e$. The [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) $\det(A-\lambda I)$ has degree equal to the positive [matrix](../../vector-space.md#matrix) size. The [fundamental theorem of algebra](../../algebra.md#fundamental-theorem-of-algebra) gives a complex root, at which $A-\lambda I$ is singular and therefore has a nontrivial kernel. Hence every nonempty square complex [matrix](../../vector-space.md#matrix) has an [eigenvector](../../linear-operator-theory.md#eigenvector).

A nondiagonalizable example is the [Jordan block](../../linear-operator-theory.md#jordan-block) $\begin{pmatrix}0&1\\0&0\end{pmatrix}$: its only [eigenvalue](../../linear-operator-theory.md#eigenvalue) is zero, and its eigenspace is one-dimensional. A [Hermitian matrix](../../hilbert-space.md#hermitian-operator) satisfies $A^\dagger=A$ and has an [orthonormal eigenbasis](../../linear-operator-theory.md#orthonormal-eigenbasis) by the [spectral theorem](../../hilbert-space.md#spectral-theorem). One proof finds an [eigenvector](../../linear-operator-theory.md#eigenvector), notes that its [orthogonal complement](../../hilbert-space.md#orthogonal-complement) is invariant, and repeats. Its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are real because

$$
\lambda\,e^\dagger e=e^\dagger Ae=\overline{e^\dagger Ae}=\overline\lambda\,e^\dagger e,
$$

where $e^\dagger e>0$.

With all [eigenvalues](../../linear-operator-theory.md#eigenvalue) negative, $A$ is invertible. Its same complete eigenbasis gives

$$
\boxed{A^{-1}e_i=\lambda_i^{-1}e_i,\qquad A^me_i=\lambda_i^me_i\quad(m=1,2,\ldots).}
$$

Some powered [eigenvalues](../../linear-operator-theory.md#eigenvalue) can coincide, but the original [eigenvectors](../../linear-operator-theory.md#eigenvector) remain a complete basis. Writing $A=U\operatorname{diag}(\lambda_i)U^\dagger$, the convergent [matrix exponential](../../linear-operator-theory.md#matrix-exponential) series gives

$$
\int_0^\infty e^{tA}dt=U\operatorname{diag}\left(\int_0^\infty e^{t\lambda_i}dt\right)U^\dagger=U\operatorname{diag}(-\lambda_i^{-1})U^\dagger.
$$

Thus the [matrix inverse from a decaying matrix exponential](../../linear-operator-theory.md#matrix-inverse-from-a-decaying-matrix-exponential) is

$$
\boxed{\int_0^\infty e^{tA}dt=-A^{-1},\qquad A^{-1}=-\int_0^\infty e^{tA}dt.}
$$

**The identity printed in the original PDF is missing a minus sign.** Already for the one-by-one [matrix](../../vector-space.md#matrix) $A=(-1)$ its integral is $1$, whereas its inverse is $-1$. Equivalently, integrating $d(e^{tA})/dt=Ae^{tA}$ gives $A\int_0^\infty e^{tA}dt=-I$, confirming the correction without diagonalization.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Complete the square in the [quadratic form](../../quadratic-form.md):

$$
Q_1=(x_1+2x_2)^2+x_2^2+6x_3^2.
$$

The real invertible [linear transformation](../../vector-space.md#linear-map)

$$
\boxed{x=Ly,\qquad L=\begin{pmatrix}1&-2&0\\0&1&0\\0&0&1/\sqrt6\end{pmatrix}}
$$

sets $x_1+2x_2=y_1$, $x_2=y_2$, $\sqrt6x_3=y_3$, giving $Q_1=y_1^2+y_2^2+y_3^2$. The same transformation gives

$$
\boxed{Q_2=y_1^2+y_2^2-y_3^2.}
$$

Its signature is $(2,1)$. By [Sylvester's law of inertia](../../quadratic-form.md#sylvester-s-law-of-inertia) no real invertible change of variables can turn this second form into a sum of three positive squares.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [trace](../../linear-algebra.md#matrix-trace) of a square [matrix](../../vector-space.md#matrix) is $\operatorname{tr}A=\sum_iA_{ii}$. Expanding a product and interchanging its finite sums gives

$$
\boxed{\operatorname{tr}(AB)=\sum_{i,j}A_{ij}B_{ji}=\sum_{j,i}B_{ji}A_{ij}=\operatorname{tr}(BA).}
$$

Hence every [commutator](../../lie-algebra.md#commutator) has trace zero. Taking the trace of $AB-BA=cI$ gives $0=cn$. Over the complex numbers, with $n\geq1$, this forces

$$
\boxed{c=0.}
$$

For that value, choose $A=B=0$, or any commuting pair. For every nonzero $c$ the trace contradiction proves nonexistence. The finite [matrix](../../vector-space.md#matrix) size is essential to this trace argument.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Differentiate the [eigenvalue equation](../../linear-operator-theory.md#eigenvalue-equation) along the assumed smooth normalized eigenbranch:

$$
A'x+Ax'=\lambda'x+\lambda x'.
$$

Since $A$ is real symmetric, $x^TA=\lambda x^T$. Multiplying the differentiated equation by $x^T$ and using $x^Tx=1$ cancels the terms containing $x'$:

$$
x^TA'x+\lambda x^Tx'=\lambda'+\lambda x^Tx'.
$$

Thus the finite-dimensional [Hellmann–Feynman theorem](../../quantum-mechanics.md#hellmann-feynman-theorem) gives

$$
\boxed{\left.\frac{d\lambda}{d\epsilon}\right|_{\epsilon=0}=x(0)^T\left.\frac{dA}{d\epsilon}\right|_{\epsilon=0}x(0).}
$$

Equivalently, differentiating the normalization gives $2x^Tx'=0$ and eliminates those terms from the [derivative](../../calculus.md#derivative) of $\lambda=x^TAx$. The proof needs the smooth eigenbranch assumed in the question; the smallest [eigenvalue](../../linear-operator-theory.md#eigenvalue) need not be differentiable at an arbitrary crossing without that assumption.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

Evaluate the [derivative](../../calculus.md#derivative) along real and imaginary increments. For a [holomorphic function](../../holomorphic-function.md), both give the same value:

$$
f'(z)=u_x+iv_x=\frac{u_y+iv_y}{i}=v_y-iu_y.
$$

Equating real and imaginary parts yields the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations)

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

Differentiate the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) and use equality of mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative), which holds because [holomorphic functions](../../holomorphic-function.md) are smooth:

$$
\boxed{\Delta u=(v_y)_x-(v_x)_y=0,\qquad\Delta v=-(u_y)_x+(u_x)_y=0.}
$$

Thus both parts are [harmonic functions](../../partial-differential-equation.md#harmonic-function).

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) give $\nabla v=(-u_y,u_x)$. Therefore

$$
\boxed{\nabla u\cdot\nabla v=-u_xu_y+u_yu_x=0.}
$$

The [gradient](../../multivariable-calculus.md#gradient) is normal to a regular [level set](../../topology.md#level-set), so these curves intersect orthogonally wherever their [gradients](../../multivariable-calculus.md#gradient) are nonzero. At a [stationary point](../../calculus-of-variations.md#stationary-point), where both [gradients](../../multivariable-calculus.md#gradient) vanish, a regular curve tangent need not exist; the algebraic identity remains valid.

<h3 id="7/iii">iii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7/iii)

The rotation $\nabla v=(-u_y,u_x)$ from the [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) is invertible. Hence

$$
\boxed{\nabla u=0\quad\Longleftrightarrow\quad\nabla v=0.}
$$

Thus their [stationary points](../../calculus-of-variations.md#stationary-point) coincide, including degenerate ones.

<h3 id="7/iv">iv</h3>

↑ **Parent:** [7](#7)

<h4 id="7/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#7/iv)

For a [harmonic function](../../partial-differential-equation.md#harmonic-function), put $a=u_{xx}$ and $b=u_{xy}=u_{yx}$. Since $u_{yy}=-u_{xx}$, its [Hessian matrix](../../multivariable-calculus.md#hessian-matrix) is

$$
D^2u=\begin{pmatrix}a&b\\b&-a\end{pmatrix},\qquad\det D^2u=-a^2-b^2.
$$

A nonzero determinant is therefore negative, and the two real Hessian [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $\pm\sqrt{a^2+b^2}$. At a [stationary point](../../calculus-of-variations.md#stationary-point) the quadratic term of the [Taylor expansion](../../calculus.md#taylor-expansion) has both signs. Consequently **every such nondegenerate [stationary point](../../calculus-of-variations.md#stationary-point) is a [saddle point](../../analysis.md#saddle-point)**. This is the [nondegenerate stationary points of a planar harmonic function](../../partial-differential-equation.md#nondegenerate-stationary-points-of-a-planar-harmonic-function) criterion. The same argument applies to $v$, whose [stationary points](../../calculus-of-variations.md#stationary-point) coincide with those of $u$. A zero Hessian determinant is outside this second-order classification.

<h3 id="7/v">v</h3>

↑ **Parent:** [7](#7)

<h4 id="7/v/solution">Solution</h4>

↑ **Parent:** [V](#7/v)

Assume the image of the domain of $f$ lies in the domain where $g$ is [holomorphic](../../holomorphic-function.md). The complex [chain rule](../../calculus.md#chain-rule) gives

$$
\boxed{(g\circ f)'(z)=g'(f(z))f'(z),}
$$

so the composition is holomorphic, including at points where $f'=0$. Its real part $S(x,y)=s(u(x,y),v(x,y))$ is therefore a [harmonic function](../../partial-differential-equation.md#harmonic-function).

A direct verification uses the [composition of harmonic conjugate pairs](../../partial-differential-equation.md#composition-of-harmonic-conjugate-pairs). The multivariable [chain rule](../../calculus.md#chain-rule) gives

$$
\Delta S=s_{uu}|\nabla u|^2+2s_{uv}\nabla u\cdot\nabla v+s_{vv}|\nabla v|^2+s_u\Delta u+s_v\Delta v.
$$

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) imply $|\nabla u|^2=|\nabla v|^2$; parts (i) and (ii) remove the last three terms. Since $s$ is harmonic in its own variables,

$$
\boxed{\Delta S=|\nabla u|^2(s_{uu}+s_{vv})=0.}
$$

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

In monic form the [Chebyshev differential equation](../../numerical-analysis.md#chebyshev-differential-equation) has $P(x)=-x/(1-x^2)$ and $Q(x)=p^2/(1-x^2)$. Both are analytic near zero, so it is an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation). At $x=1$, $(x-1)P=x/(x+1)$ and $(x-1)^2Q=-p^2(x-1)/(x+1)$ are analytic; at $x=-1$, $(x+1)P=x/(x-1)$ and $(x+1)^2Q=-p^2(x+1)/(x-1)$ are analytic. Thus both endpoints are [regular singular points](../../complex-analysis.md#regular-singular-point).

Insert $y_q=\sum_{n\geq0}a_nx^{n+q}$ and equate coefficients. The [recurrence relation](../../sequence-and-series.md#recurrence-relation) is

$$
\boxed{a_{n+2}=\frac{(n+q)^2-p^2}{(n+q+2)(n+q+1)}a_n,\qquad q=0,1.}
$$

Explicitly the factors are $(n^2-p^2)/[(n+2)(n+1)]$ for $q=0$ and $[(n+1)^2-p^2]/[(n+3)(n+2)]$ for $q=1$. The lowest equation for $q=1$ forces $a_1=0$. For $q=0$, one may choose $a_1=0$ to select an even solution, independent of the odd $q=1$ solution. The leading coefficient $a_0$ is free in either chosen parity branch.

For a nonterminating branch the consecutive parity-term ratio tends to $x^2$. Hence the [ratio test](../../sequence-and-series.md#ratio-test) gives convergence for $|x|<1$, and [radius of convergence](../../sequence-and-series.md#radius-of-convergence) one. Terminating branches are [polynomials](../../polynomial.md) with infinite radius. For $p=m\geq0$ an integer, choose $q$ of the same parity as $m$: the recurrence stops once $n+q=m$, producing a degree-$m$ [Chebyshev polynomial](../../numerical-analysis.md#chebyshev-polynomial). Normalization at $1$ gives all nonzero coefficients through degree three:

$$
\boxed{T_0=1,\qquad T_1=x,\qquad T_2=2x^2-1,\qquad T_3=4x^3-3x.}
$$

Set $Y(\theta)=y(\cos\theta)$. Direct [differentiation](../../calculus.md#differentiation) gives $Y''=\sin^2\theta\,y''-\cos\theta\,y'$, so the equation becomes $Y''+m^2Y=0$. For $m>0$, $Y=A\cos(m\theta)+B\sin(m\theta)$. A [polynomial](../../polynomial.md) $y$ has finite [derivative](../../calculus.md#derivative) at $x=1$, and therefore $Y'(0)=-\sin0\,y'(1)=0$, forcing $B=0$. Also $Y(0)=T_m(1)=1$, so $A=1$. For $m=0$, the transformed solution is affine in $\theta$ and the same [derivative](../../calculus.md#derivative) condition removes its linear term. Thus

$$
\boxed{T_m(x)=\cos(m\arccos x),\qquad -1\leq x\leq1,\quad m=0,1,2,\ldots.}
$$

The endpoint values follow by continuity. The finite-derivative condition is what excludes the independent nonpolynomial branch, rather than normalization alone.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

For fixed endpoint values, the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is $f_y-df_{y'}/dx=0$. Along a stationary curve, the [chain rule](../../calculus.md#chain-rule) gives

$$
\frac{d}{dx}(y'f_{y'}-f)=y'\left(\frac{df_{y'}}{dx}-f_y\right)-f_x.
$$

When $f_x=0$, the [Beltrami identity](../../analysis.md#beltrami-identity) therefore takes the requested sign convention

$$
\boxed{y'f_{y'}-f=A.}
$$

By [Fermat principle](../../mathematical-physics.md#fermat-principle), the elapsed-time integrand for the given speed is $f=c_0^{-1}\sqrt{1-ky}\sqrt{1+(y')^2}$. Thus

$$
y'f_{y'}-f=-\frac{\sqrt{1-ky}}{c_0\sqrt{1+(y')^2}}=A.
$$

The constant is negative for a finite regular ray. Squaring gives $(1-ky)/(1+(y')^2)=c_0^2A^2$. At a maximum height $y_0$, the slope is zero, so $c_0^2A^2=1-ky_0>0$. Hence

$$
(y')^2=\frac{k(y_0-y)}{1-ky_0}.
$$

Separate variables on either side of the turning point. Integration gives the [parabolic light rays in a reciprocal-square-root speed profile](../../mathematical-physics.md#parabolic-light-rays-in-a-reciprocal-square-root-speed-profile)

$$
\boxed{y(x)=y_0-\frac{k(x-x_c)^2}{4(1-ky_0)}.}
$$

The quadratic opens downwards, with its greatest height $y_0$ at $x=x_c$. The positive index condition holds throughout the layer because $kh<1$. Vertical rays are a separate zero-horizontal-momentum case, outside the regular graph representation $y(x)$; they are not returning rays of the type considered below.

Equal endpoint heights at $x=\pm x_0$ force $x_c=0$. Setting $y(\pm x_0)=0$ gives

$$
\boxed{(kx_0)^2=4ky_0(1-ky_0).}
$$

For nonzero separation, a real returning ray requires $kx_0\leq1$ and has candidate turning heights

$$
\boxed{y_0=\frac{1\pm\sqrt{1-k^2x_0^2}}{2k}.}
$$

Only choices satisfying $0<y_0<h$ are rays wholly within the specified layer. Depending on its thickness there may be two, one, or no admissible choices; at zero discriminant the two algebraic candidates coincide. The entry and exit points at $y=0$ are interpreted as limiting boundary points of the open medium.

<a id="9/image-two-possible-returning-parabolic-rays-subject-to-the-optical-layer-height"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1-q9-parabolic-rays.png)

**[Figure 1](#9/image-two-possible-returning-parabolic-rays-subject-to-the-optical-layer-height). Two possible returning parabolic rays, subject to the optical layer height**.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

Use the real [weighted inner product](../../inner-product.md#weighted-inner-product) $\langle u,v\rangle_w=\int_a^bwuv\,dx$ and the energy bilinear form $B(u,v)=\int_a^b(pu'v'+quv)dx$. [Integration by parts](../../calculus.md#integration-by-parts), the endpoint conditions, and the [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem) give

$$
B(y_i,y_j)=\int_a^by_i[-(py_j')'+qy_j]dx=\lambda_j\langle y_i,y_j\rangle_w=\lambda_j\delta_{ij}.
$$

Thus [orthonormality](../../inner-product.md#orthonormal-set) in the stated expansion gives

$$
F[y_{\rm trial}]=A^2\left(\lambda_0+\sum_{i\geq1}c_i^2\lambda_i\right),\qquad G[y_{\rm trial}]=A^2\left(1+\sum_{i\geq1}c_i^2\right),
$$

and hence the [Rayleigh quotient](../../linear-operator-theory.md#rayleigh-quotient)

$$
\boxed{\lambda_{\rm trial}=\frac{\lambda_0+\sum_{i\geq1}c_i^2\lambda_i}{1+\sum_{i\geq1}c_i^2}.}
$$

The expansion is understood for nonzero admissible functions with finite norm and energy.

For a general endpoint-preserving variation $y+\varepsilon\eta$, explicitly

$$
\delta F=2\int_a^b[-(py')'+qy]\eta\,dx,\qquad\delta G=2\int_a^bwy\eta\,dx,
$$

so

$$
\delta\Lambda=\frac{\delta F-\Lambda\delta G}{G}=\frac2G\int_a^b[-(py')'+qy-\Lambda wy]\eta\,dx.
$$

The [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) shows that stationarity is exactly the [eigenvalue](../../linear-operator-theory.md#eigenvalue) equation with $\lambda=\Lambda$. Conversely an [eigenfunction](../../linear-operator-theory.md#eigenfunction) has vanishing first variation and quotient equal to its [eigenvalue](../../linear-operator-theory.md#eigenvalue). Completeness gives the same weighted-average formula for any nonzero admissible expansion, even one with zero ground-state coefficient. Since every $\lambda_i\geq\lambda_0$,

$$
\boxed{\Lambda[y]\geq\lambda_0.}
$$

This is the [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle).

For the interval problem, the normalized [Dirichlet eigenfunctions](../../linear-operator-theory.md#dirichlet-eigenfunction) and their [eigenvalues](../../linear-operator-theory.md#eigenvalue), with the paper's zero-based indexing, are

$$
y_i(x)=\sqrt2\sin[(i+1)\pi x],\qquad\lambda_i=(i+1)^2\pi^2.
$$

For $u=x(1-x)$, direct integration gives $F=\int_0^1(1-2x)^2dx=1/3$ and $G=\int_0^1x^2(1-x)^2dx=1/30$. Therefore

$$
\boxed{\lambda_{\rm trial}=10>\lambda_0=\pi^2.}
$$

The [sine expansion and Rayleigh quotient of a parabolic Dirichlet trial](../../fourier-series.md#sine-expansion-and-rayleigh-quotient-of-a-parabolic-dirichlet-trial) follow from the coefficient integral

$$
\int_0^1x(1-x)y_i(x)dx=\frac{2\sqrt2[1-(-1)^{i+1}]}{(i+1)^3\pi^3}.
$$

Consequently the requested expansion has

$$
\boxed{A=\frac{4\sqrt2}{\pi^3},\qquad c_i=\frac{1-(-1)^{i+1}}{2(i+1)^3}.}
$$

Equivalently $u=(8/\pi^3)\sum_{n\geq1,\ n\text{ odd}}\sin(n\pi x)/n^3$. In particular $c_1=0$: the first excited [eigenfunction](../../linear-operator-theory.md#eigenfunction) $\sqrt2\sin(2\pi x)$ is antisymmetric about $1/2$, whereas the trial function is symmetric. Since $10-\pi^2>0$, the final ratio is exactly

$$
\boxed{\frac{c_1^2(\lambda_1-\lambda_0)}{\lambda_{\rm trial}-\lambda_0}=0.}
$$

The first nonzero correction is $c_2=1/27$, not $c_1$. Reindexing only the nonzero terms would change the meaning of the requested ratio and is not used here.

## ↑ Ancestors (10)

1. [2010](../2010.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
