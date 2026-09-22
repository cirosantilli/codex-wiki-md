# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2009/PaperIA_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2009/PaperIA_2.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3F](#3f)
  - [a](#3f/a)
    - [Solution](#3f/a/solution)
  - [b](#3f/b)
    - [Solution](#3f/b/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
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
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12F](#12f)
  - [Solution](#12f/solution)

## 1C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

This is a [logistic equation](../../../differential-equation.md#logistic-differential-equation), with positive [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) $N=\alpha$ and initial population above that value. On the positive branch, put $v=1/N$. It satisfies the [linear ordinary differential equation](../../../differential-equation.md#linear-ordinary-differential-equation) $v'+\alpha v=1$, so $v=\alpha^{-1}+Ce^{-\alpha t}$. The initial condition gives $C=-1/(2\alpha)$, hence

$$
\boxed{N(t)=\frac{\alpha}{1-\tfrac12e^{-\alpha t}}
=\frac{2\alpha}{2-e^{-\alpha t}},\qquad \lim_{t\to\infty}N(t)=\alpha.}
$$

The population decreases monotonically toward the stable [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system); it never reaches it at a finite time.

## 2C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

The [characteristic roots](../../../differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) of the homogeneous [linear ordinary differential equation](../../../differential-equation.md#linear-ordinary-differential-equation) are $2$ and $3$. The forcing is resonant with the $e^{3x}$ solution, so the [method of undetermined coefficients](../../../differential-equation.md#method-of-undetermined-coefficients) uses the particular solution $xe^{3x}$. Thus $y=Ae^{2x}+Be^{3x}+xe^{3x}$. The two initial conditions are $A+B=0$ and $2A+3B+1=0$, giving

$$
\boxed{y=e^{2x}+(x-1)e^{3x}.}
$$

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/a">a</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/a/solution">Solution</h4>

↑ **Parent:** [A](#3f/a)

With $\sigma_1,\sigma_2>0$ and $|\rho|<1$, the [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) has [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
\boxed{f(x_1,x_2)=\frac{1}{2\pi\sigma_1\sigma_2\sqrt{1-\rho^2}}
\exp\left[-\frac{1}{2(1-\rho^2)}
\left(\frac{(x_1-\mu_1)^2}{\sigma_1^2}
-\frac{2\rho(x_1-\mu_1)(x_2-\mu_2)}{\sigma_1\sigma_2}
+\frac{(x_2-\mu_2)^2}{\sigma_2^2}\right)\right].}
$$

The strict correlation bound makes its [covariance matrix](../../../variance.md#covariance-matrix) positive definite, so this is an ordinary two-dimensional density rather than a distribution supported on a line.

<h3 id="3f/b">b</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/b/solution">Solution</h4>

↑ **Parent:** [B](#3f/b)

If $\rho=0$, the [bivariate normal density](../../../probability-and-statistics.md#bivariate-normal-distribution) in part (a) factorizes as

$$
f(x_1,x_2)=
\frac{e^{-(x_1-\mu_1)^2/(2\sigma_1^2)}}{\sqrt{2\pi}\sigma_1}
\frac{e^{-(x_2-\mu_2)^2/(2\sigma_2^2)}}{\sqrt{2\pi}\sigma_2}
=f_1(x_1)f_2(x_2).
$$

Integrating over any product of measurable sets proves [independence of random variables](../../../random-variable.md#independent-random-variables). Conversely, independent variables with finite second moments have $\mathbb E[X_1X_2]=\mathbb E[X_1]\mathbb E[X_2]$, so their [covariance](../../../variance.md#covariance) is zero and $\rho=\operatorname{Cov}(X_1,X_2)/(\sigma_1\sigma_2)=0$. This proves [independence of uncorrelated jointly normal variables](../../../probability-and-statistics.md#independence-of-uncorrelated-jointly-normal-variables); zero correlation alone would not imply independence without the joint normal assumption.

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

The events $B\cap A_i$ are pairwise disjoint and their union is $B$. Finite additivity and the definition of [conditional probability](../../../probability-theory.md#conditional-probability) therefore give the [law of total probability](../../../probability-theory.md#law-of-total-probability):

$$
P(B)=\sum_{i=1}^nP(B\cap A_i)
=\sum_{i=1}^nP(A_i)P(B\mid A_i).
$$

For the [birthday problem](../../../probability-and-statistics.md#birthday-problem), let $D$ mean that all birthdays differ. For $n\leq365$, sequential conditioning on previous distinct birthdays and [independence of random variables](../../../random-variable.md#independent-random-variables) give

$$
P(D)=\prod_{j=0}^{n-1}\left(1-\frac{j}{365}\right)
\leq\exp\left(-\sum_{j=0}^{n-1}\frac{j}{365}\right)
=\exp\left(-\frac{n(n-1)}{730}\right).
$$

Here each factor uses the stated bound $1-x\leq e^{-x}$. For $n\geq29$, $n(n-1)\geq812>730\log3$, so

$$
\boxed{P(\text{at least one shared birthday})=1-P(D)\geq\frac23.}
$$

For $n>365$ a match is certain by the [pigeonhole principle](../../../algebra.md#pigeonhole-principle). The threshold from the exponential bound is $(1+\sqrt{1+2920\log3})/2\approx28.8$, so $29$ suffices.

## 5C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

On an interval where $y>0$, the [Bernoulli differential equation](../../../differential-equation.md#bernoulli-differential-equation) is transformed by $u=y^{1-p}$:

$$
u'=(1-p)y^{-p}y'=(1-p)(f_1u+f_2).
$$

For $f_1=1$, $f_2=x$, put $s=1-p\ne0$. An [integrating factor](../../../differential-equation.md#integrating-factor) $e^{-sx}$ solves $u'-su=sx$, giving $u=Ce^{sx}-x-s^{-1}$. Thus the positive branches are

$$
\boxed{y(x)=\left(Ce^{(1-p)x}-x-\frac1{1-p}\right)^{1/(1-p)},}
$$

on intervals where the expression in parentheses is positive. The transformation omits the separate solution $y\equiv0$. For $0<p<1$, the right-hand side need not be locally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) at zero, so nonnegative solutions can also join zero and positive branches where the original equation permits; the formula describes every strictly positive segment.

For the autonomous case, $y'=y-\alpha^2y^p$. Its two nonnegative [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are

$$
\boxed{y=0,\qquad y_*=|\alpha|^{2/(1-p)}.}
$$

At the positive [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), $f'(y_*)=1-p$. If $p>1$, $f(y)>0$ below $y_*$ and $f(y)<0$ above it; hence **$0$ is unstable and $y_*$ is asymptotically stable**. Every strictly positive solution tends to $y_*$ forward in time.

If $0<p<1$, those signs reverse: **$0$ is stable from the nonnegative side and $y_*$ is unstable**. The stability at zero follows from the phase-line signs, not a finite derivative there. For initial value $0<y_0<y_*$, the transformed equation is $u'=s(u-\alpha^2)$ with $s>0$. The solution reaches zero at

$$
T=\frac1{1-p}\log\frac{\alpha^2}{\alpha^2-y_0^{1-p}},
$$

and remains zero thereafter as a nonnegative forward solution. This is [finite-time extinction in a sublinear Bernoulli equation](../../../differential-equation.md#finite-time-extinction-in-a-sublinear-bernoulli-equation). Initial values above $y_*$ increase without bound; the sublinear negative term prevents neither that growth nor the instability of $y_*$.

## 6C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

Assume $\omega>0$. The [characteristic roots](../../../differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) of the [damped harmonic oscillator](../../../analysis.md#damped-harmonic-oscillator) are $-k\pm\sqrt{k^2-\omega^2}$. Its general homogeneous solution is

$$
\boxed{\begin{array}{ll}
k<\omega:&x=e^{-kt}(C\cos pt+D\sin pt),\quad p=\sqrt{\omega^2-k^2},\\
k=\omega:&x=(C+Dt)e^{-kt},\\
k>\omega:&x=e^{-kt}(C\cosh qt+D\sinh qt),\quad q=\sqrt{k^2-\omega^2}.
\end{array}}
$$

These are respectively the underdamped, [critically damped](../../../wave-equation.md#critical-damping) and overdamped regimes.

For the [velocity-switched driven oscillator](../../../analysis.md#velocity-switched-driven-oscillator), the initial acceleration is $-\omega^2x_1<0$. Its velocity is therefore negative on the first half-cycle, and the forcing is zero:

$$
\boxed{x(t)=x_1e^{-kt}\left(\cos pt+\frac{k}{p}\sin pt\right),\qquad 0\leq t\leq\frac\pi p.}
$$

Indeed $\dot x=-(\omega^2x_1/p)e^{-kt}\sin pt<0$ in that open interval. Set $r=e^{-k\pi/p}$; at the first turning point, $x_2=-rx_1$ and $\dot x=0$.

Put $\tau=t-\pi/p$. On the second half-cycle the velocity is positive, so the particular solution is $a/\omega^2$. Matching position and velocity gives

$$
\boxed{x(t)=\frac a{\omega^2}
+\left(-rx_1-\frac a{\omega^2}\right)e^{-k\tau}
\left(\cos p\tau+\frac{k}{p}\sin p\tau\right),\quad
\frac\pi p\leq t\leq\frac{2\pi}p.}
$$

Its derivative is positive for $0<\tau<\pi/p$. At the next turning point,

$$
x_3=r^2x_1+(1+r)\frac a{\omega^2},\qquad \dot x_3=0.
$$

The [turning-point return map](../../../dynamical-systems.md#poincare-map) therefore repeats the initial state exactly when

$$
\boxed{x_1=\frac{a}{\omega^2(1-r)},\qquad r=e^{-k\pi/p},\qquad T=\frac{2\pi}{p}.}
$$

This value exceeds $a/\omega^2$, so the subsequent acceleration initiates the required negative-velocity half-cycle again. The switched solution is continuous with continuous velocity, and is piecewise twice differentiable; acceleration has one-sided jumps where the forcing switches.

<a id="6c/image-periodic-motion-of-the-oscillator-with-forcing-applied-only-during-positive-velocity"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2-switched-oscillator.png)

**[Figure 1](#6c/image-periodic-motion-of-the-oscillator-with-forcing-applied-only-during-positive-velocity). Periodic motion of the oscillator with forcing applied only during positive velocity**.

For $k>\omega$, the specified positive initial value gives

$$
x=x_1e^{-kt}\left(\cosh qt+\frac{k}{q}\sinh qt\right),\qquad
\dot x=-\frac{\omega^2x_1}{q}e^{-kt}\sinh qt<0\quad(t>0).
$$

There is no next turning point: the forcing stays zero and $x$ approaches zero monotonically. **The motion from the specified initial state cannot be periodic.** More generally, a solution started at any positive maximum has this same obstruction; a nonconstant periodic orbit would require such a maximum. The zero equilibrium is a separate constant solution.

## 7C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

The origin is a [regular singular point](../../../complex-analysis.md#regular-singular-point) of this [Kummer differential equation](../../../differential-equation.md#kummer-differential-equation). Apply the [Frobenius method](../../../complex-analysis.md#frobenius-method), writing $y=\sum_{n=0}^\infty a_nx^{n+r}$ with $a_0\ne0$. The lowest power gives the [indicial equation](../../../differential-equation.md#indicial-equation)

$$
r(r+c-1)=0,\qquad r=0,\ 1-c.
$$

For $n\geq1$, comparison of the coefficient of $x^{n+r-1}$ gives

$$
(n+r)(n+r+c-1)a_n-(n+r)a_{n-1}=0,\qquad
a_n=\frac{a_{n-1}}{n+r+c-1}.
$$

Since $0<c<1$, both roots give valid independent branches. Normalize $a_0=1$:

$$
\boxed{y_1(x)=\sum_{n=0}^\infty\frac{\Gamma(c)}{\Gamma(c+n)}x^n
=\sum_{n=0}^\infty\frac{x^n}{(c)_n},\qquad
y_2(x)=x^{1-c}\sum_{n=0}^\infty\frac{x^n}{n!}=x^{1-c}e^x.}
$$

Here $(c)_n$ is the [rising factorial](../../../combinatorics.md#rising-factorial), and the first series is the [confluent hypergeometric function of the first kind](../../../differential-equation.md#confluent-hypergeometric-function-of-the-first-kind) $M(1,c,x)$. The two leading powers are distinct, proving [linear independence](../../../vector-space.md#linear-independence). We describe real solutions on $x>0$, with their one-sided behavior at zero.

For the inhomogeneous equation a particular solution is $-(x+c)/2$, verified by direct substitution. Thus $y=Ay_1+By_2-(x+c)/2$. Since $y_2'\sim(1-c)x^{-c}$, a finite derivative at zero forces $B=0$. Then $y(0)=0$ forces $A=c/2$, and the required solution is

$$
\boxed{y(x)=\frac c2\left[M(1,c,x)-1-\frac xc\right]
=\frac c2\sum_{n=2}^\infty\frac{x^n}{(c)_n}.}
$$

In particular $y'(0)=0$. The singular homogeneous branch cannot be added without violating the derivative condition.

## 8C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8c/a">a</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/a/solution">Solution</h4>

↑ **Parent:** [A](#8c/a)

The [chain rule](../../../calculus.md#chain-rule) gives $\partial_x=\partial_u+\partial_v$ and $\partial_t=\partial_u-\partial_v$. Hence $\partial_x^2-\partial_t^2=4\partial_u\partial_v$, and the forced [wave equation](../../../wave-equation.md) becomes $y_{uv}=1$. Integrating twice gives $y=uv+F(u)+G(v)$. At $t=0$ the initial conditions are

$$
x^2+F(x)+G(x)=\sin x,\qquad F'(x)-G'(x)=0.
$$

Thus $F-G$ is constant, which cancels from the final expression. Combining the remaining sum yields

$$
y=uv+\tfrac12(\sin u+\sin v-u^2-v^2)
=\boxed{\sin x\cos t-2t^2.}
$$

Differentiation checks the forcing and both initial conditions.

<h3 id="8c/b">b</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/b/solution">Solution</h4>

↑ **Parent:** [B](#8c/b)

Apply [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) on the moving drop:

$$
\frac{dM}{dt}=R\,h(R,t)\dot R+\int_0^Rrh_t\,dr
=\left[rh^3h_r\right]_0^R.
$$

The moving-boundary term vanishes because $h(R,t)=0$. At the origin, symmetry and regularity give $h_r(0,t)=0$. At the front, the stated $h\propto(R-r)^{1/3}$ gives $h^3h_r=O((R-r)^{1/3})\to0$. Thus $\boxed{dM/dt=0}$, expressing [volume conservation](../../../physics.md#volume-conservation) for this [axisymmetric viscous gravity current](../../../reduced-gravity.md#axisymmetric-viscous-gravity-current).

With $\eta=r/t^\alpha$ and $R=\eta_0t^\alpha$, substitute the [self-similar solution](../../../partial-differential-equation.md#similarity-solution) into the conserved integral:

$$
M=t^{2\alpha-1/4}\int_0^{\eta_0}\eta f(\eta)\,d\eta.
$$

For a nonzero finite drop volume, the power of $t$ must vanish, so $\boxed{\alpha=1/8}$. Balancing powers in the evolution equation gives the same result: its left side scales as $t^{-5/4}$ and its right side as $t^{-1-2\alpha}$. The front-edge exponent alone would not determine this spreading exponent without the conserved volume.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

Use the usual assumption that the two die scores are [independent random variables](../../../random-variable.md#independent-random-variables). A fair score has [expected value](../../../probability-theory.md#expected-value) $7/2$ and [variance](../../../variance.md) $35/12$. [Linearity of expectation](../../../probability-theory.md#linearity-of-expectation) and the [variance of a sum](../../../variance.md#variance-of-a-sum) therefore give

$$
\boxed{\mathbb EX=7,\quad\mathbb EY=0,\quad
\operatorname{Var}X=\operatorname{Var}Y=\frac{35}{6}.}
$$

Count the ordered pairs of scores to obtain the [probability mass functions](../../../probability-theory.md#probability-mass-function)

$$
P(X=x)=\frac{6-|x-7|}{36},\quad x=2,\ldots,12;\qquad
P(Y=y)=\frac{6-|y|}{36},\quad y=-5,\ldots,5.
$$

On these attainable [probability supports](../../../probability-theory.md#support-of-a-probability-distribution), **the maxima occur at $x=7$ and $y=0$, each with probability $1/6$; the minima occur at $x=2,12$ and $y=-5,5$, each with probability $1/36$**. Outside the respective [probability support](../../../probability-theory.md#support-of-a-probability-distribution), the mass is zero.

They are not independent: $Y=0$ implies equal die scores and hence $X$ is an [even number](../../../number-theory.md#even-number), so $P(X=7,Y=0)=0$, whereas $P(X=7)P(Y=0)=1/36>0$. In fact $\operatorname{Cov}(X,Y)=\operatorname{Var}(S_1)-\operatorname{Var}(S_2)=0$: this is an example of [uncorrelated random variables](../../../variance.md#uncorrelated-random-variables) that are dependent.

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

Again assume independent die scores. Their sum has the discrete [convolution](../../../fourier-analysis.md#convolution) of the two score distributions, so

$$
\boxed{P(X=2)=p_1q_1,\qquad
P(X=7)=\sum_{i=1}^6p_iq_{7-i},\qquad
P(X=12)=p_6q_6.}
$$

All terms are nonnegative. The [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) applied to the two extreme-score contributions gives

$$
P(X=7)\geq p_1q_6+p_6q_1
\geq2\sqrt{p_1q_6p_6q_1}
=2\sqrt{P(X=2)P(X=12)}.
$$

If all eleven probabilities were equal, normalization would make each $1/11$, but the inequality would require $1/11\geq2/11$. This contradiction proves **the sum cannot be uniform on $\{2,\ldots,12\}$**, whatever the individual die probabilities.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

View the accessible rooms as the open cluster of [bond percolation](../../../bond-percolation.md) on a rooted ternary [tree](../../../combinatorics.md#tree-graph-theory). Each accessible room has three forward corridors, independently open with probability $2/3$, so its number of accessible children has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) $\operatorname{Bin}(3,2/3)$. The counts at successive levels form a [binomial branching process](../../../probability-and-statistics.md#binomial-branching-process) with offspring [probability generating function](../../../probability-theory.md#probability-generating-function)

$$
\boxed{\phi(t)=\left(\frac13+\frac23t\right)^3.}
$$

Let $q_N$ be the probability that the root has no open path to level $N$. Then $q_0=0$, and independence of the three descendant subtrees gives

$$
q_{N+1}=\left(\frac13+\frac23q_N\right)^3=\phi(q_N).
$$

The sequence increases to the smallest fixed point $q=\phi(q)$ in $[0,1]$, the [branching extinction probability](../../../probability-and-statistics.md#extinction-probability-of-a-branching-process). Thus $q_N$ is close to that solution for large $N$.

Connectivity is the relevant escape event: if no window is reachable, escape is impossible; if one is reachable, ordinary random wandering reaches a window eventually with probability one. Before reaching level $N$ the guest moves within a finite connected graph, so an accessible exit cannot be avoided forever. This interpretation does not require the guest to move monotonically outward.

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

The [Galton-Watson extinction fixed point](../../../probability-and-statistics.md#galton-watson-extinction-fixed-point) equation is

$$
(1+2q)^3=27q,\qquad
8q^3+12q^2-21q+1=(q-1)(8q^2+20q-1)=0.
$$

Its smallest root in $[0,1]$ is $q=(3\sqrt3-5)/4$, not the other allowed fixed point $1$. Consequently the large-depth escape probability is

$$
\boxed{1-q=\frac{9-3\sqrt3}{4}\approx0.95096.}
$$

For finite $N$, the exact escape probability is $1-q_N$ and is slightly larger. Indeed $\phi'(q)=2-\sqrt3<1$, and the [mean value theorem](../../../calculus.md#mean-value-theorem) on $[q_N,q]$ gives $0\leq q-q_N\leq q(2-\sqrt3)^N$. This also quantifies how quickly the finite-depth answer approaches the displayed limit.

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

Integrating the [uniform density](../../../continuous-probability-distribution.md#continuous-uniform-distribution) gives $\mathbb EX^k=\int_0^1x^k\,dx=1/(k+1)$. By [independence of random variables](../../../random-variable.md#independent-random-variables), $\mathbb E(XY)^k=\mathbb EX^k\,\mathbb EY^k=1/(k+1)^2$. For the remaining [expected value](../../../probability-theory.md#expected-value), integrate first in $x$:

$$
\begin{aligned}
\mathbb E(1-XY)^k
&=\int_0^1\int_0^1(1-xy)^k\,dx\,dy\\
&=\frac1{k+1}\int_0^1\frac{1-(1-y)^{k+1}}y\,dy
=\frac1{k+1}\sum_{j=0}^k\int_0^1(1-y)^j\,dy.
\end{aligned}
$$

The value at $y=0$ is supplied by continuity. Therefore, with the [harmonic number](../../../analytic-number-theory.md#harmonic-number) $H_m=\sum_{j=1}^m1/j$,

$$
\boxed{\mathbb E(1-XY)^k=\frac{H_{k+1}}{k+1}.}
$$

Conditional on one sample point being $(x,y)$, it is a [maximal external point](../../../set.md#maximal-external-point) precisely when none of the other $n-1$ points falls in the upper-right rectangle $(x,1]\times(y,1]$. Its area is $(1-x)(1-y)$, so its conditional probability of being maximal is $[1-(1-x)(1-y)]^{n-1}$. Both $1-X$ and $1-Y$ are independent [uniform random variables](../../../continuous-probability-distribution.md#uniform-random-variable), hence a given point is maximal with probability $H_n/n$. Summing their [indicator random variables](../../../probability-theory.md#indicator-random-variable) and applying [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) gives the [expected number of coordinatewise maxima](../../../set.md#expected-number-of-coordinatewise-maxima):

$$
\boxed{\mathbb E[\text{number of maximal external points}]=H_n.}
$$

This grows only logarithmically with the sample size, even though all $n$ points are potential candidates.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

The [law of total probability](../../../probability-theory.md#law-of-total-probability) and the definition of [conditional probability](../../../probability-theory.md#conditional-probability) give [Bayes' theorem](../../../probability-theory.md#bayes-theorem):

$$
P(A_i\mid E)=\frac{P(A_i\cap E)}{P(E)}
=\frac{P(A_i)P(E\mid A_i)}{\sum_{j=1}^3P(A_j)P(E\mid A_j)}.
$$

The denominator is positive because $P(E)>0$.

For the observed cargo, set $p_A=0.05$, $p_B=0.03$, $p_C=0.01$. The [binomial likelihood](../../../discrete-probability-distribution.md#binomial-likelihood) under origin $i$ is

$$
L_i=P(E\mid A_i)=\binom{10000}{200}p_i^{200}(1-p_i)^{9800}.
$$

Equal prior probabilities and [Bayes' theorem](../../../probability-theory.md#bayes-theorem) make the posterior proportional to these likelihoods. The binomial coefficient cancels in the [likelihood ratios](../../../statistical-modelling.md#likelihood-ratio):

$$
\begin{aligned}
\log\frac{L_A}{L_B}
&=200\log\frac53+9800\log\frac{0.95}{0.97}\approx-102.00893,\\
\log\frac{L_C}{L_B}
&=-200\log3+9800\log\frac{0.99}{0.97}\approx-19.71552.
\end{aligned}
$$

Thus $L_A/L_B\approx4.99\times10^{-45}$ and $L_C/L_B\approx2.74\times10^{-9}$, giving

$$
\boxed{P(B\mid E)=\frac1{1+L_A/L_B+L_C/L_B}
\approx0.99999999726.}
$$

Even the permitted approximation $\log(1-p)\approx-p$ gives log ratios about $-93.83$ and $-23.72$, which already show overwhelming posterior preference for B. The exact logarithms are preferable because multiplication by $9800$ magnifies the approximation error. An observed contamination fraction halfway between two hypothesized rates does not give equal [likelihoods](../../../statistical-modelling.md#likelihood-function): the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) assigns asymmetric probabilities to those deviations, especially at this large sample size.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
