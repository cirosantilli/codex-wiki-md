# Paper 1

↑ **Parent:** [2011](../2011.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2011/PaperNST_IB_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2011/PaperNST_IB_1.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a twice continuously differentiable [vector field](../../multivariable-calculus.md#vector-field) in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system), the [curl](../../multivariable-calculus.md#curl) and [divergence](../../multivariable-calculus.md#divergence) are

$$
\nabla\times\mathbf v=(\partial_yv_z-\partial_zv_y,\ \partial_zv_x-\partial_xv_z,\ \partial_xv_y-\partial_yv_x),\qquad\nabla\cdot\mathbf v=\partial_xv_x+\partial_yv_y+\partial_zv_z.
$$

Put $\boldsymbol\omega=\nabla\times\mathbf v$. Using the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol), the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta) contraction and the [product rule](../../calculus.md#product-rule),

$$
\begin{aligned}
[\nabla\times(\mathbf v\times\boldsymbol\omega)]_i
&=\partial_j(v_i\omega_j-v_j\omega_i)\\
&=\omega_j\partial_jv_i-v_j\partial_j\omega_i-\omega_i\partial_jv_j+v_i\partial_j\omega_j.
\end{aligned}
$$

The last term vanishes because the [divergence of a curl is zero](../../multivariable-calculus.md#divergence-of-a-curl-is-zero): the symmetric mixed derivatives contract against an antisymmetric symbol. Thus the [curl of a cross product](../../multivariable-calculus.md#curl-of-a-cross-product) identity becomes

$$
\boxed{\nabla\times(\mathbf v\times\boldsymbol\omega)=(\boldsymbol\omega\cdot\nabla)\mathbf v-(\mathbf v\cdot\nabla)\boldsymbol\omega-\boldsymbol\omega(\nabla\cdot\mathbf v).}
$$

For [orthogonal coordinates](../../multivariable-calculus.md#orthogonal-coordinates) $q_i$ with [position vector](../../classical-mechanics.md#position-vector) $\mathbf r(q_1,q_2,q_3)$, the [scale factors of orthogonal coordinates](../../multivariable-calculus.md#scale-factors-of-orthogonal-coordinates) and local [unit vectors](../../vector-space.md#unit-vector) are

$$
h_i=\left|\frac{\partial\mathbf r}{\partial q_i}\right|,\qquad\mathbf e_i=\frac1{h_i}\frac{\partial\mathbf r}{\partial q_i},\qquad d\mathbf r=\sum_i h_i\mathbf e_i\,dq_i.
$$

Orthogonality gives $ds^2=\sum_i h_i^2dq_i^2$, and right-handedness fixes $\mathbf e_1\times\mathbf e_2=\mathbf e_3$. In [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system), $\mathbf r=(\rho\cos\phi,\rho\sin\phi,z)$, so

$$
\boxed{h_\rho=1,\quad h_\phi=\rho,\quad h_z=1,\qquad \mathbf e_\rho=(\cos\phi,\sin\phi,0),\quad\mathbf e_\phi=(-\sin\phi,\cos\phi,0),\quad\mathbf e_z=(0,0,1).}
$$

The radial vector points away from the axis; the azimuthal vector is tangent in the direction of increasing $\phi$; $\mathbf e_z$ is the Cartesian positive $z$ direction. The azimuthal basis is undefined on the coordinate axis itself.

<a id="1/image-cylindrical-unit-vectors-relative-to-cartesian-axes-viewed-from-positive-z"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1-q1-cylindrical-basis.png)

**[Figure 1](#1/image-cylindrical-unit-vectors-relative-to-cartesian-axes-viewed-from-positive-z). Cylindrical unit vectors relative to Cartesian axes, viewed from positive z**.

For the axial velocity profile, the [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system) formula gives

$$
\boxed{\boldsymbol\omega=\nabla\times\mathbf u=-\partial_\rho u_z\,\mathbf e_\phi=2u_0\rho\,\mathbf e_\phi.}
$$

The associated [cross product](../../vector-space.md#cross-product) is

$$
\boxed{\mathbf u\times\boldsymbol\omega=-2u_0^2\rho(1-\rho^2)\mathbf e_\rho.}
$$

This field has only a radial component depending on $\rho$, so its [curl](../../multivariable-calculus.md#curl) is zero. Also $\nabla\cdot\mathbf u=\partial_z u_z=0$. The identity above therefore yields

$$
\boxed{(\boldsymbol\omega\cdot\nabla)\mathbf u=(\mathbf u\cdot\nabla)\boldsymbol\omega.}
$$

In fact both [directional derivatives](../../multivariable-calculus.md#directional-derivative) vanish: the first differentiates $u_z\mathbf e_z$ only in the azimuthal direction, and the second differentiates $\boldsymbol\omega$ only in the $z$ direction. All physical vector fields extend smoothly through $\rho=0$, despite the coordinate-basis singularity.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The substitution separates the uniform equilibrium from the decaying perturbation. Direct [differentiation](../../calculus.md#differentiation) gives

$$
u_t=e^{-\beta t}(v_t-\beta v),\qquad u_{xx}=e^{-\beta t}v_{xx},\qquad\beta(u-u_0)=\beta e^{-\beta t}v.
$$

Consequently the [reaction-diffusion equation](../../diffusion-equation.md#reaction-diffusion-system) reduces to the [heat equation](../../diffusion-equation.md#heat-equation) $v_t=v_{xx}$. Its data become

$$
\boxed{v(0,t)=e^{\beta t}(u_1-u_0),\quad v(\pi,t)=e^{\beta t}(u_2-u_0),\quad v(x,0)=f(x)-u_0.}
$$

When the three constants coincide, the [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition) for $v$ are homogeneous. [Separation of variables](../../partial-differential-equation.md#separation-of-variables) gives $X''+n^2X=0$ and $T'=-n^2T$, selecting the [normal modes](../../wave-equation.md#normal-mode) $\sin(nx)e^{-n^2t}$ for $n\geq1$. Thus

$$
v(x,t)=\sum_{n=1}^\infty b_n\sin(nx)e^{-n^2t},\qquad b_n=\frac2\pi\int_0^\pi[x(\pi-x)-u_0]\sin(nx)\,dx.
$$

Two [integrations by parts](../../calculus.md#integration-by-parts) give $\int_0^\pi x(\pi-x)\sin(nx)dx=2[1-(-1)^n]/n^3$, while the constant term uses $\int_0^\pi\sin(nx)dx=[1-(-1)^n]/n$. Therefore the [Fourier sine series](../../fourier-series.md#fourier-sine-series) is

$$
\boxed{v(x,t)=\frac4\pi\sum_{\substack{n\geq1\\n\text{ odd}}}\left(\frac2{n^3}-\frac{u_0}n\right)e^{-n^2t}\sin(nx).}
$$

For $u_0\ne2$, its first coefficient is nonzero. Multiplying by $e^{-\beta t}$ and retaining the slowest-decaying mode gives

$$
\boxed{u(x,t)=u_0-\frac4\pi(u_0-2)e^{-(\beta+1)t}\sin x+O(e^{-(\beta+9)t})\quad(t\to\infty).}
$$

The remainder estimate holds uniformly in $x$ for sufficiently large positive time. If $u_0=2$, the fundamental vanishes and the next possible mode has decay rate $\beta+9$, explaining the exclusion.

There is an initial endpoint compatibility issue unless $u_0=0$: the given polynomial profile vanishes at the endpoints, whereas the boundary values equal $u_0$. The series realizes the initial data in [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space) and pointwise in the open interval, imposing the prescribed boundary values for $t>0$. For nonzero $u_0$ it cannot also be continuous at both initial endpoint corners.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Trying $y=x^m$ in the [Cauchy-Euler equation](../../linear-ordinary-differential-equation.md#cauchy-euler-equation) gives

$$
m(m-1)+4m-4=(m-1)(m+4)=0,
$$

so the [homogeneous solution](../../linear-ordinary-differential-equation.md#homogeneous-solution) is

$$
\boxed{y=C_1x+C_2x^{-4}.}
$$

Continuity with zero value at the singular endpoint excludes the second branch. Use the left and right adapted solutions $\ell(x)=x$, $r(x)=x^{-4}-x$, whose [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is

$$
W(x)=\ell r'-\ell'r=-5x^{-4}.
$$

The [Dirichlet Green kernel for an Euler operator with exponents one and minus four](../../green-s-function.md#dirichlet-green-kernel-for-an-euler-operator-with-exponents-one-and-minus-four) is therefore

$$
\boxed{G(x,\xi)=\frac15\begin{cases}x(\xi^5-1),&x\leq\xi,\\\xi^5(x-x^{-4}),&x\geq\xi.\end{cases}}
$$

It vanishes at both endpoints, is continuous at $x=\xi$, and has first-derivative jump

$$
G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=\frac{\ell(\xi)r'(\xi)-\ell'(\xi)r(\xi)}{W(\xi)}=1.
$$

Thus $L_xG=\delta(x-\xi)$ with ordinary source measure $d\xi$. For bounded forcing the [Green function](../../green-s-function.md) representation is

$$
\boxed{u(x)=\frac{x-x^{-4}}5\int_0^x\xi^5f(\xi)d\xi+\frac x5\int_x^1(\xi^5-1)f(\xi)d\xi.}
$$

The apparent singular prefactor in the first term is canceled by the integral's decay at zero. The only regular homogeneous solution vanishing at $1$ is zero, so this solution is unique in the stated regular class.

For the piecewise source, split the integrals at $1/2$. If $x<1/2$, the needed integrals are $\int_0^x\xi^6d\xi=x^7/7$ and $\int_x^{1/2}(\xi^6-\xi)d\xi$. If $x>1/2$, only $\int_0^{1/2}\xi^6d\xi=1/896$ remains. Simplification yields

$$
\boxed{u(x)=\begin{cases}\displaystyle\frac{x^3}{14}-\frac{111x}{4480},&0\leq x\leq\frac12,\\\displaystyle\frac{x-x^{-4}}{4480},&\frac12\leq x\leq1.\end{cases}}
$$

At the interface both expressions have value $-31/8960$ and derivative $129/4480$, so no unintended [Dirac delta](../../distribution-theory.md#dirac-delta-function) source appears. Their second derivatives have the allowed jump associated with the discontinuous forcing.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

With the stated [Fourier transform](../../fourier-transform.md) convention, the [inverse Fourier transform](../../fourier-transform.md#inverse-fourier-transform) and the deterministic [autocorrelation of a square-integrable function](../../fourier-analysis.md#autocorrelation-of-a-square-integrable-function) are

$$
\boxed{f(x)=\frac1{2\pi}\int_{\mathbb R}\widetilde f(k)e^{ikx}dk,\qquad h(x)=\int_{\mathbb R}\overline{f(y)}f(x+y)dy.}
$$

Assume initially sufficient decay and smoothness, for example a [Schwartz function](../../fourier-analysis.md#schwartz-function), to justify interchanging integrations and [Fourier inversion](../../fourier-analysis.md#fourier-inversion-theorem). With $s=x+y$, the [cross-correlation](../../fourier-analysis.md#cross-correlation) identity is

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}\overline{f(y)}f(x+y)dy\,dx\\
&=\left[\int_{\mathbb R}e^{iky}\overline{f(y)}dy\right]\left[\int_{\mathbb R}e^{-iks}f(s)ds\right]=|\widetilde f(k)|^2.
\end{aligned}
$$

Evaluating $h$ directly and by its inverse transform at zero proves the [Parseval identity](../../fourier-analysis.md#parseval-identity):

$$
\boxed{\int_{\mathbb R}|f(x)|^2dx=h(0)=\frac1{2\pi}\int_{\mathbb R}|\widetilde f(k)|^2dk.}
$$

Approximation extends the identity to [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space), as the [Plancherel theorem](../../fourier-analysis.md#plancherel-theorem).

For the compact cosine profile, the [Fourier transform of a truncated cosine](../../fourier-transform.md#fourier-transform-of-a-truncated-cosine) follows from $\cos x=(e^{ix}+e^{-ix})/2$:

$$
\begin{aligned}
\widetilde f(k)&=\frac{\sin[(k-1)\pi/2]}{k-1}+\frac{\sin[(k+1)\pi/2]}{k+1}\\
&=\boxed{\frac{2\cos(k\pi/2)}{1-k^2}}.
\end{aligned}
$$

At $k=\pm1$ the apparent singularities are removable, with value $\pi/2$. The direct squared norm is $\int_{-\pi/2}^{\pi/2}\cos^2x\,dx=\pi/2$. Hence [Parseval identity](../../fourier-analysis.md#parseval-identity) and evenness give

$$
\int_0^\infty\frac{\cos^2(k\pi/2)}{(1-k^2)^2}dk=\frac{\pi^2}{8}.
$$

Putting $t=\pi k/2$ makes the left side $\pi^3/8$ times the requested integral. Therefore

$$
\boxed{\int_0^\infty\frac{\cos^2t}{(\pi^2/4-t^2)^2}dt=\frac1\pi.}
$$

At $t=\pi/2$ the integrand's continuous extension is $1/\pi^2$, so no principal-value prescription is required.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A square [matrix](../../vector-space.md#matrix) is invertible precisely when its [determinant](../../multilinear-algebra.md#determinant) is nonzero. Equivalent conditions are full [rank](../../quadratic-form.md#rank-one-quadratic-form), a trivial [kernel](../../kernel-of-a-linear-map.md), and zero not being an [eigenvalue](../../linear-operator-theory.md#eigenvalue).

For a lower [triangular matrix](../../linear-algebra.md#triangular-matrix), the first row has only the possibly nonzero entry $A_{11}$. A [Laplace expansion](../../multilinear-algebra.md#laplace-expansion) along that row gives $\det A=A_{11}\det A^{(1)}$, where the remaining principal submatrix is again lower triangular. Induction from the one-by-one case yields

$$
\boxed{\det A=\prod_{j=1}^nA_{jj}.}
$$

This proof includes singular triangular matrices; it makes no division by diagonal entries.

For the diagonal example, put $N=n(n+1)/2$. Its [determinant](../../multilinear-algebra.md#determinant) is $b^{1+2+\cdots+n}=b^N$, and invertibility requires $b\ne0$. Write the [complex number](../../complex-analysis.md#complex-number) as $b=re^{i\theta}$ with $r>0$. A nonzero purely imaginary determinant requires $\cos(N\theta)=0$. Thus

$$
\boxed{b=r\exp\left[\frac{(2m+1)\pi i}{n(n+1)}\right],\qquad r>0,\quad m\in\mathbb Z.}
$$

Equivalently $b^N\in i\mathbb R\setminus\{0\}$; the angle is understood modulo $2\pi$.

For [skew-Hermitian matrices](../../linear-operator-theory.md#skew-hermitian-matrix), reversing products under the [conjugate transpose](../../linear-operator-theory.md#conjugate-transpose) gives $(CD)^\dagger=D^\dagger C^\dagger=DC$. Consequently

$$
\boxed{CD\text{ is skew-Hermitian}\ \Longleftrightarrow\ DC=-CD\ \Longleftrightarrow\ CD+DC=0.}
$$

The latter condition is vanishing of the [anticommutator](../../vector-space.md#anticommutator). A universal choice for the last request is

$$
\boxed{\alpha=-1,\qquad CD-DC=[C,D].}
$$

Indeed $(CD-DC)^\dagger=DC-CD=-(CD-DC)$, so the [commutator](../../lie-algebra.md#commutator) of two skew-Hermitian matrices is skew-Hermitian.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Over the chosen scalar field, an $n$-by-$n$ [matrix](../../vector-space.md#matrix) is [diagonalizable](../../linear-operator-theory.md#diagonalizable-matrix) if and only if it has $n$ [linearly independent](../../vector-space.md#linear-independence) [eigenvectors](../../linear-operator-theory.md#eigenvector). Repeated eigenvalues are allowed provided all [eigenspaces](../../linear-operator-theory.md#eigenspace) together supply a basis.

For the given matrix, the [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $\lambda^2-4\lambda-5=(\lambda-5)(\lambda+1)$. One may choose

$$
\boxed{\lambda_1=5,\quad V_1=\begin{pmatrix}5\\1\end{pmatrix},\qquad\lambda_2=-1,\quad V_2=\begin{pmatrix}-1\\1\end{pmatrix}.}
$$

Taking these as columns gives the [change of basis](../../linear-algebra.md#change-of-basis)

$$
\boxed{P=\begin{pmatrix}5&-1\\1&1\end{pmatrix},\qquad P^{-1}=\frac16\begin{pmatrix}1&1\\-1&5\end{pmatrix},\qquad P^{-1}AP=\begin{pmatrix}5&0\\0&-1\end{pmatrix}.}
$$

**This is not a rotation matrix.** The PDF's terminology cannot hold literally: $A$ is real and nonsymmetric, whereas a real matrix orthogonally similar to a real diagonal matrix is symmetric. Also $V_1\cdot V_2=-4\ne0$, so scaling these eigenvectors cannot make an orthonormal rotation basis. A general invertible similarity is the valid construction.

Let $D=P^{-1}AP$. Inserting $PP^{-1}$ between successive factors gives $A^n=PD^nP^{-1}$, and hence

$$
\boxed{P^{-1}A^nP=\operatorname{diag}(5^n,(-1)^n).}
$$

To write $A^n=\alpha_nA+\beta_nI$, match its action on the two eigenspaces:

$$
5\alpha_n+\beta_n=5^n,\qquad-\alpha_n+\beta_n=(-1)^n.
$$

Solving gives the [matrix powers for a diagonalizable matrix with two eigenvalues](../../vector-space.md#matrix-powers-for-a-diagonalizable-matrix-with-two-eigenvalues)

$$
\boxed{A^n=\frac{5^n+(-1)^{n+1}}6A+\frac{5^n+5(-1)^n}6I,\qquad n\geq0.}
$$

The cases $n=0,1$ recover $I,A$, respectively. Equivalently the [spectral projections of a diagonalizable matrix](../../linear-operator-theory.md#spectral-projection-of-a-diagonalizable-matrix) are $(A+I)/6$ and $(5I-A)/6$, and the power multiplies them by $5^n$ and $(-1)^n$.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

The [Cauchy-Riemann equations](../../analysis.md#cauchy-riemann-equations) are $u_x=v_y$ and $u_y=-v_x$. A [holomorphic function](../../holomorphic-function.md) is smooth, so equality of mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative) gives

$$
\boxed{\Delta u=(v_y)_x-(v_x)_y=0,\qquad\Delta v=-(u_y)_x+(u_x)_y=0.}
$$

Thus its real and imaginary parts are [harmonic functions](../../partial-differential-equation.md#harmonic-function).

An [entire function](../../holomorphic-function.md#entire-function) is holomorphic at every finite point of the complex plane. The globally convergent [power series](../../sequence-and-series.md#power-series) for the exponential implies that $e^z$ and $e^{-z}$ are entire. Their difference therefore gives

$$
\sinh z=\frac{e^z-e^{-z}}2,\qquad (\sinh z)'=\cosh z
$$

at every complex $z$, proving that the [hyperbolic sine](../../calculus.md#hyperbolic-sine) is entire. For powers, the base case $f_1(z)=z$ has derivative one everywhere. If $z^n$ is entire with derivative $nz^{n-1}$, the [product rule](../../calculus.md#product-rule) gives $(z^{n+1})'=z^n+z\,nz^{n-1}=(n+1)z^n$ everywhere. Induction proves that every positive integer power is entire.

A function has a [pole](../../isolated-singularity.md#pole) of order $n$ at $z_0$ when it is holomorphic in a punctured neighbourhood and $g(z)=(z-z_0)^nf(z)$ extends holomorphically to $z_0$ with $g(z_0)\ne0$. An isolated [essential singularity](../../isolated-singularity.md#essential-singularity) is neither a removable singularity nor a pole; equivalently its [Laurent series](../../analysis.md#laurent-series) has infinitely many nonzero negative-power terms. In particular

$$
e^{1/z}=\sum_{m=0}^\infty\frac{z^{-m}}{m!},\qquad 0<|z|<\infty,
$$

has an essential singularity at zero.

For $f_N$, the [Laurent series](../../analysis.md#laurent-series) about infinity is

$$
\boxed{f_N(z)=\sum_{m=0}^\infty\frac{z^{N-m}}{m!}=z^N+z^{N-1}+\frac{z^{N-2}}{2!}+\cdots+\frac1{N!}+\frac{z^{-1}}{(N+1)!}+\cdots.}
$$

To classify the point correctly, use $w=1/z$. Then $f_N(1/w)=w^{-N}e^w$, and $e^w$ is holomorphic with value one at zero. Therefore

$$
\boxed{f_N\text{ has a pole of order }N\text{ at infinity}.}
$$

The [pole at infinity](../../isolated-singularity.md#pole-at-infinity) is compatible with an essential singularity at the finite point zero. Negative powers of $z$ are regular powers of the local coordinate $w$ near infinity, so they do not make that point essential.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

Write a second-order [linear ordinary differential equation](../../linear-ordinary-differential-equation.md) in monic form $y''+P(x)y'+Q(x)y=0$. At a finite point $x_0$, an [ordinary point](../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) has analytic $P,Q$. A singular point is a [regular singular point](../../complex-analysis.md#regular-singular-point) if $(x-x_0)P$ and $(x-x_0)^2Q$ extend analytically there. A singular point failing this condition is an [irregular singular point](../../complex-analysis.md#irregular-singular-point). The point at infinity is classified by the reciprocal coordinate $t=1/x$.

For the [Laguerre differential equation](../../linear-ordinary-differential-equation.md#laguerre-differential-equation), $P=1/x-1$ and $Q=\nu/x$. Thus $xP=1-x$ and $x^2Q=\nu x$ are analytic at zero, while $P$ itself is singular: zero is regular singular. Put $Y(t)=y(1/t)$. Since $y'=-t^2Y'$ and $y''=t^4Y''+2t^3Y'$, the transformed equation is

$$
Y''+\left(\frac1t+\frac1{t^2}\right)Y'+\frac\nu{t^3}Y=0.
$$

Here $tP_t=1+1/t$ is not analytic at zero, so **infinity is an irregular singular point**, for every real $\nu$.

For the [Frobenius solution](../../complex-analysis.md#frobenius-solution), the lowest power $x^{\sigma-1}$ has coefficient $a_0\sigma^2$. Hence the [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) is $\sigma^2=0$, and equating the remaining powers gives

$$
(k+1+\sigma)^2a_{k+1}+(\nu-k-\sigma)a_k=0.
$$

With the repeated root $\sigma=0$, the [Frobenius series for the Laguerre differential equation](../../linear-ordinary-differential-equation.md#frobenius-series-for-the-laguerre-differential-equation) obeys

$$
\boxed{a_{k+1}=\frac{k-\nu}{(k+1)^2}a_k.}
$$

If the series does not terminate, its consecutive term ratio is asymptotic to $x/k$, so the [ratio test](../../sequence-and-series.md#ratio-test) gives infinite [radius of convergence](../../sequence-and-series.md#radius-of-convergence). It is an [entire function](../../holomorphic-function.md#entire-function), even though the differential equation has a singular coefficient at zero. The repeated indicial root yields only one analytic Frobenius branch; an independent solution generally has a logarithmic term there.

For $\nu=n\geq0$, the factor $k-n$ stops the recurrence at degree $n$. With $a_0=1$ its coefficients are $a_k=(-1)^k\binom nk/k!$, giving the [Laguerre polynomials](../../linear-operator-theory.md#laguerre-polynomial)

$$
\boxed{L_0=1,\qquad L_1=1-x,\qquad L_2=1-2x+\frac{x^2}{2},\qquad L_3=1-3x+\frac{3x^2}{2}-\frac{x^3}{6}.}
$$

The same termination argument includes $n=0$, as required for $L_0$ despite the earlier reference to positive integers.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

For endpoint-preserving variations of a [functional](../../calculus-of-variations.md#functional), the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is

$$
\boxed{F_y-\frac{d}{dx}F_{y'}=0.}
$$

Along an extremal, the [chain rule](../../calculus.md#chain-rule) gives $d(F-y'F_{y'})/dx=F_x+y'[F_y-dF_{y'}/dx]=F_x$. Thus when $F$ has no explicit $x$ dependence, the [Beltrami identity](../../analysis.md#beltrami-identity) is

$$
\boxed{F-y'F_{y'}=A.}
$$

For a positive speed profile, the elapsed-time integrand in [Fermat principle](../../mathematical-physics.md#fermat-principle) is $F=\sqrt{1+(y')^2}/c(y)$. Its first integral gives

$$
\frac1{c(y)\sqrt{1+(y')^2}}=A>0,\qquad\frac{dx}{dy}=\pm\frac{Ac(y)}{\sqrt{1-A^2c(y)^2}}.
$$

Integrating each monotone-height branch yields

$$
\boxed{\int^y\frac{Ac(\widehat y)}{\sqrt{1-A^2c(\widehat y)^2}}d\widehat y=\pm(x+B).}
$$

Real branches require $Ac(y)\leq1$. Turning points are joined in the original graph $y(x)$, even though the inverse derivative is singular there.

For the inverse-height speed profile, this becomes $dx/dy=\pm a/\sqrt{y^2-a^2}$, with $a=A>0$. Integration gives $x-b=\pm a\operatorname{arcosh}(y/a)$, so the [light rays](../../geometrical-optics.md#light-ray) are [catenaries](../../analysis.md#catenary)

$$
y(x)=a\cosh\frac{x-b}{a}.
$$

Equal endpoint heights at opposite $x$ values force $b=0$, since the real hyperbolic cosine is even and strictly increases with the absolute value of its argument. The remaining endpoint condition is $a\cosh(1/a)=\cosh1$. One exact solution is $a=1$, giving

$$
\boxed{y(x)=\cosh x,\qquad y_{\min}=1,\qquad T=\int_{-1}^1\cosh^2x\,dx=1+\frac12\sinh2\simeq2.813430204.}
$$

Here $ds/dx=\cosh x$ and $1/c(y)=y=\cosh x$ account for the squared hyperbolic cosine in the time integral.

**The stated endpoints also allow a second stationary ray.** Set $t=1/a$. The function $\cosh t/t$ decreases and then increases: its derivative has the sign of $t\sinh t-\cosh t$, whose derivative is $t\cosh t>0$. Its unique minimum occurs where $t\tanh t=1$, at $t\simeq1.199679$. Since the known root $t=1$ lies below this minimum's location, there is exactly one further root, $t\simeq1.4242930655$. Thus the [two stationary catenary rays in an inverse-height speed profile](../../geometrical-optics.md#two-stationary-catenary-rays-in-an-inverse-height-speed-profile) also include

$$
\boxed{y(x)=a\cosh(x/a),\qquad a\simeq0.7021026952,\qquad y_{\min}=a,\qquad T=a+\frac{a^2}{2}\sinh\frac2a\simeq2.822449145.}
$$

No extra condition in the question selects uniquely between these rays. The minimum height is a minimum along the chosen ray, not a global travel-time assertion. Indeed, competitors descending vertically to height $\eta>0$, crossing horizontally, and rising again have time $\cosh^2(1)-\eta^2+2\eta$. As $\eta\downarrow0$ this tends to $\cosh^2(1)\simeq2.381098$, below both stationary times. Their corners can be smoothed, so [Fermat principle](../../mathematical-physics.md#fermat-principle) here must be understood as stationarity rather than unrestricted global minimization.

<a id="9/image-two-stationary-light-rays-through-the-same-endpoints-in-an-inverse-height-speed-profile"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1-q9-two-catenary-rays.png)

**[Figure 2](#9/image-two-stationary-light-rays-through-the-same-endpoints-in-an-inverse-height-speed-profile). Two stationary light rays through the same endpoints in an inverse-height speed profile**.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

Use a [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) $\mu$ for the norm constraint. For real variations $u+\delta\eta$ with $\eta(0)=\eta(\pi)=0$, [integration by parts](../../calculus.md#integration-by-parts) gives

$$
\begin{aligned}
\delta(F-\mu G)&=2\int_0^\pi[u'\eta'+(\epsilon x-\mu)u\eta]dx\\
&=2\int_0^\pi[-u''+(\epsilon x-\mu)u]\eta\,dx.
\end{aligned}
$$

Thus stationarity is equivalent to the [Sturm-Liouville problem](../../sturm-liouville-theory.md#sturm-liouville-problem)

$$
-u''+\epsilon xu=\mu u,\qquad u(0)=u(\pi)=0.
$$

Multiplying by $u$ and integrating shows $F[u]=\mu G[u]=\mu$, so the constrained stationary values are the [eigenvalues](../../linear-operator-theory.md#eigenvalue), and the normalized stationary functions are their [eigenfunctions](../../linear-operator-theory.md#eigenfunction). Conversely the eigenvalue equation makes the constrained first variation vanish. The [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator) has weight one.

For $\epsilon=0$, zero and negative eigenvalues yield no nonzero solution with both [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition). Positive eigenvalues have solutions $u=A\sin(\sqrt\lambda x)$ after the left condition, and the right condition gives $\sqrt\lambda=n$, $n\geq1$. Hence the lowest eigenpair is

$$
\boxed{\lambda_0=1,\qquad Y_1(x)=\sqrt{\frac2\pi}\sin x,}
$$

where the amplitude follows from $\int_0^\pi\sin^2x\,dx=\pi/2$.

The [Rayleigh-Ritz variational principle](../../linear-operator-theory.md#rayleigh-ritz-variational-principle) bounds the full lowest eigenvalue by $F[Y_1]$. Its derivative contribution is one. For the linear potential, reflection about $\pi/2$ gives

$$
\int_0^\pi x\sin^2x\,dx=\frac\pi2\int_0^\pi\sin^2x\,dx=\frac{\pi^2}{4}.
$$

Thus the [sine trial bound for a linear potential on an interval](../../linear-operator-theory.md#sine-trial-bound-for-a-linear-potential-on-an-interval) is

$$
\boxed{\lambda_\epsilon\leq1+\frac{\epsilon\pi}{2}.}
$$

For $\epsilon>0$ the bound is strict, since $-Y_1''+\epsilon xY_1=(1+\epsilon x)Y_1$ is not a constant multiple of $Y_1$. Also $\lambda_\epsilon\geq1$ by the [Poincaré inequality](../../sobolev-space.md#poincare-inequality) and the nonnegative potential. Equality in the upper bound holds at $\epsilon=0$.

## ↑ Ancestors (10)

1. [2011](../2011.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
