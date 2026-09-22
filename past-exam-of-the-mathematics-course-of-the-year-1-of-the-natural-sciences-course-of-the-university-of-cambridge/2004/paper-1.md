# Paper 1

↑ **Parent:** [2004](../2004.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2004/PaperNST_IA_1.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2004/PaperNST_IA_1.pdf)

The printed label `99E` is treated as question 9.

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
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
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
    - [iv](#5/b/iv)
      - [Solution](#5/b/iv/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
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
    - [iv](#7/b/iv)
      - [Solution](#7/b/iv/solution)
- [8](#8)
  - [i](#8/i)
    - [Solution](#8/i/solution)
  - [ii](#8/ii)
    - [Solution](#8/ii/solution)
  - [iii](#8/iii)
    - [Solution](#8/iii/solution)
- [9](#9)
  - [a](#9/a)
    - [i](#9/a/i)
      - [Solution](#9/a/i/solution)
    - [ii](#9/a/ii)
      - [Solution](#9/a/ii/solution)
    - [iii](#9/a/iii)
      - [Solution](#9/a/iii/solution)
    - [iv](#9/a/iv)
      - [Solution](#9/a/iv/solution)
    - [v](#9/a/v)
      - [Solution](#9/a/v/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
    - [i](#9/b/i)
      - [Solution](#9/b/i/solution)
    - [ii](#9/b/ii)
      - [Solution](#9/b/ii/solution)
    - [iii](#9/b/iii)
      - [Solution](#9/b/iii/solution)
  - [c](#9/c)
    - [i](#9/c/i)
      - [Solution](#9/c/i/solution)
    - [ii](#9/c/ii)
      - [Solution](#9/c/ii/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
    - [i](#10/b/i)
      - [Solution](#10/b/i/solution)
    - [ii](#10/b/ii)
      - [Solution](#10/b/ii/solution)
    - [iii](#10/b/iii)
      - [Solution](#10/b/iii/solution)
  - [c](#10/c)
    - [i](#10/c/i)
      - [Solution](#10/c/i/solution)
    - [ii](#10/c/ii)
      - [Solution](#10/c/ii/solution)
- [11](#11)
  - [a](#11/a)
    - [Solution](#11/a/solution)
  - [b](#11/b)
    - [Solution](#11/b/solution)
  - [c](#11/c)
    - [Solution](#11/c/solution)
- [12](#12)
  - [Solution](#12/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

In components, the [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) is

$$
\mathbf a\cdot(\mathbf b\times\mathbf c)=a_1(b_2c_3-b_3c_2)+a_2(b_3c_1-b_1c_3)+a_3(b_1c_2-b_2c_1).
$$

It is the [determinant](../../multilinear-algebra.md#determinant) with rows $\mathbf a,\mathbf b,\mathbf c$. A cyclic permutation of the rows has positive sign, so $\mathbf a\cdot(\mathbf b\times\mathbf c)=\mathbf c\cdot(\mathbf a\times\mathbf b)=(\mathbf a\times\mathbf b)\cdot\mathbf c$. Equivalently the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) expression $\epsilon_{ijk}a_ib_jc_k$ is unchanged by that cyclic relabeling.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Take $P=(2,-1,2)$, $Q=(1,2,3)$ and $R=(4,1,0)$. The two plane directions are $Q-P=(-1,3,1)$ and $R-P=(2,2,-2)$. Their [cross product](../../vector-space.md#cross-product) is $(-8,0,-8)$, so a [normal vector](../../differential-geometry.md#normal-vector) is $(1,0,1)$. The [Cartesian equation of a plane](../../geometry-and-topology.md#cartesian-equation-of-a-plane) is therefore

$$
\boxed{x+z=4.}
$$

Each given point satisfies it, and the nonzero cross product confirms that the points determine a unique plane.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [volume](../../geometry-and-topology.md#volume) of a [parallelepiped](../../euclidean-geometry.md#parallelepiped) is the absolute [scalar triple product](../../multilinear-algebra.md#scalar-triple-product) of its edge vectors. Here

$$
\boxed{V=\left|\det\begin{pmatrix}1&3&0\\-1&3&-2\\0&1&1\end{pmatrix}\right|=|8|=8.}
$$

The absolute value removes the orientation of the chosen edge ordering.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [comparison test for series](../../sequence-and-series.md#comparison-test-for-series) says that $0\leq v_n\leq Cw_n$ eventually and convergence of $\sum w_n$ imply convergence of $\sum v_n$. Conversely, an eventual positive lower comparison with a divergent positive series proves divergence. The [ratio test](../../sequence-and-series.md#ratio-test) uses $L=\lim_{n\to\infty}v_{n+1}/v_n$: $L<1$ proves convergence, $L>1$ proves divergence, and $L=1$ is inconclusive. Removing finitely many initial zero terms does not affect these conclusions.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For $n\geq1$, $\ln n\leq n$ and $2n^3+1\geq2n^3$. Hence $0\leq\ln n/(2n^3+1)\leq1/(2n^2)$. The comparison [p-series](../../sequence-and-series.md#p-series) has exponent two and converges, so **the series converges** by the [comparison test](../../sequence-and-series.md#direct-comparison-test).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The summand $n/(n+4)$ tends to one rather than zero. The [term test for divergence](../../sequence-and-series.md#term-test-for-divergence) therefore proves **the series diverges**. A ratio limit equal to one would be inconclusive and is unnecessary here.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The elementary bound $|\sin t|\leq|t|$ gives $0\leq\sin^2(1/n)\leq1/n^2$. Comparison with a convergent [p-series](../../sequence-and-series.md#p-series) proves **the series converges**.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For $n\geq1$, the ratio of positive terms is

$$
\frac{(n+1)^4e^{-(n+1)^2}}{n^4e^{-n^2}}=\left(1+\frac1n\right)^4e^{-2n-1}\longrightarrow0.
$$

The [ratio test](../../sequence-and-series.md#ratio-test) proves **the series converges**. Its zero term at $n=0$ has no effect.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For an oriented piecewise smooth surface $S$ with boundary $C=\partial S$ and a vector field $\mathbf A$ with continuous first derivatives near $S$, the [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) states

$$
\boxed{\oint_C\mathbf A\cdot d\mathbf r=\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS.}
$$

Here $\mathbf n$ is the chosen unit [normal vector](../../differential-geometry.md#normal-vector), $dS$ the positive area element, and $d\mathbf r$ the oriented tangent line element. The traversal of $C$ follows the right-hand rule relative to the surface orientation.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Differentiate the Cartesian components to calculate the [curl](../../multivariable-calculus.md#curl):

$$
\nabla\times\mathbf A=\left(-2yz-(-2yz),\ 0-0,\ 0-(-1)\right)=\boxed{(0,0,1)}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Orient the three faces outward from the tetrahedron. The two coordinate-plane faces have normals parallel to $-\mathbf e_x$ or $-\mathbf e_y$, so their flux of the [curl](../../multivariable-calculus.md#curl) is zero. On the inclined face $z=1-x-y$, its upward vector area is $(1,1,1)\,dx\,dy$, with $x,y\geq0$, $x+y\leq1$. Thus the direct [surface integral](../../multivariable-calculus.md#surface-integral) is

$$
\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS=\int_0^1\int_0^{1-x}1\,dy\,dx=\frac12.
$$

This surface induces the counterclockwise boundary $O\to X\to Y\to O$ viewed from above, where $X=(1,0,0)$ and $Y=(0,1,0)$. At $z=0$, $\mathbf A=(2x-y,0,0)$. On $OX$, take $(x,y)=(t,0)$, giving integral $\int_0^12t\,dt=1$. On $XY$, take $(x,y)=(1-t,t)$, giving $\int_0^1(-2+3t)dt=-1/2$. On $YO$, $dx=0$ and the integral vanishes. Therefore

$$
\boxed{\oint_C\mathbf A\cdot d\mathbf r=1-\frac12+0=\frac12=\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS.}
$$

Both sides have been calculated directly, verifying the [Stokes theorem](../../multivariable-calculus.md#stokes-theorem) with consistent orientations.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [partial fraction decomposition](../../isolated-singularity.md#partial-fraction-decomposition) is $(x-1)/[x(x+1)]=-1/x+2/(x+1)$. Since both endpoints are positive, integration gives

$$
\boxed{\int_a^b\frac{x-1}{x(x+1)}dx=\left[-\ln x+2\ln(x+1)\right]_a^b=\ln\frac{a(b+1)^2}{b(a+1)^2}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use $\tan^2x=\sec^2x-1$ and the derivative of the [tangent](../../geometry-and-topology.md#tangent):

$$
\boxed{\int\tan^2x\,dx=\tan x-x+C.}
$$

The antiderivative applies on each interval avoiding the poles of $\tan x$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $1<x<e$, the [natural logarithm](../../calculus.md#natural-logarithm) satisfies $0<\ln x<1$. Squaring therefore decreases its value, while $\ln(x^2)=2\ln x$. Pointwise comparison gives $(\ln x)^2<\ln x<\ln(x^2)$, so

$$
\boxed{I_3<I_1<I_2.}
$$

As a check, [integration by parts](../../calculus.md#integration-by-parts) gives $I_1=1$, $I_2=2$ and $I_3=e-2$, consistent with this order.

<a id="4/c/image-pointwise-ordering-of-the-three-logarithmic-integrands"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1-logarithm-comparison.png)

**[Figure 1](#4/c/image-pointwise-ordering-of-the-three-logarithmic-integrands). Pointwise ordering of the three logarithmic integrands**. Original plot on $[1,e]$. The natural logarithm rises from zero to one, so its square lies below it, and twice the logarithm lies above it. Integrating preserves the strict order.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [cumulative distribution function](../../probability-distribution.md#cumulative-distribution-function) must tend to one at infinity, so $\boxed{k=1}$. Differentiation gives the [probability density function](../../continuous-probability-distribution.md#probability-density-function) $f_X(x)=e^{-x}$ for $x>0$ and zero for $x<0$; there is no atom at zero. This is an [exponential distribution](../../continuous-probability-distribution.md#exponential-distribution) of rate one. Its first two moments are $\int_0^\infty xe^{-x}dx=1$ and $\int_0^\infty x^2e^{-x}dx=2$, so

$$
\boxed{\mathbb E[X]=1,\qquad\operatorname{Var}(X)=2-1^2=1.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

The continuous nonnegative part has total mass $\lim_{y\to\infty}(1-e^{-y})/2=1/2$. The remaining mass is at $-1$, giving $\boxed{m=1/2}$. This is a [mixed probability distribution](../../probability-distribution.md#mixed-probability-distribution), specifically a [mixture of a point mass and an exponential distribution](../../probability-distribution.md#mixture-of-a-point-mass-and-an-exponential-distribution); its atom must be included in normalization.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Include the negative atom as well as the continuous part in the [expected value](../../expected-value.md):

$$
\boxed{\mathbb E[Y]=\frac12(-1)+\frac12\int_0^\infty ye^{-y}dy=-\frac12+\frac12=0.}
$$

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

The second moment of the [mixed probability distribution](../../probability-distribution.md#mixed-probability-distribution) is $\mathbb E[Y^2]=\tfrac12(-1)^2+\tfrac12\int_0^\infty y^2e^{-y}dy=1/2+1=3/2$. Since the mean is zero,

$$
\boxed{\operatorname{Var}(Y)=\frac32.}
$$

<h4 id="5/b/iv">iv</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/b/iv)

The conditioning event selects the exponential component: $P(Y\geq0)=1/2$ and $P(Y\geq1)=e^{-1}/2$. Thus [conditional probability](../../probability-theory.md#conditional-probability) gives

$$
\boxed{P(Y\geq1\mid Y\geq0)=\frac{e^{-1}/2}{1/2}=e^{-1}.}
$$

The atom at $-1$ is excluded by the conditioning event.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

The [determinant](../../multilinear-algebra.md#determinant) is $k-6$, so for $k\ne6$ the [inverse matrix](../../matrix-inverse.md) is

$$
\boxed{A^{-1}=\frac1{k-6}\begin{pmatrix}k&-3&0\\-2&1&0\\-4k&12&k-6\end{pmatrix}.}
$$

The specified equations use $k=4$, with right-hand side $(2,3,1)^T$. Multiplying by $A^{-1}|_{k=4}$ gives

$$
\boxed{(x,y,z)=\left(\frac12,\frac12,-1\right).}
$$

In particular the parameter in the inverse formula must be set to four, not left arbitrary for this numerical system.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

For $k=1$, the required right-hand matrix has twice the first row of $A$, the same second row, and twice the third row. Left multiplication scales rows, so

$$
\boxed{B=\operatorname{diag}(2,1,2).}
$$

Equivalently, right multiply the given equation $BA=C$ by $A^{-1}$ to obtain the same answer.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

At $k=6$, the second row is twice the first. The independent equations are $x+3y=0$ and $4x+z=0$. Therefore the [null space](../../kernel-of-a-linear-map.md) is

$$
\boxed{(x,y,z)=t(-3,1,12),\qquad t\in\mathbb R.}
$$

It has dimension one, consistent with matrix rank two.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

The [trace](../../linear-algebra.md#matrix-trace) is unchanged by transposition and is cyclic under a product. With $S^T=S$ and $A^T=-A$,

$$
\operatorname{tr}(AS)=\operatorname{tr}[(AS)^T]=\operatorname{tr}(-SA)=-\operatorname{tr}(AS).
$$

Thus $\boxed{\operatorname{tr}(AS)=0}$. In components this is the vanishing contraction of a [symmetric tensor](../../multilinear-algebra.md#symmetric-tensor) with an [antisymmetric tensor](../../multilinear-algebra.md#antisymmetric-tensor).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

The [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) vanishes when two indices coincide, so

$$
\boxed{\operatorname{tr}M=\delta_{ii}+2\epsilon_{iik}a_k=3.}
$$

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

The antisymmetric contribution is the negative of twice the [cross-product matrix](../../linear-algebra.md#cross-product-matrix) for $\mathbf a$:

$$
M=\begin{pmatrix}1&2a_3&-2a_2\\-2a_3&1&2a_1\\2a_2&-2a_1&1\end{pmatrix}.
$$

The [cross-product matrix spectrum](../../linear-algebra.md#cross-product-matrix-spectrum) is $0,\pm i|\mathbf a|$, so $M$ has eigenvalues $1,1\pm2i|\mathbf a|$. Multiplication gives

$$
\boxed{\det M=1+4|\mathbf a|^2.}
$$

Direct expansion of the displayed matrix yields the same real positive determinant.

<h4 id="7/b/iii">iii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/b/iii)

Use index contraction:

$$
(MN)_{ij}=(\delta_{ik}+2\epsilon_{ik\ell}a_\ell)a_kb_j=a_ib_j+2\epsilon_{ik\ell}a_ka_\ell b_j=N_{ij}.
$$

The last term vanishes because $a_ka_\ell$ is symmetric in the contracted indices while the [Levi-Civita symbol](../../multivariable-calculus.md#levi-civita-symbol) is antisymmetric. Hence $\boxed{MN=N}$.

<h4 id="7/b/iv">iv</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#7/b/iv)

Taking [determinants](../../multilinear-algebra.md#determinant) in $MN=N$ gives $(\det M-1)\det N=0$. Here $\det M-1=4|\mathbf a|^2>0$ because $\mathbf a\ne0$, so $\boxed{\det N=0}$. This also agrees with $N=\mathbf a\mathbf b^T$ being an [outer product](../../vector-space.md#outer-product) of rank one.

## 8

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8/i">i</h3>

↑ **Parent:** [8](#8)

<h4 id="8/i/solution">Solution</h4>

↑ **Parent:** [I](#8/i)

On the straight path $\mathbf r(t)=(t,t,t)$, $0\leq t\leq1$, both fields restrict to $(3t^5,2t^5,t^5)$. Dotting with $\mathbf r'=(1,1,1)$ gives

$$
\boxed{\int\mathbf F\cdot d\mathbf r=\int\mathbf G\cdot d\mathbf r=\int_0^16t^5dt=1.}
$$

<h3 id="8/ii">ii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8/ii)

For $\mathbf r(t)=(t,t^2,t^2)$, the velocity is $(1,2t,2t)$. Because $y=z$ throughout this path, both fields again agree pointwise, now as $(3t^8,2t^7,t^7)$. Thus

$$
\boxed{\int\mathbf F\cdot d\mathbf r=\int\mathbf G\cdot d\mathbf r=\int_0^1(3t^8+4t^8+2t^8)dt=1.}
$$

These equal values alone do not establish [path independence](../../multivariable-calculus.md#path-independence) for either field on all of space.

<h3 id="8/iii">iii</h3>

↑ **Parent:** [8](#8)

<h4 id="8/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8/iii)

Direct differentiation gives $\boxed{\Phi=x^3y^2z+C}$ with $\nabla\Phi=\mathbf G$, so $\mathbf G$ is a [conservative vector field](../../multivariable-calculus.md#conservative-vector-field) and its integral depends only on the endpoints. In contrast,

$$
\nabla\times\mathbf F=\left(-2x^3y,\ 3x^2z(2y-z),\ 3x^2z(2y-z)\right)
$$

is nonzero, for example at $(1,1,1)$. Thus **$\mathbf F$ is not conservative**. Both earlier paths lie in the surface $y=z$, where the two fields happen to coincide. This illustrates why [coinciding path integrals need not imply a conservative field](../../multivariable-calculus.md#coinciding-path-integrals-need-not-imply-a-conservative-field).

## 9

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/i">i</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/i/solution">Solution</h5>

↑ **Parent:** [I](#9/a/i)

By [Euler's formula](../../complex-analysis.md#euler-s-formula), $\boxed{e^{2i}=\cos2+i\sin2}$, with the angle measured in radians.

<h4 id="9/a/ii">ii</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/a/ii)

Since the arguments of $-1$ are $(2k+1)\pi$, the [complex logarithm](../../analysis.md#complex-logarithm) has values $\boxed{\log(-1)=i(2k+1)\pi}$ for $k\in\mathbb Z$. The principal value is $\boxed{i\pi}$.

<h4 id="9/a/iii">iii</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9/a/iii)

The modulus of $i$ is one and its arguments are $\pi/2+2k\pi$. Thus $\boxed{\log i=i(\pi/2+2k\pi)}$, with principal value $\boxed{i\pi/2}$.

<h4 id="9/a/iv">iv</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#9/a/iv)

For the positive real base ten, use its real [natural logarithm](../../calculus.md#natural-logarithm). Then [Euler's formula](../../complex-analysis.md#euler-s-formula) gives

$$
\boxed{10^i=e^{i\ln10}=\cos(\ln10)+i\sin(\ln10).}
$$

<h4 id="9/a/v">v</h4>

↑ **Parent:** [A](#9/a)

<h5 id="9/a/v/solution">Solution</h5>

↑ **Parent:** [V](#9/a/v)

Using a value of the [complex logarithm](../../analysis.md#complex-logarithm), $i^i=\exp(i\log i)=\exp[-(\pi/2+2k\pi)]$. Thus every logarithmic-branch value is real and positive:

$$
\boxed{i^i=e^{-\pi/2-2k\pi}+0i,\quad k\in\mathbb Z.}
$$

The principal value is $\boxed{e^{-\pi/2}}$.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

The [hyperbolic cosine](../../calculus.md#hyperbolic-cosine) and [hyperbolic sine](../../calculus.md#hyperbolic-sine) are defined by $\boxed{\cosh x=(e^x+e^{-x})/2,\quad\sinh x=(e^x-e^{-x})/2}$. Their quotient is $\tanh x=\sinh x/\cosh x$.

<h4 id="9/b/i">i</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9/b/i)

Expand the two squares using the exponential definitions:

$$
\boxed{\cosh^2x-\sinh^2x=\frac{(e^x+e^{-x})^2-(e^x-e^{-x})^2}{4}=1.}
$$

<h4 id="9/b/ii">ii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/b/ii)

The exponential definitions show that $\sinh$ is [odd](../../calculus.md#odd-function) and $\cosh$ is [even](../../calculus.md#even-function). Their quotient therefore satisfies $\boxed{\tanh(-x)=-\tanh x}$.

<h4 id="9/b/iii">iii</h4>

↑ **Parent:** [B](#9/b)

<h5 id="9/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9/b/iii)

Differentiating the exponential definition gives $\boxed{(\cosh x)'=(e^x-e^{-x})/2=\sinh x}$.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/i">i</h4>

↑ **Parent:** [C](#9/c)

<h5 id="9/c/i/solution">Solution</h5>

↑ **Parent:** [I](#9/c/i)

The fifth power of the [odd](../../calculus.md#odd-function) function $\tanh x$ is odd and continuous. Its integral over the symmetric interval is therefore $\boxed{\int_{-1000}^{1000}\tanh^5x\,dx=0}$.

<h4 id="9/c/ii">ii</h4>

↑ **Parent:** [C](#9/c)

<h5 id="9/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9/c/ii)

The derivative of $\ln\cosh x$ is $\tanh x$. Since $\cosh(\ln2)=(2+1/2)/2=5/4$,

$$
\boxed{\int_0^{\ln2}\tanh x\,dx=[\ln\cosh x]_0^{\ln2}=\ln\frac54.}
$$

## 10

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Take the real part of [De Moivre's theorem](../../analysis.md#de-moivre-s-theorem). Put $c=\cos\theta$ and use $\sin^2\theta=1-c^2$:

$$
\cos5\theta=c^5-10c^3(1-c^2)+5c(1-c^2)^2=\boxed{16\cos^5\theta-20\cos^3\theta+5\cos\theta}.
$$

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

The modulus equation says that $z$ has fixed distance eight from $-1-i$. Thus its locus is **a circle of radius eight centered at $(-1,-1)$**, with Cartesian equation $(x+1)^2+(y+1)^2=64$.

<a id="10/b/image-the-original-circle-a-horizontal-stretch-a-translation-and-a-quarter-turn"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1-complex-loci.png)

**[Figure 2](#10/b/image-the-original-circle-a-horizontal-stretch-a-translation-and-a-quarter-turn). The original circle, a horizontal stretch, a translation and a quarter-turn**. Original complex-plane loci. The map $u=2x+iy$ stretches only the horizontal coordinate; $v=z+4+3i$ translates the circle; $w=iv$ rotates that translated circle about the origin. Marked dots show each center.

<h4 id="10/b/i">i</h4>

↑ **Parent:** [B](#10/b)

<h5 id="10/b/i/solution">Solution</h5>

↑ **Parent:** [I](#10/b/i)

Writing $u=X+iY$ gives $X=2x$, $Y=y$. Substitute $x=X/2$, $y=Y$ into the original circle equation. This [affine image of a circle](../../euclidean-geometry.md#affine-image-of-a-circle) is the [ellipse](../../euclidean-geometry.md#ellipse)

$$
\boxed{\frac{(X+2)^2}{16^2}+\frac{(Y+1)^2}{8^2}=1,}
$$

centered at $(-2,-1)$ with horizontal semiaxis sixteen and vertical semiaxis eight. The map covers the whole ellipse as $z$ covers the circle.

<h4 id="10/b/ii">ii</h4>

↑ **Parent:** [B](#10/b)

<h5 id="10/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10/b/ii)

The complex translation adds four to the real coordinate and three to the imaginary coordinate. The locus is therefore **a circle centered at $(3,2)$ with radius eight**:

$$
\boxed{(X-3)^2+(Y-2)^2=64.}
$$

<h4 id="10/b/iii">iii</h4>

↑ **Parent:** [B](#10/b)

<h5 id="10/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10/b/iii)

Multiplication by $i$ rotates the plane counterclockwise through $\pi/2$. The center $3+2i$ maps to $-2+3i$, while distances are preserved. Thus the locus is **a circle centered at $(-2,3)$ with radius eight**:

$$
\boxed{(X+2)^2+(Y-3)^2=64.}
$$

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/i">i</h4>

↑ **Parent:** [C](#10/c)

<h5 id="10/c/i/solution">Solution</h5>

↑ **Parent:** [I](#10/c/i)

For $ab\ne0$, elimination of the trigonometric parameter gives

$$
\boxed{\frac{x^2}{a^2}+\frac{y^2}{b^2}=1.}
$$

As real $\theta$ varies, the whole [ellipse](../../euclidean-geometry.md#ellipse) is traced, with semiaxes $|a|,|b|$. Signs of $a,b$ affect the traversal direction but not the set. If $a=0$, the locus is the vertical segment $x=0$, $|y|\leq|b|$; if $b=0$, it is the horizontal segment $y=0$, $|x|\leq|a|$. Both zero give only the origin.

<h4 id="10/c/ii">ii</h4>

↑ **Parent:** [C](#10/c)

<h5 id="10/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10/c/ii)

For $ab\ne0$, the hyperbolic identity gives $x^2/a^2-y^2/b^2=1$. The [hyperbolic parametrization of a hyperbola](../../euclidean-geometry.md#hyperbolic-parametrization-of-a-hyperbola) also imposes $x/a=\cosh\theta\geq1$, so the exact traced locus is

$$
\boxed{\frac{x^2}{a^2}-\frac{y^2}{b^2}=1,\qquad\frac xa\geq1.}
$$

It is only one branch: the right branch for $a>0$ and the left branch for $a<0$. Its vertex is $(a,0)$ and its asymptotes are $y=\pm(b/a)x$. If $a=0$, $b\ne0$, the entire vertical axis is traced. If $b=0$, $a\ne0$, the locus is the ray $y=0$, $x/a\geq1$. Both zero give the origin.

<a id="10/c/ii/image-a-trigonometric-ellipse-and-the-single-hyperbolic-branch-traced-by-real-parameters"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1-ellipse-hyperbola.png)

**[Figure 3](#10/c/ii/image-a-trigonometric-ellipse-and-the-single-hyperbolic-branch-traced-by-real-parameters). A trigonometric ellipse and the single hyperbolic branch traced by real parameters**. Original example with $a=2,b=1$. The ellipse is closed, whereas $(a\cosh\theta,b\sinh\theta)$ traces only the right branch of the hyperbola. Dashed lines show its two asymptotes.

## 11

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/solution">Solution</h4>

↑ **Parent:** [A](#11/a)

First retain the [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) solution $y=0$. For $y\ne0$ and $x\ne\pm1$, [separation of variables](../../partial-differential-equation.md#separation-of-variables) gives $\int y^{-2}dy=\int x/(1-x^2)dx$, hence $-1/y=-\tfrac12\ln|1-x^2|+C$. Renaming the constant yields

$$
\boxed{y=0,\qquad\text{or}\qquad y=\frac2{\ln|1-x^2|+C}.}
$$

A nonzero solution is considered on a regular interval avoiding $x=\pm1$ and zeros of its denominator. The zero solution itself extends through both singular points of the divided equation.

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/solution">Solution</h4>

↑ **Parent:** [B](#11/b)

The initial value is positive, so set $z=y^{-2}$. The [chain rule](../../calculus.md#chain-rule) gives $z'=-2y^{-3}y'=-2(y^{-2}-1)$, making $z'+2z=2$. Its solution is $z=1+Ce^{-2x}$. Since $y(0)=1/2$, $z(0)=4$ and $C=3$. Choosing the positive branch gives

$$
\boxed{y(x)=\frac1{\sqrt{1+3e^{-2x}}},\qquad x\in\mathbb R.}
$$

It satisfies the initial condition and approaches the stable positive equilibrium one as $x\to\infty$.

<h3 id="11/c">c</h3>

↑ **Parent:** [11](#11)

<h4 id="11/c/solution">Solution</h4>

↑ **Parent:** [C](#11/c)

On an interval with $\sin x\ne0$, divide by $\sin x$ and use [integrating factor](../../linear-ordinary-differential-equation.md#integrating-factor) $1/\sin x$. Then

$$
\left(\frac y{\sin x}\right)'=\frac{\cos^3x}{\sin^2x}.
$$

Put $u=\sin x$ in the integral: $\int\cos^3x\,dx/\sin^2x=\int(u^{-2}-1)du=-u^{-1}-u+C$. Multiplying back gives

$$
\boxed{y(x)=-1-\sin^2x+C\sin x.}
$$

Although the derivation divided by $\sin x$, this final expression is smooth and directly satisfies the original undivided equation at every real $x$, including multiples of $\pi$.

## 12

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12/solution">Solution</h3>

↑ **Parent:** [12](#12)

Use [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system) with $dV=r\,dr\,d\theta\,dz$, $0\leq\theta<2\pi$, $0\leq z\leq h$ and $0\leq r\leq a(1-z/h)$. Set $s=1-z/h$. Integrating first over radius gives the mass per unit height

$$
\frac{dM}{dz}=2\pi\rho_0\left[\frac{a^2s^2}{2}+\frac{a^2s^3}{3}\right]=\pi\rho_0a^2\left(s^2+\frac23s^3\right).
$$

Therefore

$$
\boxed{M=\pi\rho_0a^2h\int_0^1\left(s^2+\frac23s^3\right)ds=\frac12\pi\rho_0a^2h.}
$$

For the first moment about the base, use $z=h(1-s)$:

$$
Md=\pi\rho_0a^2h^2\int_0^1(1-s)\left(s^2+\frac23s^3\right)ds=\frac7{60}\pi\rho_0a^2h^2.
$$

Dividing by the total mass gives

$$
\boxed{d=\frac{7h}{30}.}
$$

The [center of mass of a cone with a power-law radial density](../../classical-mechanics.md#center-of-mass-of-a-cone-with-a-power-law-radial-density) gives an independent decomposition: the uniform-density component has centroid $h/4$, while the component proportional to $r$ has centroid $h/5$ and half as much mass. Their mass-weighted mean is $7h/30$. Density increasing toward the wider outer parts consequently moves the center below the uniform cone's $h/4$.

## ↑ Ancestors (10)

1. [2004](../2004.md)
2. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
