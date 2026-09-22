# Paper 2

↑ **Parent:** [2006](../2006.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2006/PaperNST_IA_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2006/PaperNST_IA_2.pdf)

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
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
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
  - [c](#8/c)
    - [i](#8/c/i)
      - [Solution](#8/c/i/solution)
    - [ii](#8/c/ii)
      - [Solution](#8/c/ii/solution)
- [9](#9)
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
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)
  - [d](#10/d)
    - [Solution](#10/d/solution)
  - [e](#10/e)
    - [Solution](#10/e/solution)
- [11](#11)
  - [a](#11/a)
    - [Solution](#11/a/solution)
  - [b](#11/b)
    - [Solution](#11/b/solution)
  - [c](#11/c)
    - [Solution](#11/c/solution)
  - [d](#11/d)
    - [Solution](#11/d/solution)
- [12](#12)
  - [a](#12/a)
    - [Solution](#12/a/solution)
  - [b](#12/b)
    - [Solution](#12/b/solution)
  - [c](#12/c)
    - [Solution](#12/c/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For real $x$, the angle $\arctan x$ lies in $(-\pi/2,\pi/2)$ and has sine $x/\sqrt{1+x^2}$. Thus the principal [arcsine](../../geometry-and-topology.md#inverse-sine) in the expression equals the [arctangent](../../geometry-and-topology.md#inverse-tangent) of $x$. Its [derivative](../../calculus.md#derivative) is

$$
\boxed{\frac{dy}{dx}=\frac1{1+x^2},\qquad x\in\mathbb R.}
$$

The [chain rule](../../calculus.md#chain-rule) gives the same result directly, using $1-x^2/(1+x^2)=1/(1+x^2)$ with a positive square root.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The lower-order terms cancel, so the numerator must be expanded through sixth order. The [Taylor series](../../calculus.md#taylor-series) give $\sin(\sin x)=x-x^3/3+x^5/10+O(x^7)$ and $\sin^2x=x^2-x^4/3+2x^6/45+O(x^8)$. Therefore

$$
\frac{x\sin(\sin x)-\sin^2x}{x^4}=\frac{x^2}{18}+O(x^4).
$$

The **first nonzero term is $x^2/18$**, with the quotient continuously extended to zero if needed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

With the [change of variables](../../multivariable-calculus.md#change-of-variables-formula) $u=\tan x$, one has $dx=du/(1+u^2)$, $\sin x=u/\sqrt{1+u^2}$ and $\cos x=1/\sqrt{1+u^2}$. The transformed [improper integral](../../real-analysis.md#improper-integral) is integrable at its zero endpoint and becomes

$$
\int_0^{1/\sqrt3}(u^{-1/2}+u^{3/2})du=\left[2u^{1/2}+\frac25u^{5/2}\right]_0^{1/\sqrt3}.
$$

Hence

$$
\boxed{I=\frac{32}{15\sqrt[4]3}.}
$$

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $P=\mathbf a\mathbf a^T$. Since $\mathbf a$ is a [unit vector](../../vector-space.md#unit-vector), $P^2=\mathbf a(\mathbf a^T\mathbf a)\mathbf a^T=P$ and $P^T=P$. Thus this [Householder reflection](../../linear-algebra.md#householder-transformation) satisfies

$$
\boxed{A^2=(I-2P)^2=I,\qquad A^T=I-2P^T=A.}
$$

Geometrically, the mirror preserves the component tangent to its plane and reverses the normal component; doing it twice restores the original [vector](../../vector-space.md#vector).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Expanding the two products of [Householder reflections](../../linear-algebra.md#householder-transformation) gives

$$
\boxed{BA-AB=4(\mathbf a\cdot\mathbf b)(\mathbf b\mathbf a^T-\mathbf a\mathbf b^T).}
$$

The [commuting plane reflections](../../linear-algebra.md#commuting-plane-reflections) criterion follows: the operator vanishes if the normals are [orthogonal](../../inner-product.md#orthogonal-vectors), or if they are parallel. Conversely, if $c=\mathbf a\cdot\mathbf b\ne0$ and the operator vanishes, applying $\mathbf b\mathbf a^T-\mathbf a\mathbf b^T$ to $\mathbf a$ gives $\mathbf b-c\mathbf a=0$, proving parallelism.

This establishes equality of the reflected directions **for every incident ray** exactly in those two cases. For one fixed ray the claim needs that qualification: if nonparallel normals are not orthogonal, a ray along $\mathbf a\times\mathbf b$ has zero normal component for both mirrors and is unchanged in either order. Algebraically it lies in the [kernel](../../kernel-of-a-linear-map.md) of the commutator; it is a special direction rather than a pair of commuting reflection operators.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For an arbitrary [vector](../../vector-space.md#vector) $\mathbf x$, expansion in the [orthonormal basis](../../inner-product.md#orthonormal-basis) gives $x_i=(a_i a_j+b_i b_j+c_i c_j)x_j$, with summation over $j$. Since this holds for every $\mathbf x$, the [resolution of the identity in an orthonormal basis](../../inner-product.md#resolution-of-the-identity-in-an-orthonormal-basis) is

$$
a_i a_j+b_i b_j+c_i c_j=\delta_{ij}.
$$

Let $P_a=\mathbf a\mathbf a^T$, and similarly for $b,c$. The three [orthogonal projection matrices](../../inner-product.md#orthogonal-projection-matrix) sum to $I$ and have pairwise products zero. Thus

$$
\boxed{(I-2P_c)(I-2P_b)(I-2P_a)=I-2(P_a+P_b+P_c)=-I,\qquad\mathbf s_{\rm out}=-\mathbf s_{\rm in}.}
$$

Any ray meeting all three ideal perpendicular mirrors therefore returns in the opposite direction, independently of reflection order. This is the geometry of a [corner reflector](../../energy.md#corner-reflector), a kind of [retroreflector](../../energy.md#retroreflector) used in [lunar laser ranging](../../energy.md#lunar-laser-ranging).

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Integrating the first component with respect to $x$ suggests $\phi=xy+g(y,z)$. Matching the other components gives $g=\sin(yz)+C$. Direct differentiation verifies

$$
\boxed{\phi_1=xy+\sin(yz)+C,\qquad\mathbf F_1=\nabla\phi_1.}
$$

Thus the [vector field](../../multivariable-calculus.md#vector-field) is [conservative](../../multivariable-calculus.md#conservative-vector-field), with the displayed [scalar potential](../../classical-field-theory.md#scalar-potential).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The $z$ component of the [curl](../../multivariable-calculus.md#curl) is $\partial_xF_y-\partial_yF_x=e^{x+y}-xe^{xy}$, which is not identically zero; at the origin it is one. Hence **the field is not conservative on $\mathbb R^3$** and has no global [scalar potential](../../classical-field-theory.md#scalar-potential).

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Integrating the first component and checking the remaining [partial derivatives](../../multivariable-calculus.md#partial-derivative) gives

$$
\boxed{\phi_3=x^2yz-\cos x+C,\qquad\mathbf F_3=\nabla\phi_3.}
$$

This explicit [scalar potential](../../classical-field-theory.md#scalar-potential) proves that the field is [conservative](../../multivariable-calculus.md#conservative-vector-field).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Parametrize the straight path by $\mathbf r(t)=(t,t,t)$, $0\leq t\leq\pi$. Then $\mathbf F_3\cdot d\mathbf r=(4t^3+\sin t)dt$, so direct evaluation of the [line integral](../../multivariable-calculus.md#line-integral) gives

$$
\boxed{\int_C\mathbf F_3\cdot d\mathbf r=\int_0^\pi(4t^3+\sin t)dt=\pi^4+2.}
$$

The [fundamental theorem for line integrals](../../multivariable-calculus.md#fundamental-theorem-for-line-integrals) supplies an independent check: this is $\phi_3(\pi,\pi,\pi)-\phi_3(0,0,0)$.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

On the first segment only $z$ varies and $F_z=x^2y=0$. On the second only $y$ varies and $F_y=x^2z=0$. On the last segment $y=z=\pi$, so the [line integral](../../multivariable-calculus.md#line-integral) is

$$
\boxed{0+0+\int_0^\pi(2\pi^2x+\sin x)dx=\pi^4+2.}
$$

The agreement is the expected [path independence](../../multivariable-calculus.md#path-independence) of a [conservative vector field](../../multivariable-calculus.md#conservative-vector-field).

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Where $f_z\ne0$, the [implicit function theorem](../../multivariable-calculus.md#implicit-function-theorem) makes the surface a local graph $z=h(x,y)$ with $h_x=-f_x/f_z$ and $h_y=-f_y/f_z$. Its upward [vector area element](../../differential-geometry.md#vector-area-element) is $(-h_x,-h_y,1)dx\,dy$. Therefore the [vector area element of an implicit surface](../../differential-geometry.md#vector-area-element-of-an-implicit-surface) is

$$
\boxed{d\mathbf S=\frac{\nabla f}{f_z}\,dx\,dy,\qquad\mathbf F=\frac{\nabla f}{f_z},\quad\mathbf F\cdot\mathbf k=1.}
$$

Dividing by $f_z$ fixes the upward orientation even if the initially chosen gradient points downward. The restriction excludes a locally vertical graph, where this particular projected-area representation cannot be used.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose $f=x^2(1+y)+y^2z-1$. Since $f_z=y^2>0$ on the stated open domain, its upward [vector area element](../../differential-geometry.md#vector-area-element) is

$$
\boxed{d\mathbf S=\left(\frac{2x(1+y)}{y^2},\ \frac{x^2+2yz}{y^2},\ 1\right)dx\,dy,\qquad z=\frac{1-x^2(1+y)}{y^2}.}
$$

The graph becomes unbounded near parts of $y=0$; the flux integrals below are understood as limits from $y>0$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Subtract the integrands before integrating: $\mathbf G_2-\mathbf G_1=(0,y^3,0)$. With the upward [vector area element](../../differential-geometry.md#vector-area-element),

$$
(\mathbf G_2-\mathbf G_1)\cdot d\mathbf S=(x^2y+2y^2z)dx\,dy=(2-2x^2-x^2y)dx\,dy.
$$

This extends continuously to the lower edge, so

$$
\boxed{|I_1-I_2|=\left|\int_0^1\int_0^2(2-2x^2-x^2y)dy\,dx\right|=2.}
$$

The individual [flux integrals](../../multivariable-calculus.md#flux-integral) also converge: $\mathbf G_1\cdot d\mathbf S=x(3+2y)dx\,dy$ gives $I_1=5$, and hence $I_2=7$. Reversing the surface orientation changes both signs and leaves the requested magnitude unchanged.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

In the plane $x=0$, the right half of the cross-section has coordinates $y=a(1-\cos\theta)\sin\theta$, $z=a(1-\cos\theta)\cos\theta$, $0\leq\theta\leq\pi$. Reflect across the $z$ axis for the other half. The [cardioid](../../multivariable-calculus.md#cardioid) has a cusp at $(y,z)=(0,0)$ for $\theta=0$, crosses $z=0$ at $(\pm a,0)$ for $\theta=\pi/2$, and reaches $(0,-2a)$ for $\theta=\pi$. The small upper lobes reach $z=a/4$; the widest section is below the equator.

<a id="5/a/image-cardioid-cross-section-and-a-horizontal-slice-of-the-apple-shaped-solid"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2-apple-cross-section.png)

**[Figure 1](#5/a/image-cardioid-cross-section-and-a-horizontal-slice-of-the-apple-shaped-solid). Cardioid cross-section and a horizontal slice of the apple-shaped solid**. Original plot in units of $a$. The shaded lower portion has polar angles above $\pi/2$. The thin marked slice is bounded by horizontal planes, rather than by rays from the origin.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For [horizontal slices of a surface of revolution in spherical coordinates](../../differential-geometry.md#horizontal-slices-of-a-surface-of-revolution-in-spherical-coordinates), use disk area times vertical thickness. Here the cylindrical radius is $\rho=a(1-\cos\theta)\sin\theta$ and the height is $z=a(\cos\theta-\cos^2\theta)$. For $\theta>\pi/2$, $dz/d\theta=-a(1-2\cos\theta)\sin\theta<0$. Hence a positive angular increment gives

$$
\boxed{dV=\pi a^3(1-\cos\theta_0)^2(1-2\cos\theta_0)\sin^3\theta_0\,d\theta.}
$$

These are horizontal disks in the lower part of the solid. A spherical angular-wedge element $r^2\sin\theta\,dr\,d\theta\,d\phi$ describes a different infinitesimal slice.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Integrate the horizontal-disk expression over $\pi/2<\theta<\pi$. With $u=\cos\theta$ and $\sin\theta\,d\theta=-du$,

$$
V=\pi a^3\int_{-1}^0(1-u)^2(1-2u)(1-u^2)du=\pi a^3\int_{-1}^0(1-4u+4u^2+2u^3-5u^4+2u^5)du.
$$

Evaluating the [integral](../../integral.md) of this [polynomial](../../polynomial.md) gives

$$
\boxed{V=\frac{5\pi a^3}{2}.}
$$

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For $x>0$, the kernel is smooth between the two positive endpoints. The [Leibniz integral rule](../../analysis.md#leibniz-integral-rule) gives both endpoint terms and the parameter derivative:

$$
I'(x)=\frac{3\cos(x^4)-2\cos(x^3)}x-\int_{x^2}^{x^3}\sin(xt)dt.
$$

The remaining integral equals $[\cos(x^3)-\cos(x^4)]/x$, so

$$
\boxed{I'(x)=\frac{4\cos(x^4)-3\cos(x^3)}x,\qquad x>0.}
$$

The substitution $u=xt$ gives the same result directly from limits $x^3,x^4$. Negative $x$ would make the original interval cross the nonintegrable $1/t$ singularity, so it is not part of this ordinary-integral domain.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For $n<x<n+1$, monotonicity gives $1/x<1/n<1/(x-1)$. Integrating over that unit interval proves the strict inequalities, equivalently $\ln(1+1/n)<1/n<\ln(n/(n-1))$ for $n>1$.

Let $H_N$ be the [harmonic number](../../analytic-number-theory.md#harmonic-number) and define $u_N=H_N-\ln N$, $v_N=H_N-\ln(N+1)$. The same integral comparison gives $u_{N+1}-u_N=1/(N+1)-\ln(1+1/N)<0$ and $v_{N+1}-v_N=1/(N+1)-\ln(1+1/(N+1))>0$. Also $v_N<u_N$ and $u_N-v_N=\ln(1+1/N)\to0$. The [monotone convergence theorem for sequences](../../sequence-and-series.md#bounded-monotone-sequence-theorem) therefore gives a common finite limit, [Euler's constant](../../complex-analysis.md#euler-s-constant) $\gamma$.

The [integral bounds for Euler's constant](../../complex-analysis.md#integral-bounds-for-euler-s-constant) start at $v_1=1-\ln2$ and $u_1=1$. Strict monotonicity, already at the next index, makes the limit bounds strict:

$$
\boxed{0<1-\ln2<\gamma<1.}
$$

Positivity is explicit because $\ln2=\int_1^2dx/x<1$. This establishes the required limit without assuming its decimal value.

<a id="6/b/image-integral-comparison-and-nested-bounds-for-euler-s-constant"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2-harmonic-logarithmic-bounds.png)

**[Figure 2](#6/b/image-integral-comparison-and-nested-bounds-for-euler-s-constant). Integral comparison and nested bounds for Euler's constant**. Original graph: the height $1/n$ lies between $1/x$ and $1/(x-1)$ on $[n,n+1]$, illustrated for $n=2$. The second panel shows the decreasing upper and increasing lower sequences; their gap tends to zero.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

With $M=2xy^2+4$ and $N=2x^2y-6$, the cross derivatives agree: $M_y=N_x=4xy$. This is an [exact first-order ordinary differential equation](../../differential-equation.md#exact-first-order-ordinary-differential-equation). Integrating $M$ with respect to $x$ gives a potential $x^2y^2+4x+g(y)$; matching $N$ gives $g'=-6$. The implicit solution is

$$
\boxed{x^2y^2+4x-6y=C.}
$$

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Here $M_y=2y$ whereas $N_x=0$, so the equation is not exact. The identity $M_y-N_x=N$ gives the [integrating factor for a differential one-form](../../linear-ordinary-differential-equation.md#integrating-factor-for-a-differential-one-form) $\mu(x)=e^x$. Multiplying makes the left-hand side the [exact differential](../../differential-form.md#exact-differential) of $e^x(y^2-x+1)$. Thus

$$
\boxed{e^x(y^2-x+1)=C,\qquad\text{or}\qquad y^2=x-1+Ce^{-x}.}
$$

For real graph solutions, the right-hand side must be nonnegative; a smooth choice of square-root branch is made on the interval concerned. Finding the factor did not require dividing by $y$ at zero.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

The cross derivatives are both $2y$, so the equation is exact. The function $x\cos x+xy^2$ differentiates to the given one-form. Hence

$$
\boxed{x\cos x+xy^2=C.}
$$

Differentiating this implicit equation checks both coefficients of the [exact differential](../../differential-form.md#exact-differential) directly.

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/i">i</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8/a/i)

Assuming the egg colours are [independent](../../random-variable.md#independent-random-variables) with the same probability $p$, the number of white eggs has the [binomial distribution](../../discrete-probability-distribution.md#binomial-distribution) with four trials. The possibilities are

| Contents | Probability | $W_0B_4$ | $(1-p)^4$ | $W_1B_3$ | $4p(1-p)^3$ | $W_2B_2$ | $6p^2(1-p)^2$ | $W_3B_1$ | $4p^3(1-p)$ | $W_4B_0$ | $p^4$ |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |

The [binomial coefficients](../../binomial-coefficient.md) count which eggs are white. Marginal colour probabilities alone would not determine nest probabilities without the [independence](../../random-variable.md#independent-random-variables) assumption.

<h4 id="8/a/ii">ii</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/a/ii)

For $p=3/4$, the five [probabilities](../../probability-theory.md#probability) in increasing white-egg order are $(1,12,54,108,81)/256$. The largest is $108/256=27/64$, so the **most common nest has three white eggs and one brown egg**, $W_3B_1$.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/i">i</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8/b/i)

The [expected value](../../expected-value.md) of the discrete [uniform distribution](../../continuous-probability-distribution.md#continuous-uniform-distribution) is

$$
\boxed{\mathbb E[X]=\frac{1+2+3+4+5+6}{6}=\frac72.}
$$

<h4 id="8/b/ii">ii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/b/ii)

Using the [sum of squares](../../arithmetic.md#sum-of-squares), the second [moment](../../expected-value.md#moment) is

$$
\boxed{\mathbb E[X^2]=\frac{1+4+9+16+25+36}{6}=\frac{91}{6}.}
$$

<h4 id="8/b/iii">iii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8/b/iii)

The [variance](../../variance.md) is the second [moment](../../expected-value.md#moment) minus the square of the [expected value](../../expected-value.md):

$$
\boxed{\operatorname{Var}(X)=\frac{91}{6}-\left(\frac72\right)^2=\frac{35}{12}.}
$$

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/i">i</h4>

↑ **Parent:** [C](#8/c)

<h5 id="8/c/i/solution">Solution</h5>

↑ **Parent:** [I](#8/c/i)

The function is a [probability density function](../../continuous-probability-distribution.md#probability-density-function), rather than a cumulative distribution: its integral over both intervals must be one. Thus $2\alpha+2\alpha=1$ and

$$
\boxed{\alpha=\frac14.}
$$

<h4 id="8/c/ii">ii</h4>

↑ **Parent:** [C](#8/c)

<h5 id="8/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/c/ii)

The density is symmetric about $7/2$, giving [expected value](../../expected-value.md) $\mathbb E[X]=7/2$. Its second [moment](../../expected-value.md#moment) is $\mathbb E[X^2]=\frac14(\int_1^3x^2dx+\int_4^6x^2dx)=89/6$. Therefore

$$
\boxed{\operatorname{Var}(X)=\frac{89}{6}-\frac{49}{4}=\frac{31}{12}.}
$$

Equivalently, each equally weighted interval has variance $1/3$ and its centre is $3/2$ from the overall mean, giving $1/3+9/4$ by the [law of total variance](../../probability-theory.md#law-of-total-variance).

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

Separate variables away from the equilibrium solutions. Partial fractions give

$$
\frac1{a-b}\ln\left|\frac{y-a}{y-b}\right|=-x+C,\qquad\frac{y-a}{y-b}=K e^{(b-a)x}.
$$

Thus the [constant-coefficient Riccati equation](../../analysis.md#constant-coefficient-riccati-equation) has real solution family

$$
\boxed{y=\frac{a e^{ax}-bK e^{bx}}{e^{ax}-K e^{bx}},\quad K\in\mathbb R,\qquad\text{together with }y=b,}
$$

on intervals where the denominator is nonzero. The value $K=0$ includes $y=a$. Setting $K=e^{(b-a)c}$ recovers the printed expression after factoring out $e^{ac}$. For real $c$ that substitution covers positive $K$ only; negative $K$ gives additional real branches between the equilibria, and the constant solutions must not be discarded when separating variables.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

For the printed family, put $D(x)=e^{a(x+c)}-e^{b(x+c)}$. Its [logarithmic derivative](../../analytic-number-theory.md#logarithmic-derivative) is $D'/D=y$, so $z'=yz$ integrates to

$$
\boxed{z=C_1\bigl[e^{a(x+c)}-e^{b(x+c)}\bigr].}
$$

This includes $z=0$ and is valid on each interval on which the corresponding $y$ is finite. For the full real family, write $z=Ae^{ax}+Be^{bx}$ and $y=z'/z$, with $(A,B)\ne(0,0)$. The pure exponentials include the two equilibrium values of $y$; arbitrary relative coefficient signs include the branches missing from real $c$ in the printed expression.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

When the two roots coincide, $y'=-(y-a)^2$. Separation gives $y=a+1/(x+c)$, and the equilibrium $y=a$ must be added. Integrating $z'=yz$ gives

$$
\boxed{y=a+\frac1{x+c},\quad z=C_1(x+c)e^{ax};\qquad\text{or}\qquad y=a,\quad z=C_1e^{ax}.}
$$

The nonconstant pair is restricted to an interval excluding $x=-c$. Equivalently every nonzero linearizing function is $z=(A+Bx)e^{ax}$, with $y=a+B/(A+Bx)$ wherever its denominator is nonzero.

<h3 id="9/d">d</h3>

↑ **Parent:** [9](#9)

<h4 id="9/d/solution">Solution</h4>

↑ **Parent:** [D](#9/d)

Differentiate $z'=yz$ without dividing by $z$:

$$
z''=(y'+y^2)z=[(a+b)y-ab]z=(a+b)z'-abz.
$$

Thus the [linearization of a Riccati equation](../../analysis.md#linearization-of-a-riccati-equation) gives

$$
\boxed{z''-(a+b)z'+abz=0.}
$$

Its [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is $(\lambda-a)(\lambda-b)$, explaining both the distinct-root exponentials and the repeated-root factor $A+Bx$. Nonzero solutions reconstruct $y=z'/z$ between their zeros; the identically zero $z$ also satisfies the linear equation.

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

A [convergent series](../../sequence-and-series.md#convergent-series) $\sum_{n\geq1}u_n$ has [partial sums](../../sequence-and-series.md#partial-sum) $S_N=\sum_{n=1}^Nu_n$ tending to a finite limit $S$. Explicitly, for every $\varepsilon>0$ there is an integer $N_0$ such that $|S_N-S|<\varepsilon$ whenever $N\geq N_0$. The convergence of the individual terms to zero is necessary but is not sufficient for convergence of the series.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

The [telescoping series](../../sequence-and-series.md#telescoping-series) has partial sum $S_N=w_{N+1}-w_1$. Therefore the necessary and sufficient condition is **that $w_n$ have a finite limit** $L$. The sum is then $L-w_1$.

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

The [comparison test for series](../../sequence-and-series.md#comparison-test-for-series) states that if $0\leq u_n\leq v_n$ for all sufficiently large $n$, convergence of $\sum v_n$ implies convergence of $\sum u_n$. Equivalently, divergence of the smaller nonnegative series forces divergence of the larger one. Finitely many initial terms do not affect either convergence conclusion.

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

Subtract the right side from the left and write $g(x)=1-(1+x)^{-p}-px(1+x)^{-p-1}$. Then $g(0)=0$ and $g'(x)=p(p+1)x(1+x)^{-p-2}>0$ for $x>0$, so the strict inequality follows. Set $x=1/n$ and multiply by $n^{-p}>0$ to obtain

$$
\boxed{n^{-p}-(n+1)^{-p}>p(n+1)^{-p-1},\qquad p,n>0.}
$$

This decreasing-power difference supplies a [telescoping bound for a p-series](../../sequence-and-series.md#telescoping-bound-for-a-p-series).

<h3 id="10/e">e</h3>

↑ **Parent:** [10](#10)

<h4 id="10/e/solution">Solution</h4>

↑ **Parent:** [E](#10/e)

Put $p=k-1>0$. The preceding inequality bounds $n^{-k}<[ (n-1)^{-p}-n^{-p}]/p$ for $n\geq2$. For $N\geq2$, summing the [telescoping series](../../sequence-and-series.md#telescoping-series) gives

$$
\sum_{n=1}^Nn^{-k}<1+\frac{1-N^{-(k-1)}}{k-1}<1+\frac1{k-1}.
$$

These nonnegative partial sums increase and are bounded, so the [monotone convergence theorem for sequences](../../sequence-and-series.md#bounded-monotone-sequence-theorem) proves **convergence for every $k>1$**. This is the [telescoping bound for a p-series](../../sequence-and-series.md#telescoping-bound-for-a-p-series), an alternative to the [integral test](../../sequence-and-series.md#integral-test-for-convergence).

## 11

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/solution">Solution</h4>

↑ **Parent:** [A](#11/a)

Applying the [multivariable chain rule](../../calculus.md#multivariable-chain-rule) at fixed $y$ gives

$$
\boxed{\left(\frac{\partial f}{\partial x}\right)_y=\left(\frac{\partial f}{\partial u}\right)_v\left(\frac{\partial u}{\partial x}\right)_y+\left(\frac{\partial f}{\partial v}\right)_u\left(\frac{\partial v}{\partial x}\right)_y.}
$$

The held-fixed variables distinguish the two coordinate descriptions; the same scalar function is being differentiated.

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/solution">Solution</h4>

↑ **Parent:** [B](#11/b)

Differentiate the first-order [chain rule](../../calculus.md#chain-rule) again, including derivatives of the coordinate coefficients. The [second derivatives under a two-variable coordinate change](../../calculus.md#second-derivatives-under-a-two-variable-coordinate-change) are

$$
\boxed{f_{xx}=f_{uu}u_x^2+2f_{uv}u_xv_x+f_{vv}v_x^2+f_u\,u_{xx}+f_v\,v_{xx},}
$$

and

$$
\boxed{f_{yy}=f_{uu}u_y^2+2f_{uv}u_yv_y+f_{vv}v_y^2+f_u\,u_{yy}+f_v\,v_{yy}.}
$$

The last two terms account for derivatives of the coordinate functions; they vanish for an [affine map](../../geometry-and-topology.md#affine-map). Smoothness justifies equality of the two mixed partial derivatives.

<h3 id="11/c">c</h3>

↑ **Parent:** [11](#11)

<h4 id="11/c/solution">Solution</h4>

↑ **Parent:** [C](#11/c)

For [polar coordinates](../../multivariable-calculus.md#polar-coordinates) with $u>0$, $\partial_x=\cos v\,\partial_u-(\sin v/u)\partial_v$ and $\partial_y=\sin v\,\partial_u+(\cos v/u)\partial_v$. Write $c=\cos v$, $s=\sin v$. Applying these operators twice, including their variable coefficients, gives the [Cartesian second derivatives in polar coordinates](../../multivariable-calculus.md#cartesian-second-derivatives-in-polar-coordinates):

$$
\boxed{f_{xx}=c^2f_{uu}-\frac{2sc}{u}f_{uv}+\frac{s^2}{u^2}f_{vv}+\frac{s^2}{u}f_u+\frac{2sc}{u^2}f_v,}
$$



$$
\boxed{f_{yy}=s^2f_{uu}+\frac{2sc}{u}f_{uv}+\frac{c^2}{u^2}f_{vv}+\frac{c^2}{u}f_u-\frac{2sc}{u^2}f_v.}
$$

In particular their sum is the [Laplacian in polar coordinates](../../multivariable-calculus.md#laplacian-in-polar-coordinates), $f_{uu}+f_u/u+f_{vv}/u^2$.

<h3 id="11/d">d</h3>

↑ **Parent:** [11](#11)

<h4 id="11/d/solution">Solution</h4>

↑ **Parent:** [D](#11/d)

The substitution gives $x^2-y^2=u^2\cos2v$. For this function $f_{uu}=2\cos2v$, $f_u/u=2\cos2v$, and $f_{vv}/u^2=-4\cos2v$, whose sum is zero. Thus it satisfies the polar form of [Laplace's equation](../../partial-differential-equation.md#laplace-equation) for $u>0$. The apparent coordinate singularity at $u=0$ does not make the original Cartesian [polynomial](../../polynomial.md) singular; it is a smooth [harmonic function](../../partial-differential-equation.md#harmonic-function) through the origin.

## 12

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12/a">a</h3>

↑ **Parent:** [12](#12)

<h4 id="12/a/solution">Solution</h4>

↑ **Parent:** [A](#12/a)

Let $D=1+x^2+y^2$. The [gradient](../../multivariable-calculus.md#gradient) has components $f_x=[D-2x(x+y)]/D^2$ and $f_y=[D-2y(x+y)]/D^2$. At a [critical point](../../analysis.md#critical-point), subtraction gives $(x-y)(x+y)=0$. The case $x+y=0$ cannot make either numerator zero, so $x=y=t$. The remaining equation is $1+2t^2=4t^2$, giving

$$
\boxed{(x,y)=(1/\sqrt2,1/\sqrt2),\quad f=1/\sqrt2;\qquad(x,y)=(-1/\sqrt2,-1/\sqrt2),\quad f=-1/\sqrt2.}
$$

These are the only stationary points; the denominator is positive everywhere.

<h3 id="12/b">b</h3>

↑ **Parent:** [12](#12)

<h4 id="12/b/solution">Solution</h4>

↑ **Parent:** [B](#12/b)

At $(t,t)$ with $t^2=1/2$, differentiating the [gradient](../../multivariable-calculus.md#gradient) yields the [Hessian matrix](../../multivariable-calculus.md#hessian-matrix) $H=-tI$. At the positive point it is [negative definite](../../quadratic-form.md#negative-definite-matrix), and at the negative point it is [positive-definite](../../bilinear-form.md#positive-definite-bilinear-form); in both cases $f_{xy}=0$ and $\det H=1/2$. Therefore the **positive point is a maximum, the negative point is a minimum, and there are no saddle points**.

They are global extrema: with $r=\sqrt{x^2+y^2}$, the [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $|f|\leq\sqrt2r/(1+r^2)\leq1/\sqrt2$, with equality at exactly those two points. This is the extremum bound underlying the [level sets of a linear numerator over a radial quadratic](../../topology.md#level-sets-of-a-linear-numerator-over-a-radial-quadratic).

<h3 id="12/c">c</h3>

↑ **Parent:** [12](#12)

<h4 id="12/c/solution">Solution</h4>

↑ **Parent:** [C](#12/c)

For a nonzero level $h$, completing the square gives

$$
\boxed{\left(x-\frac1{2h}\right)^2+\left(y-\frac1{2h}\right)^2=\frac1{2h^2}-1.}
$$

Thus the [level sets of a linear numerator over a radial quadratic](../../topology.md#level-sets-of-a-linear-numerator-over-a-radial-quadratic) are circles centred on $y=x$, real only for $0<|h|\leq1/\sqrt2$. The extreme levels shrink to points. The zero contour is the straight line $x+y=0$, separating positive and negative heights; near it, small nonzero levels are large circles. Heights tend to zero at infinity.

<a id="12/c/image-circular-nonzero-contours-around-the-two-extrema-of-a-rational-height-function"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2-rational-height-contours.png)

**[Figure 3](#12/c/image-circular-nonzero-contours-around-the-two-extrema-of-a-rational-height-function). Circular nonzero contours around the two extrema of a rational height function**. Original contour plot. Blue positive and orange negative circles surround the marked maximum and minimum; the black line is the zero contour. Circle centres lie on $y=x$.

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
