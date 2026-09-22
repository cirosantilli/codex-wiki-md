# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2017/paperia_2_0.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2017/paperia_2_0.pdf)

**Table of contents**

- [1C](#1c)
  - [a](#1c/a)
    - [Solution](#1c/a/solution)
  - [b](#1c/b)
    - [Solution](#1c/b/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [i](#4f/i)
    - [Solution](#4f/i/solution)
  - [ii](#4f/ii)
    - [Solution](#4f/ii/solution)
- [5C](#5c)
  - [a](#5c/a)
    - [Solution](#5c/a/solution)
  - [b](#5c/b)
    - [Solution](#5c/b/solution)
  - [c](#5c/c)
    - [i](#5c/c/i)
      - [Solution](#5c/c/i/solution)
    - [ii](#5c/c/ii)
      - [Solution](#5c/c/ii/solution)
- [6C](#6c)
  - [a](#6c/a)
    - [Solution](#6c/a/solution)
  - [b](#6c/b)
    - [Solution](#6c/b/solution)
- [7C](#7c)
  - [Solution](#7c/solution)
- [8C](#8c)
  - [a](#8c/a)
    - [Solution](#8c/a/solution)
  - [b](#8c/b)
    - [Solution](#8c/b/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [Solution](#9f/c/solution)
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
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)
  - [c](#12f/c)
    - [Solution](#12f/c/solution)

## 1C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1c/a">a</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/a/solution">Solution</h4>

↑ **Parent:** [A](#1c/a)

Subtract successive terms and use a [telescoping series](../../../real-analysis.md#telescoping-series):

$$
z_{n+1}-z_1=\sum_{j=1}^n(z_{j+1}-z_j)=\sum_{j=1}^nc_j.
$$

Thus the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) has solution

$$
\boxed{z_{n+1}=z_1+\sum_{j=1}^nc_j.}
$$

<h3 id="1c/b">b</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/b/solution">Solution</h4>

↑ **Parent:** [B](#1c/b)

Put $U_0=1$, so the same definition $z_n=x_n/U_{n-1}$ includes $n=1$. Since $U_n=a_nU_{n-1}$ and every $a_n$ is nonzero,

$$
z_{n+1}=\frac{a_nx_n+b_n}{U_n}=z_n+\frac{b_n}{U_n}.
$$

The factor $U_n^{-1}$ is a [discrete integrating factor](../../../algebra.md#discrete-integrating-factor) for this [variable-coefficient affine recurrence](../../../algebra.md#variable-coefficient-affine-recurrence). Sum the increments as a [telescoping series](../../../real-analysis.md#telescoping-series) and multiply back by $U_n$:

$$
\boxed{z_{n+1}-z_n=\frac{b_n}{U_n},\qquad
x_{n+1}=U_n\left(x_1+\sum_{j=1}^n\frac{b_j}{U_j}\right).}
$$

The identity requires no assumption that the coefficients have the same sign.

## 2C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

The first [partial derivatives](../../../calculus.md#partial-derivative) are

$$
f_x=\frac1y-\frac{y}{x^2}-\frac{2(x-y)}{a^2},\qquad
f_y=\frac1x-\frac{x}{y^2}+\frac{2(x-y)}{a^2}.
$$

Both vanish at $(\lambda,\lambda)$, so every positive diagonal point is a [stationary point](../../../calculus-of-variations.md#stationary-point). The [Hessian matrix](../../../calculus.md#hessian-matrix) there is

$$
\boxed{H=2\left(\frac1{\lambda^2}-\frac1{a^2}\right)
\begin{pmatrix}1&-1\\-1&1\end{pmatrix}.}
$$

Its [eigenvectors](../../../linear-operator-theory.md#eigenvector) $(1,1)$ and $(1,-1)$ have respective [eigenvalues](../../../linear-operator-theory.md#eigenvalue)

$$
\boxed{0,\qquad4\left(\frac1{\lambda^2}-\frac1{a^2}\right).}
$$

The zero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) reflects the entire line of [nonisolated stationary points](../../../analysis.md#nonisolated-stationary-point): $f(\lambda,\lambda)=2$. In fact $f-2=(x-y)^2[1/(xy)-1/a^2]$, showing a non-strict [local minimum](../../../analysis.md#local-minimum) when $\lambda<|a|$, a non-strict [local maximum](../../../analysis.md#local-maximum) when $\lambda>|a|$, and values on both sides of two near $\lambda=|a|$. At that last point the whole [Hessian matrix](../../../calculus.md#hessian-matrix) vanishes, so its signs alone cannot classify the point.

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

Because $X$ is a nonnegative integer, its [indicator function](../../../measure-theory.md#indicator-function) satisfies $\mathbf1_{\{X>0\}}\leq X$. Taking [expected values](../../../probability-theory.md#expected-value) proves the upper bound. The finite [second moment](../../../probability-theory.md#second-moment) also gives a finite [expected value](../../../probability-theory.md#expected-value), by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Applying that inequality to $X$ and $\mathbf1_{\{X>0\}}$ gives

$$
(\mathbb EX)^2
=\bigl(\mathbb E[X\mathbf1_{\{X>0\}}]\bigr)^2
\leq\mathbb E[X^2]\,\mathbb P(X>0).
$$

The assumed positive [second moment](../../../probability-theory.md#second-moment) permits division, yielding

$$
\boxed{\frac{(\mathbb EX)^2}{\mathbb E[X^2]}\leq\mathbb P(X>0)\leq\mathbb EX.}
$$

The lower bound is the basic [second moment method](../../../probability-inequality.md#second-moment-method); the upper bound also follows from [Markov's inequality](../../../probability-inequality.md#markov-inequality) at threshold one. Integer-valuedness is essential for that upper bound, but not for the lower bound. For example, a constant $X=1/2$ would violate the upper bound.

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/i">i</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/i/solution">Solution</h4>

↑ **Parent:** [I](#4f/i)

Integrate the [joint probability density](../../../continuous-probability-distribution.md#joint-probability-density) over $y$ to obtain the [marginal density](../../../probability-theory.md#marginal-density) of $X$:

$$
f_X(x)=\int_0^\infty xe^{-x(y+1)}\,dy=e^{-x},\qquad x>0.
$$

Thus $X$ has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate one. Dividing the [joint probability density](../../../continuous-probability-distribution.md#joint-probability-density) by this [marginal density](../../../probability-theory.md#marginal-density) gives the [conditional density](../../../probability-theory.md#conditional-density)

$$
\boxed{f_{Y\mid X=x}(y)=xe^{-xy}\mathbf1_{\{y\geq0\}},\qquad x>0.}
$$

Equivalently, $Y\mid X=x$ has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $x$. The value at $x=0$ can be assigned arbitrarily: it is a probability-zero conditioning value and the density ratio there is not meaningful.

<h3 id="4f/ii">ii</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4f/ii)

The [conditional density](../../../probability-theory.md#conditional-density) gives

$$
\mathbb E[Y\mid X=x]=\int_0^\infty yxe^{-xy}\,dy=\frac1x,
$$

using either [integration by parts](../../../calculus.md#integration-by-parts) or the [expected value](../../../probability-theory.md#expected-value) of an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution). Hence

$$
\boxed{\mathbb E[Y\mid X]=\frac1X\quad\text{almost surely}.}
$$

This is a finite value for almost every realization of $X$, but not an integrable [random variable](../../../random-variable.md): $\mathbb E[1/X]=\int_0^\infty e^{-x}/x\,dx=\infty$. Since $Y\geq0$, its [conditional expectation](../../../measure-theory.md#conditional-expectation) remains well-defined in the nonnegative, extended-expectation sense; the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) then gives $\mathbb EY=\infty$.

## 5C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5c/a">a</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/a/solution">Solution</h4>

↑ **Parent:** [A](#5c/a)

With no [electrical resistance](../../../electromagnetism.md#electrical-resistance) or applied [electric potential difference](../../../electromagnetism.md#electric-potential-difference), divide the equation by the [inductance](../../../electromagnetism.md#inductance) $L$ to get a [simple harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) with angular frequency $\omega_0=(LC)^{-1/2}$. Its general real solution is

$$
\boxed{I(t)=A\cos(\omega_0t)+B\sin(\omega_0t),\qquad
\omega_0=\frac1{\sqrt{LC}}.}
$$

Each nonzero solution has period $2\pi\sqrt{LC}$. Here $\omega_0$ is an [angular frequency](../../../classical-mechanics.md#angular-frequency); the ordinary frequency in cycles per unit time is $\omega_0/(2\pi)$.

<h3 id="5c/b">b</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/b/solution">Solution</h4>

↑ **Parent:** [B](#5c/b)

The PDF gives $V=H(t)$, the [Heaviside step function](../../../analysis.md#heaviside-step-function); the TeX incorrectly changes this to $V=I(t)$. A unit voltage step has derivative the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function), so the current is the causal [Green function](../../../analysis.md#green-s-function) for $L\,d^2/dt^2+R\,d/dt+1/C$.

The current must be continuous at zero: a jump would create a delta derivative through $LI''$, absent on the right-hand side. Integrating across zero therefore gives $L[I']+R[I]=1$, so $I(0^+)=0$ and $I'(0^+)=1/L$. Put

$$
r_\pm=\frac{-R\pm\sqrt{R^2-4L/C}}{2L}.
$$

These distinct negative [characteristic roots](../../../differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) give the [overdamped RLC response](../../../electromagnetism.md#overdamped-rlc-response)

$$
\boxed{I(t)=\frac{e^{r_+t}-e^{r_-t}}{L(r_+-r_-)}
=\frac{e^{r_+t}-e^{r_-t}}{\sqrt{R^2-4L/C}},\qquad t\geq0.}
$$

Together with $I(t)=0$ for $t<0$, this solves the step response. The eventual current is zero: the [capacitor](../../../electromagnetism.md#capacitor) charges and blocks steady current in the [series RLC circuit](../../../electromagnetism.md#series-rlc-circuit).

<h3 id="5c/c">c</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/c/i">i</h4>

↑ **Parent:** [C](#5c/c)

<h5 id="5c/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5c/c/i)

First construct the periodic response required in the introductory clause. At $\omega_0^2=1/(LC)$, the terms $LI_0''+I_0/C$ cancel for a sinusoid, leaving $RI_0'=\omega_0\cos(\omega_0t)$. Thus

$$
\boxed{I_0(t)=\frac1R\sin(\omega_0t),\qquad I_M=\frac1R.}
$$

This [resonant series RLC response](../../../electromagnetism.md#resonant-series-rlc-response) dissipates [energy](../../../classical-mechanics.md#energy) through [Joule heating](../../../electromagnetism.md#joule-heating). Over one period,

$$
\boxed{D=\frac1R\int_0^T\sin^2(\omega_0t)\,dt
=\frac{T}{2R}=\frac{\pi}{R\omega_0}.}
$$

The [Q factor](../../../dynamical-systems.md#q-factor), using the maximum magnetic [energy](../../../classical-mechanics.md#energy) $LI_M^2/2$, is consequently

$$
\boxed{Q=\frac{2\pi}{D}\frac{LI_M^2}{2}=\frac{L\omega_0}{R},\qquad
Q\omega_0RC=LC\omega_0^2=1.}
$$

<h4 id="5c/c/ii">ii</h4>

↑ **Parent:** [C](#5c/c)

<h5 id="5c/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5c/c/ii)

Every solution is the [resonant series RLC response](../../../electromagnetism.md#resonant-series-rlc-response) $I_0(t)=R^{-1}\sin(\omega_0t)$ plus a solution of the homogeneous [damped harmonic oscillator](../../../analysis.md#damped-harmonic-oscillator). Define $\gamma=R/(2L)$ and $\omega_0^2=1/(LC)$. The three possibilities are

$$
\boxed{I(t)=\frac{\sin(\omega_0t)}R+
\begin{cases}
e^{-\gamma t}\bigl(A\cos(\Omega t)+B\sin(\Omega t)\bigr),
&\gamma<\omega_0,\quad\Omega=\sqrt{\omega_0^2-\gamma^2},\\
e^{-\gamma t}(A+Bt),&\gamma=\omega_0,\\
Ae^{(-\gamma+\kappa)t}+Be^{(-\gamma-\kappa)t},
&\gamma>\omega_0,\quad\kappa=\sqrt{\gamma^2-\omega_0^2}.
\end{cases}}
$$

These are respectively the [underdamped RLC response](../../../electromagnetism.md#underdamped-rlc-response), [critically damped RLC response](../../../electromagnetism.md#critically-damped-rlc-response) and [overdamped RLC response](../../../electromagnetism.md#overdamped-rlc-response). Both exponents in the last case are negative because $0<\kappa<\gamma$. All three homogeneous contributions tend to zero as $t\to\infty$, so **every response approaches the unique periodic steady current $I_0(t)$.** No initial conditions were specified in this clause; they determine $A,B$.

## 6C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6c/a">a</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/a/solution">Solution</h4>

↑ **Parent:** [A](#6c/a)

Use the complete system in the PDF: the TeX omits $\dot y=y(4x-1)/8$. Both coordinate axes are invariant, and the [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are $(0,0)$, $(1,0)$ and $(1/4,3/4)$. The [Jacobian matrix](../../../calculus.md#jacobian-matrix) is

$$
J(x,y)=\begin{pmatrix}1-2x-y&-x\\y/2&(4x-1)/8\end{pmatrix}.
$$

At $(0,0)$ its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,-1/8$, and at $(1,0)$ they are $-1,3/8$: both points are [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium). At the coexistence point,

$$
J_* =\begin{pmatrix}-1/4&-1/4\\3/8&0\end{pmatrix},\qquad
\boxed{\lambda_\pm=\frac{-1\pm i\sqrt5}{8}.}
$$

Thus the interior point is a [stable spiral](../../../dynamical-systems.md#stable-spiral). The nontrivial [nullclines](../../../dynamical-systems.md#nullcline) are $x+y=1$ and $x=1/4$: $x$ increases below the first and decreases above it, while $y$ increases to the right of the second and decreases to the left. The rotation near coexistence is counterclockwise.

<a id="6c/a/image-trajectories-of-a-predator-prey-system"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2-predator-prey.png)

**[Figure 1](#6c/a/image-trajectories-of-a-predator-prey-system). Trajectories of a predator-prey system**.

A local [linearization](../../../algebra.md#linearization) by itself does not prove that every interior solution has the same limit. For this [logistic predator-prey model](../../../mathematical-biology.md#logistic-predator-prey-model), let $x_*=1/4,y_*=3/4$ and use the [Lyapunov function](../../../dynamical-systems.md#lyapunov-function)

$$
V=x-x_*-x_*\log(x/x_*)
+2\bigl[y-y_*-y_*\log(y/y_*)\bigr].
$$

The inequality $u-1-\log u\geq0$ makes $V$ nonnegative, with equality only at coexistence. Its sublevel sets are compact inside the positive quadrant, because $V$ diverges both at the axes and at infinity. Direct differentiation cancels the predator-prey cross terms and gives

$$
\dot V=-(x-x_*)^2\leq0.
$$

On $\{\dot V=0\}$ one has $x=x_*$, and remaining there requires $\dot x=-x_*(y-y_*)=0$. The largest invariant subset is therefore the coexistence point. The [LaSalle invariance principle](../../../dynamical-systems.md#lasalle-s-invariance-principle) proves

$$
\boxed{(x(t),y(t))\longrightarrow(1/4,3/4)
\quad\text{for every }x(0)>0,\ y(0)>0.}
$$

On $x=0$, $y$ decays as $e^{-t/8}$ toward the origin. On $y=0$, the [logistic differential equation](../../../differential-equation.md#logistic-differential-equation) takes every $x(0)>0$ to one. The origin itself stays fixed. These boundary trajectories are the exceptions to the interior convergence statement.

<h3 id="6c/b">b</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/b/solution">Solution</h4>

↑ **Parent:** [B](#6c/b)

For $r>0$, differentiate $r^2=x^2+y^2$ and use the angular derivative $(x\dot y-y\dot x)/r^2$. The [polar coordinates](../../../calculus.md#polar-coordinates) satisfy

$$
\boxed{\dot r=r(1-r^2),\qquad\dot\theta=-1.}
$$

Hence the rotation is clockwise. The origin is an [unstable equilibrium](../../../dynamical-systems.md#unstable-equilibrium), while $r=1$ is a [limit cycle](../../../dynamical-systems.md#limit-cycle) of period $2\pi$. Writing $u=r^2$ gives the [logistic differential equation](../../../differential-equation.md#logistic-differential-equation) $\dot u=2u(1-u)$. For $r(t_0)=r_0>0$,

$$
\boxed{r(t)^2=\frac1{1+(r_0^{-2}-1)e^{-2(t-t_0)}},\qquad
\theta(t)=\theta_0-(t-t_0).}
$$

All nonzero solutions tend to the [unit-circle attracting limit cycle](../../../dynamical-systems.md#unit-circle-attracting-limit-cycle) as $t\to\infty$, spiralling outward for $r_0<1$ and inward for $r_0>1$. For $0<r_0<1$ the solution exists for every real time and approaches the origin as $t\to-\infty$; for $r_0=1$ it remains periodic in both time directions. For $r_0>1$, the denominator first vanishes at

$$
\boxed{t_*=t_0+\frac12\log(1-r_0^{-2}),\qquad r(t)\to\infty\text{ as }t\downarrow t_*.}
$$

This [finite-time blow-up of an ordinary differential equation](../../../dynamical-systems.md#finite-time-blow-up-of-an-ordinary-differential-equation) occurs backward in time. Such exterior solutions have no $t\to-\infty$ behavior: their maximal time interval is $(t_*,\infty)$. The zero solution exists for all time and has no defined polar angle.

## 7C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

Assume the usual continuous-coefficient setting for a [second-order linear differential equation](../../../differential-equation.md#second-order-linear-differential-equation). The [Wronskian](../../../differential-equation.md#wronskian) $W=y_1y_2'-y_1'y_2$ has derivative

$$
W'=y_1y_2''-y_1''y_2=-p(x)W,
\qquad
W(x)=W(x_0)\exp\!\left[-\int_{x_0}^xp(s)\,ds\right],
$$

which proves the [Abel identity](../../../differential-equation.md#abel-s-identity). If $W(x_0)=0$, the two initial-value columns are [linearly dependent](../../../vector-space.md#linear-dependence), so some nonzero $(\alpha,\beta)$ gives $\alpha y_1(x_0)+\beta y_2(x_0)=0$ and $\alpha y_1'(x_0)+\beta y_2'(x_0)=0$. The [uniqueness theorem for ordinary differential equations](../../../analysis.md#uniqueness-theorem-for-ordinary-differential-equations) makes that linear combination identically zero. If $W(x_0)\ne0$, the initial-value matrix is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), giving

$$
\boxed{a=\frac{Ay_2'(x_0)-By_2(x_0)}{W(x_0)},\qquad
b=\frac{By_1(x_0)-Ay_1'(x_0)}{W(x_0)}.}
$$

This establishes the alternative and supplies any prescribed initial data.

For the [Airy ordinary differential equation](../../../differential-equation.md#airy-ordinary-differential-equation), substitute a [power series](../../../real-analysis.md#power-series) $y=\sum_{m\geq0}a_mx^m$. Coefficient comparison gives $a_2=0$ and

$$
a_{m+3}=\frac{a_m}{(m+3)(m+2)},\qquad m\geq0.
$$

Choose $(a_0,a_1)=(1,0)$ and $(0,1)$. The [Airy power-series fundamental pair](../../../differential-equation.md#airy-power-series-fundamental-pair) is

$$
\boxed{y_1(x)=\sum_{k=0}^\infty
\frac{x^{3k}}{\prod_{j=1}^k(3j)(3j-1)},\qquad
y_2(x)=\sum_{k=0}^\infty
\frac{x^{3k+1}}{\prod_{j=1}^k(3j)(3j+1)}.}
$$

Empty products mean one. Their first terms are $y_1=1+x^3/6+x^6/180+\cdots$ and $y_2=x+x^4/12+x^7/504+\cdots$. The [ratio test](../../../real-analysis.md#ratio-test) gives convergence for every finite $x$, so termwise differentiation verifies the equation. Their [Wronskian](../../../differential-equation.md#wronskian) is one at zero, and hence everywhere because $p=0$. Thus every solution is $Ay_1+By_2$.

## 8C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8c/a">a</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/a/solution">Solution</h4>

↑ **Parent:** [A](#8c/a)

For real initial data, [separation of variables](../../../partial-differential-equation.md#separation-of-variables) gives

$$
\boxed{z(t)=\frac{z_0}{1-z_0t}.}
$$

This includes $z_0=0$, whose solution is identically zero. Every other real $z_0$ has a pole at $t=1/z_0$, so only $z_0=0$ gives a finite solution on the whole real line. If complex-valued initial data are allowed, a nonreal $z_0$ has no real-time pole; the whole-real-line conclusion here uses the usual real-valued differential-equation convention.

Along a [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) $y=u+ax$, the [chain rule](../../../calculus.md#chain-rule) gives $d f(x,u+ax)/dx=f_x+af_y$. For the homogeneous [transport equation](../../../partial-differential-equation.md#transport-equation) this is zero, so $f(x,y)=F(y-ax)$. For the nonlinear equation, the same [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) reduces the problem to $d f/dx=f^2$, with initial value $g(u)$. Therefore

$$
\boxed{f(x,y)=\frac{g(y-ax)}{1-xg(y-ax)}.}
$$

For [differentiable](../../../analysis.md#differentiable-function) real $g$, this is the classical solution wherever its denominator is nonzero, on the characteristic intervals containing the initial line. If $g(u)\ne0$ for some $u$, that characteristic blows up at $x=1/g(u)$, $y=u+a/g(u)$. Thus **the only real-valued solution bounded on all of $\mathbb R^2$ has $g\equiv0$, giving $f\equiv0$.**

<h3 id="8c/b">b</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/b/solution">Solution</h4>

↑ **Parent:** [B](#8c/b)

Choose $X=x-2y$ and $T=x$, so $(\alpha,\beta,\gamma,\delta)=(1,-2,1,0)$. The [Jacobian determinant](../../../calculus.md#jacobian-determinant) of the coordinate change is two, so it is an [invertible linear map](../../../calculus.md#invertible-linear-map). By the [chain rule](../../../calculus.md#chain-rule), $\partial_x=\partial_X+\partial_T$ and $\partial_y=-2\partial_X$. Consequently

$$
\partial_x^2+\partial_x\partial_y
=(\partial_X+\partial_T)(\partial_T-\partial_X)
=\partial_T^2-\partial_X^2.
$$

This is the [wave equation](../../../wave-equation.md) with $c=1$. The [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula) is $F(X,T)=U(X+T)+V(X-T)$, with arbitrary twice [differentiable functions](../../../analysis.md#differentiable-function) $U,V$. Returning to the old coordinates and absorbing factors of two into the arbitrary functions gives

$$
\boxed{f(x,y)=G(x-y)+H(y).}
$$

Direct differentiation checks the cancellation. Equivalently, first integrating $\partial_x(f_x+f_y)=0$ produces the same two-function family.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

The [binomial theorem](../../../combinatorics.md#binomial-theorem) makes the sum of the proposed [probability mass function](../../../probability-theory.md#probability-mass-function) equal to $(p+1-p)^N=1$; every term is nonnegative. Realize the associated [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) as $K=B_1+\cdots+B_N$, where the $B_j$ are [independent](../../../random-variable.md#independent-random-variables) variables with the [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) of parameter $p$. Each has [expected value](../../../probability-theory.md#expected-value) $p$ and [variance](../../../variance.md) $p(1-p)$. [Linearity of expectation](../../../probability-theory.md#linearity-of-expectation) and [variance additivity for independent random variables](../../../variance.md#variance-additivity-for-independent-random-variables) yield

$$
\boxed{\mathbb EK=Np,\qquad\operatorname{Var}K=Np(1-p).}
$$

At $p=0$ or $p=1$ this is a constant [random variable](../../../random-variable.md); the same formulas apply, with the endpoint mass understood by continuity.

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

For fixed $k$ and sufficiently large $N$,

$$
p_k(N,\lambda/N)
=\frac{\lambda^k}{k!}\left[\prod_{j=0}^{k-1}\left(1-\frac jN\right)\right]
\left(1-\frac\lambda N\right)^N
\left(1-\frac\lambda N\right)^{-k}.
$$

The finite product and last factor tend to one, while $(1-\lambda/N)^N\to e^{-\lambda}$. Thus the [Poisson limit theorem](../../../convergence-of-random-variables.md#poisson-limit-theorem) gives

$$
\boxed{\lim_{N\to\infty}p_k(N,\lambda/N)=e^{-\lambda}\frac{\lambda^k}{k!}.}
$$

These numbers form a [probability mass function](../../../probability-theory.md#probability-mass-function) because they are nonnegative and their sum is $e^{-\lambda}\sum_{k\geq0}\lambda^k/k!=1$, by the [exponential series](../../../calculus.md#exponential-series). They define the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) of parameter $\lambda$. Only $N\geq\lambda$ is needed to make the binomial parameter valid, which is sufficient for the limit.

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

Let $\sigma_N=\sqrt{Np(1-p)}$ and use the [floor function](../../../calculus.md#floor-function) to choose

$$
\boxed{k_a(N)=\max\{0,\lfloor Np+a\sigma_N\rfloor+1\},\qquad
k_b(N)=\min\{N,\lfloor Np+b\sigma_N\rfloor\}.}
$$

Interpret an empty integer interval as an empty sum. These bounds give exactly the event $a<(K_N-Np)/\sigma_N\leq b$, where $K_N$ has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) of parameters $N,p$. Since $0<p<1$, the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) for a sum of [independent](../../../random-variable.md#independent-random-variables) [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) variables gives [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) of that standardized count to the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). Its [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) is continuous at both endpoints, so

$$
\boxed{\sum_{k=k_a(N)}^{k_b(N)}p_k(N,p)
\longrightarrow\Phi(b)-\Phi(a)
=\frac1{\sqrt{2\pi}}\int_a^be^{-u^2/2}\,du.}
$$

The TeX's additional malformed inequality involving $p/k_a(N)$ and $p/k_b(N)$ is absent from the PDF and is not a condition on the requested integers.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

Apply [Markov's inequality](../../../probability-inequality.md#markov-inequality) to the nonnegative [random variable](../../../random-variable.md) $e^{\lambda X}$, since $X>t$ implies $e^{\lambda X}>e^{\lambda t}$:

$$
\boxed{\mathbb P(X>t)\leq e^{-\lambda t}\mathbb E[e^{\lambda X}].}
$$

This [exponential Markov bound](../../../probability-inequality.md#exponential-markov-bound) remains true, though uninformative, when the [expected value](../../../probability-theory.md#expected-value) is infinite. For a [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), completion of the square gives its [moment-generating function](../../../probability-theory.md#moment-generating-function)

$$
\mathbb E[e^{\lambda X}]
=\frac1{\sqrt{2\pi}}\int_{\mathbb R}e^{\lambda x-x^2/2}\,dx
=e^{\lambda^2/2}.
$$

Minimize $\lambda^2/2-\lambda t$ over positive $\lambda$; the choice $\lambda=t$ gives the [Chernoff bound](../../../probability-inequality.md#chernoff-bound)

$$
\boxed{\mathbb P(X>t)\leq e^{-t^2/2}.}
$$

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

Use the rate convention for the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution). By [convolution of independent random variables](../../../probability-theory.md#convolution-of-independent-random-variables), the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of $S=X+Y$ is, for $s\geq0$,

$$
f_S(s)=\int_0^s\lambda e^{-\lambda x}\mu e^{-\mu(s-x)}\,dx
=\boxed{\frac{\lambda\mu}{\mu-\lambda}
\left(e^{-\lambda s}-e^{-\mu s}\right)}.
$$

It is zero for $s<0$. The expression is nonnegative whichever rate is larger, and defines a two-stage [hypoexponential distribution](../../../continuous-probability-distribution.md#hypoexponential-distribution). As a check, its limit as $\mu\to\lambda$ is $\lambda^2s e^{-\lambda s}$, the shape-two [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution).

For $M=\min\{X,Y\}$, [independence](../../../random-variable.md#independent-random-variables) gives the [survival function](../../../survival-analysis.md#survival-function) $\mathbb P(M>s)=e^{-\lambda s}e^{-\mu s}$ for $s\geq0$. Differentiating its complement gives

$$
\boxed{f_M(s)=(\lambda+\mu)e^{-(\lambda+\mu)s}\mathbf1_{\{s\geq0\}}.}
$$

Thus the minimum has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) whose rate is the sum of the rates.

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

Use the positive exponent in the PDF. The TeX introduces a minus sign in the numerator while retaining the positive-sign normalizing constant, which would not define the stated [probability distribution](../../../probability-theory.md#probability-distribution). The [Curie–Weiss model](../../../statistical-physics.md#curie-weiss-model) assigns equal weights to $s$ and $-s$, since $(\sum_js_j)^2$ is unchanged by simultaneous reversal. This [spin inversion symmetry](../../../statistical-physics.md#spin-inversion-symmetry) pairs every configuration with one having the opposite value of $S_i$, so

$$
\boxed{\mathbb ES_i=0,\qquad\mathbb P(S_i=1)=\mathbb P(S_i=-1)=\frac12.}
$$

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

Let $C_{12}=\mathbb E[S_1S_2]\geq0$, using the supplied correlation property of the [Curie–Weiss model](../../../statistical-physics.md#curie-weiss-model). Since $\mathbf1_{\{S_i=1\}}=(1+S_i)/2$ and each spin has zero [expected value](../../../probability-theory.md#expected-value),

$$
\mathbb P(S_1=1,S_2=1)
=\frac14\mathbb E[(1+S_1)(1+S_2)]=\frac{1+C_{12}}4.
$$

Divide by $\mathbb P(S_1=1)=1/2$ to obtain

$$
\boxed{\mathbb P(S_2=1\mid S_1=1)=\frac{1+C_{12}}2
\geq\frac12=\mathbb P(S_2=1).}
$$

The expression assumes $n\geq2$, as required for $S_2$ to exist. It makes the connection between the spin correlation and the requested [conditional probability](../../../probability-theory.md#conditional-probability) explicit.

<h3 id="11f/c">c</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/c/solution">Solution</h4>

↑ **Parent:** [C](#11f/c)

If exactly $k$ spins equal $+1$, then $M=(2k-n)/n$. Therefore its possible values are $E_n$, with $k=n(1+m)/2$ for $m\in E_n$. Choosing the $k$ positive spins gives the [binomial coefficient](../../../combinatorics.md#binomial-coefficient)

$$
\binom nk=\frac{n!}{[n(1+m)/2]!\,[n(1-m)/2]!}.
$$

Every such configuration has the same [Curie–Weiss model](../../../statistical-physics.md#curie-weiss-model) weight because $\sum_{i,j}s_is_j=(\sum_is_i)^2=n^2m^2$. The [probability mass function](../../../probability-theory.md#probability-mass-function) of this [spin magnetization](../../../statistical-physics.md#spin-magnetization) is consequently

$$
\boxed{\mathbb P(M=m)=\frac1{Z_{n,\beta}}
\binom{n}{n(1+m)/2}e^{\beta nm^2/2},\qquad m\in E_n,}
$$

and zero elsewhere. Grouping the original [partition function](../../../statistical-physics.md#canonical-partition-function) by the same count also gives

$$
Z_{n,\beta}=\sum_{k=0}^n\binom nk
\exp\!\left[\frac{\beta(2k-n)^2}{2n}\right],
$$

which verifies normalization without counting any configuration twice.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

Write $K=k+1$ and $h_j=\mathbb E_jD_j$. The [expected duration of symmetric gambler's ruin](../../../markov-process.md#expected-duration-of-symmetric-gambler-s-ruin) satisfies $h_0=h_K=0$ and, by conditioning on the first step,

$$
h_j=1+\frac12h_{j-1}+\frac12h_{j+1},\qquad1\leq j\leq K-1.
$$

These [expected values](../../../probability-theory.md#expected-value) are finite: from any interior state, $K$ consecutive right steps ensure absorption, an event of probability at least $2^{-K}$. Blocks of $K$ steps therefore bound the survival probability by a decreasing geometric sequence. The candidate $h_j=j(K-j)$ has the required boundary values and satisfies $h_{j+1}-2h_j+h_{j-1}=-2$. Hence

$$
\boxed{\mathbb E D_j=j(k+1-j).}
$$

For completeness, the difference of two solutions of this [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) has zero second difference and is affine in $j$; its two zero boundary values force it to vanish.

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

The vertices visited by a [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) form an integer interval: nearest-neighbour steps cannot skip a vertex. At the [stopping time](../../../martingale.md#stopping-time) $T_k$, write that interval as $[\ell,r]$, with $r-\ell+1=k$. The walk is at one of its endpoints, because the $k$th new vertex must extend the earlier interval. This also covers $k=1$, when both endpoints coincide.

The [Strong Markov property](../../../markov-process.md#strong-markov-property) restarts the walk from this endpoint. Visiting a new vertex is exactly exiting $[\ell,r]$, or reaching $\ell-1$ or $r+1$. Translate these absorbing boundaries to $0,k+1$. The starting point becomes either $1$ or $k$, so the [expected duration of symmetric gambler's ruin](../../../markov-process.md#expected-duration-of-symmetric-gambler-s-ruin) is $k$ in both cases. Taking [conditional expectations](../../../measure-theory.md#conditional-expectation) and then [expected values](../../../probability-theory.md#expected-value) gives the [expected time to expand a random-walk range](../../../probability-theory.md#expected-time-to-expand-a-random-walk-range):

$$
\boxed{\mathbb E[T_{k+1}-T_k]=k.}
$$

<h3 id="12f/c">c</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/c/solution">Solution</h4>

↑ **Parent:** [C](#12f/c)

Couple the walk on the [cycle graph](../../../graph-theory.md#cycle-graph) to a [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) $S_j$ on the integer line by taking $Y_j=S_j\bmod n$, using the same $\pm1$ increments. The visited integer interval has distinct residues until its length reaches $n$; an interval of exactly $n$ consecutive integers contains every residue once. Consequently the [cover time](../../../probability-and-statistics.md#cover-time) on the cycle is exactly $T_n$ in this coupling.

Since $T_1=0$, telescope the range-expansion times and use [linearity of expectation](../../../probability-theory.md#linearity-of-expectation), without assuming those times are independent:

$$
\boxed{\mathbb ET=\mathbb ET_n
=\sum_{k=1}^{n-1}\mathbb E[T_{k+1}-T_k]
=\sum_{k=1}^{n-1}k=\frac{n(n-1)}2.}
$$

This is the [expected cover time of a cycle](../../../probability-and-statistics.md#expected-cover-time-of-a-cycle). The restriction $n\geq3$ makes the two neighbours distinct, matching the supplied transition rule.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
