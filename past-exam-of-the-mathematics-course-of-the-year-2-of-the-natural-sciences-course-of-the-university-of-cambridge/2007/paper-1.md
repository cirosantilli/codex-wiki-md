# Paper 1

↑ **Parent:** [2007](../2007.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2007/PaperNST_IB_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2007/PaperNST_IB_1.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
    - [a](#1/ii/a)
      - [Solution](#1/ii/a/solution)
    - [b](#1/ii/b)
      - [Solution](#1/ii/b/solution)
    - [c](#1/ii/c)
      - [Solution](#1/ii/c/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
- [7](#7)
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [Solution](#10/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Away from the origin, $\hat{\mathbf r}=\nabla r$. Hence the [curl of a gradient](../../multivariable-calculus.md#curl-of-a-gradient) gives $\nabla\times\hat{\mathbf r}=\mathbf0$. Its [divergence](../../multivariable-calculus.md#divergence) is the [Laplacian](../../multivariable-calculus.md#laplacian) of the radial coordinate, which in [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system) is

$$
\boxed{\nabla\cdot\hat{\mathbf r}=\nabla^2r=\frac1{r^2}\frac{d}{dr}(r^2)=\frac2r,\qquad r>0.}
$$

Equivalently, differentiating $x_i/r$ in [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system) gives $3/r-r^2/r^3=2/r$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Use the right-handed orthonormal basis $(\mathbf e_r,\mathbf e_\theta,\mathbf e_\phi)$. The [cross product](../../vector-space.md#cross-product) with $\mathbf e_r$ rotates tangential components by a right angle; taking its [cross product](../../vector-space.md#cross-product) again in the opposite order projects a [gradient](../../multivariable-calculus.md#gradient) onto the tangent plane. The [radial curl of angular gradient fields](../../riemannian-geometry.md#radial-curl-of-angular-gradient-fields) then depends only on the rotated-gradient part. All coordinate calculations are made away from the polar coordinate singularities and extend wherever the original fields are smooth.

<h4 id="1/ii/a">a</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#1/ii/a)

Since $\hat{\mathbf r}=\mathbf e_r$, the [gradient](../../multivariable-calculus.md#gradient) formula gives

$$
\mathbf e_r\times\nabla F=-\frac{F_\phi}{r\sin\theta}\mathbf e_\theta+\frac{F_\theta}{r}\mathbf e_\phi.
$$

The [vector triple product identity](../../multivariable-calculus.md#vector-triple-product) gives $(\mathbf e_r\times\nabla G)\times\mathbf e_r=\nabla G-\mathbf e_rG_r=(G_\theta/r)\mathbf e_\theta+[G_\phi/(r\sin\theta)]\mathbf e_\phi$. Adding the radial part yields

$$
\mathbf f=R\mathbf e_r+\frac1r\left(G_\theta-\frac{F_\phi}{\sin\theta}\right)\mathbf e_\theta+\frac1r\left(\frac{G_\phi}{\sin\theta}+F_\theta\right)\mathbf e_\phi.
$$

<h4 id="1/ii/b">b</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#1/ii/b)

The radial component of the [curl](../../multivariable-calculus.md#curl) in [spherical coordinates](../../multivariable-calculus.md#spherical-coordinate-system) is

$$
(\nabla\times\mathbf f)_r=\frac1{r\sin\theta}\left[\partial_\theta(\sin\theta f_\phi)-\partial_\phi f_\theta\right].
$$

It contains no $f_r$, so $R$ cannot contribute. Substituting the tangential components gives

$$
\partial_\theta(\sin\theta f_\phi)-\partial_\phi f_\theta=\frac1r\left[G_{\phi\theta}-G_{\theta\phi}+\partial_\theta(\sin\theta F_\theta)+\frac{F_{\phi\phi}}{\sin\theta}\right].
$$

The mixed [partial derivatives](../../multivariable-calculus.md#partial-derivative) of smooth $G$ agree, so its terms cancel. Multiplication by $r$, to take the [dot product](../../inner-product.md#dot-product) with the position [vector](../../vector-space.md#vector) $\mathbf r=r\mathbf e_r$, does not change this independence from $R,G$.

<h4 id="1/ii/c">c</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#1/ii/c)

The remaining terms give

$$
\boxed{(\nabla\times\mathbf f)\cdot\mathbf r=\frac1r\Delta_{\theta,\phi}F,\qquad\Delta_{\theta,\phi}=\frac1{\sin\theta}\partial_\theta(\sin\theta\,\partial_\theta)+\frac1{\sin^2\theta}\partial_\phi^2.}
$$

This is the [Laplace-Beltrami operator](../../differential-geometry.md#laplace-beltrami-operator) on the unit [sphere](../../euclidean-geometry.md#sphere). Taking the [dot product](../../inner-product.md#dot-product) with the unit radial [vector](../../vector-space.md#vector) instead would give $r^{-2}\Delta_{\theta,\phi}F$; the extra factor $r$ here comes from the position [vector](../../vector-space.md#vector) in the question.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

[Separation of variables](../../partial-differential-equation.md#separation-of-variables) gives $X''=-k^2X$ and $T'=-\kappa k^2T$. The periodic matching of both the [function](../../function.md) and its first [derivative](../../calculus.md#derivative) selects $k=n\pi/L$, with the constant mode at $n=0$. Thus the [periodic diffusion on a circle](../../diffusion-equation.md#periodic-diffusion-on-a-circle) solution is

$$
u(x,t)=\frac{a_0}{2}+\sum_{n=1}^{\infty}\left[a_n\cos\frac{n\pi x}{L}+b_n\sin\frac{n\pi x}{L}\right]e^{-\kappa(n\pi/L)^2t},
$$

where the [Fourier coefficients](../../fourier-series.md#fourier-coefficient) of the initial [function](../../function.md) are

$$
a_n=\frac1L\int_{-L}^Lu_0(x)\cos\frac{n\pi x}{L}\,dx,\qquad b_n=\frac1L\int_{-L}^Lu_0(x)\sin\frac{n\pi x}{L}\,dx.
$$

The formula for $a_n$ also gives $a_0$ at $n=0$. The constant mode preserves the initial spatial [mean](../../expected-value.md); every nonconstant [Fourier mode](../../fourier-analysis.md#fourier-mode) decays. For initial data in [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space), the series approaches those data in [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space) as $t\downarrow0$ and is smooth at positive times.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The initial [function](../../function.md) is [odd](../../calculus.md#odd-function), so all $a_n$, including $a_0$, vanish. Set $k_n=n\pi/L$. For $k_n\ne1$, product-to-sum and [integration by parts](../../calculus.md#integration-by-parts) give

$$
\int_0^L\sin x\sin(k_nx)\,dx=\frac{(-1)^nk_n\sin L}{1-k_n^2},\qquad\int_0^Lx\sin(k_nx)\,dx=-\frac{L(-1)^n}{k_n}.
$$

Consequently the coefficients of the [periodic sine with an endpoint-correcting linear term](../../diffusion-equation.md#periodic-sine-with-an-endpoint-correcting-linear-term) are

$$
\boxed{b_n=\frac{2(-1)^n\sin L}{n\pi[1-(n\pi/L)^2]}.}
$$

Insert them into the sine terms of the preceding solution. If $L=m\pi$ for a positive [integer](../../integer.md) $m$, the original initial profile is simply $\sin x$, with $k_m=1$. The apparent $0/0$ in the displayed coefficient has removable [limit](../../calculus.md#limit-of-a-function) $b_m=1$, while $b_n=0$ for $n\ne m$. In that case

$$
\boxed{u(x,t)=e^{-\kappa t}\sin x.}
$$

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Extend $f$ evenly to $F(x)=f(|x|)$ on the whole real line, and use the [Fourier transform](../../fourier-transform.md) convention $\widehat F(k)=\int_{\mathbb R}F(x)e^{-ikx}dx$. Its odd sine contribution vanishes, giving $\widehat F(k)=2\int_0^\infty f(x)\cos(kx)dx=\widehat f_c(k)$ for $k>0$; the transform is also [even](../../calculus.md#even-function). The [Fourier inversion theorem](../../fourier-analysis.md#fourier-inversion-theorem) therefore gives, for $x>0$,

$$
f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}\widehat F(k)e^{ikx}dk=\boxed{\frac1\pi\int_0^\infty\widehat f_c(k)\cos(kx)dk}.
$$

This is the inverse [Fourier cosine transform](../../fourier-transform.md#fourier-cosine-transform) with the factor-of-two forward convention used here.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Take the spatial [Fourier transform](../../fourier-transform.md) with the same convention. The [partial differential equation](../../partial-differential-equation.md) becomes $i\partial_t\widehat f-k^2\widehat f=0$, so $\widehat f(k,t)=e^{-ik^2t}\widehat f_0(k)$. Inverting and substituting the transform of the initial [function](../../function.md) yields the [convolution](../../fourier-analysis.md#convolution)

$$
f(x,t)=\int_{\mathbb R}f_0(\xi)K_t(x-\xi)d\xi,\qquad K_t(s)=\frac1{2\pi}\int_{\mathbb R}e^{iks-itk^2}dk.
$$

Complete the square, $iks-itk^2=is^2/(4t)-it[k-s/(2t)]^2$, and put $\ell=\sqrt t[k-s/(2t)]$. This gives

$$
\boxed{f(x,t)=\frac{c}{2\pi\sqrt t}\int_{-\infty}^{\infty}f_0(\xi)e^{i(x-\xi)^2/(4t)}d\xi,\qquad c=\int_{\mathbb R}e^{-i\ell^2}d\ell=\sqrt\pi e^{-i\pi/4}.}
$$

The oscillatory Gaussian is a [Fresnel integral](../../fourier-transform.md#fresnel-integral), understood as the limit with a positive Gaussian damping factor. That prescription also justifies the transform manipulations, first for rapidly decreasing smooth data and then by [L2 space](../../measure-theory.md#l2-space-is-a-hilbert-space) extension. The resulting kernel is the [free-particle propagator](../../quantum-system.md#free-particle-propagator) in units $\hbar=1$, $m=1/2$; its phase and normalization agree with the multiplier $e^{-ik^2t}$.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [matrix trace](../../linear-algebra.md#matrix-trace) is $\operatorname{Tr}A=\sum_iA_{ii}$. Expanding the [matrix products](../../vector-space.md#matrix-product) gives $\operatorname{Tr}(AB)=\sum_{i,j}A_{ij}B_{ji}=\sum_{j,i}B_{ji}A_{ij}=\operatorname{Tr}(BA)$. Thus the [cyclic property of the trace](../../linear-algebra.md#cyclic-property-of-the-trace) gives zero [trace](../../linear-algebra.md#matrix-trace) to every [commutator](../../lie-algebra.md#commutator). If $AB-BA=I$, taking the [trace](../../linear-algebra.md#matrix-trace) would give $0=n$, impossible for positive finite $n$ over the real or complex [field](../../algebra.md#field).

For real $A,B$, let $p(\lambda)=\det(A+\lambda B)$, a real [polynomial](../../polynomial.md) of degree at most $n$. Since $p(i)=\det C\ne0$, it is not the zero [polynomial](../../polynomial.md). It has at most finitely many real [roots of a polynomial](../../polynomial.md#root-of-a-polynomial), so $A+\lambda B$ is an [invertible matrix](../../linear-algebra.md#invertible-matrix) for some real $\lambda$, in fact for all but finitely many.

Finally write the invertible intertwiner as $R=A+iB$. The relation $PR=RQ$ and the reality of $P,Q$ give $PA=AQ$ and $PB=BQ$. Choose a real $\lambda$ for which $S=A+\lambda B$ is invertible. Then $PS=SQ$, so $P=SQS^{-1}$. This proves that [complex similarity of real matrices implies real similarity](../../linear-operator-theory.md#complex-similarity-of-real-matrices-implies-real-similarity).

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the [complex inner product](../../linear-algebra.md#hermitian-inner-product) $\langle a,b\rangle=\sum_j\overline{a_j}b_j=a^\dagger b$, conjugate-linear in its first argument. For $a\ne0$, put $c=\langle a,b\rangle/\langle a,a\rangle$. Positivity gives

$$
0\leq\|b-ca\|^2=\|b\|^2-\frac{|\langle a,b\rangle|^2}{\|a\|^2}.
$$

Hence the [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality) is $|\langle a,b\rangle|\leq\|a\|\|b\|$. If $a=0$ it is immediate; equality holds precisely when the two [vectors](../../vector-space.md#vector) are [linearly dependent](../../vector-space.md#linear-dependence).

For a [unitary matrix](../../linear-operator-theory.md#unitary-matrix), $U^\dagger U=I$, so $\|Ua\|^2=a^\dagger U^\dagger Ua=\|a\|^2$. If $Uv=\lambda v$ with a nonzero [eigenvector](../../linear-operator-theory.md#eigenvector), this implies $|\lambda|\|v\|=\|v\|$. Thus every [eigenvalue](../../linear-operator-theory.md#eigenvalue) satisfies

$$
\boxed{|\lambda|=1.}
$$

For the one-parameter family, expand unitarity to first order: $(I+tA^\dagger+O(t^2))(I+tA+O(t^2))=I$, so $A^\dagger+A=0$. Thus $A$ is a [skew-Hermitian matrix](../../linear-operator-theory.md#skew-hermitian-matrix), an element of the [unitary Lie algebra](../../lie-algebra.md#unitary-lie-algebra). If $Av=\mu v$, then $v^\dagger Av=\mu\|v\|^2$, whereas complex conjugation gives $(v^\dagger Av)^*=v^\dagger A^\dagger v=-v^\dagger Av$. Consequently $\overline\mu=-\mu$, proving that every [eigenvalue](../../linear-operator-theory.md#eigenvalue) of $A$ is purely imaginary, with zero permitted.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Put $s=z-1$ and seek the leading [Frobenius series](../../complex-analysis.md#frobenius-solution) term $y\sim s^\rho$. The coefficients of $y''$ and $y'$ become $-2s(1+s)$ and $2+s$, respectively. The lowest power, $s^{\rho-1}$, therefore has coefficient $-2\rho(\rho-1)+2\rho$. The [indicial equation](../../linear-ordinary-differential-equation.md#indicial-equation) is

$$
\boxed{\rho(\rho-2)=0,\qquad\rho=0,2.}
$$

The term $-y$ contributes only at the next order and does not enter this equation.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

The [product rule](../../calculus.md#product-rule) gives $\psi'=e^{-x^2/2}(y'-xy)$ and $\psi''=e^{-x^2/2}[y''-2xy'+(x^2-1)y]$. Substituting in the [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation) cancels the $x^2$ and constant terms, leaving the [Hermite differential equation](../../analysis.md#hermite-differential-equation)

$$
y''-2xy'+2\lambda y=0.
$$

For $y=\sum_{n\geq0}a_nx^n$, matching coefficients gives

$$
a_{n+2}=\frac{2(n-\lambda)}{(n+2)(n+1)}a_n.
$$

The [power series solutions of the Hermite differential equation](../../analysis.md#power-series-solutions-of-the-hermite-differential-equation) split into independent [even](../../calculus.md#even-function) and [odd](../../calculus.md#odd-function) series. With initial data $(y(0),y'(0))=(1,0)$ and $(0,1)$, respectively, their first three terms are

$$
y_e=1-\lambda x^2+\frac{\lambda(\lambda-2)}6x^4+O(x^6),\qquad y_o=x+\frac{1-\lambda}{3}x^3+\frac{(1-\lambda)(3-\lambda)}{30}x^5+O(x^7).
$$

Each nonterminating parity series has infinite [radius of convergence](../../sequence-and-series.md#radius-of-convergence): the ratio of successive terms of that parity has magnitude asymptotic to $2|x|^2/n$. Their initial data prove [linear independence](../../vector-space.md#linear-independence). If a coefficient shown vanishes at a special parameter, the recurrence supplies the terminating series instead.

A nonzero [polynomial](../../polynomial.md) solution of degree $N$ requires $\lambda=N$, by its highest-degree term, and the recurrence then terminates the matching parity. Thus all possible values are $\lambda=0,1,2,\ldots$. Up to nonzero [scalar multiples](../../vector-space.md#scalar-multiple), the degree-at-most-three solutions are the [Hermite polynomials](../../orthogonal-polynomial.md#hermite-polynomial)

$$
\boxed{\begin{array}{c|c} \lambda&y\\\hline0&1\\1&2x\\2&4x^2-2\\3&8x^3-12x\end{array}.}
$$

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

Multiply the equation for $y_n$ by $y_m$ and the equation for $y_m$ by $y_n$, then subtract. The common $h$ terms cancel, and [integration by parts](../../calculus.md#integration-by-parts) gives the [Lagrange identity for a Sturm-Liouville operator](../../sturm-liouville-theory.md#lagrange-identity-for-a-sturm-liouville-operator):

$$
(\lambda_n-\lambda_m)\int_a^bw y_ny_m\,dx=\left[g(y_ny_m'-y_my_n')\right]_a^b.
$$

At each endpoint the two pairs $(y_n',y_n)$ and $(y_m',y_m)$ satisfy the same nontrivial homogeneous linear equation. They therefore lie on the same one-dimensional line, and their determinant vanishes. The boundary expression is zero. Since the [eigenvalues](../../linear-operator-theory.md#eigenvalue) are distinct, division gives the required [orthogonality of Sturm-Liouville eigenfunctions](../../sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions):

$$
\boxed{\int_a^b w(x)y_n(x)y_m(x)\,dx=0.}
$$

For complex-valued eigenfunctions of a real self-adjoint problem one may choose real [eigenfunctions](../../linear-operator-theory.md#eigenfunction), or use the conjugated version as a [weighted inner product](../../inner-product.md#weighted-inner-product).

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

Multiplying by $y$ and integrating with the zero endpoint values first gives $\lambda\int_1^by^2dx/x=\int_1^bx(y')^2dx>0$ for a nonzero real [eigenfunction](../../linear-operator-theory.md#eigenfunction); hence $\lambda>0$. Using the printed [change of variables](../../multivariable-calculus.md#change-of-variables-formula) $\xi=\lambda\ln x$, write $y(x)=Y(\xi)$. Then $(xy')'=\lambda^2Y_{\xi\xi}/x$, so $Y_{\xi\xi}+Y/\lambda=0$. The first endpoint gives $Y=A\sin(\xi/\sqrt\lambda)$, and the other gives $\sin(\sqrt\lambda\ln b)=0$. Thus

$$
\boxed{\lambda_n=\left(\frac{n\pi}{\ln b}\right)^2,\qquad y_n(x)=A_n\sin\left(\frac{n\pi\ln x}{\ln b}\right),\quad n=1,2,\ldots.}
$$

This is the [logarithmic change of variable in a Sturm-Liouville problem](../../linear-ordinary-differential-equation.md#logarithmic-change-of-variable-in-a-sturm-liouville-problem). The measure $dx/x=d(\ln x)$ gives squared [weighted norm](../../inner-product.md#weighted-norm) $A_n^2\ln b/2$, so an orthonormal choice is $A_n=\sqrt{2/\ln b}$.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

Choose the left homogeneous solution $v(x)=\sinh x$ and the right one $w(x)=\sinh(1-x)$. Their [Wronskian](../../linear-ordinary-differential-equation.md#wronskian) is $vw'-v'w=-\sinh1$. The [Dirichlet modified Helmholtz Green function on an interval](../../green-s-function.md#dirichlet-modified-helmholtz-green-function-on-an-interval), with operator sign $D_x^2-1$, is therefore

$$
G(x,\xi)=-\frac{\sinh(x_<)\sinh(1-x_>)}{\sinh1},\qquad x_<=\min(x,\xi),\quad x_>=\max(x,\xi).
$$

It vanishes at both endpoints, is continuous at $x=\xi$, and its first [derivative](../../calculus.md#derivative) jumps by $+1$, giving $(D_x^2-1)G=\delta(x-\xi)$. The [Green-function representation](../../green-s-function.md#green-function-representation) then gives

$$
u(x)=-\frac{\sinh(1-x)}{\sinh1}\int_0^xe^\xi\sinh\xi\,d\xi-\frac{\sinh x}{\sinh1}\int_x^1e^\xi\sinh(1-\xi)\,d\xi.
$$

The two [integrals](../../integral.md) are $(e^{2x}-1)/4-x/2$ and $e(1-x)/2-(e-e^{2x-1})/4$, respectively. Substituting them and simplifying gives

$$
\boxed{u(x)=\frac12\left[xe^x-\frac{e\sinh x}{\sinh1}\right].}
$$

Direct [differentiation](../../calculus.md#differentiation) verifies $u''-u=e^x$ and both zero boundary values. The negative kernel also explains why the solution is negative inside the interval despite the positive right-hand side.

<a id="8/image-a-negative-dirichlet-green-kernel-produces-a-negative-response-to-positive-forcing"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1-green-response.png)

**[Figure 1](#8/image-a-negative-dirichlet-green-kernel-produces-a-negative-response-to-positive-forcing). A negative Dirichlet Green kernel produces a negative response to positive forcing**. Left: three source locations give continuous kernels with derivative jump $+1$. Right: the integrated solution of $u''-u=e^x$ returns to zero at both boundaries.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

Take a variation $y_\varepsilon=y+\varepsilon\eta$ with $\eta(a)=\eta(b)=0$. Differentiating the [functional](../../calculus-of-variations.md#functional) at zero and using [integration by parts](../../calculus.md#integration-by-parts) gives

$$
\delta F=\int_b^a(f_y\eta+f_{y'}\eta')dx=\left[f_{y'}\eta\right]_b^a+\int_b^a\left(f_y-\frac d{dx}f_{y'}\right)\eta\,dx.
$$

The boundary term vanishes. Since the remaining [integral](../../integral.md) must vanish for every smooth endpoint-zero variation, the [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) gives the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) $d(f_{y'})/dx=f_y$.

For the mechanical problem put $A(r)=1-2m/r>0$. The [Lagrangian](../../calculus-of-variations.md#lagrangian) is independent of $\theta$, a [cyclic coordinate](../../lagrangian-mechanics.md#cyclic-coordinate), so its [conjugate momentum](../../hamiltonian-mechanics.md#canonical-momentum) $\partial L/\partial\dot\theta=2r^2\dot\theta=2J$ is conserved. Therefore $J$ is constant, including the factor of two between $J$ and the canonical momentum for this normalization of $L$.

For the radial coordinate, $\partial L/\partial\dot r=2\dot r/A$ and $\partial L/\partial r=-\dot r^2A'/A^2+2r\dot\theta^2-\mu A'/A^2$. Its [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is

$$
\frac{2\ddot r}{A}-\frac{A'\dot r^2}{A^2}-2r\dot\theta^2+\frac{\mu A'}{A^2}=0.
$$

For a [circular orbit](../../classical-mechanics.md#circular-orbit) $r=R>2m$, the radial [velocity](../../classical-mechanics.md#velocity) and [acceleration](../../classical-mechanics.md#acceleration) vanish. Using $A'(R)=2m/R^2$ and $\dot\theta=J/R^2$ leaves $2J^2/R^3=2m\mu/[R^2A(R)^2]$, hence

$$
\boxed{J^2=\frac{m\mu R}{(1-2m/R)^2}.}
$$

This is the [circular orbit condition for a radial kinetic Lagrangian](../../classical-mechanics.md#circular-orbit-condition-for-a-radial-kinetic-lagrangian) applied to the coefficients here.

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

For a nonzero real [function](../../function.md), write $\Lambda=F/G$ with $G=\int_a^bw y^2dx>0$. Multiplying the [Sturm-Liouville equation](../../sturm-liouville-theory.md#sturm-liouville-equation) by $y$ and integrating gives

$$
\lambda G=\int_a^b\bigl[p(y')^2+qy^2\bigr]dx-\left[pyy'\right]_a^b.
$$

Thus the stated vanishing boundary product proves $\lambda=\Lambda[y]$.

For the variational statement, the [first variation](../../calculus-of-variations.md#first-variation) is

$$
\delta\Lambda=\frac2G\left\{\left[py'\eta\right]_a^b+\int_a^b\left[-(py')'+qy-\Lambda wy\right]\eta\,dx\right\}.
$$

With admissible [boundary conditions](../../differential-equation.md#boundary-condition) that also make $[py'\eta]_a^b=0$ for every allowed variation, the [fundamental lemma of the calculus of variations](../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) identifies stationary functions with the [eigenfunctions](../../linear-operator-theory.md#eigenfunction) and stationary values with their [eigenvalues](../../linear-operator-theory.md#eigenvalue). Zero [Dirichlet boundary conditions](../../differential-equation.md#dirichlet-boundary-condition), zero [Neumann boundary conditions](../../differential-equation.md#neumann-boundary-condition), and matched periodic data give familiar examples. The single printed condition $[pyy']_a^b=0$ proves the quotient identity but, by itself, does not specify the admissible variations needed for stationarity; the [boundary conditions for variational Rayleigh quotients](../../linear-operator-theory.md#boundary-conditions-for-variational-rayleigh-quotients) make this distinction explicit.

For the half-line equation, multiplication by $x^{n-1}$ gives $p=w=x^{n-1}$ and $q=x^{n+1}$. Use the regular radial boundary condition at zero and square-integrable decay at infinity, under which the proposed Gaussian is admissible. With $y=e^{ax^2}$, $a<0$, $y'=2axy$, so

$$
\Lambda(a)=(4a^2+1)\frac{\int_0^\infty x^{n+1}e^{2ax^2}dx}{\int_0^\infty x^{n-1}e^{2ax^2}dx}=-n\left(a+\frac1{4a}\right).
$$

The ratio of the two [Gaussian integrals](../../integral.md#gaussian-integral) is $n/(-4a)$, from a [change of variables](../../multivariable-calculus.md#change-of-variables-formula) and the [Gamma function recurrence](../../complex-analysis.md#gamma-function-recurrence). Differentiating gives $\Lambda'(a)=-n[1-1/(4a^2)]$, so the minimum on $a<0$ occurs at $a=-1/2$. The [Gaussian variational bound for a radial harmonic oscillator](../../quantum-harmonic-oscillator.md#gaussian-variational-bound-for-a-radial-harmonic-oscillator) therefore gives

$$
\boxed{\lambda_0\leq n,\qquad y_{\rm trial}=e^{-x^2/2}.}
$$

Here the trial actually satisfies the [differential equation](../../differential-equation.md) with $\lambda=n$. Moreover, on the same regular decaying domain, [integration by parts](../../calculus.md#integration-by-parts) gives $F[y]-nG[y]=\int_0^\infty x^{n-1}(y'+xy)^2dx\geq0$. Hence the estimate is exact, with $\boxed{\lambda_0=n}$. For $n=1$, regular radial data mean the [Neumann boundary condition](../../differential-equation.md#neumann-boundary-condition) $y'(0)=0$; imposing a zero [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) there would exclude this trial and give a different problem.

## ↑ Ancestors (10)

1. [2007](../2007.md)
2. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
