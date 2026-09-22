# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperia_2_2023.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperia_2_2023.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
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
  - [a](#4f/a)
    - [Solution](#4f/a/solution)
  - [b](#4f/b)
    - [Solution](#4f/b/solution)
- [5A](#5a)
  - [a](#5a/a)
    - [Solution](#5a/a/solution)
  - [b](#5a/b)
    - [Solution](#5a/b/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7A](#7a)
  - [a](#7a/a)
    - [i](#7a/a/i)
      - [Solution](#7a/a/i/solution)
    - [ii](#7a/a/ii)
      - [Solution](#7a/a/ii/solution)
    - [iii](#7a/a/iii)
      - [Solution](#7a/a/iii/solution)
  - [b](#7a/b)
    - [Solution](#7a/b/solution)
- [8A](#8a)
  - [a](#8a/a)
    - [Solution](#8a/a/solution)
  - [b](#8a/b)
    - [i](#8a/b/i)
      - [Solution](#8a/b/i/solution)
    - [ii](#8a/b/ii)
      - [Solution](#8a/b/ii/solution)
    - [iii](#8a/b/iii)
      - [Solution](#8a/b/iii/solution)
    - [iv](#8a/b/iv)
      - [Solution](#8a/b/iv/solution)
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
  - [c](#10f/c)
    - [Solution](#10f/c/solution)
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

The characteristic [polynomial](../../../polynomial.md) of the homogeneous equation is

$$
r(r-2)^2,
$$

so $y_h=C_0+(C_1+C_2x)e^{2x}$. For a particular [integral](../../../calculus.md#integral) put $y=e^{2x}v$. Then

$$
y^{(3)}-4y''+4y'=e^{2x}(v^{(3)}+2v'')=xe^{2x}.
$$

Taking $v''=x/2-1/4$ gives $v=x^3/12-x^2/8$ after discarding homogeneous terms. Therefore

$$
\boxed{y=C_0+(C_1+C_2x)e^{2x}
+e^{2x}\left(\frac{x^3}{12}-\frac{x^2}{8}\right).}
$$

## 2A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2a/a">a</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/a/solution">Solution</h4>

↑ **Parent:** [A](#2a/a)

Since $1+\cos2y=2\cos^2y$, separation gives

$$
\sec^2y\,dy=\frac{2}{x^2}\,dx,
\qquad
\tan y=C-\frac2x.
$$

The limiting condition gives $C=1$. Taking $\tan^{-1}$ with range $(-\pi/2,\pi/2)$ and selecting the branch approaching $9\pi/4$ yields

$$
y(x)=2\pi+\tan^{-1}\left(1-\frac2x\right)
$$

for $x>0$.

<h3 id="2a/b">b</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/b/solution">Solution</h4>

↑ **Parent:** [B](#2a/b)

Write $u=xv$ on an interval not containing zero. The equation becomes $x^2v'=x$, so $v'=1/x$. Hence

$$
\boxed{u(x)=x\{\log|x|+C\}.}
$$

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/a">a</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/a/solution">Solution</h4>

↑ **Parent:** [A](#3f/a)

For a nonnegative [random variable](../../../random-variable.md) $Y$ and $a>0$, the [Markov inequality](../../../probability-inequality.md#markov-inequality) is

$$
\mathbb P(Y\geq a)\leq\frac{\mathbb EY}{a}.
$$

Indeed, $Y\geq a\mathbf1_{\{Y\geq a\}}$ pointwise. Taking expectations and dividing by $a$ proves the claim.

<h3 id="3f/b">b</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/b/solution">Solution</h4>

↑ **Parent:** [B](#3f/b)

Completing the square gives

$$
\boxed{M_X(t)=\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}
 e^{tx-x^2/2}dx
=e^{t^2/2}\frac1{\sqrt{2\pi}}
\int_{-\infty}^{\infty}e^{-(x-t)^2/2}dx
=e^{t^2/2}.}
$$

<h3 id="3f/c">c</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/c/solution">Solution</h4>

↑ **Parent:** [C](#3f/c)

For any $t>0$, the [exponential Markov bound](../../../probability-inequality.md#exponential-markov-bound) and part (b) give

$$
\mathbb P(X\geq v)
\leq e^{-tv}M_X(t)=e^{-tv+t^2/2}.
$$

The minimum occurs at $t=v$, so the [Gaussian tail bound](../../../probability-and-statistics.md#gaussian-tail-bound) is

$$
\boxed{\int_v^\infty\frac{e^{-x^2/2}}{\sqrt{2\pi}}dx
\leq e^{-v^2/2}.}
$$

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/a">a</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/a/solution">Solution</h4>

↑ **Parent:** [A](#4f/a)

The first $k$ digits must be distinct and may be chosen in

$$
(10)_k=10\cdot9\cdots(10-k+1)
$$

ways; the remaining digits are then forced in reverse order. Thus, for $k\leq10$,

$$
\mathbb P(E)=\frac{(10)_k}{10^{2k}},
$$

and the probability is zero for $k>10$.

<h3 id="4f/b">b</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/b/solution">Solution</h4>

↑ **Parent:** [B](#4f/b)

Let $E_\ell$ be the event that the block beginning at position $\ell$, $1\leq\ell\leq k+1$, is a spalindrome. Each has probability $(10)_k/10^{2k}$. If two starting positions differ by $d<k$, the first half of the later block contains the middle digit of the earlier palindrome twice, contradicting distinctness. Thus the only possible overlap is $E_1\cap E_{k+1}$.

That intersection consists of words $A\,A^{\rm rev}A$, where $A$ has $k$ distinct digits, and hence has probability $(10)_k/10^{3k}$. This [overlap structure of digit spalindromes](../../../combinatorics.md#overlap-structure-of-digit-spalindromes) makes inclusion--exclusion give

$$
\boxed{\mathbb P\left(\bigcup_{\ell=1}^{k+1}E_\ell\right)
=(k+1)\frac{(10)_k}{10^{2k}}
-\frac{(10)_k}{10^{3k}}.}
$$

## 5A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5a/a">a</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/a/solution">Solution</h4>

↑ **Parent:** [A](#5a/a)

Let

$$
I(x)=\exp\left(\int^xp(s)\,ds\right).
$$

The [integrating factor](../../../differential-equation.md#integrating-factor) identity $(Iy)'=If$ gives

$$
y(x)=I(x)^{-1}\left(C+\int^xI(t)f(t)\,dt\right).
$$

If $y_1,y_2$ are distinct solutions, their difference is a nonzero homogeneous solution, so every solution is

$$
\boxed{y=y_1+C(y_2-y_1).}
$$

<h3 id="5a/b">b</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/b/solution">Solution</h4>

↑ **Parent:** [B](#5a/b)

For $x>0$, division by $x$ gives

$$
y'-(2x+x^{-1})y=x.
$$

An integrating factor is $e^{-x^2}/x$, so

$$
y=xe^{x^2}\left(C+\int_0^xe^{-t^2}dt\right).
$$

Every choice except

$$
C=-\int_0^\infty e^{-t^2}dt=-\frac{\sqrt\pi}{2}
$$

grows like $xe^{x^2}$. The [bounded solution selected by a terminal condition](../../../differential-equation.md#bounded-solution-selected-by-a-terminal-condition) is therefore

$$
y_b(x)=-xe^{x^2}\int_x^\infty e^{-t^2}dt.
$$

Integration by parts, or the Gaussian-tail asymptotic, gives

$$
\int_x^\infty e^{-t^2}dt\sim\frac{e^{-x^2}}{2x},
\qquad y_b(x)\to-\frac12.
$$

It starts from $0$ at $x=0$, remains negative, and decreases monotonically toward the horizontal asymptote $-1/2$.

## 6A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

The [parameter sensitivity equation](../../../differential-equation.md#parameter-sensitivity-equation) follows by differentiating with respect to $\mu$ and writing $u=y_\mu$:

$$
u_x=u+x+y^2+2\mu yu,
\qquad u(0,\mu)=0.
$$

At $\mu=0$, $y_x=y$, $y(0)=1$, so $y(x,0)=e^x$. Then

$$
u_x-u=x+e^{2x},\qquad u(0,0)=0,
$$

and the integrating factor $e^{-x}$ yields

$$
u(x,0)=e^{2x}-x-1.
$$

Equating powers in $y=y_0+\mu y_1+\mu^2y_2+\cdots$ gives

$$
y_0=e^x,\qquad y_1=e^{2x}-x-1,
$$



$$
y_2'-y_2=2y_0y_1,\qquad y_2(0)=0.
$$

Consequently

$$
\boxed{y_2=e^x(e^{2x}-1-x^2-2x).}
$$

## 7A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7a/a">a</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/a/i">i</h4>

↑ **Parent:** [A](#7a/a)

<h5 id="7a/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7a/a/i)

For every test [function](../../../function.md) $\varphi$ and nonzero $p$, substitution $u=pt$ with the orientation handled by $|p|$ gives

$$
\int\varphi(t)\delta(pt)dt=\frac1{|p|}\varphi(0).
$$

**Hence the [Dirac delta scaling](../../../distribution-theory.md#dirac-delta-scaling) identity is $\delta(pt)=\delta(t)/|p|$.**

<h4 id="7a/a/ii">ii</h4>

↑ **Parent:** [A](#7a/a)

<h5 id="7a/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7a/a/ii)

The [derivative](../../../calculus.md#derivative) of a distribution is defined by integration by parts. Therefore

$$
\boxed{\int_{-\infty}^{\infty}f(t)\delta'(t)dt
=-\int_{-\infty}^{\infty}f'(t)\delta(t)dt
=-f'(0).}
$$

<h4 id="7a/a/iii">iii</h4>

↑ **Parent:** [A](#7a/a)

<h5 id="7a/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7a/a/iii)

For a compactly supported test [function](../../../function.md) $f$,

$$
\langle H',f\rangle=-\langle H,f'\rangle
=-\int_0^\infty f'(t)dt=f(0)
=\langle\delta,f\rangle.
$$

**Thus this is the [distributional derivative of the Heaviside step function](../../../distribution-theory.md#distributional-derivative-of-the-heaviside-step-function): $H'=\delta$.**

<h3 id="7a/b">b</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/b/solution">Solution</h4>

↑ **Parent:** [B](#7a/b)

For $t<0$ both inputs vanish. Eliminating $y$ gives $x''+4x=0$, and the data at $t=-\pi$ give

$$
x(t)=\cos2t.
$$

For all $t$, differentiating the first equation and using the second gives

$$
x''+4x=\delta(t)-2H(t-\pi).
$$

Thus $x$ is continuous at zero while $x'$ jumps by one. For $t>0$ the resulting solution is

$$
x(t)=\cos2t+\frac12\sin2t
+\frac12H(t-\pi)(\cos2t-1).
$$

Since $\cos2t=1-2\sin^2t$, this is

$$
x(t)=\frac12\sin2t+1+q(t)\sin^2t,
$$

where

$$
q(t)=\begin{cases}-2,&0<t<\pi,\\-3,&t\geq\pi.
\end{cases}
$$

**Thus $a=1/2$, $b=1$, and the sketch of $q$ is a downward unit step at $t=\pi$.**

## 8A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8a/a">a</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/a/solution">Solution</h4>

↑ **Parent:** [A](#8a/a)

The system [matrix](../../../vector-space.md#matrix) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2$ and $3$, with [eigenvectors](../../../linear-operator-theory.md#eigenvector) in the directions $y=-x$ and $y=-x/2$, respectively. Both [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are positive, so the origin is an unstable node. The two eigendirections are straight trajectories directed away from the origin. Every other trajectory also moves outward, tangent near the origin in backward time to the faster eigendirection and asymptotic in forward time to the eigenvalue-$3$ direction.

<h3 id="8a/b">b</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/b/i">i</h4>

↑ **Parent:** [B](#8a/b)

<h5 id="8a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8a/b/i)

With $y=\dot x$, the system is

$$
\dot x=y,
\qquad
\dot y=-3y+4\log\frac{x^2+1}{2}.
$$

At equilibrium $y=0$ and $x^2=1$, so the equilibrium points are $(1,0)$ and $(-1,0)$.

<h4 id="8a/b/ii">ii</h4>

↑ **Parent:** [B](#8a/b)

<h5 id="8a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8a/b/ii)

The Jacobian is

$$
J(x,y)=\begin{pmatrix}0&1\\8x/(x^2+1)&-3\end{pmatrix}.
$$

At $(1,0)$ its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,-4$, so this point is a saddle. At $(-1,0)$ they are $(-3\pm i\sqrt7)/2$, so this point is a stable spiral.

<h4 id="8a/b/iii">iii</h4>

↑ **Parent:** [B](#8a/b)

<h5 id="8a/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8a/b/iii)

The sign of $\dot x$ is the sign of $y$. The $\dot y=0$ nullcline is

$$
y=\frac43\log\frac{x^2+1}{2};
$$

$\dot y$ is positive below this curve and negative above it. Combining the upper and lower half-planes with the regions above and below this even curve labels the four requested sign combinations.

<h4 id="8a/b/iv">iv</h4>

↑ **Parent:** [B](#8a/b)

<h5 id="8a/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#8a/b/iv)

Draw the even $\dot y=0$ nullcline through $(\pm1,0)$ and use the arrows from part (iii). Trajectories near $(-1,0)$ spiral clockwise inward because, immediately to its right on the $x$-axis, $\dot y<0$. At $(1,0)$ the stable and unstable eigendirections have slopes $-4$ and $1$. Their four separatrix branches divide the portrait; the only trajectory actually reaching $(1,0)$ at finite time is the constant one, while these branches approach it as $t\to\pm\infty$. All remaining curves follow the sign field, with those in its basin spiralling into $(-1,0)$.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

Conditional on $N=n$, there are $\binom n2$ pairs, and each is both friendly and birthday-matched with probability $1/(2\cdot365)$. Since $\mathbb E[N(N-1)]=365^2$ for a Poisson variable,

$$
\boxed{\mathbb E[\text{matching friend pairs}]
=\frac{365^2}{2}\frac1{730}=\frac{365}{4}.}
$$

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

By [Poisson thinning](../../../probability-theory.md#poisson-thinning), allocating a Poisson$(365)$ population independently and uniformly among $365$ days gives independent Poisson$(1)$ counts. Hence

$$
\boxed{\mathbb P(Z_1=z_1,\ldots,Z_{365}=z_{365})
=e^{-365}\prod_{i=1}^{365}\frac1{z_i!},
\qquad z_i\in\mathbb Z_{\geq0}.}
$$

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

Given $Z_i=n$, the probability of no friendship among people sharing day $i$ is $2^{-n(n-1)/2}$. The day counts are independent, so

$$
\boxed{\mathbb P(\text{no matching friend pair})
=\left[
 e^{-1}\sum_{n=0}^\infty\frac{2^{-n(n-1)/2}}{n!}
\right]^{365}
=\left(\frac{2+C}{e}\right)^{365}.}
$$

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

This is the [Erlang distribution](../../../continuous-probability-distribution.md#erlang-distribution) with shape $n$ and rate one. Direct integration gives, for $t<1$,

$$
\boxed{M_X(t)=\frac1{(n-1)!}\int_0^\infty x^{n-1}e^{-(1-t)x}dx
=(1-t)^{-n}.}
$$

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

Differentiating the moment-generating [function](../../../function.md) at zero gives

$$
\mathbb EX=M_X'(0)=n,
$$



$$
\operatorname{var}X=M_X''(0)-M_X'(0)^2
=n(n+1)-n^2=n.
$$

<h3 id="10f/c">c</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/c/solution">Solution</h4>

↑ **Parent:** [C](#10f/c)

An Erlang$(n,1)$ variable is a sum of $n$ independent rate-one exponential variables, each with mean and variance one. The central [limit](../../../calculus.md#limit-of-a-function) theorem therefore gives

$$
\frac{X-n}{\sqrt n}\Rightarrow N(0,1).
$$

Consequently, for every fixed $q\geq0$,

$$
\boxed{\int_0^{n+q\sqrt n}\frac{x^{n-1}e^{-x}}{(n-1)!}dx
=\mathbb P\left(\frac{X-n}{\sqrt n}\leq q\right)
\longrightarrow\Phi(q).}
$$

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

The [competing exponential clocks](../../../continuous-probability-distribution.md#competing-exponential-clocks) calculation gives

$$
\mathbb P(V>t)=e^{-(\lambda_1+\lambda_2)t},
$$

so $V$ is exponential with rate $\lambda_1+\lambda_2$. Also

$$
\boxed{\mathbb P(V=T_1)=\int_0^\infty\lambda_1e^{-(\lambda_1+\lambda_2)t}dt
=\frac{\lambda_1}{\lambda_1+\lambda_2}.}
$$

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

The exponential memoryless property gives

$$
\boxed{\mathbb P(V\leq t\mid V>s)
=1-\mathbb P(V>t\mid V>s)
=1-e^{-(\lambda_1+\lambda_2)(t-s)}.}
$$

<h3 id="11f/c">c</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/c/solution">Solution</h4>

↑ **Parent:** [C](#11f/c)

After the first of two equal-rate clocks [rings](../../../commutative-algebra.md#ring), the residual lifetime of the other clock is, by memorylessness, a fresh exponential variable of rate $\lambda$, independent of the first ringing time and of which clock rang. Hence

$$
V\sim\operatorname{Exp}(2\lambda),
\qquad W-V\sim\operatorname{Exp}(\lambda),
$$

and these variables are independent.

<h3 id="11f/d">d</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/d/solution">Solution</h4>

↑ **Parent:** [D](#11f/d)

Take the spatial [Fourier transform](../../../analysis.md#fourier-transform) of the [wave equation](../../../wave-equation.md). The transformed initial-value problem is

$$
\widetilde u_{tt}+k^2\widetilde u=0,
\qquad
\widetilde u(k,0)=\widetilde f(k),
\qquad
\widetilde u_t(k,0)=\widetilde g(k),
$$

and hence

$$
\widetilde u(k,t)
=\widetilde f(k)\cos(kt)
+\widetilde g(k)\frac{\sin(kt)}k.
$$

Part (c) and the [convolution theorem](../../../fourier-analysis.md#convolution-theorem) turn the first term into

$$
\frac12\bigl[f(x+t)+f(x-t)\bigr].
$$

For the second term, choose $p$ with $p'=g$. Part (b) says $\widetilde g=ik\widetilde p$, so

$$
\widetilde g(k)\frac{\sin(kt)}k
=i\widetilde p(k)\sin(kt).
$$

Part (c) now makes its inverse transform

$$
\frac12\bigl[p(x+t)-p(x-t)\bigr]
=\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi.
$$

Combining the two terms gives the [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula)

$$
\boxed{
u(x,t)=\frac12\bigl[f(x+t)+f(x-t)\bigr]
+\frac12\int_{x-t}^{x+t}g(\xi)\,d\xi.
}
$$

Let $A=2V$ and $B=W-V$. Part (c) makes $A$ and $B$ independent identically distributed exponential variables of rate $\lambda$. The change of variables $(A,B)=(rs,(1-r)s)$ has Jacobian $s$, and integrating $\lambda^2se^{-\lambda s}$ over $s>0$ gives density one for $0<r<1$. Therefore the [uniform ratio of independent exponential variables](../../../continuous-probability-distribution.md#uniform-ratio-of-independent-exponential-variables) gives

$$
\boxed{\frac{2V}{W+V}=\frac A{A+B}\sim\operatorname{Uniform}(0,1).}
$$

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

The probability generating [function](../../../function.md) is

$$
G_X(t)=\mathbb E[t^X]=\sum_{k=0}^\infty p_kt^k,
\qquad 0\leq t\leq1.
$$

Termwise [differentiation](../../../calculus.md#differentiation) gives

$$
G_X'(t)=\sum_{k\geq1}kp_kt^{k-1},
\qquad
G_X''(t)=\sum_{k\geq2}k(k-1)p_kt^{k-2}.
$$

The coefficients are nonnegative, and $\mathbb P(X\geq2)>0$, so both [derivatives](../../../calculus.md#derivative) are positive and nondecreasing on $(0,1]$.

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

Let $d_n$ be the probability of extinction by generation $n$. Conditioning on the initial individual's offspring gives

$$
d_0=0,
\qquad d_{n+1}=G_X(d_n).
$$

The events increase to eventual extinction, so $d_n\uparrow d$ and continuity gives $d=G_X(d)$. If $r\geq0$ is any other fixed point, induction from $d_0=0\leq r$ and monotonicity of $G_X$ gives $d_n\leq r$ for every $n$. Hence $d\leq r$, proving the [Galton-Watson extinction fixed point](../../../probability-and-statistics.md#galton-watson-extinction-fixed-point) characterization.

<h3 id="12f/c">c</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/c/solution">Solution</h4>

↑ **Parent:** [C](#12f/c)

Since $G_X(1)=1$ and $G_X'(1)=\mu>1$, for $t<1$ sufficiently close to one,

$$
G_X(t)-t<0.
$$

At zero, $G_X(0)-0\geq0$. Continuity therefore gives a fixed point in $[0,1)$, and part (b) implies $d<1$.

<h3 id="12f/d">d</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/d/solution">Solution</h4>

↑ **Parent:** [D](#12f/d)

Taylor's theorem about $1$ gives, for some $\xi\in[t,1]$,

$$
G_X(t)=1-\mu(1-t)+\frac12G_X''(\xi)(1-t)^2.
$$

Since $G_X''$ is nondecreasing and

$$
G_X''(1)=\mathbb E[X(X-1)]=\sigma^2+\mu^2-\mu=:A,
$$

the stated inequality follows. At the fixed point $d<1$,

$$
0\leq(1-d)\left[1-\mu+\frac A2(1-d)\right].
$$

Therefore the [quadratic Galton-Watson extinction bound](../../../probability-and-statistics.md#quadratic-galton-watson-extinction-bound) is

$$
d\leq d^*:=1-\frac{2(\mu-1)}{\sigma^2+\mu^2-\mu}<1.
$$

The denominator is at least $2(\mu-1)$ because $X$ is integer-valued and $\mathbb E[(X-1)(X-2)]\geq0$, so $d^*\geq0$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
