# Paper 1

↑ **Parent:** [2001](../2001.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2001/PaperNST_IA_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2001/PaperNST_IA_1.pdf)

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
  - [Solution](#2/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
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
    - [iv](#7/a/iv)
      - [Solution](#7/a/iv/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
  - [c](#9/c)
    - [Solution](#9/c/solution)
  - [d](#9/d)
    - [Solution](#9/d/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
    - [i](#10/a/i)
      - [Solution](#10/a/i/solution)
    - [ii](#10/a/ii)
      - [Solution](#10/a/ii/solution)
    - [iii](#10/a/iii)
      - [Solution](#10/a/iii/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
- [11](#11)
  - [a](#11/a)
    - [i](#11/a/i)
      - [Solution](#11/a/i/solution)
    - [ii](#11/a/ii)
      - [Solution](#11/a/ii/solution)
  - [b](#11/b)
    - [i](#11/b/i)
      - [Solution](#11/b/i/solution)
    - [ii](#11/b/ii)
      - [Solution](#11/b/ii/solution)
  - [c](#11/c)
    - [Solution](#11/c/solution)
- [12](#12)
  - [a](#12/a)
    - [Solution](#12/a/solution)
  - [b](#12/b)
    - [Solution](#12/b/solution)
  - [c](#12/c)
    - [i](#12/c/i)
      - [Solution](#12/c/i/solution)
    - [ii](#12/c/ii)
      - [Solution](#12/c/ii/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Subtract the two position [vectors](../../vector-space.md#vector) to obtain the direction $\mathbf b-\mathbf a=(-3,-1,3)$. The [affine line in a vector space](../../vector-space.md#affine-line-in-a-vector-space) through the points is therefore

$$
\boxed{\mathbf r=(2,-1,-2)+t(-3,-1,3),\qquad t\in\mathbb R.}
$$

The values $t=0,1$ recover the two specified points.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [normal vector](../../differential-geometry.md#normal-vector) to the [plane](../../geometry-and-topology.md#plane) spanned by $\mathbf a,\mathbf b$ is their [cross product](../../vector-space.md#cross-product):

$$
\mathbf a\times\mathbf b=(-5,0,-5),\qquad |\mathbf a\times\mathbf b|=5\sqrt2.
$$

Dividing by this [Euclidean norm](../../normed-vector-space.md#euclidean-norm) gives the two possible choices of [unit normal](../../differential-geometry.md#unit-normal),

$$
\boxed{\mathbf n=\pm\frac{(1,0,1)}{\sqrt2}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The two edge [vectors](../../vector-space.md#vector) based at $A$ are $\mathbf b-\mathbf a=(-3,-1,3)$ and $\mathbf c-\mathbf a=(-3,2,2)$. Their [cross product](../../vector-space.md#cross-product) is $(-8,-3,-9)$, with squared [Euclidean norm](../../normed-vector-space.md#euclidean-norm) $64+9+81=154$. The [triangle](../../euclidean-geometry.md#triangle) occupies half the corresponding [parallelogram](../../euclidean-geometry.md#parallelogram), so

$$
\boxed{\text{area}=\frac12| (\mathbf b-\mathbf a)\times(\mathbf c-\mathbf a)|=\frac{\sqrt{154}}2.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use the [normal vector](../../differential-geometry.md#normal-vector) $\mathbf N=(-8,-3,-9)$ found from the edge [vectors](../../vector-space.md#vector), rather than the [normal vector](../../differential-geometry.md#normal-vector) to the origin-based [linear span](../../vector-space.md#linear-span) in part (b). The required [plane](../../geometry-and-topology.md#plane) satisfies $\mathbf N\cdot(\mathbf r-\mathbf a)=0$. Since $\mathbf N\cdot\mathbf a=5$,

$$
\boxed{-8x-3y-9z=5.}
$$

After dividing by $|\mathbf N|=\sqrt{154}$, its equation has a [unit normal](../../differential-geometry.md#unit-normal). Its perpendicular distance from the origin is thus $\boxed{5/\sqrt{154}}$.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

On the basic interval the graph is the pair of straight segments joining $(-\pi,0)$, $(0,1)$ and $(\pi,0)$. Its [periodic extension](../../function.md#periodic-extension) is an [even](../../calculus.md#even-function) [triangular wave](../../function.md#triangular-wave).

<a id="2/image-the-even-triangular-wave-and-its-periodic-extension"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1-triangular-wave.png)

**[Figure 1](#2/image-the-even-triangular-wave-and-its-periodic-extension). The even triangular wave and its periodic extension**. Original plot marking the basic interval and the repeated linear pieces.

The [Fourier coefficients](../../fourier-series.md#fourier-coefficient) satisfy $b_n=0$ by evenness, and

$$
a_0=\frac2\pi\int_0^\pi(1-x/\pi)dx=1,\qquad a_n=\frac2\pi\int_0^\pi(1-x/\pi)\cos(nx)dx=\frac{2[1-(-1)^n]}{\pi^2n^2}.
$$

For the second formula, [integration by parts](../../calculus.md#integration-by-parts) gives $\int_0^\pi x\cos(nx)dx=[(-1)^n-1]/n^2$. Only odd indices survive, giving this rescaled [Fourier cosine series of a triangular wave](../../function.md#fourier-cosine-series-of-a-triangular-wave):

$$
\boxed{f(x)=\frac12+\frac4{\pi^2}\sum_{m=0}^\infty\frac{\cos[(2m+1)x]}{(2m+1)^2}.}
$$

The [pointwise convergence of a piecewise smooth Fourier series](../../fourier-series.md#pointwise-convergence-of-a-piecewise-smooth-fourier-series) applies throughout the interval, including the continuous joined endpoints. The coefficients also imply [uniform convergence](../../sequence-and-series.md#uniform-convergence) by the [Weierstrass M-test](../../probability-and-statistics.md#weierstrass-m-test). At $x=0$, the value is one, so

$$
\boxed{\sum_{m=0}^\infty\frac1{(2m+1)^2}=\frac{\pi^2}8.}
$$

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $c=\cos\theta$, $s=\sin\theta$. The [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $(c-\lambda)^2-s^2$, giving

$$
\boxed{\lambda_+=c+s,\qquad\lambda_-=c-s.}
$$

When $s=0$, these [eigenvalues](../../linear-operator-theory.md#eigenvalue) coincide and $A=cI=\pm I$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Adding and subtracting the two coordinates shows that $A(1,1)^T=(c+s)(1,1)^T$ and $A(1,-1)^T=(c-s)(1,-1)^T$. The normalized [eigenvectors](../../linear-operator-theory.md#eigenvector) can therefore be chosen as

$$
\boxed{v_+=\frac1{\sqrt2}(1,1)^T,\qquad v_-=\frac1{\sqrt2}(1,-1)^T.}
$$

Their [inner product](../../inner-product.md) is $(1-1)/2=0$, and their squared [norms](../../normed-vector-space.md#norm) are one, proving [orthonormality](../../inner-product.md#orthonormal-set). If $s=0$, every nonzero [vector](../../vector-space.md#vector) is an [eigenvector](../../linear-operator-theory.md#eigenvector); this chosen [orthonormal basis](../../inner-product.md#orthonormal-basis) still works.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

If $Av=\lambda v$, then $A^2v=\lambda^2v$. Alternatively, direct [matrix multiplication](../../vector-space.md#matrix-multiplication) gives

$$
B=\begin{pmatrix}1&\sin2\theta\\\sin2\theta&1\end{pmatrix}.
$$

Thus the normalized [eigenvectors](../../linear-operator-theory.md#eigenvector) $v_+,v_-$ from part (b) have respective [eigenvalues](../../linear-operator-theory.md#eigenvalue)

$$
\boxed{(c+s)^2=1+\sin2\theta,\qquad(c-s)^2=1-\sin2\theta.}
$$

If $\sin2\theta=0$, then $B=I$, and the whole two-dimensional space is its [eigenspace](../../linear-operator-theory.md#eigenspace). This degeneracy includes cases where the two [eigenvalues](../../linear-operator-theory.md#eigenvalue) of $A$ were distinct but opposite.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [fundamental theorem of calculus](../../calculus.md#fundamental-theorem-of-calculus) differentiates the upper endpoint, while [differentiation under the integral sign](../../analysis.md#differentiation-under-the-integral-sign) differentiates the parameter:

$$
\boxed{\left(\frac{\partial G}{\partial\theta}\right)_k=g(\theta,k),\qquad \left(\frac{\partial G}{\partial k}\right)_\theta=\int_0^\theta\frac{\partial g}{\partial k}(x,k)dx.}
$$

These formulas hold, for example, when $g$ and its displayed parameter [partial derivative](../../multivariable-calculus.md#partial-derivative) are continuous on a neighborhood of the integration interval and the parameter value.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Work first with $|k|<1$, so the real integrands and their parameter [derivatives](../../calculus.md#derivative) are smooth on every finite amplitude interval. For the [elliptic integral of the second kind](../../complex-analysis.md#elliptic-integral-of-the-second-kind),

$$
E_k=-k\int_0^\theta\frac{\sin^2x}{\sqrt{1-k^2\sin^2x}}dx.
$$

On the other hand, subtracting the integrands of the second-kind and first-kind [elliptic integrals](../../complex-analysis.md#elliptic-integral) gives

$$
E-F=\int_0^\theta\frac{(1-k^2\sin^2x)-1}{\sqrt{1-k^2\sin^2x}}dx=-k^2\int_0^\theta\frac{\sin^2x}{\sqrt{1-k^2\sin^2x}}dx.
$$

Consequently

$$
\boxed{E_k=\frac{E-F}{k}\quad(k\ne0).}
$$

This is the [modulus derivative of the incomplete elliptic integral of the second kind](../../complex-analysis.md#modulus-derivative-of-the-incomplete-elliptic-integral-of-the-second-kind). At $k=0$ its right-hand side has a removable limit zero, agreeing with $E_k(\theta,0)=0$. Both $E$ and $F$ here use amplitude $\theta$ and modulus $k$; differentiating with respect to the alternative parameter $k^2$ would give a different prefactor.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [fundamental theorem of calculus](../../calculus.md#fundamental-theorem-of-calculus) and part (a) give

$$
I_\theta=E(\theta,k)\sqrt{1-k^2\sin^2\theta}=E(\theta,k)E_\theta(\theta,k)=\partial_\theta\left(\frac12E(\theta,k)^2\right).
$$

The difference is constant in $\theta$. Since $I(0,k)=E(0,k)=0$, the constant is zero, proving

$$
\boxed{I(\theta,k)=\frac12E(\theta,k)^2.}
$$

This is simply the [chain rule](../../calculus.md#chain-rule) integrated, with $E$ itself as the antiderivative of the square-root factor.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For $f=x\ln x$, the [derivatives](../../calculus.md#derivative) are $f'=1+\ln x$ and $f''=1/x>0$. Its unique [stationary point](../../calculus-of-variations.md#stationary-point) is the global [minimum](../../set.md#minimum-of-a-subset-of-a-total-order) $(e^{-1},-e^{-1})$. For $g=\ln x/x$, $g'=(1-\ln x)/x^2$ changes from positive to negative at $x=e$, giving the global [maximum](../../set.md#maximum-of-a-subset-of-a-total-order) $(e,e^{-1})$. Their endpoint [limits](../../calculus.md#limit-of-a-function) are

$$
\boxed{\begin{array}{c|cc}&x\to0^+&x\to\infty\\\hline f(x)&0\text{ from below}&+\infty\\g(x)&-\infty&0\text{ from above}\end{array}}
$$

An intersection requires $(x^2-1)\ln x=0$, and on $x>0$ both factors vanish only at $x=1$. There $f=g=0$ and $f'=g'=1$, proving a common [tangent line](../../calculus.md#tangent-line) $y=x-1$. In fact,

$$
f-g=\frac{(x^2-1)\ln x}{x}>0\quad(x>0,\ x\ne1),
$$

because the two numerator factors always have the same sign. Thus the curves touch at $(1,0)$ without exchanging their order.

<a id="5/a/image-two-logarithmic-curves-touching-at-their-unique-intersection"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1-logarithmic-tangency.png)

**[Figure 2](#5/a/image-two-logarithmic-curves-touching-at-their-unique-intersection). Two logarithmic curves touching at their unique intersection**. Original common-axis plot marking the extrema and the shared tangent at $(1,0)$. The curve $x\ln x$ lies above $\ln x/x$ everywhere else on the positive axis.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use $u=1/x$, so $dx=-du/u^2$ and $\ln x=-\ln u$. Reversing the integration bounds gives, without evaluating either side,

$$
\boxed{\int_1^\infty\frac{\ln x}{x^2}dx=-\int_0^1\ln u\,du.}
$$

For $J=\int_0^\infty\ln x/(1+x^2)dx$, the same [change of variables](../../multivariable-calculus.md#change-of-variables-formula) gives

$$
J=-\int_0^\infty\frac{\ln u}{1+u^2}du=-J,
$$

so $\boxed{J=0}$. These are legitimate transformations of [improper integrals](../../real-analysis.md#improper-integral): $|\ln x|$ is integrable near zero, and $(\ln x)/x^2$ is integrable at infinity. In particular $J$ is absolutely convergent, so no cancellation of divergent endpoints is being assumed.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Take the outward [orientation of a surface](../../differential-geometry.md#orientation-of-a-surface). The [divergence](../../multivariable-calculus.md#divergence) is $\nabla\cdot\mathbf F=y^2+z^2+x^2$, so the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) converts the closed [surface flux](../../multivariable-calculus.md#flux-integral) into an integral over the box:

$$
\int_S\mathbf F\cdot d\mathbf S=\int_{-a}^a\int_{-b}^b\int_{-c}^c(x^2+y^2+z^2)\,dz\,dy\,dx.
$$

Each term separates; for example the $x^2$ term is $(2a^3/3)(2b)(2c)$. Summing gives

$$
\boxed{\int_S\mathbf F\cdot d\mathbf S=\frac{8abc}3(a^2+b^2+c^2).}
$$

Here $a,b,c>0$ are the box half-lengths. Reversing [orientation of a surface](../../differential-geometry.md#orientation-of-a-surface) would negate the result.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Differentiate the ellipsoidal parametrization. Its outward [vector surface element](../../differential-geometry.md#vector-area-element) is

$$
\mathbf r_\theta\times\mathbf r_\phi=(bc\sin^2\theta\cos\phi,\ ac\sin^2\theta\sin\phi,\ ab\sin\theta\cos\theta).
$$

For $a,b,c>0$, its [dot product](../../inner-product.md#dot-product) with $\mathbf r$ simplifies to $abc\sin\theta$. Thus the requested direct [surface integral](../../multivariable-calculus.md#surface-integral) is

$$
\boxed{\int_S\mathbf r\cdot d\mathbf S=abc\int_0^{2\pi}\int_0^\pi\sin\theta\,d\theta\,d\phi=4\pi abc.}
$$

As a check, the [divergence](../../multivariable-calculus.md#divergence) of $\mathbf r$ is three, and the [ellipsoid](../../euclidean-geometry.md#ellipsoid) has [volume](../../geometry-and-topology.md#volume) $4\pi abc/3$, so the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives the same value.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

Subtract corresponding entries in the two [matrices](../../vector-space.md#matrix):

$$
\boxed{\begin{pmatrix}2&-10&15\\-6&-3&-6\end{pmatrix}.}
$$

Both matrices have shape $2\times3$, so this subtraction is defined.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

Using row-column [matrix multiplication](../../vector-space.md#matrix-multiplication), the second row of the first [matrix](../../vector-space.md#matrix) is $(1,6)$. Therefore

$$
\boxed{\begin{pmatrix}3&7\\1&6\end{pmatrix}\begin{pmatrix}2&4\\0&0\end{pmatrix}=\begin{pmatrix}6&12\\2&4\end{pmatrix}.}
$$

<h4 id="7/a/iii">iii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/a/iii)

The row-column product is the [dot product](../../inner-product.md#dot-product) $4\cdot6+8\cdot3+1\cdot0$, giving $\boxed{48}$. Its shape is $1\times1$.

<h4 id="7/a/iv">iv</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#7/a/iv)

The first [matrix product](../../vector-space.md#matrix-product) gives the column $(37,37,37)^T$. Its product with the final row is an [outer product](../../vector-space.md#outer-product), not a scalar:

$$
\boxed{\begin{pmatrix}37\\37\\37\end{pmatrix}\begin{pmatrix}-2&0&2\end{pmatrix}=\begin{pmatrix}-74&0&74\\-74&0&74\\-74&0&74\end{pmatrix}.}
$$

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Row reduction, or the [cofactor](../../linear-algebra.md#cofactor) formula for a [matrix inverse](../../matrix-inverse.md), gives

$$
\boxed{\begin{pmatrix}1&1&1\\1&2&3\\1&4&9\end{pmatrix}^{-1}=\begin{pmatrix}3&-5/2&1/2\\-3&4&-1\\1&-3/2&1/2\end{pmatrix}.}
$$

Multiplying by the right-hand-side column $(5,13,35)^T$ gives, at $\lambda=3$,

$$
\boxed{(x,y,z)=(0,2,3).}
$$

For general $\lambda$, the [coefficient matrix](../../linear-algebra.md#coefficient-matrix) has [determinant](../../multilinear-algebra.md#determinant) $(\lambda-1)(\lambda-2)$. Thus other parameter values give a unique solution. If $\lambda=1$, subtracting the first equation from the second gives $y=8$, while subtracting it from the third gives $3y=30$, a contradiction. If $\lambda=2$, subtraction gives $y+z=8$ and $3y+3z=30$, again inconsistent. Hence

$$
\boxed{\text{no solution exactly when }\lambda=1\text{ or }2.}
$$

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

Write $r=|\mathbf r|$ and $q=\mathbf p\cdot\mathbf r$. Away from the origin, $\nabla q=\mathbf p$ and $\nabla r^{-m}=-m\mathbf r/r^{m+2}$. The [product rule](../../calculus.md#product-rule) gives

$$
\nabla\cdot(q\mathbf r r^{-5})=q r^{-5}+q(3r^{-5}-5r^{-5})=-q r^{-5},\qquad \nabla\cdot(\mathbf p r^{-3})=-3q r^{-5}.
$$

Consequently the [divergence](../../multivariable-calculus.md#divergence) of $\mathbf E=3q\mathbf r r^{-5}-\mathbf p r^{-3}$ is zero. For any closed surface bounding a region that excludes the origin, the field is smooth throughout that region, and the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) proves

$$
\boxed{\int_A\mathbf E\cdot d\mathbf S=0.}
$$

For the infinite cylinder, use $\mathbf r=(a\cos\phi,a\sin\phi,z)$ and outward [unit normal](../../differential-geometry.md#unit-normal) $(\cos\phi,\sin\phi,0)$. With $\mathbf p=(0,0,1)$, $q=z$, $dS=a\,d\phi\,dz$, and $\mathbf E\cdot\mathbf n=3az/(a^2+z^2)^{5/2}$. Hence the direct [surface flux](../../multivariable-calculus.md#flux-integral) is

$$
\int_0^{2\pi}\int_{-\infty}^\infty\frac{3a^2z}{(a^2+z^2)^{5/2}}dz\,d\phi=\boxed0.
$$

The integrand is [odd](../../calculus.md#odd-function) in $z$ and absolutely integrable. This calculation treats the unbounded cylindrical side directly, without applying the bounded-region [divergence theorem](../../multivariable-calculus.md#divergence-theorem) across the field's singularity.

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

For an $N+1$ times continuously differentiable [function](../../function.md), [Taylor's theorem](../../calculus.md#taylor-s-theorem) gives

$$
\boxed{f(x)=\sum_{n=0}^N\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n+\frac{f^{(N+1)}(\xi)}{(N+1)!}(x-x_0)^{N+1},}
$$

where $\xi$ lies between $x_0$ and $x$. An infinite [Taylor series](../../calculus.md#taylor-series) represents the function when its remainder tends to zero; this holds locally for an [analytic function](../../holomorphic-function.md), rather than for every smooth function automatically.

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Integrate the [geometric series](../../sequence-and-series.md#geometric-series) for $1/(1+x)$ from zero to $x$. The first three nonzero terms are

$$
\boxed{\ln(1+x)=x-\frac{x^2}2+\frac{x^3}3+O(x^4).}
$$

The resulting [Taylor series](../../calculus.md#taylor-series) converges for $|x|<1$.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

For fixed real $a\ne0$, write the square root as $|a|\sqrt{1+x^2/a^2}$ and use the [binomial series](../../sequence-and-series.md#binomial-series) with exponent $-1/2$:

$$
\boxed{\frac{x}{\sqrt{x^2+a^2}}=\frac x{|a|}-\frac{x^3}{2|a|^3}+\frac{3x^5}{8|a|^5}+O(x^7).}
$$

The [absolute values](../../real-analysis.md#absolute-value) are necessary for negative $a$. This [Taylor series](../../calculus.md#taylor-series) is valid for $|x|<|a|$. If $a=0$, the quotient is $x/|x|$ for $x\ne0$; it has no continuous extension at zero and therefore **has no Taylor expansion about zero**.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

Factor the [Gaussian function](../../calculus.md#gaussian-function) as $e^{-(x-a)^2}=e^{-a^2}e^{2ax}e^{-x^2}$. Multiplying the two [exponential series](../../calculus.md#exponential-series) gives

$$
e^{-(x-a)^2}=e^{-a^2}\left[1+2ax+(2a^2-1)x^2+\left(\frac43a^3-2a\right)x^3+O(x^4)\right].
$$

For $a\ne0,\pm1/\sqrt2$, its first three nonzero terms are

$$
\boxed{e^{-a^2}\bigl[1+2ax+(2a^2-1)x^2\bigr].}
$$

Vanishing coefficients require separate treatment in this [Taylor expansion of a translated Gaussian](../../calculus.md#taylor-expansion-of-a-translated-gaussian). If $a=0$, the first three nonzero terms are $\boxed{1-x^2+x^4/2}$. If $a=\pm1/\sqrt2$, they are

$$
\boxed{e^{-1/2}\left(1+2ax-\frac{4a}3x^3\right).}
$$

The latter expression retains the cubic term because the quadratic coefficient is zero.

<h3 id="9/d">d</h3>

↑ **Parent:** [9](#9)

<h4 id="9/d/solution">Solution</h4>

↑ **Parent:** [D](#9/d)

Use the real [logarithm](../../calculus.md#logarithm) near zero and subtract its two [Taylor series](../../calculus.md#taylor-series):

$$
\ln\frac{1-x}{1+2x^2}=\ln(1-x)-\ln(1+2x^2)=\left(-x-\frac{x^2}2-\frac{x^3}3\right)-2x^2+O(x^4).
$$

Thus the first three nonzero terms are

$$
\boxed{-x-\frac52x^2-\frac13x^3.}
$$

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Use the [Einstein summation convention](../../multilinear-algebra.md#einstein-notation), with repeated component indices summed. The following three expressions are listed separately below. For cyclic invariance of the [trace](../../linear-algebra.md#matrix-trace),

$$
\operatorname{tr}(ABC)=a_{ij}b_{jk}c_{ki}=c_{ki}a_{ij}b_{jk}=\operatorname{tr}(CAB),
$$

where the middle equality commutes scalar entries, not the [matrices](../../vector-space.md#matrix) themselves. If $A$ is invertible, this gives

$$
\boxed{\operatorname{tr}(ABA^{-1})=\operatorname{tr}(BA^{-1}A)=\operatorname{tr}B.}
$$

This is [similarity invariance of trace](../../linear-algebra.md#similarity-invariance-of-trace).

<h4 id="10/a/i">i</h4>

↑ **Parent:** [A](#10/a)

<h5 id="10/a/i/solution">Solution</h5>

↑ **Parent:** [I](#10/a/i)

Taking the diagonal sum of the [matrix product](../../vector-space.md#matrix-product) gives

$$
\boxed{\operatorname{tr}(AB)=a_{ij}b_{ji}.}
$$

Both repeated indices are summed from one to $n$.

<h4 id="10/a/ii">ii</h4>

↑ **Parent:** [A](#10/a)

<h5 id="10/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10/a/ii)

Apply row-column [matrix multiplication](../../vector-space.md#matrix-multiplication) twice:

$$
\boxed{(ABC)_{ij}=a_{ik}b_{k\ell}c_{\ell j}.}
$$

The indices $i,j$ are free, while $k,\ell$ are summed.

<h4 id="10/a/iii">iii</h4>

↑ **Parent:** [A](#10/a)

<h5 id="10/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10/a/iii)

The [identity matrix](../../vector-space.md#identity-matrix) has entries given by the [Kronecker delta](../../multilinear-algebra.md#kronecker-delta), so

$$
\boxed{\operatorname{tr}I=\delta_{ii}=n.}
$$

Each of the $n$ diagonal entries is one.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Expand $(I+B)^2$ in components:

$$
(A^2)_{ij}=(\delta_{ik}+b_{ik})(\delta_{kj}+b_{kj})=\boxed{\delta_{ij}+2b_{ij}+b_{ik}b_{kj}}.
$$

If $B^2=0$, all powers $B^k$ for $k\geq2$ vanish. The matrix [binomial theorem](../../binomial-coefficient.md#binomial-theorem), valid here because $I$ commutes with $B$, therefore yields

$$
\boxed{A^n=I+nB,\qquad(A^n)_{ij}=\delta_{ij}+nb_{ij}.}
$$

These [powers of the identity plus a square-zero matrix](../../linear-operator-theory.md#powers-of-the-identity-plus-a-square-zero-matrix) can also be proved by induction: $(I+nB)(I+B)=I+(n+1)B$. For the displayed example, $B^2=0$ directly, and

$$
\boxed{\begin{pmatrix}1&p\\0&1\end{pmatrix}^{n}=\begin{pmatrix}1&np\\0&1\end{pmatrix}.}
$$

This is the repeated [function composition](../../function.md#function-composition) of a [shear mapping](../../vector-space.md#shear-mapping). The argument gives every nonnegative integer $n$; since $(I+B)^{-1}=I-B$, the same formula also holds for negative integers.

## 11

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/i">i</h4>

↑ **Parent:** [A](#11/a)

<h5 id="11/a/i/solution">Solution</h5>

↑ **Parent:** [I](#11/a/i)

Multiply the numerator and denominator by the [complex conjugate](../../complex-analysis.md#complex-conjugate) $1+i$: $(1+i)/(1-i)=(1+i)^2/2=i$, whose square is $-1$. Thus

$$
\boxed{\operatorname{Re}=-1,\qquad\operatorname{Im}=0.}
$$

<h4 id="11/a/ii">ii</h4>

↑ **Parent:** [A](#11/a)

<h5 id="11/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11/a/ii)

The number $ie^{i\phi}$ has [modulus](../../complex-analysis.md#modulus) one and [argument](../../complex-analysis.md#argument-complex-analysis) $\phi+\pi/2$ modulo $2\pi$. Therefore its [complex logarithm](../../analysis.md#complex-logarithm) has values

$$
\boxed{\ln(ie^{i\phi})=i(\phi+\pi/2+2\pi k),\quad k\in\mathbb Z.}
$$

Every value has [real part](../../complex-analysis.md#real-part) zero. For the [principal complex logarithm](../../analysis.md#principal-complex-logarithm), choose the unique integer giving imaginary part in $(-\pi,\pi]$. The unwrapped value $\phi+\pi/2$ is the principal imaginary part only when it already lies in that interval.

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/i">i</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11/b/i)

In [polar form](../../complex-analysis.md#polar-form-of-a-complex-number), a cube root of one has [modulus](../../complex-analysis.md#modulus) one and [argument](../../complex-analysis.md#argument-complex-analysis) $2\pi k/3$. The three [roots of unity](../../algebra.md#root-of-unity) are

$$
\boxed{1,\qquad\frac{-1+i\sqrt3}2,\qquad\frac{-1-i\sqrt3}2.}
$$

They are equally spaced on the [unit circle](../../complex-analysis.md#complex-unit-circle).

<h4 id="11/b/ii">ii</h4>

↑ **Parent:** [B](#11/b)

<h5 id="11/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11/b/ii)

Write $-8=8e^{i(\pi+2\pi k)}$. Its cube roots have [modulus](../../complex-analysis.md#modulus) two and [arguments](../../complex-analysis.md#argument-complex-analysis) $(\pi+2\pi k)/3$, for $k=0,1,2$. Thus

$$
\boxed{1+i\sqrt3,\qquad -2,\qquad 1-i\sqrt3.}
$$

Each cube equals $-8$, and a cubic [polynomial](../../polynomial.md) has no further distinct roots.

<h3 id="11/c">c</h3>

↑ **Parent:** [11](#11)

<h4 id="11/c/solution">Solution</h4>

↑ **Parent:** [C](#11/c)

For $b\ne0$, write $z=bw$. The equation becomes $w^2+w+1=0$, whose roots are $(-1\pm i\sqrt3)/2$, both of [modulus](../../complex-analysis.md#modulus) one. Hence $|z|=|b|$. If $b=0$, the double root is $z=0$, giving the same relation. Therefore

$$
\boxed{|z|\leq1\quad\Longleftrightarrow\quad -1\leq b\leq1.}
$$

## 12

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12/a">a</h3>

↑ **Parent:** [12](#12)

<h4 id="12/a/solution">Solution</h4>

↑ **Parent:** [A](#12/a)

For a [probability density function](../../continuous-probability-distribution.md#probability-density-function) $P$, the [mean](../../expected-value.md) and [variance](../../variance.md) are

$$
\boxed{\mu=\int_{-\infty}^\infty xP(x)dx,\qquad \sigma^2=\int_{-\infty}^\infty(x-\mu)^2P(x)dx=\mathbb E[X^2]-\mu^2.}
$$

These formulas assume the required [moments](../../expected-value.md#moment) are finite; finiteness of the second moment ensures a finite mean as well.

<h3 id="12/b">b</h3>

↑ **Parent:** [12](#12)

<h4 id="12/b/solution">Solution</h4>

↑ **Parent:** [B](#12/b)

The triangular [probability density function](../../continuous-probability-distribution.md#probability-density-function) is normalized because $2\int_0^1(1-x)dx=1$. It is [even](../../calculus.md#even-function), so the mean integrand is [odd](../../calculus.md#odd-function) and $\mu=0$. Its [variance](../../variance.md) is consequently its second [moment](../../expected-value.md#moment):

$$
\boxed{\mu=0,\qquad\sigma^2=2\int_0^1x^2(1-x)dx=2\left(\frac13-\frac14\right)=\frac16.}
$$

<h3 id="12/c">c</h3>

↑ **Parent:** [12](#12)

<h4 id="12/c/i">i</h4>

↑ **Parent:** [C](#12/c)

<h5 id="12/c/i/solution">Solution</h5>

↑ **Parent:** [I](#12/c/i)

The standard [normal density](../../probability-distribution.md#normal-density) is [even](../../calculus.md#even-function), so $x^3P(x)$ is [odd](../../calculus.md#odd-function). Since [Gaussian decay dominates every power](../../calculus.md#gaussian-decay-dominates-every-power), the integrand is absolutely integrable. Therefore

$$
\boxed{\mathbb E[X^3]=\int_{-\infty}^\infty x^3P(x)dx=0.}
$$

<h4 id="12/c/ii">ii</h4>

↑ **Parent:** [C](#12/c)

<h5 id="12/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12/c/ii)

For the standard [normal density](../../probability-distribution.md#normal-density), $P'(x)=-xP(x)$. Using [integration by parts](../../calculus.md#integration-by-parts),

$$
\mathbb E[X^4]=-\int_{-\infty}^\infty x^3P'(x)dx=-[x^3P(x)]_{-\infty}^\infty+3\int_{-\infty}^\infty x^2P(x)dx.
$$

The boundary term vanishes because [Gaussian decay dominates every power](../../calculus.md#gaussian-decay-dominates-every-power). Since the given [mean](../../expected-value.md) is zero and [variance](../../variance.md) is one, $\mathbb E[X^2]=1$, yielding the [Gaussian fourth moment](../../probability-distribution.md#gaussian-fourth-moment)

$$
\boxed{\mathbb E[X^4]=3.}
$$

## ↑ Ancestors (10)

1. [2001](../2001.md)
2. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
