# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperia_2_2024.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperia_2_2024.pdf)

**Table of contents**

- [1A](#1a)
  - [a](#1a/a)
    - [Solution](#1a/a/solution)
  - [b](#1a/b)
    - [Solution](#1a/b/solution)
- [2A](#2a)
  - [i](#2a/i)
    - [Solution](#2a/i/solution)
  - [ii](#2a/ii)
    - [Solution](#2a/ii/solution)
  - [iii](#2a/iii)
    - [Solution](#2a/iii/solution)
- [3F](#3f)
  - [a](#3f/a)
    - [Solution](#3f/a/solution)
  - [b](#3f/b)
    - [i](#3f/b/i)
      - [Solution](#3f/b/i/solution)
    - [ii](#3f/b/ii)
      - [Solution](#3f/b/ii/solution)
- [4F](#4f)
  - [a](#4f/a)
    - [Solution](#4f/a/solution)
  - [b](#4f/b)
    - [Solution](#4f/b/solution)
  - [c](#4f/c)
    - [Solution](#4f/c/solution)
- [5A](#5a)
  - [i](#5a/i)
    - [Solution](#5a/i/solution)
  - [ii](#5a/ii)
    - [Solution](#5a/ii/solution)
  - [iii](#5a/iii)
    - [Solution](#5a/iii/solution)
  - [iv](#5a/iv)
    - [Solution](#5a/iv/solution)
- [6A](#6a)
  - [a](#6a/a)
    - [Solution](#6a/a/solution)
  - [b](#6a/b)
    - [Solution](#6a/b/solution)
- [7A](#7a)
  - [i](#7a/i)
    - [Solution](#7a/i/solution)
  - [ii](#7a/ii)
    - [Solution](#7a/ii/solution)
  - [iii](#7a/iii)
    - [Solution](#7a/iii/solution)
  - [iv](#7a/iv)
    - [Solution](#7a/iv/solution)
- [8A](#8a)
  - [i](#8a/i)
    - [Solution](#8a/i/solution)
  - [ii](#8a/ii)
    - [Solution](#8a/ii/solution)
  - [iii](#8a/iii)
    - [Solution](#8a/iii/solution)
  - [iv](#8a/iv)
    - [Solution](#8a/iv/solution)
- [9F](#9f)
  - [i](#9f/i)
    - [Solution](#9f/i/solution)
  - [ii](#9f/ii)
    - [Solution](#9f/ii/solution)
  - [iii](#9f/iii)
    - [Solution](#9f/iii/solution)
  - [iv](#9f/iv)
    - [Solution](#9f/iv/solution)
- [10F](#10f)
  - [i](#10f/i)
    - [Solution](#10f/i/solution)
  - [ii](#10f/ii)
    - [Solution](#10f/ii/solution)
  - [iii](#10f/iii)
    - [Solution](#10f/iii/solution)
  - [iv](#10f/iv)
    - [Solution](#10f/iv/solution)
  - [v](#10f/v)
    - [Solution](#10f/v/solution)
- [11F](#11f)
  - [i](#11f/i)
    - [Solution](#11f/i/solution)
  - [ii](#11f/ii)
    - [Solution](#11f/ii/solution)
  - [iii](#11f/iii)
    - [Solution](#11f/iii/solution)
  - [iv](#11f/iv)
    - [Solution](#11f/iv/solution)
- [12F](#12f)
  - [i](#12f/i)
    - [Solution](#12f/i/solution)
  - [ii](#12f/ii)
    - [Solution](#12f/ii/solution)
  - [iii](#12f/iii)
    - [Solution](#12f/iii/solution)
  - [iv](#12f/iv)
    - [Solution](#12f/iv/solution)
  - [v](#12f/v)
    - [Solution](#12f/v/solution)

## 1A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1a/a">a</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/a/solution">Solution</h4>

↑ **Parent:** [A](#1a/a)

The zero [function](../../../function.md) is a solution. On an interval where $y\ne0$, put

$$
z=\frac{y'}y.
$$

Then

$$
z'=\frac{yy''-(y')^2}{y^2}.
$$

The differential equation becomes

$$
xz'=z.
$$

Hence $z=Cx$, and integration gives

$$
\log|y|=\frac C2x^2+C_0.
$$

Thus all nonzero solutions are

$$
\boxed{y(x)=A\exp\left(\frac C2x^2\right)},
\qquad A\ne0,
$$

together with $\boxed{y\equiv0}$.

<h3 id="1a/b">b</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/b/solution">Solution</h4>

↑ **Parent:** [B](#1a/b)

Multiplying

$$
y'+P(x)y=Q(x)y^n
$$

by $y^{-n}$ and setting $z=y^{1-n}$ gives

$$
\frac1{1-n}z'+Pz=Q.
$$

Therefore the [Bernoulli differential equation](../../../differential-equation.md#bernoulli-differential-equation) becomes

$$
\boxed{z'+(1-n)Pz=(1-n)Q}.
$$

For the stated equation,

$$
\dot x+6t^2x=2te^{-t^3}x^{1/2}.
$$

Set $z=\sqrt x$. Then

$$
\dot z+3t^2z=te^{-t^3}.
$$

The integrating factor is $e^{t^3}$, so

$$
\frac d{dt}(e^{t^3}z)=t.
$$

Hence

$$
e^{t^3}\sqrt{x}=\frac{t^2}{2}+C.
$$

The condition $x(1)=4$ gives $C=2e-\tfrac12$. Consequently

$$
\boxed{x(t)=e^{-2t^3}
\left(\frac{t^2}{2}+2e-\frac12\right)^2}.
$$

## 2A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2a/i">i</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/i/solution">Solution</h4>

↑ **Parent:** [I](#2a/i)

Set $x=y=0$ in the functional equation:

$$
f(0)=\frac{2f(0)}{1-f(0)^2}.
$$

The denominator is defined. If $f(0)\ne0$, cancellation would give $f(0)^2=-1$, impossible for a real-valued [function](../../../function.md). Hence

$$
\boxed{f(0)=0}.
$$

<h3 id="2a/ii">ii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2a/ii)

Using the addition law with $y=h$,

$$
\frac{f(x+h)-f(x)}h
=\frac{f(h)}h
\frac{1+f(x)^2}{1-f(x)f(h)}.
$$

Differentiability makes $f$ continuous, so $f(h)\to f(0)=0$, and

$$
\frac{f(h)}h\to f'(0).
$$

Writing $C=f'(0)$ and taking the [limit](../../../calculus.md#limit-of-a-function) gives

$$
\boxed{f'(x)=C(1+f(x)^2)}.
$$

<h3 id="2a/iii">iii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2a/iii)

Since

$$
\frac{f'}{1+f^2}=C,
$$

integration gives

$$
\arctan f(x)=Cx+D.
$$

Part (i) gives $D=0$, so the [tangent addition functional equation](../../../differential-equation.md#tangent-addition-functional-equation) has the solutions

$$
\boxed{f(x)=\tan(Cx)},
$$

for constants $C$ such that no pole lies in $(-a,a)$. Conversely, the tangent addition formula verifies the functional equation. If $f'(0)=2$, then $C=2$, and

$$
\boxed{f(x)=\tan(2x)}
$$

on any such interval, necessarily with $a\leq\pi/4$.

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/a">a</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/a/solution">Solution</h4>

↑ **Parent:** [A](#3f/a)

The [Markov inequality](../../../probability-inequality.md#markov-inequality) states that for a nonnegative [random variable](../../../random-variable.md) $Y$ and $a>0$,

$$
\Pr(Y\geq a)\leq\frac{\mathbb EY}{a}.
$$

For $t>0$, the event $X\geq x$ is the same as $e^{tX}\geq e^{tx}$. Applying Markov's inequality to the nonnegative variable $e^{tX}$ gives the [exponential Markov bound](../../../probability-inequality.md#exponential-markov-bound)

$$
\boxed{\Pr(X\geq x)\leq e^{-tx}M_X(t)}.
$$

<h3 id="3f/b">b</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/b/i">i</h4>

↑ **Parent:** [B](#3f/b)

<h5 id="3f/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3f/b/i)

Independence gives

$$
M_S(t)=\prod_{j=1}^nM_{X_j}(t)
=\left[\exp(e^t-1)\right]^n
=\exp\{n(e^t-1)\}.
$$

This is the moment generating [function](../../../function.md) of a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $n$. Hence

$$
\boxed{S\sim\operatorname{Poisson}(n)}.
$$

<h4 id="3f/b/ii">ii</h4>

↑ **Parent:** [B](#3f/b)

<h5 id="3f/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3f/b/ii)

The exponential Markov bound gives, for every $t>0$,

$$
\Pr(S\geq2n)
\leq\exp\{-2nt+n(e^t-1)\}.
$$

The exponent is minimized when $e^t=2$, so take $t=\log2$. Then

$$
\Pr(S\geq2n)
\leq\exp\{n(1-2\log2)\}
=\boxed{\left(\frac e4\right)^n}.
$$

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/a">a</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/a/solution">Solution</h4>

↑ **Parent:** [A](#4f/a)

The [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) has density

$$
\boxed{
f(x_1,x_2)
=\frac1{2\pi\sigma_1\sigma_2\sqrt{1-\rho^2}}
\exp\left\{
-\frac1{2(1-\rho^2)}
\left[
\frac{(x_1-\mu_1)^2}{\sigma_1^2}
-\frac{2\rho(x_1-\mu_1)(x_2-\mu_2)}
{\sigma_1\sigma_2}
+\frac{(x_2-\mu_2)^2}{\sigma_2^2}
\right]\right\}.}
$$

<h3 id="4f/b">b</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/b/solution">Solution</h4>

↑ **Parent:** [B](#4f/b)

Completing the square in $x_1$ in the joint density shows that the [conditional distribution of a bivariate normal variable](../../../probability-and-statistics.md#conditional-distribution-of-a-bivariate-normal-variable) is

$$
\boxed{
X_1\mid X_2=x_2
\sim N\left(
\mu_1+\rho\frac{\sigma_1}{\sigma_2}(x_2-\mu_2),
\sigma_1^2(1-\rho^2)\right).}
$$

Thus its conditional density is

$$
\boxed{\frac1{\sqrt{2\pi\sigma_1^2(1-\rho^2)}}
\exp\left[
-\frac{\left(x_1-\mu_1-\rho\frac{\sigma_1}{\sigma_2}
(x_2-\mu_2)\right)^2}
{2\sigma_1^2(1-\rho^2)}
\right].}
$$

<h3 id="4f/c">c</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/c/solution">Solution</h4>

↑ **Parent:** [C](#4f/c)

Let

$$
U=X_1+X_2,\qquad V=X_1-X_2.
$$

They are jointly normal because they are linear combinations of a Gaussian [vector](../../../vector-space.md#vector). When $\sigma_1=\sigma_2=\sigma$,

$$
\operatorname{cov}(U,V)
=\operatorname{var}(X_1)-\operatorname{var}(X_2)=0.
$$

Hence [uncorrelated jointly normal variables are independent](../../../probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent). Their means and variances are

$$
\mathbb EU=\mu_1+\mu_2,
\qquad
\operatorname{var}U=2\sigma^2(1+\rho),
$$

and

$$
\mathbb EV=\mu_1-\mu_2,
\qquad
\operatorname{var}V=2\sigma^2(1-\rho).
$$

Therefore

$$
\boxed{U\sim N(\mu_1+\mu_2,2\sigma^2(1+\rho))},
$$



$$
\boxed{V\sim N(\mu_1-\mu_2,2\sigma^2(1-\rho))},
$$

independently.

## 5A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5a/i">i</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/i/solution">Solution</h4>

↑ **Parent:** [I](#5a/i)

After multiplying either solution by $-1$ if necessary, suppose both are positive on $(x_1,x_2)$. Set

$$
W=\varphi_1'\varphi_2-\varphi_1\varphi_2'.
$$

The equations give

$$
W'=(q_2-q_1)\varphi_1\varphi_2\geq0.
$$

Since $\varphi_1$ is positive between consecutive zeros,

$$
\varphi_1'(x_1)>0,\qquad \varphi_1'(x_2)<0.
$$

Therefore

$$
W(x_1)=\varphi_1'(x_1)\varphi_2(x_1)\geq0,
\qquad
W(x_2)=\varphi_1'(x_2)\varphi_2(x_2)\leq0.
$$

But $W$ is nondecreasing, so both endpoint values coincide at zero and $W'\equiv0$. Since both solutions are strictly positive inside,

$$
\boxed{q_1(x)=q_2(x)\quad(x_1<x<x_2)}.
$$

This is the equality case in the [wronskian proof of Sturm comparison](../../../differential-equation.md#wronskian-proof-of-sturm-comparison).

<h3 id="5a/ii">ii</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5a/ii)

Suppose $\varphi_2$ has no zero in $(x_1,x_2)$. It has a constant sign there, so replace it by its negative if needed and apply part (i). The conclusion is $q_1\equiv q_2$ on that interval. Taking the contrapositive proves the [Sturm comparison theorem](../../../differential-equation.md#sturm-comparison-theorem): unless the coefficients agree identically, $\varphi_2$ has a zero between the consecutive zeros of $\varphi_1$.

<h3 id="5a/iii">iii</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5a/iii)

Take

$$
q_1(x)=1,\qquad
\varphi_1(x)=\sin(x+1).
$$

Its consecutive zeros are $-1$ and $\pi-1$. For the stated equation,

$$
q_2(x)=2+\cos3x\geq1=q_1(x),
$$

and $q_2$ is not identically equal to $1$ on the interval. The [Sturm comparison theorem](../../../differential-equation.md#sturm-comparison-theorem) therefore shows that every nontrivial solution has at least one zero in

$$
\boxed{[-1,\pi-1]}.
$$

<h3 id="5a/iv">iv</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5a/iv)

Rewrite the equation as

$$
y''+q(x)y=0,
\qquad
q(x)=\frac1{\sqrt{1+x^3}}.
$$

On $[2,6]$, one has $q(x)\leq1/3$. If a nontrivial solution had two zeros, choose two consecutive ones $\alpha<\beta$ in that interval. Then $\beta-\alpha\leq4<\pi\sqrt3$.

The solution

$$
\varphi(x)=
\cos\left(\frac{x-(\alpha+\beta)/2}{\sqrt3}\right)
$$

of $\varphi''+\frac13\varphi=0$ is strictly positive on $[\alpha,\beta]$. Since $q\leq1/3$ and the coefficients are not identical on this interval, the [Sturm comparison theorem](../../../differential-equation.md#sturm-comparison-theorem) requires $\varphi$ to have a zero between $\alpha$ and $\beta$, a contradiction. Hence every nontrivial solution has

$$
\boxed{\text{at most one zero on }[2,6]}.
$$

## 6A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6a/a">a</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/a/solution">Solution</h4>

↑ **Parent:** [A](#6a/a)

The homogeneous characteristic equation is

$$
r^2+r-6=(r-2)(r+3)=0.
$$

A linear particular solution $u_n=an+b$ gives

$$
-4an+11a-4b=n,
$$

so $a=-1/4$ and $b=-11/16$. Thus

$$
u_n=A2^n+B(-3)^n-\frac n4-\frac{11}{16}.
$$

The initial data yield $A=1$ and $B=-5/16$, hence

$$
\boxed{u_n=2^n-\frac5{16}(-3)^n-\frac n4-\frac{11}{16}}.
$$

For the [ordinary generating function of a recurrence](../../../algebra.md#ordinary-generating-function-of-a-recurrence), multiply by $x^n$ and sum for $n\geq2$. Using $u_0=0,u_1=2$ gives

$$
(1+x-6x^2)G(x)
=x+\frac{x}{(1-x)^2}.
$$

Equivalently,

$$
\boxed{
G(x)=
\frac1{1-2x}
-\frac5{16(1+3x)}
-\frac{x}{4(1-x)^2}
-\frac{11}{16(1-x)}}.
$$

Expanding each geometric [series](../../../real-analysis.md#series-mathematics) gives exactly the displayed formula for $u_n$, verifying consistency.

<h3 id="6a/b">b</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/b/solution">Solution</h4>

↑ **Parent:** [B](#6a/b)

The [floor-half generating function](../../../algebra.md#floor-half-generating-function) is

$$
H(x)=\sum_{n\geq1}\left\lfloor\frac n2\right\rfloor x^n
=\frac{x^2}{(1-x)^2(1+x)}.
$$

Summing $u_n-2u_{n-1}=\lfloor n/2\rfloor$ for $n\geq1$ gives

$$
G(x)-1-2xG(x)=H(x),
$$

so

$$
\boxed{
G(x)=\frac{1+\dfrac{x^2}{(1-x)^2(1+x)}}{1-2x}}.
$$

Since

$$
\left\lfloor\frac n2\right\rfloor
=\frac n2-\frac14+\frac14(-1)^n,
$$

a particular solution is

$$
-\frac n2-\frac34+\frac1{12}(-1)^n.
$$

Adding the homogeneous term $C2^n$ and imposing $u_0=1$ gives $C=5/3$. Therefore

$$
\boxed{
u_n=\frac53\,2^n-\frac n2-\frac34+\frac1{12}(-1)^n}.
$$

## 7A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7a/i">i</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/i/solution">Solution</h4>

↑ **Parent:** [I](#7a/i)

Take

$$
F=x^2+y^2.
$$

Then

$$
\dot F=2x\dot x+2y\dot y
=2k(x^2+y^2)^2
=2kF^2.
$$

With $F(0)=1$, separation gives

$$
-\frac1F=2kt-1,
$$

and hence

$$
\boxed{F(t)=\frac1{1-2kt}}
$$

on its maximal interval of existence.

<h3 id="7a/ii">ii</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7a/ii)

The only equilibrium is $(0,0)$. Its linearization is

$$
\begin{pmatrix}\dot x\\\dot y\end{pmatrix}
=
\begin{pmatrix}0&1\\-1&0\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix},
$$

whose [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\pm i$, so the linearized system has a centre.

The exact radial identity from part (i) gives

$$
\dot r=kr^3.
$$

Thus the origin is asymptotically stable for $k<0$, neutrally stable for $k=0$, and unstable for $k>0$. Moreover,

$$
\dot\theta=\frac{x\dot y-y\dot x}{r^2}=-1,
$$

so trajectories rotate clockwise.

<h3 id="7a/iii">iii</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7a/iii)

The [radially symmetric planar dynamical system](../../../dynamical-systems.md#radially-symmetric-planar-dynamical-system) formulas give

$$
\boxed{f(r)=kr^3,\qquad g(\theta)=-1}.
$$

With $r(0)=1$ and $\theta(0)=0$,

$$
\boxed{r(t)=\frac1{\sqrt{1-2kt}}},
\qquad
\boxed{\theta(t)=-t},
$$

again on the maximal interval for which the denominator is positive.

<h3 id="7a/iv">iv</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#7a/iv)

For the modified system, $F=x^2+y^2$ satisfies

$$
\dot F=2F-4F^2=2F(1-2F).
$$

With $F(0)=1$, the logistic solution is

$$
\boxed{x(t)^2+y(t)^2
=\frac1{2-e^{-2t}}}.
$$

Consequently,

$$
\boxed{\lim_{t\to\infty}(x(t)^2+y(t)^2)=\frac12}.
$$

## 8A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8a/i">i</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/i/solution">Solution</h4>

↑ **Parent:** [I](#8a/i)

Write $\psi=a e^{iS}$ with $a=\sqrt\rho$ and $v=S_x$. Then

$$
\psi_{xx}=e^{iS}
\left(a_{xx}-av^2+i(2a_xv+av_x)\right),
$$

while

$$
-2i\psi_t=e^{iS}(2aS_t-2ia_t).
$$

Equating imaginary parts gives

$$
\rho_t=-(\rho v)_x,
$$

and equating real parts and differentiating in $x$ gives

$$
v_t=
\partial_x\left[
\frac{(\sqrt\rho)_{xx}}{2\sqrt\rho}
+\frac{1-\rho}{2}\right]
+\partial_x\left(-\frac{v^2}{2}\right).
$$

Thus

$$
\boxed{A=-\rho v},
\qquad
\boxed{B=\frac{(\sqrt\rho)_{xx}}{2\sqrt\rho}
+\frac{1-\rho}{2}},
\qquad
\boxed{C=-\frac{v^2}{2}}.
$$

This is the hydrodynamic form of the [defocusing nonlinear Schrödinger equation](../../../integrable-systems.md#defocusing-nonlinear-schrodinger-equation).

<h3 id="8a/ii">ii</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8a/ii)

For a stationary gas with constant phase, $\psi=a(x)$ is real and time independent. The field equation reduces to

$$
\boxed{a''+(1-a^2)a=0}.
$$

A positive constant solution obeys $d(1-d^2)=0$, so

$$
\boxed{d=1}.
$$

<h3 id="8a/iii">iii</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8a/iii)

The travelling-wave substitution $\xi=x-Ut$ gives

$$
\boxed{\psi_0''-2iU\psi_0'
+(1-|\psi_0|^2)\psi_0=0}.
$$

Write

$$
\psi_0(\xi)=u(\xi)+i\sqrt2U.
$$

Its real part satisfies

$$
\boxed{u''+(1-2U^2-u^2)u=0}.
$$

For $U>0$, the imaginary part also gives

$$
\sqrt2\,u'=1-2U^2-u^2.
$$

With $\alpha=\sqrt{1-2U^2}$ and a translation chosen so that the notch is centred at zero,

$$
\boxed{
\psi_0(\xi)=
\alpha\tanh\left(\frac{\alpha\xi}{\sqrt2}\right)
+i\sqrt2U}.
$$

Its limiting [modulus](../../../complex-analysis.md#modulus) is $\sqrt{\alpha^2+2U^2}=1=d$, as required. The same expression at $U=0$ is obtained directly from the second-order equation.

<h3 id="8a/iv">iv</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#8a/iv)

The [dark soliton](../../../integrable-systems.md#dark-soliton) density is

$$
|\psi_0(\xi)|^2
=1-(1-2U^2)
\operatorname{sech}^2\left(
\frac{\sqrt{1-2U^2}}{\sqrt2}\xi\right).
$$

For $U=0$,

$$
\boxed{|\psi_0(\xi)|^2=\tanh^2(\xi/\sqrt2)},
$$

a stationary notch reaching zero at its centre. For $U=1/2$,

$$
\boxed{|\psi_0(\xi)|^2
=1-\frac12\operatorname{sech}^2(\xi/2)},
$$

a shallower notch with minimum $1/2$. Since $\xi=x-Ut$, the first profile remains fixed and the second translates rigidly to the right at speed $1/2$.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/i">i</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/i/solution">Solution</h4>

↑ **Parent:** [I](#9f/i)

Put $Q=\sum_{j=1}^nq_j$. Since the variables have continuous distributions, the minimum is unique almost surely. Integrating over its possible value gives

$$
\begin{aligned}
\mathbb P(K=k,T\geq t)
&=\int_t^\infty q_ke^{-q_ks}
   \prod_{j\ne k}\mathbb P(S_j>s)\,ds\\
&=\int_t^\infty q_ke^{-Qs}\,ds
=\boxed{\frac{q_k}{Q}e^{-Qt}}.
\end{aligned}
$$

This is the joint tail calculation for [competing exponential clocks](../../../continuous-probability-distribution.md#competing-exponential-clocks).

<h3 id="9f/ii">ii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9f/ii)

Setting $t=0$ in part (i) gives

$$
\boxed{\mathbb P(K=k)=\frac{q_k}{Q}}.
$$

Also

$$
\mathbb P(T\geq t)
=\prod_{j=1}^ne^{-q_jt}
=e^{-Qt},
$$

so

$$
\boxed{T\sim\operatorname{Exp}(Q)}.
$$

Part (i) now factors as

$$
\mathbb P(K=k,T\geq t)
=\mathbb P(K=k)\mathbb P(T\geq t),
$$

which proves that $K$ and $T$ are independent.

<h3 id="9f/iii">iii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#9f/iii)

This is the unit-rate [Erlang distribution](../../../continuous-probability-distribution.md#erlang-distribution). For completeness, use convolution. The result is clear for $n=1$. If

$$
f_n(x)=\frac{x^{n-1}}{(n-1)!}e^{-x}\mathbf1_{\{x>0\}},
$$

then independence and the unit exponential density give, for $x>0$,

$$
\begin{aligned}
f_{n+1}(x)
&=\int_0^xf_n(y)e^{-(x-y)}\,dy\\
&=\frac{e^{-x}}{(n-1)!}\int_0^xy^{n-1}\,dy
=\frac{x^n}{n!}e^{-x}.
\end{aligned}
$$

Induction therefore proves

$$
\boxed{f_{X_n}(x)=\frac{x^{n-1}}{(n-1)!}e^{-x}},
\qquad x>0.
$$

<h3 id="9f/iv">iv</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#9f/iv)

Conditioning on $N$ and using the [moment-generating function](../../../probability-theory.md#moment-generating-function) of a unit exponential variable,

$$
\begin{aligned}
\mathbb E(e^{\theta Y})
&=\sum_{n=1}^\infty p(1-p)^{n-1}
  \left(\frac1{1-\theta}\right)^n\\
&=\frac{p}{1-\theta}
  \sum_{m=0}^\infty
  \left(\frac{1-p}{1-\theta}\right)^m
=\boxed{\frac{p}{p-\theta}},
\end{aligned}
$$

where the geometric [series](../../../real-analysis.md#series-mathematics) converges precisely when $\theta<p$. This is the moment-generating [function](../../../function.md) of an exponential variable of rate $p$, so the [geometric sum of exponential variables](../../../continuous-probability-distribution.md#geometric-sum-of-exponential-variables) satisfies

$$
\boxed{Y\sim\operatorname{Exp}(p)}.
$$

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/i">i</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/i/solution">Solution</h4>

↑ **Parent:** [I](#10f/i)

The $n$ possible matching events are independent, each with probability $1/n$. Hence

$$
\boxed{p_n=1-\left(1-\frac1n\right)^n},
$$

and therefore

$$
\boxed{\lim_{n\to\infty}p_n=1-e^{-1}}.
$$

<h3 id="10f/ii">ii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10f/ii)

When exactly $n-j$ faces have appeared, there are $j$ unseen faces, so each new roll discovers one with probability $j/n$. Let $G_j$ be the number of further rolls needed at that stage. Then

$$
G_j\sim\operatorname{Geom}\left(\frac jn\right),
\qquad j=n,n-1,\ldots,1.
$$

These waiting times concern disjoint successive blocks of independent rolls, so they are independent. Thus the [coupon collector problem](../../../discrete-probability-distribution.md#coupon-collector-problem) has the decomposition

$$
\boxed{T_n=\sum_{j=1}^nG_j}.
$$

<h3 id="10f/iii">iii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10f/iii)

Using the mean $1/p$ of a [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) and the decomposition in part (ii),

$$
\boxed{\mathbb E(T_n)
=\sum_{j=1}^n\frac{n}{j}
=n\sum_{j=1}^n\frac1j
=nH_n}.
$$

<h3 id="10f/iv">iv</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#10f/iv)

Independence and the geometric variance formula yield

$$
\begin{aligned}
\operatorname{var}(T_n)
&=\sum_{j=1}^n
\frac{1-j/n}{(j/n)^2}\\
&=\boxed{\sum_{j=1}^n\frac{n(n-j)}{j^2}}.
\end{aligned}
$$

Since $n(n-j)\leq n^2$,

$$
\operatorname{var}(T_n)
\leq n^2\sum_{j=1}^n\frac1{j^2}
\leq\boxed{Cn^2}.
$$

<h3 id="10f/v">v</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/v/solution">Solution</h4>

↑ **Parent:** [V](#10f/v)

Part (iii) and the given harmonic-sum asymptotic show that

$$
\frac{\mathbb ET_n}{n\log n}
=\frac{H_n}{\log n}\longrightarrow1.
$$

For any fixed $\varepsilon>0$, this deterministic ratio lies within $\varepsilon/2$ of $1$ for all sufficiently large $n$. The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) and part (iv) then give

$$
\begin{aligned}
\mathbb P\left(
\left|\frac{T_n}{n\log n}-1\right|>\varepsilon
\right)
&\leq
\mathbb P\left(
|T_n-\mathbb ET_n|>\frac{\varepsilon}{2}n\log n
\right)\\
&\leq
\frac{4\operatorname{var}(T_n)}
{\varepsilon^2n^2(\log n)^2}\\
&\leq\frac{4C}{\varepsilon^2(\log n)^2}
\longrightarrow0.
\end{aligned}
$$

Thus

$$
\boxed{\frac{T_n}{n\log n}\longrightarrow1
\quad\hbox{in probability}.}
$$

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/i">i</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/i/solution">Solution</h4>

↑ **Parent:** [I](#11f/i)

Let $B_n$ count the $+1$ steps. Then

$$
B_n\sim\operatorname{Binomial}(n,p),
\qquad S_n=B_n-(n-B_n)=2B_n-n.
$$

Consequently

$$
\boxed{
\mathbb P(S_n=2k-n)
=\binom nkp^kq^{\,n-k},
\quad k=0,\ldots,n,
}
$$

and $S_n$ has probability zero at integers of the other parity. This is the finite-time law of a [simple random walk on the integer line](../../../markov-process.md#simple-random-walk-on-the-integer-line).

<h3 id="11f/ii">ii</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11f/ii)

The preceding representation and the [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) give

$$
\frac{B_n-np}{\sqrt{npq}}
\ \xrightarrow{\ d\ }\ N(0,1).
$$

Since

$$
S_n-n(p-q)=2(B_n-np),
$$

one may take

$$
\boxed{b_n=n(p-q),\qquad c_n=2\sqrt{npq}}.
$$

For $0<p<1$ this gives the required convergence to $\Phi(x)$ at every real $x$.

<h3 id="11f/iii">iii</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11f/iii)

Let $m_j$ be the expected remaining time when the walk is at $j$. The first-step recurrence for [gambler's ruin](../../../markov-process.md#gambler-s-ruin) is

$$
m_j=1+\frac12m_{j-1}+\frac12m_{j+1},
\qquad -a<j<b,
$$

with $m_{-a}=m_b=0$. The quadratic

$$
m_j=(j+a)(b-j)
$$

satisfies both the recurrence and the [boundary conditions](../../../differential-equation.md#boundary-condition), and their finite linear system has a unique solution. Starting from zero therefore gives

$$
\boxed{\mathbb E(T)=m_0=ab}.
$$

<h3 id="11f/iv">iv</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#11f/iv)

Only even times contribute, and at time $2k$ the walk is at zero exactly when it has made $k$ steps in each direction. By [linearity of expectation](../../../probability-theory.md#linearity-of-expectation),

$$
\mathbb E(V_{2n})
=\sum_{j=0}^{2n}\mathbb P(S_j=0)
=\sum_{k=0}^n\frac{\binom{2k}{k}}{4^k}.
$$

The [Stirling formula](../../../real-analysis.md#stirling-formula) implies that

$$
\frac{\binom{2k}{k}}{4^k}\sim\frac1{\sqrt{\pi k}}.
$$

Hence there is a constant $c_0>0$ such that this term is at least $c_0/\sqrt{k}$ for every $k\geq1$, after decreasing $c_0$ to cover the finitely many small values. Therefore

$$
\mathbb E(V_{2n})
\geq c_0\sum_{k=1}^n\frac1{\sqrt{k}}
\geq c_0\int_1^{n+1}x^{-1/2}\,dx.
$$

The final expression is $2c_0(\sqrt{n+1}-1)$, so, after another adjustment for small $n$, there is a constant $c>0$ with

$$
\boxed{\mathbb E(V_{2n})\geq c\sqrt n}
$$

for every $n$. This is the lower bound recorded by [expected visits to the origin by a simple random walk](../../../markov-process.md#expected-visits-to-the-origin-by-a-simple-random-walk).

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/i">i</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/i/solution">Solution</h4>

↑ **Parent:** [I](#12f/i)

The degree of $v_i$ counts the $n-1$ incident edges, each present independently with probability $p$. Thus in the [Erdős-Rényi model](../../../graph-theory.md#erdos-renyi-model),

$$
\boxed{\deg(v_i)\sim\operatorname{Binomial}(n-1,p)}.
$$

<h3 id="12f/ii">ii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12f/ii)

Let $I_i$ indicate that $v_i$ is isolated. All its $n-1$ incident edges must be absent, so

$$
\mathbb E I_i=\mathbb P(I_i=1)=(1-p)^{n-1}.
$$

Since $N=\sum_{i=1}^nI_i$, [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) gives

$$
\boxed{\mathbb E(N)=n(1-p)^{n-1}}.
$$

<h3 id="12f/iii">iii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12f/iii)

With $p=c\log n/n$, the inequality $1-p\leq e^{-p}$ gives

$$
\mathbb E(N)
=n(1-p)^{n-1}
\leq ne^{-p(n-1)}
=n^{\,1-c(n-1)/n}
\longrightarrow0
$$

when $c>1$. The [Markov inequality](../../../probability-inequality.md#markov-inequality) now gives

$$
\mathbb P(N>0)\leq\mathbb E(N)\longrightarrow0.
$$

Consequently the upper side of the [isolated-vertex threshold in the Erdős-Rényi model](../../../graph-theory.md#isolated-vertex-threshold-in-the-erdos-renyi-model) is

$$
\boxed{\mathbb P(N=0)\longrightarrow1}.
$$

<h3 id="12f/iv">iv</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#12f/iv)

If $N=0$, then $|N-\mathbb EN|=\mathbb EN$. Hence the [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) gives

$$
\mathbb P(N=0)
\leq
\mathbb P\bigl(|N-\mathbb EN|\geq\mathbb EN\bigr)
\leq
\frac{\operatorname{var}(N)}{(\mathbb EN)^2}.
$$

The assumed [limit](../../../calculus.md#limit-of-a-function) therefore proves

$$
\boxed{\mathbb P(N=0)\longrightarrow0}.
$$

This is the [second moment method](../../../probability-inequality.md#second-moment-method) in its simplest form.

<h3 id="12f/v">v</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/v/solution">Solution</h4>

↑ **Parent:** [V](#12f/v)

Write $N=\sum_iI_i$ as in part (ii). For $i\ne j$, the two vertices are both isolated exactly when their combined $2n-3$ incident edges are absent, so

$$
\mathbb E(I_iI_j)=(1-p)^{2n-3}.
$$

Therefore

$$
\boxed{
\mathbb E(N^2)
=n(1-p)^{n-1}
+n(n-1)(1-p)^{2n-3}.
}
$$

Let $A=\mathbb EN=n(1-p)^{n-1}$. The displayed formula gives

$$
\frac{\operatorname{var}(N)}{A^2}
=\frac1A+\frac{n-1}{n(1-p)}-1
=\frac1A+\frac{p-1/n}{1-p}.
$$

Now take $p=c\log n/n$ with $c<1$, and choose $\alpha>1$ such that $\alpha c<1$. For all sufficiently large $n$, the supplied inequality gives $1-p\geq e^{-\alpha p}$, whence

$$
A\geq ne^{-\alpha p(n-1)}
=n^{\,1-\alpha c(n-1)/n}
\longrightarrow\infty.
$$

Also $p\to0$, so both terms in the variance ratio tend to zero. Part (iv) now applies and proves the lower side of the isolated-vertex threshold:

$$
\boxed{\mathbb P(N=0)\longrightarrow0}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
