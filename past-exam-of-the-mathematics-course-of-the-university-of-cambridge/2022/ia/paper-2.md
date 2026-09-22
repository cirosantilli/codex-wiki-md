# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperia_2_2022.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperia_2_2022.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
- [2B](#2b)
  - [Solution](#2b/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5C](#5c)
  - [a](#5c/a)
    - [Solution](#5c/a/solution)
  - [b](#5c/b)
    - [Solution](#5c/b/solution)
- [6A](#6a)
  - [a](#6a/a)
    - [Solution](#6a/a/solution)
  - [b](#6a/b)
    - [Solution](#6a/b/solution)
- [7C](#7c)
  - [a](#7c/a)
    - [Solution](#7c/a/solution)
  - [b](#7c/b)
    - [Solution](#7c/b/solution)
  - [c](#7c/c)
    - [Solution](#7c/c/solution)
- [8B](#8b)
  - [a](#8b/a)
    - [Solution](#8b/a/solution)
  - [b](#8b/b)
    - [Solution](#8b/b/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [Solution](#9f/c/solution)
  - [d](#9f/d)
    - [Solution](#9f/d/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
  - [d](#10f/d)
    - [Solution](#10f/d/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [Solution](#11f/b/solution)
  - [c](#11f/c)
    - [Solution](#11f/c/solution)
  - [d](#11f/d)
    - [Solution](#11f/d/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)
  - [c](#12f/c)
    - [Solution](#12f/c/solution)
  - [d](#12f/d)
    - [Solution](#12f/d/solution)

## 1A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1a/solution">Solution</h3>

↑ **Parent:** [1A](#1a)

[Differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) first gives

$$
I'(x)=\int_0^\pi \cos\theta\,e^{x\cos\theta}\,d\theta.
$$

On the other hand,

$$
\frac d{d\theta}\left(\sin\theta\,e^{x\cos\theta}\right)
=\cos\theta\,e^{x\cos\theta}
-x\sin^2\theta\,e^{x\cos\theta}.
$$

Its integral is zero because $\sin\theta$ vanishes at both endpoints. Hence

$$
\boxed{I'(x)=\int_0^\pi x\sin^2\theta\,e^{x\cos\theta}\,d\theta}.
$$

Differentiating once more,

$$
I''(x)=\int_0^\pi\cos^2\theta\,e^{x\cos\theta}\,d\theta.
$$

For $x\ne0$, the preceding identity and $\sin^2\theta+\cos^2\theta=1$ give

$$
I''+\frac1xI'-I
=\int_0^\pi(\cos^2\theta+\sin^2\theta-1)e^{x\cos\theta}\,d\theta=0.
$$

The equation extends through $x=0$ in its regular limiting form.

## 2B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2b/solution">Solution</h3>

↑ **Parent:** [2B](#2b)

The characteristic polynomial of the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) is

$$
r^3-6r^2+12r-8=(r-2)^3.
$$

The repeated-root rule therefore gives

$$
x_n=(A+Bn+Cn^2)2^n.
$$

The condition $x_0=0$ gives $A=0$. The other two conditions give

$$
2(B+C)=4,\qquad
4(2B+4C)=24,
$$

so $B+C=2$ and $B+2C=3$. Thus $B=C=1$, and

$$
\boxed{x_n=n(n+1)2^n}.
$$

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

A function $f$ on an interval is a [convex function](../../../real-analysis.md#convex-function) if

$$
f(tx+(1-t)y)\leq tf(x)+(1-t)f(y)
\qquad(0\leq t\leq1).
$$

[Jensen inequality](../../../real-analysis.md#jensen-s-inequality) states that for an integrable random variable $X$, when all terms are defined,

$$
f(\mathbb E X)\leq\mathbb E[f(X)].
$$

The function $\phi(x)=x\log x$ is convex on $(0,\infty)$ because

$$
\phi''(x)=\frac1x>0.
$$

Applying Jensen's inequality to the uniform distribution on the positive numbers $x_1,\ldots,x_n$ gives

$$
\frac1n\sum_{i=1}^nx_i\log x_i
\geq
\left(\frac1n\sum_{i=1}^nx_i\right)
\log\left(\frac1n\sum_{i=1}^nx_i\right).
$$

Writing $S=\sum_i x_i$ and multiplying by $n/S$ yields

$$
\boxed{
\frac{\sum_{i=1}^nx_i\log x_i}{\sum_{i=1}^nx_i}
\geq\log\left(\frac{\sum_{i=1}^nx_i}{n}\right)}.
$$

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

Expanding around the [expected value](../../../probability-theory.md#expected-value) $\mu$,

$$
G(a)=\mathbb E[(X-\mu+\mu-a)^2]
=\mathbb E[(X-\mu)^2]+(\mu-a)^2,
$$

because $\mathbb E[X-\mu]=0$. Therefore

$$
\boxed{G(a)=\sigma^2+(\mu-a)^2\geq\sigma^2},
$$

with equality exactly when $a=\mu$.

For the absolute loss,

$$
H(a)=\int_{-\infty}^a(a-x)f(x)\,dx
+\int_a^\infty(x-a)f(x)\,dx.
$$

Leibniz differentiation gives, with $F(a)=\int_{-\infty}^af(x)\,dx$,

$$
H'(a)=F(a)-(1-F(a))=2F(a)-1.
$$

Thus $H$ decreases while $F(a)<1/2$ and increases while $F(a)>1/2$. It is minimized at any [median](../../../probability-theory.md#median), characterized in the continuous case by

$$
\boxed{\int_{-\infty}^af(x)\,dx=\frac12}.
$$

## 5C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5c/a">a</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/a/solution">Solution</h4>

↑ **Parent:** [A](#5c/a)

For a normalized equation

$$
y''+P(x)y'+Q(x)y=0,
$$

$x_0$ is an ordinary point when $P,Q$ are analytic there. It is a regular singular point when $(x-x_0)P(x)$ and $(x-x_0)^2Q(x)$ are analytic there. These are the [ordinary point criterion for a second-order equation](../../../complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) and [regular singular point criterion for a second-order equation](../../../complex-analysis.md#regular-singular-point-criterion-for-a-second-order-equation).

Here

$$
P(x)=\frac1x-1,\qquad Q(x)=\frac{\lambda}{x},
$$

so $x=0$ is regular singular. Seek a [power-series solution of a differential equation](../../../differential-equation.md#power-series-solution-of-a-differential-equation)

$$
y=\sum_{n=0}^{\infty}a_nx^n.
$$

Equating the coefficient of $x^n$ gives

$$
(n+1)^2a_{n+1}+(\lambda-n)a_n=0,
$$

and hence

$$
a_{n+1}=\frac{n-\lambda}{(n+1)^2}a_n.
$$

Therefore

$$
\boxed{
a_n=a_0\frac{\prod_{j=0}^{n-1}(j-\lambda)}{(n!)^2}},
\qquad
y=a_0\sum_{n=0}^{\infty}
\frac{\prod_{j=0}^{n-1}(j-\lambda)}{(n!)^2}x^n.
$$

The series terminates exactly when $\lambda=N$ is a nonnegative integer: the factor with $j=N$ then makes $a_{N+1}=0$. Thus the polynomial solutions occur for

$$
\boxed{\lambda=0,1,2,\ldots}.
$$

<h3 id="5c/b">b</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/b/solution">Solution</h4>

↑ **Parent:** [B](#5c/b)

After division by $x$, the coefficient of $y'$ is $P(x)=1/x-1$. The [Abel identity](../../../differential-equation.md#abel-s-identity) for the [Wronskian](../../../differential-equation.md#wronskian) gives

$$
W'=-P(x)W=\left(1-\frac1x\right)W,
$$

so

$$
\boxed{W(x)=C\frac{e^x}{x}}.
$$

For $\lambda=1$, direct substitution confirms that $y_1=1-x$. [Reduction of order](../../../differential-equation.md#reduction-of-order) gives a second solution proportional to

$$
y_2=(1-x)\int\frac{e^x}{x(1-x)^2}\,dx.
$$

To extract the requested coefficients, put

$$
y_2=(1-x)\log x+b_1x+b_2x^2+\cdots.
$$

For the differential operator

$$
L[y]=xy''+(1-x)y'+y,
$$

one finds

$$
L[(1-x)\log x]=x-3.
$$

The analytic correction $h=\sum_{n\geq1}b_nx^n$ must therefore satisfy $L[h]=3-x$. Its constant and linear coefficients give

$$
b_1=3,\qquad 4b_2=-1.
$$

Hence

$$
\boxed{
y_2=(1-x)\log x+3x-\frac14x^2+\cdots}.
$$

## 6A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6a/a">a</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/a/solution">Solution</h4>

↑ **Parent:** [A](#6a/a)

The multivariable [chain rule](../../../calculus.md#chain-rule) gives, at $(x,y)=(a+t\cos\gamma,b+t\sin\gamma)$,

$$
g'(t)=f_x\cos\gamma+f_y\sin\gamma,
$$



$$
g''(t)=f_{xx}\cos^2\gamma
+2f_{xy}\sin\gamma\cos\gamma
+f_{yy}\sin^2\gamma.
$$

Sufficient conditions for a strict local minimum at $t=0$ are $g'(0)=0$ and $g''(0)>0$.

At a [stationary point](../../../calculus-of-variations.md#stationary-point), $g'(0)=0$ in every direction. Its second derivative is the quadratic form of the [Hessian matrix](../../../calculus.md#hessian-matrix). If

$$
f_{yy}>0,\qquad f_{xx}f_{yy}-f_{xy}^2>0,
$$

then completing the square gives

$$
f_{xx}u^2+2f_{xy}uv+f_{yy}v^2
=f_{yy}\left(v+\frac{f_{xy}}{f_{yy}}u\right)^2
+\frac{f_{xx}f_{yy}-f_{xy}^2}{f_{yy}}u^2>0
$$

for every nonzero direction $(u,v)$. The Hessian is therefore [positive definite](../../../linear-algebra.md#positive-definite-matrix), and the stationary point is a strict local minimum.

<h3 id="6a/b">b</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/b/solution">Solution</h4>

↑ **Parent:** [B](#6a/b)

The stationary equations are

$$
4x^3-6x+2y=0,\qquad 2x+2y=0.
$$

Thus $y=-x$ and $4x(x^2-2)=0$, giving

$$
(0,0),\qquad(\sqrt2,-\sqrt2),\qquad(-\sqrt2,\sqrt2).
$$

The [Hessian matrix](../../../calculus.md#hessian-matrix) is

$$
H=\begin{pmatrix}12x^2-6&2\\2&2\end{pmatrix}.
$$

At either nonzero stationary point,

$$
H=\begin{pmatrix}18&2\\2&2\end{pmatrix},
\qquad \det H=32>0,
$$

so both are strict local minima.

Along a line through the origin,

$$
g(t)=f(t\cos\gamma,t\sin\gamma)
=t^2q(\gamma)+t^4\cos^4\gamma,
$$

where

$$
q(\gamma)=-3\cos^2\gamma
+2\sin\gamma\cos\gamma+\sin^2\gamma.
$$

When $\cos\gamma\ne0$ and $r=\tan\gamma$,

$$
q(\gamma)=\cos^2\gamma(r-1)(r+3).
$$

Consequently the origin is a local minimum along the line when

$$
\boxed{\tan\gamma\leq-3\quad\text{or}\quad\tan\gamma\geq1},
$$

including the equality cases because the positive quartic term then leads. It is also a minimum on the vertical line. It is a local maximum along the line when

$$
\boxed{-3<\tan\gamma<1}.
$$

In the first case the graph is locally bowl-shaped. In the second it initially bends downward from the origin, but the positive quartic term eventually turns it upward, producing the usual double-well profile.

## 7C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7c/a">a</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/a/solution">Solution</h4>

↑ **Parent:** [A](#7c/a)

The [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is

$$
\det(A-\lambda I)=\lambda(\lambda-1).
$$

For $\lambda_1=0$ and $\lambda_2=1$, corresponding [eigenvectors](../../../linear-operator-theory.md#eigenvector) are

$$
u_1=\begin{pmatrix}2\\1\end{pmatrix},
\qquad
u_2=\begin{pmatrix}3\\1\end{pmatrix}.
$$

They are linearly independent, so the general homogeneous solution is

$$
\boxed{
z(t)=\alpha\begin{pmatrix}2\\1\end{pmatrix}
+\beta e^t\begin{pmatrix}3\\1\end{pmatrix}}.
$$

<h3 id="7c/b">b</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/b/solution">Solution</h4>

↑ **Parent:** [B](#7c/b)

Resolve the forcing in the eigenbasis:

$$
\begin{pmatrix}1\\a\end{pmatrix}
=(3a-1)u_1+(1-2a)u_2.
$$

In the zero-eigenvalue direction, a constant forcing produces the particular integral $(3a-1)t\,u_1$. In the unit-eigenvalue direction, a constant particular integral is $-(1-2a)u_2$. Thus a particular integral depends on time exactly when

$$
\boxed{a\ne\frac13}.
$$

Adding the complementary solution from part (a), the general solution is

$$
\boxed{
z(t)=\alpha u_1+\beta e^tu_2
+(3a-1)t\,u_1-(1-2a)u_2}.
$$

This is the eigenvector form of the usual [variation of parameters](../../../differential-equation.md#variation-of-parameters) calculation.

<h3 id="7c/c">c</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/c/solution">Solution</h4>

↑ **Parent:** [C](#7c/c)

For either eigenpair above, $\lambda_i\in\{0,1\}$ and hence $\lambda_i^n=\lambda_i$ for every positive integer $n$. Therefore

$$
\frac{d^n}{dt^n}(u_i e^{\lambda_it})
=\lambda_i^n u_i e^{\lambda_it}
=A u_i e^{\lambda_it},
$$

so both terms in the solution from part (a), and every linear combination of them, solve the higher-order system.

A system of two scalar differential equations of order $n$ has a $2n$-dimensional solution space. The displayed family supplies two independent solutions, so there must be

$$
\boxed{2n-2}
$$

further linearly independent solutions.

## 8B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8b/a">a</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/a/solution">Solution</h4>

↑ **Parent:** [A](#8b/a)

Write the vector field as

$$
\dot x=2x(4-x-y^2),\qquad \dot y=y(x-1).
$$

The [equilibrium points of a dynamical system](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) in the closed first quadrant are

$$
\boxed{(0,0),\quad(4,0),\quad(1,\sqrt3)}.
$$

The [Jacobian matrix](../../../calculus.md#jacobian-matrix) is

$$
J(x,y)=
\begin{pmatrix}
8-4x-2y^2&-4xy\\
y&x-1
\end{pmatrix}.
$$

At $(0,0)$ its eigenvalues are $8,-1$, so this is a [saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium). Its unstable direction is the positive $x$-axis and its stable direction is the positive $y$-axis; to first order, nearby trajectories satisfy $\dot x=8x$, $\dot y=-y$.

At $(4,0)$ the eigenvalues are $-8,3$, so it is also a saddle. The $x$-axis is the stable direction, while trajectories entering the quadrant in the $y$ direction move away.

At $(1,\sqrt3)$,

$$
J=\begin{pmatrix}-2&-4\sqrt3\\ \sqrt3&0\end{pmatrix},
$$

whose eigenvalues are

$$
-1\mathbin{\pm}i\sqrt{11}.
$$

It is therefore a [stable spiral](../../../dynamical-systems.md#stable-spiral). A point immediately to its right moves upward, so nearby trajectories spiral counterclockwise into the equilibrium. These eigendirections and the inward spiral give the requested local phase-portrait sketches.

<h3 id="8b/b">b</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/b/solution">Solution</h4>

↑ **Parent:** [B](#8b/b)

The only positive equilibrium solves $1-y=0$ and $x-1=0$, hence is

$$
\boxed{(x,y)=(1,1)}.
$$

Away from a nullcline,

$$
\frac{dy}{dx}
=\frac{3y(x-1)}{x(1-y)}.
$$

This is separable:

$$
\left(\frac1y-1\right)dy
=3\left(1-\frac1x\right)dx.
$$

Integration gives the [first integral](../../../differential-equation.md#first-integral)

$$
\log y-y=3x-3\log x+C.
$$

Thus one convenient conserved quantity is

$$
\boxed{E(x,y)=3x-3\log x+y-\log y}.
$$

Its gradient is

$$
\nabla E=\left(3-\frac3x,\,1-\frac1y\right),
$$

so $(1,1)$ is its only stationary point in the positive quadrant. Its [Hessian matrix](../../../calculus.md#hessian-matrix) is

$$
\nabla^2E=
\begin{pmatrix}3/x^2&0\\0&1/y^2\end{pmatrix},
$$

which is positive definite everywhere. Hence $(1,1)$ is a strict, indeed global, minimum.

The nearby level curves of $E$ are closed curves surrounding this minimum. Since $E$ is constant along every trajectory, a solution starting on a sufficiently small nearby level set cannot leave the region bounded by a slightly larger level set. This proves [Lyapunov stability](../../../dynamical-systems.md#lyapunov-stability) of the equilibrium: solutions initially close to $(1,1)$ remain close for all time.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

Because $U$ and $V$ are bounded, their exponential series may be integrated term by term for every real $t$. Thus their [moment-generating functions](../../../probability-theory.md#moment-generating-function) satisfy

$$
M_U(t)=\mathbb E[e^{tU}]
=\sum_{j=0}^{\infty}\frac{t^j}{j!}\mathbb E[U^j],
$$

and similarly for $V$. Equality of every moment gives equality term by term, so

$$
\boxed{M_U(t)=M_V(t)\quad\text{for every }t\in\mathbb R}.
$$

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

Normalization of the [Gaussian distribution](../../../probability-theory.md#normal-distribution) gives

$$
A=\frac1{\sqrt{2\pi}}.
$$

Completing the square,

$$
tx-\frac{x^2}{2}
=-\frac{(x-t)^2}{2}+\frac{t^2}{2}.
$$

Therefore

$$
M_X(t)=\frac1{\sqrt{2\pi}}
\int_{-\infty}^{\infty}e^{tx-x^2/2}\,dx
=e^{t^2/2},
$$

and hence

$$
\boxed{M_X(t)=e^{t^2/2}}.
$$

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

The normalizing constant satisfies

$$
B^{-1}=\sum_{n\in\mathbb Z}e^{-n^2/2}.
$$

For an integer $k$,

$$
\mathbb E[e^{kY}]
=B\sum_{n\in\mathbb Z}e^{kn-n^2/2}
=Be^{k^2/2}\sum_{n\in\mathbb Z}e^{-(n-k)^2/2}.
$$

Translation by the integer $k$ merely permutes the summation indices, so the final sum is $B^{-1}$. Consequently

$$
\boxed{\mathbb E[e^{kY}]=e^{k^2/2}
=\mathbb E[e^{kX}]}.
$$

The last equality uses the [moment-generating function](../../../probability-theory.md#moment-generating-function) of the standard normal variable from part (b).

<h3 id="9f/d">d</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/d/solution">Solution</h4>

↑ **Parent:** [D](#9f/d)

**No.** A standard counterexample comes from the [log-normal distribution](../../../probability-theory.md#log-normal-distribution). Let

$$
f(x)=\frac1{x\sqrt{2\pi}}
\exp\left(-\frac{(\log x)^2}{2}\right),
\qquad x>0,
$$

and, for a fixed $0<|\varepsilon|\leq1$, let

$$
f_\varepsilon(x)
=f(x)\left[1+\varepsilon\sin(2\pi\log x)\right].
$$

This is a nonnegative density distinct from $f$. For every nonnegative integer $n$, substituting $z=\log x$ makes the difference of the $n$th moments proportional to

$$
\mathbb E[e^{nZ}\sin(2\pi Z)],
\qquad Z\sim N(0,1).
$$

It is the imaginary part of

$$
\mathbb E[e^{(n+2\pi i)Z}]
=\exp\left(\frac{(n+2\pi i)^2}{2}\right),
$$

which vanishes because its phase is $2\pi n$. The case $n=0$ also proves that $f_\varepsilon$ is normalized. Thus the two distributions have every finite moment equal but are different. Unbounded random variables need not be determined by their moments.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

The [probability generating function](../../../probability-theory.md#probability-generating-function) is

$$
G_X(s)=\sum_{m=1}^{\infty}\mathbb P(X=m)s^m.
$$

Differentiating $n$ times,

$$
G_X^{(n)}(s)
=\sum_{m=n}^{\infty}
\frac{m!}{(m-n)!}\mathbb P(X=m)s^{m-n}.
$$

At $s=0$, only the term $m=n$ remains. Hence

$$
\boxed{\mathbb P(X=n)=\frac{G_X^{(n)}(0)}{n!}}.
$$

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

For $0\leq s\leq1$, independence gives

$$
G_{X+Y}(s)
=\mathbb E[s^{X+Y}]
=\mathbb E[s^Xs^Y]
=\mathbb E[s^X]\,\mathbb E[s^Y].
$$

Therefore

$$
\boxed{G_{X+Y}(s)=G_X(s)G_Y(s)}.
$$

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

For the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) on $\{1,2,\ldots\}$,

$$
\mathbb P(X=m)=p(1-p)^{m-1}.
$$

Summing the [geometric series](../../../real-analysis.md#geometric-series),

$$
G_X(s)
=\sum_{m=1}^{\infty}p(1-p)^{m-1}s^m
=\boxed{\frac{ps}{1-(1-p)s}}.
$$

<h3 id="10f/d">d</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/d/solution">Solution</h4>

↑ **Parent:** [D](#10f/d)

When $r$ red marbles remain, the next draw reduces their number with probability $r/n$. The waiting time $W_r$ for that reduction has a [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) on $\{1,2,\ldots\}$ and therefore

$$
G_{W_r}(s)
=\frac{(r/n)s}{1-(1-r/n)s}
=\frac{rs}{n-(n-r)s}.
$$

The successive waiting times are independent, and

$$
T=W_n+W_{n-1}+\cdots+W_1.
$$

Using the product rule for probability-generating functions,

$$
\boxed{
G_T(s)=\prod_{r=1}^{n}
\frac{rs}{n-(n-r)s}}.
$$

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

The number of heads has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution). Choosing the $k$ head positions gives

$$
\boxed{\mathbb P(\text{exactly }k\text{ heads})
=\binom nk p^k(1-p)^{n-k}}.
$$

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

Conditioned on exactly $k$ heads, every $k$-element set of head positions is equally likely. There are $\binom nk$ such sets. A run containing all $k$ heads can begin at any of the positions

$$
1,2,\ldots,n-k+1,
$$

and each beginning determines one admissible set. Thus, for $k\geq1$,

$$
\boxed{
\mathbb P(\text{the }k\text{ heads are consecutive}\mid
\text{exactly }k\text{ heads})
=\frac{n-k+1}{\binom nk}}.
$$

<h3 id="11f/c">c</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/c/solution">Solution</h4>

↑ **Parent:** [C](#11f/c)

For the process to stop on toss $n$, the last toss must be the $k$th head, while the first $n-1$ tosses must contain exactly $k-1$ heads. Hence the [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) gives

$$
\boxed{
\mathbb P(T=n)
=\binom{n-1}{k-1}p^k(1-p)^{n-k}},
\qquad n\geq k.
$$

<h3 id="11f/d">d</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/d/solution">Solution</h4>

↑ **Parent:** [D](#11f/d)

Let $E_j$ be the expected additional number of tosses when the current terminal run contains $j$ consecutive heads. Then $E_k=0$, and for $0\leq j<k$,

$$
E_j=1+pE_{j+1}+(1-p)E_0.
$$

For $0<p<1$, iterating this recurrence from $j=k-1$ down to $0$ gives

$$
E_0=\bigl(1+(1-p)E_0\bigr)
\frac{1-p^k}{1-p}.
$$

Solving,

$$
\boxed{
E_0=\frac{1-p^k}{(1-p)p^k}}.
$$

When $p=1$, the waiting time is deterministically $k$, which is also the continuous limit of this formula as $p\to1$.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

By [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) for the nonnegative indicators,

$$
\mathbb E[N]
=\mathbb E\left[\sum_{n\geq1}\mathbf1_{A_n}\right]
=\sum_{n\geq1}\mathbb P(A_n).
$$

If this is finite, then $N$ is finite almost surely: alternatively, [Markov inequality](../../../probability-inequality.md#markov-inequality) gives

$$
\mathbb P(N\geq m)\leq\frac{\mathbb E[N]}m\longrightarrow0.
$$

Since $\{N=\infty\}\subseteq\{N\geq m\}$ for every $m$,

$$
\boxed{\mathbb P(N=\infty)=0}.
$$

This is the first [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas).

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

Write $p_n=\mathbb P(A_n)$. Independence gives, first for finite partial counts and then by monotone convergence,

$$
\mathbb E[2^{-N}]
=\prod_{n\geq1}
\mathbb E[2^{-\mathbf1_{A_n}}]
=\prod_{n\geq1}\left(1-\frac{p_n}{2}\right).
$$

Using $1-x\leq e^{-x}$ factor by factor,

$$
\boxed{
\mathbb E[2^{-N}]
\leq\exp\left(-\frac12\sum_{n\geq1}p_n\right)
=e^{-\mathbb E[N]/2}}.
$$

<h3 id="12f/c">c</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/c/solution">Solution</h4>

↑ **Parent:** [C](#12f/c)

If $\sum_n\mathbb P(A_n)=\infty$, part (b) gives

$$
0\leq\mathbb E[2^{-N}]\leq e^{-\infty}=0.
$$

Thus $2^{-N}=0$ almost surely. By the convention in the question, this occurs exactly when $N=\infty$. Therefore

$$
\boxed{\mathbb P(N=\infty)=1}.
$$

This is the second [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) for independent events.

<h3 id="12f/d">d</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/d/solution">Solution</h4>

↑ **Parent:** [D](#12f/d)

Divide the keystrokes into disjoint blocks of five, and let $A_n$ be the event that block $n$ is exactly HELLO. The events are [independent events](../../../probability-theory.md#independent-events), and

$$
\mathbb P(A_n)=26^{-5}.
$$

Consequently

$$
\sum_{n=1}^{\infty}\mathbb P(A_n)=\infty.
$$

Part (c) shows that infinitely many of these block events occur almost surely. Each occurrence is an occurrence of HELLO in the full typed sequence, so

$$
\boxed{\mathbb P(\text{HELLO appears infinitely often})=1}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
