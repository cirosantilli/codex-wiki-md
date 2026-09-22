# Paper 2

↑ **Parent:** [2010](../2010.md)

[https://www.maths.cam.ac.uk/undergradnst/files/2010/PaperNST_IA_2.pdf](https://www.maths.cam.ac.uk/undergradnst/files/2010/PaperNST_IA_2.pdf)

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
  - [c](#12/c)
    - [Solution](#12/c/solution)
- [13](#13)
  - [a](#13/a)
    - [Solution](#13/a/solution)
  - [b](#13/b)
    - [Solution](#13/b/solution)
- [14](#14)
  - [a](#14/a)
    - [i](#14/a/i)
      - [Solution](#14/a/i/solution)
    - [ii](#14/a/ii)
      - [Solution](#14/a/ii/solution)
  - [b](#14/b)
    - [i](#14/b/i)
      - [Solution](#14/b/i/solution)
    - [ii](#14/b/ii)
      - [Solution](#14/b/ii/solution)
- [15](#15)
  - [Solution](#15/solution)
- [16](#16)
  - [Solution](#16/solution)
  - [a](#16/a)
    - [Solution](#16/a/solution)
  - [b](#16/b)
    - [Solution](#16/b/solution)
- [17](#17)
  - [a](#17/a)
    - [i](#17/a/i)
      - [Solution](#17/a/i/solution)
    - [ii](#17/a/ii)
      - [Solution](#17/a/ii/solution)
  - [b](#17/b)
    - [Solution](#17/b/solution)
  - [c](#17/c)
    - [i](#17/c/i)
      - [Solution](#17/c/i/solution)
    - [ii](#17/c/ii)
      - [Solution](#17/c/ii/solution)
- [18](#18)
  - [a](#18/a)
    - [Solution](#18/a/solution)
  - [b](#18/b)
    - [Solution](#18/b/solution)
  - [c](#18/c)
    - [Solution](#18/c/solution)
- [19](#19)
  - [a](#19/a)
    - [Solution](#19/a/solution)
  - [b](#19/b)
    - [Solution](#19/b/solution)
- [20](#20)
  - [a](#20/a)
    - [Solution](#20/a/solution)
  - [b](#20/b)
    - [Solution](#20/b/solution)
  - [c](#20/c)
    - [Solution](#20/c/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [dot product](../../inner-product.md#dot-product) is $\mathbf a\cdot\mathbf b=-1+2+3=4$, while the [Euclidean norms](../../normed-vector-space.md#euclidean-norm) are $\sqrt3$ and $\sqrt{14}$. Thus the angle in the stated range is

$$
\boxed{\theta=\arccos\frac4{\sqrt{42}}}.
$$

The positive cosine shows that it is an acute angle.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The integrand is an [even function](../../calculus.md#even-function), since both $x$ and $\sin x$ are [odd functions](../../calculus.md#odd-function). Using [integration by parts](../../calculus.md#integration-by-parts),

$$
\int_{-\pi/2}^{\pi/2}x\sin x\,dx
=2[-x\cos x+\sin x]_0^{\pi/2}
=\boxed{2}.
$$

The endpoint cosine terms vanish, leaving the sine contribution.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The first [partial derivatives](../../multivariable-calculus.md#partial-derivative) factor as

$$
f_x=4x(x^2+2y^2-1),\qquad f_y=4y(2x^2+1).
$$

Both vanish at the origin, verifying that it is a [stationary point](../../calculus-of-variations.md#stationary-point). Since $2x^2+1>0$, every [stationary point](../../calculus-of-variations.md#stationary-point) has $y=0$; the first equation then gives $x=0,\pm1$. Thus one requested additional point is $\boxed{(1,0)}$; the other is $\boxed{(-1,0)}$.

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [characteristic polynomial](../../linear-operator-theory.md#characteristic-polynomial) is

$$
\det(\lambda I-A)=(\lambda-1/3)(\lambda+1/3)-3
=\lambda^2-\frac{28}{9}.
$$

Its roots give the two [eigenvalues](../../linear-operator-theory.md#eigenvalue)

$$
\boxed{\lambda=\pm\frac{2\sqrt7}{3}}.
$$

Their sum is zero, agreeing with the [trace](../../linear-algebra.md#matrix-trace) of the [matrix](../../vector-space.md#matrix).

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Multiply numerator and denominator by the [complex conjugate](../../complex-analysis.md#complex-conjugate) $5+4i$:

$$
\frac{3+5i}{5-4i}=\frac{(3+5i)(5+4i)}{25+16}
=\frac{-5+37i}{41}.
$$

The [real part](../../complex-analysis.md#real-part) and [imaginary part](../../complex-analysis.md#imaginary-part) are therefore

$$
\boxed{\operatorname{Re}=-\frac5{41},\qquad\operatorname{Im}=\frac{37}{41}}.
$$

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Put $h=x-\pi/3$. The values $f(\pi/3)=1/2$, $f'(\pi/3)=-\sqrt3/2$, and $f''(\pi/3)=-1/2$ give the [Taylor expansion](../../calculus.md#taylor-expansion)

$$
\boxed{\cos x=\frac12-\frac{\sqrt3}{2}\left(x-\frac\pi3\right)
-\frac14\left(x-\frac\pi3\right)^2+O((x-\pi/3)^3)}.
$$

The [factorial](../../combinatorics.md#factorial) in the quadratic term accounts for its coefficient $-1/4$.

## 7

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

For this [separable differential equation](../../differential-equation.md#separable-differential-equation), away from $x=1$, separation gives $\ln|y+1|=\ln|x-1|+C$, or $y+1=K(x-1)$ on a connected interval. The [initial condition](../../differential-equation.md#initial-condition) gives $2=-K$, hence

$$
\boxed{y=1-2x}.
$$

The maximal interval containing $x=0$ on which this solves the printed [differential equation](../../differential-equation.md) is $\boxed{-\infty<x<1}$. Although the linear formula extends through one, the right-hand side there is $0/0$ and the original equation is undefined. The [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) solution $y=-1$, lost if one divides by $y+1$, does not satisfy the [initial condition](../../differential-equation.md#initial-condition).

## 8

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

For independent fair dice, the [probability](../../probability-theory.md#probability) of avoiding one on each die is $5/6$. Therefore

$$
\boxed{P(\text{neither is one})=\left(\frac56\right)^2=\frac{25}{36}}.
$$

The [complement of an event](../../probability-space.md#complement-of-an-event) gives

$$
\boxed{P(\text{at least one is one})=1-\frac{25}{36}=\frac{11}{36}}.
$$

## 9

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

The [product rule](../../calculus.md#product-rule) and [chain rule](../../calculus.md#chain-rule) give $y'=\sin(x^2)+2x^2\cos(x^2)$. At zero the slope is zero and the [curve](../../topology.md#curve) passes through $(0,1)$. Consequently the [tangent line](../../calculus.md#tangent-line) is

$$
\boxed{y=1}.
$$

## 10

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

Differentiate the three components with respect to their matching [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system):

$$
\boxed{\nabla\cdot\mathbf F=y^2z^2+4y^3+x^3y^2}.
$$

The $3xz^2$ term contributes nothing to the $y$ [derivative](../../calculus.md#derivative) because it is independent of $y$.

## 11

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11/a">a</h3>

↑ **Parent:** [11](#11)

<h4 id="11/a/solution">Solution</h4>

↑ **Parent:** [A](#11/a)

In [plane polar coordinates](../../classical-mechanics.md#plane-polar-coordinates), $r$ is distance from the origin and $\theta$ is the angle from positive $x$ toward positive $y$. The conversion to [Cartesian coordinates](../../linear-algebra.md#cartesian-coordinate-system) is

$$
\boxed{x=r\cos\theta,\qquad y=r\sin\theta}.
$$

Conversely $r=\sqrt{x^2+y^2}$, with the angular coordinate undefined at the origin.

<h3 id="11/b">b</h3>

↑ **Parent:** [11](#11)

<h4 id="11/b/solution">Solution</h4>

↑ **Parent:** [B](#11/b)

Multiplying the polar equation by its denominator gives $Ar-Bx=1$. Squaring and using $r^2=x^2+y^2$ yields

$$
(A^2-B^2)x^2+A^2y^2-2Bx=1.
$$

Take $C=\sqrt{A^2-B^2}>0$. [Completing the square](../../polynomial.md#completing-the-square) gives

$$
C^2\left(x-\frac{B}{C^2}\right)^2+A^2y^2
=1+\frac{B^2}{C^2}=\frac{A^2}{C^2}.
$$

The standard [ellipse](../../euclidean-geometry.md#ellipse) equation is consequently

$$
\boxed{\frac{(x-B/C^2)^2}{A^2/C^4}+\frac{y^2}{1/C^2}=1},
$$

whose centre is $\boxed{(B/C^2,0)}$. Squaring has introduced no unwanted branch: on this [ellipse](../../euclidean-geometry.md#ellipse) the minimum of $1+Bx$ is $A/(A+B)>0$, so $Ar=1+Bx$ follows with the correct positive sign.

<h3 id="11/c">c</h3>

↑ **Parent:** [11](#11)

<h4 id="11/c/solution">Solution</h4>

↑ **Parent:** [C](#11/c)

Read the squared semiaxis lengths from the denominators in the standard equation obtained in (b). With the positive choice of $C$ there,

$$
\boxed{a=\frac{A}{C^2},\qquad b=\frac1C}.
$$

Since $C^2=A^2-B^2<A^2$, the horizontal semiaxis $a$ is the larger. Thus these are the [semi-major and semi-minor axes](../../euclidean-geometry.md#semi-major-and-semi-minor-axes), respectively.

## 12

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12/a">a</h3>

↑ **Parent:** [12](#12)

<h4 id="12/a/solution">Solution</h4>

↑ **Parent:** [A](#12/a)

Differentiate the sum of [kinetic energy](../../energy.md#kinetic-energy) and [potential energy](../../energy.md#potential-energy) using the [dot product](../../inner-product.md#dot-product) product rule:

$$
\frac{dE}{dt}=m\dot{\mathbf r}\cdot\ddot{\mathbf r}
+k\mathbf r\cdot\dot{\mathbf r}
=\dot{\mathbf r}\cdot(m\ddot{\mathbf r}+k\mathbf r)=0.
$$

The equations of motion make the bracket zero. Hence the [mechanical energy](../../energy.md#mechanical-energy) is **constant in [time](../../classical-mechanics.md#time-in-physics)**. The central [restoring force](../../force.md#restoring-force) can exchange kinetic and [potential energy](../../energy.md#potential-energy) but supplies no change in their sum.

<h3 id="12/b">b</h3>

↑ **Parent:** [12](#12)

<h4 id="12/b/solution">Solution</h4>

↑ **Parent:** [B](#12/b)

Set $\omega=\sqrt{k/m}$. Each coordinate satisfies the [harmonic oscillator equation](../../classical-mechanics.md#simple-harmonic-motion), so the [general solution](../../linear-ordinary-differential-equation.md#general-solution) is

$$
x=A\cos\omega t+B\sin\omega t,\qquad
y=C\cos\omega t+D\sin\omega t.
$$

The four initial data give $A=X_0$, $B=C=0$, and $D=V_0/\omega$. Thus

$$
\boxed{x(t)=X_0\cos\omega t,\qquad y(t)=\frac{V_0}{\omega}\sin\omega t}.
$$

This is the position component of the [isotropic harmonic oscillator flow](../../hamiltonian-mechanics.md#isotropic-harmonic-oscillator-flow). Substitution also gives the constant [energy](../../energy.md) $E=(kX_0^2+mV_0^2)/2$.

<h3 id="12/c">c</h3>

↑ **Parent:** [12](#12)

<h4 id="12/c/solution">Solution</h4>

↑ **Parent:** [C](#12/c)

The stated condition is equivalent to $(V_0/\omega)^2=X_0^2$. Therefore the solution from (b) obeys

$$
x(t)^2+y(t)^2=X_0^2(\cos^2\omega t+\sin^2\omega t)=X_0^2.
$$

For nonzero initial data this is a **[circle](../../topology.md#circle) centred at the origin with radius $|X_0|$**. The sign of $X_0V_0$ chooses its direction of traversal. If $X_0=V_0=0$, the same algebra gives only the stationary origin, a degenerate radius-zero case rather than a genuine circular orbit.

## 13

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13/a">a</h3>

↑ **Parent:** [13](#13)

<h4 id="13/a/solution">Solution</h4>

↑ **Parent:** [A](#13/a)

**As printed, the [function](../../function.md) is undefined at the origin.** For $r^2=x^2+y^2>0$, its [gradient](../../multivariable-calculus.md#gradient) is

$$
\nabla f=\frac{2e^{-1/r^2}}{r^4}(x,y).
$$

The [scalar](../../vector-space.md#scalar) prefactor is positive, and $(x,y)\ne(0,0)$, so this [gradient](../../multivariable-calculus.md#gradient) never vanishes. Thus there are **no [stationary points](../../calculus-of-variations.md#stationary-point) on the stated domain**. Its [infimum](../../real-analysis.md#infimum) is three, approached as $r\to0$, but that value is not attained there.

If the intended definition includes the natural extension $f(0,0)=3$, that extension has a **unique strict [global minimum](../../analysis.md#global-minimum) at the origin**, with value three. Indeed, $e^{-1/r^2}>0$ off zero, and $e^{-1/r^2}/r\to0$ proves differentiability at zero with zero [gradient](../../multivariable-calculus.md#gradient). More strongly, subtracting three gives the [radial Gaussian flat function](../../analysis.md#radial-gaussian-flat-function): every [derivative](../../calculus.md#derivative) of that difference vanishes at the origin. The vanishing [Hessian matrix](../../multivariable-calculus.md#hessian-matrix) does not turn this minimum into an [inflection point](../../topology.md#inflection-point). These are two different domain interpretations; the extension must be stated rather than silently inserted.

<h3 id="13/b">b</h3>

↑ **Parent:** [13](#13)

<h4 id="13/b/solution">Solution</h4>

↑ **Parent:** [B](#13/b)

Write $h(x,y)=y(r-4)$, where $r=\sqrt{x^2+y^2}$. Because this [hyperbolic function](../../calculus.md#hyperbolic-function) has strictly positive [derivative](../../calculus.md#derivative) $\cosh$, [stationary points under an increasing outer function](../../calculus-of-variations.md#stationary-points-under-an-increasing-outer-function) have the same positions and types for $g=\sinh h$ and $h$. For $r>0$,

$$
h_x=\frac{xy}{r},\qquad h_y=r+\frac{y^2}{r}-4.
$$

The first equation requires $x=0$ or $y=0$. If $y=0$, the second gives $|x|=4$. If $x=0$, it gives $2|y|=4$. These are all the nonzero [stationary points](../../calculus-of-variations.md#stationary-point). At the origin, $h=-4y+O(r^2)$, so its [gradient](../../multivariable-calculus.md#gradient) is $(0,-4)$; the origin is not stationary.

At $(0,2)$ the [Hessian matrix](../../multivariable-calculus.md#hessian-matrix) of $h$ is $\operatorname{diag}(1,2)$, and at $(0,-2)$ it is $\operatorname{diag}(-1,-2)$. At $(4,0)$ and $(-4,0)$ its [Hessian matrices](../../multivariable-calculus.md#hessian-matrix) are respectively $\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and $\begin{pmatrix}0&-1\\-1&0\end{pmatrix}$. Therefore

$$
\boxed{\begin{array}{c|c|c}
(x,y)&g(x,y)&\text{type}\\\hline
(0,2)&-\sinh4&\text{strict local minimum}\\
(0,-2)&\sinh4&\text{strict local maximum}\\
(4,0),\ (-4,0)&0&\text{saddles}
\end{array}}
$$

The extrema are local: $g$ is unbounded above and below on the full [plane](../../geometry-and-topology.md#plane).

For the [level curve](../../topology.md#level-curve) geometry, a level $g=c$ is $y(r-4)=\operatorname{arsinh}c$. In particular, the zero [level curve](../../topology.md#level-curve) is the union of the entire $x$ axis and the [circle](../../topology.md#circle) $r=4$, crossing at the two [saddle points](../../analysis.md#saddle-point). Inside the [circle](../../topology.md#circle), $g<0$ above the axis and $g>0$ below it; outside, these signs reverse. Levels between $-\sinh4$ and zero have closed loops around the upper minimum as well as unbounded lower-half-plane components. Reflection across the $x$ axis reverses the sign and gives the loops about the lower maximum. At the two extremal heights, the corresponding closed loop shrinks to its extremum. These features determine the sketch.

<a id="13/b/image-level-curves-and-all-four-stationary-points-of-the-radial-hyperbolic-sine-function"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2-sinh-radial-contours.png)

**[Figure 1](#13/b/image-level-curves-and-all-four-stationary-points-of-the-radial-hyperbolic-sine-function). Level curves and all four stationary points of the radial hyperbolic-sine function**.

## 14

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14/a">a</h3>

↑ **Parent:** [14](#14)

<h4 id="14/a/i">i</h4>

↑ **Parent:** [A](#14/a)

<h5 id="14/a/i/solution">Solution</h5>

↑ **Parent:** [I](#14/a/i)

Let $N=\sqrt8\,A$ be the unscaled [matrix](../../vector-space.md#matrix). Expansion along its third row gives

$$
\det N=2(\sqrt2+\sqrt{18})+2(\sqrt{18}+\sqrt2)=16\sqrt2.
$$

Scaling a three-by-three [matrix](../../vector-space.md#matrix) by $1/\sqrt8$ scales its [determinant](../../multilinear-algebra.md#determinant) by $(\sqrt8)^{-3}$. Therefore

$$
\boxed{\det A=\frac{16\sqrt2}{(\sqrt8)^3}=1}.
$$

<h4 id="14/a/ii">ii</h4>

↑ **Parent:** [A](#14/a)

<h5 id="14/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14/a/ii)

The three columns of $N=\sqrt8\,A$ are $(\sqrt3,1,2)$, $(-\sqrt2,\sqrt6,0)$, and $(-\sqrt3,-1,2)$. Each has squared [Euclidean norm](../../normed-vector-space.md#euclidean-norm) eight. Their pairwise [dot products](../../inner-product.md#dot-product) are

$$
-\sqrt6+\sqrt6=0,\qquad -3-1+4=0,\qquad \sqrt6-\sqrt6=0.
$$

Hence $N^{\mathsf T}N=8I$, so $\boxed{A^{\mathsf T}A=I}$. Thus $A$ is an [orthogonal matrix](../../linear-algebra.md#orthogonal-matrix), with $A^{-1}=A^{\mathsf T}$. The [determinant](../../multilinear-algebra.md#determinant) from (i) places it in the determinant-one component.

<h3 id="14/b">b</h3>

↑ **Parent:** [14](#14)

<h4 id="14/b/i">i</h4>

↑ **Parent:** [B](#14/b)

<h5 id="14/b/i/solution">Solution</h5>

↑ **Parent:** [I](#14/b/i)

The [transpose](../../vector-space.md#transpose) rule gives $(BC)^{\mathsf T}=C^{\mathsf T}B^{\mathsf T}$. If $C$ is [orthogonal](../../inner-product.md#orthogonal-vectors), $C^{-1}=C^{\mathsf T}$, and the identity becomes

$$
C^{\mathsf T}(B^{\mathsf T}+B)=0.
$$

Multiplying on the left by $C$ yields $\boxed{B^{\mathsf T}=-B}$. This is precisely the defining condition for an [antisymmetric matrix](../../linear-algebra.md#skew-symmetric-matrix).

<h4 id="14/b/ii">ii</h4>

↑ **Parent:** [B](#14/b)

<h5 id="14/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14/b/ii)

The inverse appearing in the assumption requires $\det C\ne0$. Taking [determinants](../../multilinear-algebra.md#determinant) of $(BC)^{\mathsf T}=-C^{-1}B$ gives

$$
\det B\,\det C=-\frac{\det B}{\det C},
$$

where the minus sign comes from the odd [matrix](../../vector-space.md#matrix) order. Multiplying by $\det C$ gives $\det B((\det C)^2+1)=0$. Since $C$ is real, the second factor is positive. Thus $\boxed{\det B=0}$ and $B$ is a [singular matrix](../../linear-algebra.md#singular-matrix). This is the [singularity forced by an odd-dimensional transpose-inverse identity](../../linear-algebra.md#singularity-forced-by-an-odd-dimensional-transpose-inverse-identity), with the roles of the two [matrix](../../vector-space.md#matrix) letters exchanged.

## 15

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15/solution">Solution</h3>

↑ **Parent:** [15](#15)

Use the real [Fourier series](../../fourier-series.md) convention $f=a_0/2+\sum_{n\geq1}(a_n\cos nx+b_n\sin nx)$. The [function](../../function.md) is an [even function](../../calculus.md#even-function), so $b_n=0$. For noninteger real $\mu$,

$$
a_0=\frac2\pi\int_0^\pi\cos(\mu x)\,dx=\frac{2\sin\pi\mu}{\pi\mu}.
$$

For $n\geq1$, the product-to-sum identity gives

$$
\begin{aligned}
a_n&=\frac1\pi\left(\frac{\sin\pi(\mu-n)}{\mu-n}
+\frac{\sin\pi(\mu+n)}{\mu+n}\right)\\
&=\frac{2\mu(-1)^n\sin\pi\mu}{\pi(\mu^2-n^2)}.
\end{aligned}
$$

Thus the [Fourier series of a noninteger-frequency cosine](../../fourier-series.md#fourier-series-of-a-noninteger-frequency-cosine) is

$$
\boxed{f(x)=\frac{\sin\pi\mu}{\pi\mu}
+\frac{2\mu\sin\pi\mu}{\pi}\sum_{n=1}^{\infty}
\frac{(-1)^n\cos nx}{\mu^2-n^2}}.
$$

Its [Fourier coefficients](../../fourier-series.md#fourier-coefficient) are $O(n^{-2})$, giving [absolute convergence](../../sequence-and-series.md#absolute-convergence) and [uniform convergence](../../sequence-and-series.md#uniform-convergence). The periodic [function](../../function.md) is continuous at its joins because the two endpoint cosine values coincide, so the [Dirichlet-Jordan convergence theorem](../../fourier-series.md#dirichlet-jordan-convergence-theorem) gives this value at every point.

Putting $\mu=1/3$ gives

$$
\boxed{f(x)=\frac{3\sqrt3}{2\pi}-\frac{3\sqrt3}{\pi}
\sum_{n=1}^{\infty}\frac{(-1)^n\cos nx}{9n^2-1}}.
$$

Evaluate at $x=0$, where $f(0)=1$, and multiply by $\pi/\sqrt3$:

$$
\frac\pi{\sqrt3}=\frac32-3\sum_{n=1}^{\infty}\frac{(-1)^n}{9n^2-1}
=\frac32-\sum_{n=1}^{\infty}\frac{(-1)^n}{3n^2-1/3}.
$$

Comparing with the required form gives $\boxed{A=3,\qquad B=3}$.

## 16

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16/solution">Solution</h3>

↑ **Parent:** [16](#16)

The first field is $\mathbf F_1=(z-y,x,-x)$, so direct [curl](../../multivariable-calculus.md#curl) calculation gives

$$
\boxed{\nabla\times\mathbf F_1=(0,2,2)=2\mathbf a}.
$$

It is **not conservative** because its [curl](../../multivariable-calculus.md#curl) is nonzero. The second is a radial [gradient](../../multivariable-calculus.md#gradient) field:

$$
\mathbf F_2=\nabla\left[-\frac1{\sqrt{1+r^2}}\right],
\qquad\boxed{\nabla\times\mathbf F_2=0}.
$$

The [scalar](../../vector-space.md#scalar) expression is a [smooth function](../../analysis.md#smooth-function) and single-valued on all of space, so $\mathbf F_2$ is a [conservative vector field](../../multivariable-calculus.md#conservative-vector-field). Its [potential of a conservative vector field](../../multivariable-calculus.md#potential-of-a-conservative-vector-field) is $\Phi=-(1+r^2)^{-1/2}$. Parts (a) and (b) check path dependence directly.

<h3 id="16/a">a</h3>

↑ **Parent:** [16](#16)

<h4 id="16/a/solution">Solution</h4>

↑ **Parent:** [A](#16/a)

Parametrize the segment by $\mathbf r(t)=(1-t,t,0)$, $0\leq t\leq1$, so $\mathbf r'=(-1,1,0)$. For the first field, $\mathbf F_1=(-t,1-t,-1+t)$ and its [dot product](../../inner-product.md#dot-product) with the tangent is one. Therefore

$$
\boxed{\int_{\rm segment}\mathbf F_1\cdot d\mathbf r=1}.
$$

For the second field, use the [fundamental theorem for line integrals](../../multivariable-calculus.md#fundamental-theorem-for-line-integrals). The endpoints both have $r=1$, so their potential values agree and

$$
\boxed{\int_{\rm segment}\mathbf F_2\cdot d\mathbf r=0}.
$$

Directly, its parameter integrand is $(2t-1)/[1+(1-t)^2+t^2]^{3/2}$, which changes sign under $t\mapsto1-t$ and integrates to zero.

<h3 id="16/b">b</h3>

↑ **Parent:** [16](#16)

<h4 id="16/b/solution">Solution</h4>

↑ **Parent:** [B](#16/b)

The shorter circular arc lies in the $x$-$y$ [plane](../../geometry-and-topology.md#plane) and can be written $\mathbf r(\theta)=(\cos\theta,\sin\theta,0)$, $0\leq\theta\leq\pi/2$. The first field is $(-\sin\theta,\cos\theta,-\cos\theta)$, whose [dot product](../../inner-product.md#dot-product) with $\mathbf r'$ is one. Hence

$$
\boxed{\int_{\rm arc}\mathbf F_1\cdot d\mathbf r=\frac\pi2}.
$$

The second field is radial while the circular tangent is perpendicular to the radius, so $\boxed{\int_{\rm arc}\mathbf F_2\cdot d\mathbf r=0}$. Thus the first field gives different values, $1$ and $\pi/2$, along the two paths, whereas the conservative second field gives the same endpoint difference.

As a check using [Stokes theorem](../../multivariable-calculus.md#stokes-theorem), the arc followed by the reversed segment encloses [area](../../differential-geometry.md#surface-area) $\pi/4-1/2$ in the [plane](../../geometry-and-topology.md#plane). The constant [curl](../../multivariable-calculus.md#curl) has upward component two, giving circulation $2(\pi/4-1/2)=\pi/2-1$, exactly the difference above.

<a id="16/b/image-straight-and-circular-paths-with-the-same-endpoints-enclosing-the-area-responsible-for-their-circulation-difference"></a>
![](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2-line-integral-paths.png)

**[Figure 2](#16/b/image-straight-and-circular-paths-with-the-same-endpoints-enclosing-the-area-responsible-for-their-circulation-difference). Straight and circular paths with the same endpoints, enclosing the area responsible for their circulation difference**.

## 17

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17/a">a</h3>

↑ **Parent:** [17](#17)

<h4 id="17/a/i">i</h4>

↑ **Parent:** [A](#17/a)

<h5 id="17/a/i/solution">Solution</h5>

↑ **Parent:** [I](#17/a/i)

The [law of total probability](../../probability-space.md#law-of-total-probability) weights each jar's red fraction by its selection [probability](../../probability-theory.md#probability):

$$
\boxed{P(R)=\frac12\frac{20}{50}+\frac12\frac{180}{350}
=\frac15+\frac9{35}=\frac{16}{35}}.
$$

The large difference in jar sizes does not change their equal selection [probabilities](../../probability-theory.md#probability); pooling their contents would describe a different experiment.

<h4 id="17/a/ii">ii</h4>

↑ **Parent:** [A](#17/a)

<h5 id="17/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#17/a/ii)

By [Bayes' theorem](../../probability-theory.md#bayes-theorem),

$$
\boxed{P(X\mid R)=\frac{P(R\mid X)P(X)}{P(R)}
=\frac{(20/50)(1/2)}{16/35}=\frac7{16}}.
$$

The denominator sums red outcomes from both possible jar choices, as calculated in (i).

<h3 id="17/b">b</h3>

↑ **Parent:** [17](#17)

<h4 id="17/b/solution">Solution</h4>

↑ **Parent:** [B](#17/b)

Every seven-element subset of the hundred individually identifiable tiles is equally likely. Choose three of the thirty-four vowels and four of the sixty-four consonants; the favourable draw has no blank tiles. Thus

$$
\boxed{P=\frac{\binom{34}{3}\binom{64}{4}}{\binom{100}{7}}}.
$$

This is a [multivariate hypergeometric distribution](../../discrete-probability-distribution.md#multivariate-hypergeometric-distribution) count, including the implicit factor $\binom20=1$ for blanks. Dividing by $\binom{98}{7}$ instead would incorrectly condition on having drawn no blanks.

<h3 id="17/c">c</h3>

↑ **Parent:** [17](#17)

<h4 id="17/c/i">i</h4>

↑ **Parent:** [C](#17/c)

<h5 id="17/c/i/solution">Solution</h5>

↑ **Parent:** [I](#17/c/i)

Put $p=P(A)$ and $q=P(B\mid A)$. Decompose the marginal as $P(B)=P(A\cap B)+P(A^c\cap B)=pq+t$, where $0\leq t\leq1-p$. It follows that

$$
\boxed{pq\leq P(B)\leq pq+1-p}.
$$

Both bounds are attainable: choose none or all of the mass outside $A$ to belong to $B$. More explicitly, the four joint cell masses can be $pq,p(1-q),t,1-p-t$, all nonnegative. This is the first case of [sharp bounds from binary conditional probabilities](../../probability-space.md#sharp-bounds-from-binary-conditional-probabilities).

For the usual conditional-probability ratio, the given $q$ requires $p>0$. If $p=1$, the two bounds coincide at $q$. If $p=0$, the conditional is undefined as a ratio, although its formal joint-model bounds reduce to $0\leq P(B)\leq1$.

<h4 id="17/c/ii">ii</h4>

↑ **Parent:** [C](#17/c)

<h5 id="17/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#17/c/ii)

Write $q=P(B\mid A)$, $s=P(B\mid A^c)$ and $p=P(A)$. The [law of total probability](../../probability-space.md#law-of-total-probability) gives $P(B)=pq+(1-p)s$, a [convex combination](../../convex-set.md#convex-combination) of the two fixed conditional values. Hence

$$
\boxed{\min(q,s)\leq P(B)\leq\max(q,s)}.
$$

These are the closed sharp bounds in the usual mixture-model interpretation, obtained by allowing $p$ to range from zero to one. The joint masses $pq,p(1-q),(1-p)s,(1-p)(1-s)$ realize every such mixture.

There is an endpoint qualification if both conditionals must literally be defined by ratios: then $0<p<1$. If $q\ne s$, the marginal lies strictly between them, so the stated endpoints are an [infimum](../../real-analysis.md#infimum) and [supremum](../../real-analysis.md#supremum) rather than achieved extrema. If $q=s$, every allowed mixture has exactly that common value. This is the second case of [sharp bounds from binary conditional probabilities](../../probability-space.md#sharp-bounds-from-binary-conditional-probabilities).

## 18

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18/a">a</h3>

↑ **Parent:** [18](#18)

<h4 id="18/a/solution">Solution</h4>

↑ **Parent:** [A](#18/a)

Split the integrand into its three coordinate contributions. Each integrates independently over the rectangular box:

$$
\begin{aligned}
I&=\left(\frac23\right)(4)(6)+(2)\left(\frac{16}{3}\right)(6)
+(2)(4)(18)\\
&=16+64+144=\boxed{224}.
\end{aligned}
$$

For example, the last factor is $\int_{-3}^3z^2dz=18$. No spherical or cylindrical Jacobian is needed for this Cartesian [integral](../../integral.md).

<h3 id="18/b">b</h3>

↑ **Parent:** [18](#18)

<h4 id="18/b/solution">Solution</h4>

↑ **Parent:** [B](#18/b)

The region is the [triangle](../../euclidean-geometry.md#triangle) $0\leq y\leq x\leq1$. Reversing the integration order makes the inner [integral](../../integral.md) elementary:

$$
\int_0^1\int_y^1e^{x^2}\,dx\,dy
=\int_0^1\int_0^xe^{x^2}\,dy\,dx
=\int_0^1xe^{x^2}\,dx
=\boxed{\frac{e-1}{2}}.
$$

The integrand is continuous on this compact [triangle](../../euclidean-geometry.md#triangle), so [Fubini theorem](../../measure-theory.md#fubini-s-theorem) justifies exchanging the order.

<h3 id="18/c">c</h3>

↑ **Parent:** [18](#18)

<h4 id="18/c/solution">Solution</h4>

↑ **Parent:** [C](#18/c)

In [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system), the two surfaces meet when $9-r^2=r^2$, giving $r=3/\sqrt2$ and $z=9/2$. The solid has $0\leq r\leq3/\sqrt2$, $0\leq\theta\leq2\pi$, and $r^2\leq z\leq9-r^2$. With [volume element](../../integral.md#volume-element) $r\,dz\,dr\,d\theta$,

$$
\boxed{V=2\pi\int_0^{3/\sqrt2}(9-2r^2)r\,dr
=2\pi\left[\frac92r^2-\frac12r^4\right]_0^{3/\sqrt2}
=\frac{81\pi}{4}}.
$$

The upper-minus-lower height is nonnegative throughout that radial interval.

## 19

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19/a">a</h3>

↑ **Parent:** [19](#19)

<h4 id="19/a/solution">Solution</h4>

↑ **Parent:** [A](#19/a)

Fix the total [area](../../differential-geometry.md#surface-area) at $A_0>0$. Apply [Lagrange multipliers](../../mathematical-optimization.md#lagrange-multiplier) to $V=\pi a^2\ell$ with constraint $G=2\pi a(a+\ell)=A_0$. The two [derivative](../../calculus.md#derivative) equations are

$$
2\pi a\ell=\lambda(4\pi a+2\pi\ell),\qquad
\pi a^2=\lambda\,2\pi a.
$$

Since $a>0$, the second gives $\lambda=a/2$. Substitution in the first gives $\ell=2a$. The constraint then yields $a^2=A_0/(6\pi)$. Therefore

$$
\boxed{V_{\max}=2\pi\left(\frac{A_0}{6\pi}\right)^{3/2}
=\frac13\sqrt{\frac{A_0^3}{6\pi}},\qquad C=6}.
$$

For completeness, eliminating $\ell$ makes $V=(A_0/2)a-\pi a^3$ on $0<a<\sqrt{A_0/(2\pi)}$. Its [derivative](../../calculus.md#derivative) changes from positive to negative at the calculated radius and its [volume](../../geometry-and-topology.md#volume) tends to zero at both domain endpoints. Thus this stationary [cylinder](../../geometry-and-topology.md#cylinder-geometry) is indeed the maximum. It is the fixed-area case of [optimal aspect ratios of closed cylinders](../../geometry-and-topology.md#optimal-aspect-ratios-of-closed-cylinders).

<h3 id="19/b">b</h3>

↑ **Parent:** [19](#19)

<h4 id="19/b/solution">Solution</h4>

↑ **Parent:** [B](#19/b)

Divide the objective [area](../../differential-geometry.md#surface-area) by $2\pi$, which does not change its maximizer, and use $F=a^2+a\ell$ with constraint $G=a^2+\ell^2/4=1$. The [Lagrange multiplier](../../mathematical-optimization.md#lagrange-multiplier) equations are

$$
2a+\ell=2\lambda a,\qquad a=\frac{\lambda\ell}{2}.
$$

At a nondegenerate [cylinder](../../geometry-and-topology.md#cylinder-geometry) $a,\ell>0$, the second gives $\lambda=2a/\ell$. Eliminating it gives $\ell^2+2a\ell=4a^2$. Hence $q=\ell/a$ satisfies $q^2+2q-4=0$. Select its positive root:

$$
\boxed{\frac\ell a=\sqrt5-1,\qquad D=-1,\qquad E=5}.
$$

This is the sphere-inscribed case of [optimal aspect ratios of closed cylinders](../../geometry-and-topology.md#optimal-aspect-ratios-of-closed-cylinders). One may check maximality from $A(q)=2\pi(1+q)/(1+q^2/4)$: its [derivative](../../calculus.md#derivative) has the sign of $4-2q-q^2$, so it changes from positive to negative at the selected root.

## 20

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="20/a">a</h3>

↑ **Parent:** [20](#20)

<h4 id="20/a/solution">Solution</h4>

↑ **Parent:** [A](#20/a)

In the physicists' [Hermite polynomial](../../orthogonal-polynomial.md#hermite-polynomial) convention, begin by differentiating the [Gaussian function](../../calculus.md#gaussian-function):

$$
\frac d{dx}e^{-x^2}=-2xe^{-x^2},\qquad
\frac{d^2}{dx^2}e^{-x^2}=(4x^2-2)e^{-x^2}.
$$

The defining prefactor then gives

$$
\boxed{H_0=1,\qquad H_1=2x,\qquad H_2=4x^2-2}.
$$

The derivative-based definition uses nonnegative integers; negative orders are not part of this [polynomial](../../polynomial.md) definition.

<h3 id="20/b">b</h3>

↑ **Parent:** [20](#20)

<h4 id="20/b/solution">Solution</h4>

↑ **Parent:** [B](#20/b)

Let $u=e^{-x^2}$, so $u'+2xu=0$. Differentiate this identity $n$ times, for $n\geq1$. By the [Leibniz rule](../../calculus.md#leibniz-rule), only the first two [derivatives](../../calculus.md#derivative) of the linear factor $x$ can contribute:

$$
u^{(n+1)}+2xu^{(n)}+2nu^{(n-1)}=0.
$$

Rearranging proves

$$
\boxed{\left(2x+\frac d{dx}\right)\frac{d^n}{dx^n}e^{-x^2}
=-2n\frac{d^{n-1}}{dx^{n-1}}e^{-x^2}}.
$$

The case $n=0$ is the starting identity $u'+2xu=0$, treated separately without introducing a negative [derivative](../../calculus.md#derivative) order.

<h3 id="20/c">c</h3>

↑ **Parent:** [20](#20)

<h4 id="20/c/solution">Solution</h4>

↑ **Parent:** [C](#20/c)

Differentiate the product in the definition of $H_n$. Using the identity in (b),

$$
\begin{aligned}
H_n'&=(-1)^ne^{x^2}\left(2xu^{(n)}+u^{(n+1)}\right)\\
&=-2n(-1)^ne^{x^2}u^{(n-1)}
=2n(-1)^{n-1}e^{x^2}u^{(n-1)}.
\end{aligned}
$$

The last expression is $2nH_{n-1}$, so

$$
\boxed{H_n'=2nH_{n-1}\qquad(n\geq1)}.
$$

Also $H_0'=0$ separately. This is the [Hermite polynomial derivative recurrence](../../orthogonal-polynomial.md#hermite-polynomial-derivative-recurrence) in the physicists' normalization.

## ↑ Ancestors (10)

1. [2010](../2010.md)
2. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
3. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
4. [Year 1 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-1-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
