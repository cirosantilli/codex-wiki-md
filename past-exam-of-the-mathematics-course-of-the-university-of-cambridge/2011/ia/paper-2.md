# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2011/PaperIA_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2011/PaperIA_2.pdf)

**Table of contents**

- [Section I](#section-i)
  - [1A](#1a)
    - [a](#1a/a)
      - [Solution](#1a/a/solution)
    - [b](#1a/b)
      - [Solution](#1a/b/solution)
  - [2A](#2a)
    - [a](#2a/a)
      - [Solution](#2a/a/solution)
    - [b](#2a/b)
      - [Solution](#2a/b/solution)
  - [3F](#3f)
    - [a](#3f/a)
      - [Solution](#3f/a/solution)
    - [b](#3f/b)
      - [Solution](#3f/b/solution)
    - [c](#3f/c)
      - [Solution](#3f/c/solution)
  - [4F](#4f)
    - [Solution](#4f/solution)
- [Section II](#section-ii)
  - [5A](#5a)
    - [a](#5a/a)
      - [Solution](#5a/a/solution)
    - [b](#5a/b)
      - [Solution](#5a/b/solution)
  - [6A](#6a)
    - [a](#6a/a)
      - [Solution](#6a/a/solution)
    - [b](#6a/b)
      - [i](#6a/b/i)
        - [Solution](#6a/b/i/solution)
      - [ii](#6a/b/ii)
        - [Solution](#6a/b/ii/solution)
      - [iii](#6a/b/iii)
        - [Solution](#6a/b/iii/solution)
      - [iv](#6a/b/iv)
        - [Solution](#6a/b/iv/solution)
  - [7A](#7a)
    - [a](#7a/a)
      - [Solution](#7a/a/solution)
    - [b](#7a/b)
      - [Solution](#7a/b/solution)
    - [c](#7a/c)
      - [Solution](#7a/c/solution)
  - [8A](#8a)
    - [a](#8a/a)
      - [Solution](#8a/a/solution)
    - [b](#8a/b)
      - [Solution](#8a/b/solution)
  - [9F](#9f)
    - [a](#9f/a)
      - [Solution](#9f/a/solution)
    - [b](#9f/b)
      - [Solution](#9f/b/solution)
  - [10F](#10f)
    - [a](#10f/a)
      - [Solution](#10f/a/solution)
    - [b](#10f/b)
      - [Solution](#10f/b/solution)
  - [11F](#11f)
    - [a](#11f/a)
      - [Solution](#11f/a/solution)
    - [b](#11f/b)
      - [Solution](#11f/b/solution)
    - [c](#11f/c)
      - [Solution](#11f/c/solution)
    - [d](#11f/d)
      - [Solution](#11f/d/solution)
    - [e](#11f/e)
      - [Solution](#11f/e/solution)
  - [12F](#12f)
    - [a](#12f/a)
      - [Solution](#12f/a/solution)
    - [b](#12f/b)
      - [i](#12f/b/i)
        - [Solution](#12f/b/i/solution)
      - [ii](#12f/b/ii)
        - [Solution](#12f/b/ii/solution)
      - [iii](#12f/b/iii)
        - [Solution](#12f/b/iii/solution)

## Section I

↑ **Parent:** [Paper 2](paper-2.md)

### 1A

↑ **Parent:** [Section I](#section-i)

<h4 id="1a/a">a</h4>

↑ **Parent:** [1A](#1a)

<h5 id="1a/a/solution">Solution</h5>

↑ **Parent:** [A](#1a/a)

Substitution of $y_n=\lambda^n$ into the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) gives $\lambda^n p(\lambda)=0$. Since $\lambda\ne0$, division by $\lambda^n$ proves **the sequence is a solution exactly when $p(\lambda)=0$**.

For a nonzero triple [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) $\mu$, the [repeated characteristic root of a linear recurrence](../../../algebra.md#repeated-characteristic-root-of-a-linear-recurrence) rule gives the three independent solutions $\mu^n,n\mu^n,n^2\mu^n$. One way to see the polynomial factors is to write $y_n=\mu^n z_n$: the recurrence becomes the third [forward difference operator](../../../finite-difference.md#forward-difference-operator) applied to $z_n$ equal to zero, so $z_n$ is a quadratic [polynomial](../../../polynomial.md). Thus

$$
\boxed{y_n=(A+Bn+Cn^2)\mu^n,\qquad \mu\ne0.}
$$

These three constants give arbitrary initial values $y_0,y_1,y_2$, hence the full third-order solution. If $\mu=0$, the recurrence instead reduces to $y_{n+3}=0$: **the first three values are arbitrary and every subsequent value is zero**. The nonzero-root formula must not be used to discard those initial values.

<h4 id="1a/b">b</h4>

↑ **Parent:** [1A](#1a)

<h5 id="1a/b/solution">Solution</h5>

↑ **Parent:** [B](#1a/b)

Eliminate the free constant by comparing consecutive values:

$$
y_{n+1}-2y_n=(a2^{n+1}-n-1)-2(a2^n-n)=n-1.
$$

Therefore an appropriate [inhomogeneous linear recurrence](../../../algebra.md#inhomogeneous-linear-recurrence) is

$$
\boxed{y_{n+1}-2y_n=n-1.}
$$

Its homogeneous part has solution $a2^n$, and $-n$ is a particular solution. A first-order [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) has one arbitrary initial value, so this gives exactly the desired general solution.

### 2A

↑ **Parent:** [Section I](#section-i)

<h4 id="2a/a">a</h4>

↑ **Parent:** [2A](#2a)

<h5 id="2a/a/solution">Solution</h5>

↑ **Parent:** [A](#2a/a)

An [equilibrium of an autonomous differential equation](../../../dynamical-systems.md#equilibrium-of-an-autonomous-differential-equation) is a constant $y_*$ with $f(y_*)=0$. Put $y=y_*+\eta$. For differentiable $f$, the [linear stability analysis](../../../dynamical-systems.md#linear-stability) gives

$$
\eta'=f'(y_*)\eta+o(\eta).
$$

Thus the linear perturbation is proportional to $e^{f'(y_*)x}$. More directly, continuity of $f'$ makes $f(y)$ point toward $y_*$ on both sides when $f'(y_*)<0$, and away from it when $f'(y_*)>0$. Hence

$$
\boxed{f'(y_*)<0:\ \text{asymptotically stable};\qquad f'(y_*)>0:\ \text{unstable}.}
$$

The sign refers to evolution toward increasing $x$. If $f'(y_*)=0$, [linear stability analysis](../../../dynamical-systems.md#linear-stability) is inconclusive: the leading nonzero nonlinear term or the signs of $f$ on either side are needed. For example $\eta'=-\eta^3$ is attracting whereas $\eta'=\eta^3$ is repelling, despite the same zero linear coefficient.

<h4 id="2a/b">b</h4>

↑ **Parent:** [2A](#2a)

<h5 id="2a/b/solution">Solution</h5>

↑ **Parent:** [B](#2a/b)

Factor the right-hand side as $f(y)=y(y-2)(y+1)$. Its [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are $-1,0,2$, and $f'(y)=3y^2-2y-2$ gives

$$
\boxed{y=-1:\ \text{unstable};\qquad y=0:\ \text{asymptotically stable};\qquad y=2:\ \text{unstable}.}
$$

Indeed $f'(-1)=3$, $f'(0)=-2$ and $f'(2)=6$. The [phase line](../../../dynamical-systems.md#phase-line) has downward motion for $y<-1$, upward motion for $-1<y<0$, downward motion for $0<y<2$, and upward motion for $y>2$. The uniqueness of a smooth [autonomous differential equation](../../../dynamical-systems.md#autonomous-system-mathematics) prevents trajectories from crossing an [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). Consequently trajectories starting between $-1$ and $2$ approach zero as $x\to\infty$, while those outside that interval move away from the three [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). The constant trajectories and representative nonconstant trajectories are shown below.

<a id="2a/b/image-representative-trajectories-and-equilibrium-levels-for-the-scalar-cubic-differential-equation"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2-scalar-solutions.png)

**[Figure 1](#2a/b/image-representative-trajectories-and-equilibrium-levels-for-the-scalar-cubic-differential-equation). Representative trajectories and equilibrium levels for the scalar cubic differential equation**.

### 3F

↑ **Parent:** [Section I](#section-i)

<h4 id="3f/a">a</h4>

↑ **Parent:** [3F](#3f)

<h5 id="3f/a/solution">Solution</h5>

↑ **Parent:** [A](#3f/a)

For a nonnegative integer-valued [random variable](../../../random-variable.md), the [probability generating function](../../../probability-theory.md#probability-generating-function) is

$$
G_X(s)=\mathbb E[s^X]=\sum_{n=0}^{\infty}\mathbb P(X=n)s^n,
$$

initially for $|s|\le1$, with $0^0=1$. For the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution), insert its [probability mass function](../../../probability-theory.md#probability-mass-function) and sum the exponential series:

$$
G_X(s)=e^{-\lambda}\sum_{n=0}^{\infty}\frac{(\lambda s)^n}{n!}.
$$

Thus

$$
\boxed{G_X(s)=e^{\lambda(s-1)}.}
$$

<h4 id="3f/b">b</h4>

↑ **Parent:** [3F](#3f)

<h5 id="3f/b/solution">Solution</h5>

↑ **Parent:** [B](#3f/b)

The [moment-generating function](../../../probability-theory.md#moment-generating-function) is $M_Y(t)=\mathbb E[e^{tY}]$ for real $t$ where this expectation is finite; a finite neighborhood of zero is usually required when speaking of an existing [moment-generating function](../../../probability-theory.md#moment-generating-function). For a [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), completing the square gives

$$
M_Y(t)=\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{ty-y^2/2}\,dy
=e^{t^2/2}\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{-(y-t)^2/2}\,dy.
$$

The translated [Gaussian density](../../../probability-and-statistics.md#multivariate-normal-density) integrates to one, so

$$
\boxed{M_Y(t)=e^{t^2/2}\quad(t\in\mathbb R).}
$$

<h4 id="3f/c">c</h4>

↑ **Parent:** [3F](#3f)

<h5 id="3f/c/solution">Solution</h5>

↑ **Parent:** [C](#3f/c)

Construct independent copies $Y_1,Y_2,\ldots$ of $Y$, also independent of $X$, and define the [random sum](../../../random-variable.md#random-sum) $Z=\sum_{j=1}^X Y_j$, taking the empty sum to be zero. Independence gives, conditional on $X=n$,

$$
\mathbb E[e^{tZ}\mid X=n]=M_Y(t)^n.
$$

The [law of total expectation](../../../measure-theory.md#law-of-total-expectation) gives the [transform composition for an independent random sum](../../../random-variable.md#transform-composition-for-an-independent-random-sum)

$$
\boxed{M_Z(t)=\sum_{n=0}^{\infty}\mathbb P(X=n)M_Y(t)^n=G_X(M_Y(t)).}
$$

The summands are nonnegative, so this equality is valid also as an extended-valued expectation. Where the right-hand side is finite, it is the ordinary [moment-generating function](../../../probability-theory.md#moment-generating-function) of the constructed [random sum](../../../random-variable.md#random-sum). The construction does not assert a finite [moment-generating function](../../../probability-theory.md#moment-generating-function) near zero for arbitrary $X,Y$: heavy tails can prevent this. For example a nonnegative $Y$ with no positive exponential moments and $X\equiv1$ already shows the necessary qualification.

### 4F

↑ **Parent:** [Section I](#section-i)

<h4 id="4f/solution">Solution</h4>

↑ **Parent:** [4F](#4f)

[Pairwise independent events](../../../probability-theory.md#pairwise-independent-events) satisfy $\mathbb P(A_i\cap A_j)=\mathbb P(A_i)\mathbb P(A_j)$ for every distinct pair. [Independent events](../../../probability-theory.md#independent-events) satisfy

$$
\mathbb P\!\left(\bigcap_{i\in I}A_i\right)=\prod_{i\in I}\mathbb P(A_i)
$$

for every nonempty subset $I$ of the indices. For three events this includes the triple intersection, not just the three pairwise intersections.

Write $A_i=B_i\cup C$. Disjointness gives $\mathbb P(A_i)=p+q$, while every intersection of two or three distinct $A_i$ is exactly $C$. Thus [pairwise independence](../../../probability-theory.md#pairwise-independent-events) is equivalent to $q=(p+q)^2$. Since $p+q\ge0$,

$$
\boxed{p=\sqrt q-q.}
$$

For $0\le q\le1/16$, this is an admissible nonnegative $p$: putting $u=\sqrt q\in[0,1/4]$ gives $3p+q=3u-2u^2\le5/8<1$. The four disjoint events can therefore have the stated probabilities, with the remaining probability assigned to their complement. This also covers $q=0$.

Full [independence](../../../random-variable.md#independent-random-variables) would additionally require $q=(p+q)^3$. Together with $q=(p+q)^2$, this forces $p+q$ to be zero or one. The first case gives $p=q=0$; the second gives $q=1,p=0$. Neither allows positive $p,q$. **There are no such mutually independent events with $p>0$ and $q>0$.**

## Section II

↑ **Parent:** [Paper 2](paper-2.md)

### 5A

↑ **Parent:** [Section II](#section-ii)

<h4 id="5a/a">a</h4>

↑ **Parent:** [5A](#5a)

<h5 id="5a/a/solution">Solution</h5>

↑ **Parent:** [A](#5a/a)

Combine the real variables into $z=x+iy$. The [linear system of ordinary differential equations](../../../differential-equation.md#linear-system-of-differential-equations) becomes $z'=(1-i\mu)z$, hence $z=(A+iB)e^{(1-i\mu)t}$ for arbitrary real $A,B$. Taking real and imaginary parts gives

$$
\boxed{x=e^t(A\cos\mu t+B\sin\mu t),\qquad y=e^t(-A\sin\mu t+B\cos\mu t).}
$$

The two independent constants cover every real initial condition. In the [phase plane](../../../dynamical-systems.md#phase-plane), the distance from the origin grows as $e^t$ and the polar angle changes at rate $-\mu$. For $\mu\ne0$ the trajectories are outward [logarithmic spirals](../../../topology.md#logarithmic-spiral); for $\mu=0$ they are outward straight rays.

<h4 id="5a/b">b</h4>

↑ **Parent:** [5A](#5a)

<h5 id="5a/b/solution">Solution</h5>

↑ **Parent:** [B](#5a/b)

At a [fixed point](../../../function.md#fixed-point), the first equation gives $y=-x$. Substitution into the second gives $2x(x^2-1)=0$, so the [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are $(0,0),(1,-1),(-1,1)$. The [Jacobian matrix](../../../calculus.md#jacobian-matrix) is

$$
J(x,y)=\begin{pmatrix}1&1\\-1-4xy&1-2x^2\end{pmatrix}.
$$

At the origin its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1\pm i$, so **the origin is an unstable spiral**. The local rotation is clockwise: on the positive $x$-axis the velocity points downward. At either nonzero [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system),

$$
J=\begin{pmatrix}1&1\\3&-1\end{pmatrix},\qquad \det(J-\lambda I)=\lambda^2-4.
$$

Thus **both nonzero equilibria are saddles**, with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $-2,2$. The [stable manifold](../../../dynamical-systems.md#stable-manifold) is tangent to $(1,-3)$, and the [unstable manifold](../../../dynamical-systems.md#unstable-manifold) to $(1,1)$, at each [saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium). Since all these [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are hyperbolic, [linear stability of a planar equilibrium](../../../dynamical-systems.md#linear-stability-of-a-planar-equilibrium) gives their actual local types.

For the [phase portrait](../../../dynamical-systems.md#phase-portrait), the [nullclines](../../../dynamical-systems.md#nullcline) are $y=-x$ and $y=x/(1-2x^2)$, the latter defined away from $x=\pm1/\sqrt2$. The horizontal direction has the sign of $x+y$; the vertical direction has the sign of $(1-2x^2)y-x$. The system is invariant under $(x,y)\mapsto(-x,-y)$, so trajectories occur in centrally symmetric pairs. The arrows below show these directions; the highlighted [stable manifolds](../../../dynamical-systems.md#stable-manifold) enter the [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium), whereas the highlighted [unstable manifolds](../../../dynamical-systems.md#unstable-manifold) leave them.

<a id="5a/b/image-clockwise-unstable-spiral-and-two-saddles-with-stable-and-unstable-separatrices"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2-planar-phase.png)

**[Figure 2](#5a/b/image-clockwise-unstable-spiral-and-two-saddles-with-stable-and-unstable-separatrices). Clockwise unstable spiral and two saddles with stable and unstable separatrices**.

### 6A

↑ **Parent:** [Section II](#section-ii)

<h4 id="6a/a">a</h4>

↑ **Parent:** [6A](#6a)

<h5 id="6a/a/solution">Solution</h5>

↑ **Parent:** [A](#6a/a)

Work locally where the needed derivatives of the [level set](../../../topology.md#level-set) can be represented by the [implicit function theorem](../../../calculus.md#implicit-function-theorem). Differentiating while holding the indicated coordinate fixed gives

$$
\left(\frac{\partial x}{\partial y}\right)_z=-\frac{f_y}{f_x},\qquad
\left(\frac{\partial y}{\partial z}\right)_x=-\frac{f_z}{f_y},\qquad
\left(\frac{\partial z}{\partial x}\right)_y=-\frac{f_x}{f_z}.
$$

Multiplying the three [implicit differentiation](../../../calculus.md#implicit-differentiation) formulas proves

$$
\boxed{\left(\frac{\partial x}{\partial y}\right)_z
\left(\frac{\partial y}{\partial z}\right)_x
\left(\frac{\partial z}{\partial x}\right)_y=-1.}
$$

This [cyclic partial derivative identity](../../../calculus.md#cyclic-partial-derivative-identity) is asserted where all three finite coordinate derivatives exist, in particular when $f_xf_yf_z\ne0$. It is not a globally defined product at points where one of the necessary coordinate parametrizations is singular.

<h4 id="6a/b">b</h4>

↑ **Parent:** [6A](#6a)

<h5 id="6a/b/i">i</h5>

↑ **Parent:** [B](#6a/b)

<h6 id="6a/b/i/solution">Solution</h6>

↑ **Parent:** [I](#6a/b/i)

The [partial derivatives](../../../calculus.md#partial-derivative) of $f$ are $f_x=2x$, $f_y=4y(a-y^2)$ and $f_z=2z$. Therefore the three [implicit differentiation](../../../calculus.md#implicit-differentiation) formulas are

$$
\boxed{\left(\frac{\partial x}{\partial y}\right)_z=\frac{2y(y^2-a)}x,\qquad
\left(\frac{\partial y}{\partial z}\right)_x=\frac{z}{2y(y^2-a)},\qquad
\left(\frac{\partial z}{\partial x}\right)_y=-\frac{x}z.}
$$

Their product is $-1$ wherever $xyz(y^2-a)\ne0$. The excluded factors identify exactly where these quotient formulas cannot all represent finite [partial derivatives](../../../calculus.md#partial-derivative).

<h5 id="6a/b/ii">ii</h5>

↑ **Parent:** [B](#6a/b)

<h6 id="6a/b/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#6a/b/ii)

At $(x,0,z)$ the [gradient](../../../calculus.md#gradient) is $(2x,0,2z)$. The outward radial unit [vector](../../../vector-space.md#vector) is $(x,0,z)/\sqrt{x^2+z^2}$ when $(x,z)\ne(0,0)$. Taking its scalar product with the [gradient](../../../calculus.md#gradient) gives the radial [directional derivative](../../../calculus.md#directional-derivative)

$$
\boxed{\frac{\partial f}{\partial r}=2\sqrt{x^2+z^2}.}
$$

Equivalently, on this plane $f=r^2$. At the origin the radial unit vector is undefined, but every unit [directional derivative](../../../calculus.md#directional-derivative) is zero. Differentiating along the unnormalized scaling path $(tx,0,tz)$ instead gives $2(x^2+z^2)$ at $t=1$; that is a rate per scaling parameter, not per unit radial distance.

<h5 id="6a/b/iii">iii</h5>

↑ **Parent:** [B](#6a/b)

<h6 id="6a/b/iii/solution">Solution</h6>

↑ **Parent:** [Iii](#6a/b/iii)

A [stationary point](../../../calculus-of-variations.md#stationary-point) requires $x=z=0$ and $y(a-y^2)=0$. The [Hessian matrix](../../../calculus.md#hessian-matrix) is diagonal:

$$
H_f=\operatorname{diag}(2,4a-12y^2,2).
$$

For $a>0$, the origin has positive definite [Hessian matrix](../../../calculus.md#hessian-matrix), hence is a strict [local minimum](../../../analysis.md#local-minimum), with value zero. The two additional [stationary points](../../../calculus-of-variations.md#stationary-point) $(0,\pm\sqrt a,0)$ have value $a^2$ and [Hessian matrix](../../../calculus.md#hessian-matrix) $\operatorname{diag}(2,-8a,2)$; **both are saddle points**.

For $a<0$, the origin is the only [stationary point](../../../calculus-of-variations.md#stationary-point) and has an indefinite [Hessian matrix](../../../calculus.md#hessian-matrix), so **it is a saddle point**. For $a=0$, the [Hessian matrix](../../../calculus.md#hessian-matrix) test is inconclusive, but $f(x,y,z)=x^2+z^2-y^4$ takes positive values along the $x$-axis and negative values along the $y$-axis arbitrarily near zero. Thus **the origin is a degenerate saddle point**. There are no [local maxima](../../../analysis.md#local-maximum) in any case: varying $x$ or $z$ away from a [stationary point](../../../calculus-of-variations.md#stationary-point) increases $f$.

<h5 id="6a/b/iv">iv</h5>

↑ **Parent:** [B](#6a/b)

<h6 id="6a/b/iv/solution">Solution</h6>

↑ **Parent:** [Iv](#6a/b/iv)

In the $(x,y)$-plane take $z=0$; holding another fixed $z$ merely shifts all contour labels by $z^2$. The [level sets](../../../topology.md#level-set) satisfy

$$
x^2=y^4-2ay^2+c.
$$

For $a=1$, the origin is a [local minimum](../../../analysis.md#local-minimum) and $(0,\pm1)$ are [saddle points of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function) at contour value $1$. For $0<c<1$, a closed contour around the origin is accompanied by unbounded outer components. At $c=1$ the contour satisfies $x=\pm(y^2-1)$ and crosses at the two [saddle points of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function). For $c>1$, two unbounded components remain; negative contours have only outer components.

For $a=-1$, the origin is a [saddle point of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function), and the zero contour is $x=\pm y\sqrt{y^2+2}$, with tangent lines $x=\pm\sqrt2\,y$. Positive contours form two components extending on opposite sides of the $y$-axis; negative contours form upper and lower components. These [level sets](../../../topology.md#level-set) are illustrated below.

<a id="6a/b/iv/image-contours-of-the-quartic-surface-at-z-equal-to-zero-for-a-equal-to-one-and-minus-one"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2-level-contours.png)

**[Figure 3](#6a/b/iv/image-contours-of-the-quartic-surface-at-z-equal-to-zero-for-a-equal-to-one-and-minus-one). Contours of the quartic surface at z equal to zero for a equal to one and minus one**.

### 7A

↑ **Parent:** [Section II](#section-ii)

<h4 id="7a/a">a</h4>

↑ **Parent:** [7A](#7a)

<h5 id="7a/a/solution">Solution</h5>

↑ **Parent:** [A](#7a/a)

The [Wronskian](../../../differential-equation.md#wronskian) is

$$
W=y_1y_2'-y_1'y_2.
$$

On an interval where $p,q$ are continuous, **the solutions are linearly independent exactly when $W(x_0)\ne0$ at one point**, equivalently when the [Wronskian](../../../differential-equation.md#wronskian) is nonzero throughout the interval. Differentiation and the [homogeneous linear differential equation](../../../differential-equation.md#homogeneous-linear-differential-equation) give

$$
W'=y_1y_2''-y_1''y_2
=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
$$

Hence [Abel identity](../../../differential-equation.md#abel-s-identity) reads $W(x)=W(x_0)\exp(-\int_{x_0}^x p(s)\,ds)$. If $W(x_0)=0$, the two initial-data vectors are dependent; the [uniqueness theorem for ordinary differential equations](../../../analysis.md#uniqueness-theorem-for-ordinary-differential-equations) then makes the corresponding linear combination identically zero. This proves the converse as well as the necessity.

<h4 id="7a/b">b</h4>

↑ **Parent:** [7A](#7a)

<h5 id="7a/b/solution">Solution</h5>

↑ **Parent:** [B](#7a/b)

Direct calculation gives

$$
W=(1+\cos x)\cos x+\sin^2x=1+\cos x.
$$

Where $1+\cos x\ne0$, [Abel identity](../../../differential-equation.md#abel-s-identity) gives $p=-W'/W=\sin x/(1+\cos x)$, and substitution of either solution gives $q=1/(1+\cos x)$. Thus

$$
\boxed{p(x)=\tan(x/2),\qquad q(x)=\frac1{1+\cos x},\qquad W(\pi)=0.}
$$

These coefficients have singularities at odd multiples of $\pi$. This does not contradict the [Wronskian](../../../differential-equation.md#wronskian) criterion: its continuous-coefficient interval hypothesis fails at those points.

On $0\le x<\pi$, the initial conditions uniquely select $y=\sin x$. **The normalized differential equation is not defined on the whole interval $0\le x<\infty$**, so the usual global [uniqueness theorem for ordinary differential equations](../../../analysis.md#uniqueness-theorem-for-ordinary-differential-equations) cannot give the global initial-value assertion as posed. No choice of finite coefficients at $\pi$ can repair the normalized equation while retaining both displayed solutions: at that point $1+\cos x$ and its first derivative vanish, but its second derivative equals one.

The [continuation through a zero of the leading ODE coefficient](../../../differential-equation.md#continuation-through-a-zero-of-the-leading-ode-coefficient) is a different problem: consider the multiplied, degenerate equation

$$
(1+\cos x)y''+\sin x\,y'+y=0.
$$

For this different equation, a globally $C^2$ solution with the given initial data is uniquely $\sin x$. On each regular interval every solution is $A_j(1+\cos x)+B_j\sin x$; continuity of $y'$ and $y''$ at an odd multiple of $\pi$ forces both constants to agree across it. If only $C^1$ piecewise solutions away from the singular points are required, the $A_j$ may change and uniqueness fails. Thus the coefficient singularity and the intended solution regularity must be distinguished.

<h4 id="7a/c">c</h4>

↑ **Parent:** [7A](#7a)

<h5 id="7a/c/solution">Solution</h5>

↑ **Parent:** [C](#7a/c)

Both functions satisfy the constant-coefficient [homogeneous linear differential equation](../../../differential-equation.md#homogeneous-linear-differential-equation)

$$
\boxed{y'''+y'=0.}
$$

Its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $\lambda(\lambda^2+1)$, so the general real solution is $y=A+B\cos x+C\sin x$. The three initial conditions give $A+B=0$, $C=1$, and $-B=0$, hence

$$
\boxed{y(x)=\sin x.}
$$

Here the equation has continuous coefficients and nonzero highest-derivative coefficient everywhere. The [uniqueness theorem for ordinary differential equations](../../../analysis.md#uniqueness-theorem-for-ordinary-differential-equations), applied to its three-component first-order system, gives **a unique solution on the entire half-line**.

### 8A

↑ **Parent:** [Section II](#section-ii)

<h4 id="8a/a">a</h4>

↑ **Parent:** [8A](#8a)

<h5 id="8a/a/solution">Solution</h5>

↑ **Parent:** [A](#8a/a)

Rewrite the integrand as $\sqrt{1-t\cos^2\theta}$. The [binomial series](../../../real-analysis.md#binomial-series), uniformly valid in $\theta$ for $|t|$ bounded below one, gives

$$
\sqrt{1-t\cos^2\theta}=1-\frac t2\cos^2\theta-\frac{t^2}8\cos^4\theta+O(t^3).
$$

The integrals of $1,\cos^2\theta,\cos^4\theta$ over a full period are respectively $2\pi,\pi,3\pi/4$. Termwise integration therefore yields the [ellipse perimeter expansion near a circle](../../../geometry-and-topology.md#ellipse-perimeter-expansion-near-a-circle)

$$
\boxed{y=2\pi-\frac{\pi}{2}t-\frac{3\pi}{32}t^2+O(t^3)
=2\pi\left(1-\frac t4-\frac{3t^2}{64}+O(t^3)\right).}
$$

<h4 id="8a/b">b</h4>

↑ **Parent:** [8A](#8a)

<h5 id="8a/b/solution">Solution</h5>

↑ **Parent:** [B](#8a/b)

With $t=1-x^2$ the [chain rule](../../../calculus.md#chain-rule) gives $y'=-2xu'$ and $y''=-2u'+4x^2u''$. Substitution, initially for $x>0$, gives

$$
\boxed{t(1-t)u''+(1-t)u'+\frac14u=0.}
$$

The transformed coefficients are $P(t)=1/t$ and $Q(t)=1/[4t(1-t)]$. At $t=0$, both $tP$ and $t^2Q$ are analytic; at $t=1$, both $(t-1)P$ and $(t-1)^2Q$ are analytic. Each point is singular because a normalized coefficient has a pole, but satisfies the [regular singular point criterion for a second-order equation](../../../complex-analysis.md#regular-singular-point-criterion-for-a-second-order-equation). Thus **both points are regular singular points**.

For a [Frobenius method](../../../complex-analysis.md#frobenius-method) substitution $u=t^\rho\sum_{n\ge0}a_nt^n$, the lowest power gives the [indicial equation](../../../differential-equation.md#indicial-equation)

$$
\rho(\rho-1)+\rho=\rho^2=0.
$$

The repeated [indicial root](../../../differential-equation.md#indicial-root) is zero. Setting $\rho=0$ and equating the coefficient of $t^n$ gives

$$
(n+1)^2a_{n+1}+\left(\frac14-n^2\right)a_n=0,
\qquad
\boxed{a_{n+1}=\frac{n^2-\tfrac14}{(n+1)^2}a_n.}
$$

Consequently the analytic [power-series solution of a differential equation](../../../differential-equation.md#power-series-solution-of-a-differential-equation) is

$$
u_1(t)=a_0\left(1-\frac t4-\frac{3t^2}{64}+\cdots\right).
$$

Taking $a_0=2\pi$ reproduces the [ellipse](../../../geometry-and-topology.md#ellipse) perimeter expansion.

For a second independent solution, normalize $u_1(0)=1$. [Reduction of order](../../../differential-equation.md#reduction-of-order) and $P=1/t$ give

$$
u_2(t)=u_1(t)\int^t\frac{ds}{s\,u_1(s)^2}.
$$

Since $u_1(s)^{-2}=1+O(s)$, this has the [Logarithmic Frobenius solution](../../../complex-analysis.md#logarithmic-solution-from-a-repeated-frobenius-exponent) form

$$
\boxed{u_2(t)=u_1(t)\log t+v(t),\qquad v\ \text{analytic near }0.}
$$

The logarithm is $\log|t|$ on the real negative side, or a chosen [complex logarithm](../../../analysis.md#complex-logarithm) on a slit complex neighborhood. Its nonzero logarithmic coefficient establishes independence. The physical perimeter is finite at $t=0$, so it selects the analytic branch rather than this logarithmic one.

### 9F

↑ **Parent:** [Section II](#section-ii)

<h4 id="9f/a">a</h4>

↑ **Parent:** [9F](#9f)

<h5 id="9f/a/solution">Solution</h5>

↑ **Parent:** [A](#9f/a)

By the definition of [conditional probability](../../../probability-theory.md#conditional-probability),

$$
\mathbb P(B_i\mid A)=\frac{\mathbb P(A\cap B_i)}{\mathbb P(A)}
=\frac{\mathbb P(A\mid B_i)\mathbb P(B_i)}{\mathbb P(A)}.
$$

Since the $B_j$ form a disjoint partition of the [sample space](../../../probability-theory.md#sample-space), the [law of total probability](../../../probability-theory.md#law-of-total-probability) gives $\mathbb P(A)=\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j)$. Substitution proves [Bayes' theorem](../../../probability-theory.md#bayes-theorem) in the required form:

$$
\boxed{\mathbb P(B_i\mid A)=
\frac{\mathbb P(A\mid B_i)\mathbb P(B_i)}
{\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j)}.}
$$

The hypotheses make the denominator positive and each conditioning probability well defined.

<h4 id="9f/b">b</h4>

↑ **Parent:** [9F](#9f)

<h5 id="9f/b/solution">Solution</h5>

↑ **Parent:** [B](#9f/b)

Let $N$ denote the mattress count and $U$ the event of undisturbed sleep. Use the intended model in which the presence of the pea is independent of $N$, with probability $1/2$, and without a pea sleep is undisturbed. Conditioning on $N$ gives

$$
\mathbb P(U\mid N=6)=\frac12,\qquad
\mathbb P(U\mid N=7)=\frac12+\frac12\frac15=\frac35,\qquad
\mathbb P(U\mid N=8)=\frac12+\frac12\frac25=\frac7{10}.
$$

The [law of total probability](../../../probability-theory.md#law-of-total-probability) and the equal prior probabilities give

$$
\boxed{\mathbb P(U)=\frac13\left(\frac12+\frac35+\frac7{10}\right)=\frac35.}
$$

By [Bayes' theorem](../../../probability-theory.md#bayes-theorem), the posterior probabilities of $N=6,7,8$ given $U$ are respectively $5/18,6/18,7/18$. Therefore the [conditional expectation](../../../measure-theory.md#conditional-expectation) is

$$
\boxed{\mathbb E[N\mid U]=6\frac5{18}+7\frac6{18}+8\frac7{18}=\frac{64}{9}.}
$$

Undisturbed sleep shifts the posterior toward larger mattress counts because those counts make the observation more likely.

### 10F

↑ **Parent:** [Section II](#section-ii)

<h4 id="10f/a">a</h4>

↑ **Parent:** [10F](#10f)

<h5 id="10f/a/solution">Solution</h5>

↑ **Parent:** [A](#10f/a)

For any nonnegative [random variable](../../../random-variable.md) $X$ with finite [expectation](../../../probability-theory.md#expected-value) and any $a>0$, [Markov's inequality](../../../probability-inequality.md#markov-inequality) states

$$
\boxed{\mathbb P(X\ge a)\le\frac{\mathbb E X}{a}.}
$$

Indeed $X\ge a\,\mathbf1_{\{X\ge a\}}$, and taking [expectations](../../../probability-theory.md#expected-value) proves the bound. Nonnegativity is essential.

<h4 id="10f/b">b</h4>

↑ **Parent:** [10F](#10f)

<h5 id="10f/b/solution">Solution</h5>

↑ **Parent:** [B](#10f/b)

Each waiting time has the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) on $1,2,\ldots$ with success probability $1/2$: a wait of length $n$ consists of $n-1$ failures followed by the prescribed success, so its probability is $2^{-n}$. Hence

$$
\boxed{G_{H_j}(s)=G_{T_j}(s)=\sum_{n\ge1}\left(\frac s2\right)^n=\frac{s}{2-s},\qquad
\mathbb E H_j=\mathbb E T_j=G'_{H_j}(1)=2.}
$$

Disjoint successive blocks of independent tosses give independent waiting times. More explicitly, any specified list of block lengths determines exactly one allowed sequence of heads and tails and has probability $2^{-\sum_j(h_j+t_j)}$, the product of the individual block probabilities.

There are $2r$ waiting times. Multiplication of their [probability generating functions](../../../probability-theory.md#probability-generating-function) and addition of their [expectations](../../../probability-theory.md#expected-value) give

$$
\boxed{G_{Y_r}(s)=\left(\frac{s}{2-s}\right)^{2r},\qquad \mathbb E Y_r=4r.}
$$

To recover its [probability mass function](../../../probability-theory.md#probability-mass-function), expand by the [negative binomial series](../../../real-analysis.md#negative-binomial-series):

$$
G_{Y_r}(s)=\frac{s^{2r}}{2^{2r}}(1-s/2)^{-2r}
=\frac{s^{2r}}{2^{2r}}\sum_{m\ge0}\binom{m+2r-1}{2r-1}(s/2)^m.
$$

The coefficient of $s^n$ is therefore

$$
\boxed{\mathbb P(Y_r=n)=2^{-n}\binom{n-1}{2r-1},\qquad n\ge2r,}
$$

and it is zero below $2r$. Equivalently there are $\binom{n-1}{2r-1}$ compositions of $n$ into $2r$ positive block lengths, each with probability $2^{-n}$. This is the [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) for a sum of geometric waiting times, even though the desired outcome alternates between blocks.

For $r=1$,

$$
\boxed{\mathbb P(Y_1\ge5)=1-\left(\frac14+\frac28+\frac3{16}\right)=\frac5{16}.}
$$

Since $\mathbb E Y_1=4$, [Markov's inequality](../../../probability-inequality.md#markov-inequality) gives $\mathbb P(Y_1\ge5)\le4/5$, and indeed $5/16<4/5$.

### 11F

↑ **Parent:** [Section II](#section-ii)

<h4 id="11f/a">a</h4>

↑ **Parent:** [11F](#11f)

<h5 id="11f/a/solution">Solution</h5>

↑ **Parent:** [A](#11f/a)

Let $h_k$ be the [hitting probability](../../../markov-process.md#hitting-probability) of the right endpoint before the left endpoint, starting at $k$. A surviving vase corresponds to that right-endpoint event. Conditioning on the first step of the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) gives

$$
\boxed{h_k=\frac12h_{k-1}+\frac12h_{k+1},\quad 1\le k\le19;\qquad h_0=0,\quad h_{20}=1.}
$$

The [Markov property](../../../markov-process.md#markov-property) makes the remaining probability depend only on the position after that step. These absorbing endpoint values distinguish the event of interest from its complement.

<h4 id="11f/b">b</h4>

↑ **Parent:** [11F](#11f)

<h5 id="11f/b/solution">Solution</h5>

↑ **Parent:** [B](#11f/b)

Let $m_k$ be the expected remaining [hitting time](../../../markov-process.md#first-passage-time) of either endpoint, measured in minutes. The first step consumes one minute, after which [first-step analysis](../../../analysis.md#first-step-analysis) gives

$$
\boxed{m_k=1+\frac12m_{k-1}+\frac12m_{k+1},\quad1\le k\le19;\qquad m_0=m_{20}=0.}
$$

The [expectation](../../../probability-theory.md#expected-value) is finite: from any interior state, a block of twenty leftward steps guarantees absorption and has probability $2^{-20}$. Thus the survival probability over successive twenty-step blocks has a geometric upper bound. This justifies using finite [expectations](../../../probability-theory.md#expected-value) in the recurrence.

<h4 id="11f/c">c</h4>

↑ **Parent:** [11F](#11f)

<h5 id="11f/c/solution">Solution</h5>

↑ **Parent:** [C](#11f/c)

The homogeneous [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) has characteristic polynomial $(\lambda-1)^2$, hence general solution $h_k=A+Bk$. For the expected-time recurrence, rearrangement gives $m_{k+1}-2m_k+m_{k-1}=-2$, for which $-k^2$ is a particular solution. Thus

$$
\boxed{h_k=A+Bk,\qquad m_k=C+Dk-k^2.}
$$

Imposing the absorbing [boundary conditions](../../../differential-equation.md#boundary-condition) from the preceding parts gives the [gambler's ruin](../../../markov-process.md#gambler-s-ruin) formulas

$$
\boxed{h_k=\frac{k}{20},\qquad m_k=k(20-k).}
$$

<h4 id="11f/d">d</h4>

↑ **Parent:** [11F](#11f)

<h5 id="11f/d/solution">Solution</h5>

↑ **Parent:** [D](#11f/d)

The initial position is $k=17$. Applying the [gambler's ruin](../../../markov-process.md#gambler-s-ruin) [hitting probability](../../../markov-process.md#hitting-probability) and mean [hitting time](../../../markov-process.md#first-passage-time) gives

$$
\boxed{\mathbb P(\text{vase survives})=\frac{17}{20},\qquad
\mathbb E[\text{time to fall}]=17(20-17)=51\ \text{minutes}.}
$$

For comparison, the original central starting position $k=10$ would give probability $1/2$ and mean time $100$ minutes.

<h4 id="11f/e">e</h4>

↑ **Parent:** [11F](#11f)

<h5 id="11f/e/solution">Solution</h5>

↑ **Parent:** [E](#11f/e)

Now the event is to hit $20$ before $1$, starting at $3$. Up to the first of those two [hitting times](../../../markov-process.md#first-passage-time), translate the interval by one unit; its endpoints become $0,19$ and the starting point becomes $2$. The [gambler's ruin](../../../markov-process.md#gambler-s-ruin) [hitting probability](../../../markov-process.md#hitting-probability) is therefore

$$
\boxed{\mathbb P_3(T_{20}<T_1)=\frac{3-1}{20-1}=\frac2{19}.}
$$

Stopping at $1$ is essential: using the original absorbing endpoint $0$ would answer a different event.

### 12F

↑ **Parent:** [Section II](#section-ii)

<h4 id="12f/a">a</h4>

↑ **Parent:** [12F](#12f)

<h5 id="12f/a/solution">Solution</h5>

↑ **Parent:** [A](#12f/a)

Normalization of the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) gives

$$
1=A\int_0^{2\pi}(\pi-\phi/2)\,d\phi=A\pi^2,\qquad
\boxed{A=\pi^{-2}.}
$$

The first two [moments](../../../probability-theory.md#moment) are

$$
\mathbb E\Phi=\frac1{\pi^2}\int_0^{2\pi}\phi(\pi-\phi/2)\,d\phi=\frac{2\pi}{3},\qquad
\mathbb E\Phi^2=\frac1{\pi^2}\int_0^{2\pi}\phi^2(\pi-\phi/2)\,d\phi=\frac{2\pi^2}{3}.
$$

Consequently

$$
\boxed{\mathbb E\Phi=\frac{2\pi}{3},\qquad
\operatorname{Var}\Phi=\frac{2\pi^2}{3}-\frac{4\pi^2}{9}=\frac{2\pi^2}{9}.}
$$

The [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) is $F(\phi)=\phi/\pi-\phi^2/(4\pi^2)=1-(1-\phi/(2\pi))^2$ on $[0,2\pi]$. For $U$ with the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$, [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) therefore uses

$$
\boxed{\Phi=2\pi\left(1-\sqrt{1-U}\right).}
$$

The inverse lies in the required interval and satisfies $F(\Phi)=U$.

<h4 id="12f/b">b</h4>

↑ **Parent:** [12F](#12f)

<h5 id="12f/b/i">i</h5>

↑ **Parent:** [B](#12f/b)

<h6 id="12f/b/i/solution">Solution</h6>

↑ **Parent:** [I](#12f/b/i)

Conditional on $\Phi=\phi$, the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) of the sector's centre angle gives a range of possible centre bearings of length $\phi$ that hit a specified house. Independence of the two angles therefore gives the [conditional probability](../../../probability-theory.md#conditional-probability) $\phi/(2\pi)$. By the [law of total expectation](../../../measure-theory.md#law-of-total-expectation),

$$
\boxed{\mathbb P(H_1\text{ hit})=\mathbb E\left[\frac{\Phi}{2\pi}\right]=\frac13.}
$$

<h5 id="12f/b/ii">ii</h5>

↑ **Parent:** [B](#12f/b)

<h6 id="12f/b/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#12f/b/ii)

For [coverage of antipodal points by a randomly oriented sector](../../../continuous-probability-distribution.md#coverage-of-antipodal-points-by-a-randomly-oriented-sector), the house bearings differ by $\pi$. For $\phi<\pi$, no single sector can cover both. For $\phi\ge\pi$, the two allowable arcs of centre bearings overlap in two components, each of length $\phi-\pi$. Thus the [conditional probability](../../../probability-theory.md#conditional-probability) of a double hit is $(\phi-\pi)/\pi$, not $(\phi-\pi)/(2\pi)$. Averaging against the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) gives

$$
\mathbb P(H_1,H_2\text{ both hit})
=\frac1{\pi^3}\int_\pi^{2\pi}(\phi-\pi)(\pi-\phi/2)\,d\phi.
$$

Put $v=\phi-\pi$ to obtain $\frac1{2\pi^3}\int_0^\pi v(\pi-v)\,dv$. Therefore

$$
\boxed{\mathbb P(H_1,H_2\text{ both hit})=\frac1{12}.}
$$

<h5 id="12f/b/iii">iii</h5>

↑ **Parent:** [B](#12f/b)

<h6 id="12f/b/iii/solution">Solution</h6>

↑ **Parent:** [Iii](#12f/b/iii)

The event that $H_1$ is hit but $H_2$ is not has probability $1/3-1/12=1/4$. Dividing by the [probability](../../../probability-theory.md#probability) $1/3$ that $H_1$ is covered, using the definition of [conditional probability](../../../probability-theory.md#conditional-probability), gives

$$
\boxed{\mathbb P(H_2\text{ not hit}\mid H_1\text{ hit})=
\frac{1/3-1/12}{1/3}=\frac34.}
$$

This conditioning concerns angular coverage of a sector; the two house-hit events are not independent.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2011](../../2011.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
