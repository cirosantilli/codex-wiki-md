# Paper 356

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_356.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_356.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)

## 1

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The backward generator of the drift--diffusion is $\mathcal L=\alpha\partial_y+D\partial_y^2$. The [survival probability](../../../markov-process.md#survival-probability) satisfies the [Kolmogorov backward equation](../../../stochastic-calculus.md#kolmogorov-backward-equation)

$$
\boxed{\partial_tQ=D\partial_y^2Q+\alpha\partial_yQ,
\qquad 0<y<L,}
$$

with

$$
\boxed{Q(0,t)=0,
\qquad \partial_yQ(L,t)=0,
\qquad Q(y,0)=1.}
$$

The target is absorbing, while reflection gives the Neumann boundary condition at $L$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [mean first-passage time](../../../markov-process.md#mean-first-passage-time) obeys the backward equation

$$
D\tau''+\alpha\tau'=-1,
\qquad \tau(0)=0,
\qquad \tau'(L)=0.
$$

For $\alpha\ne0$, direct integration gives

$$
\boxed{\tau(y)=
\frac D{\alpha^2}e^{\alpha L/D}
\left(1-e^{-\alpha y/D}\right)-\frac y\alpha.}
$$

In particular,

$$
\tau(L)=\frac D{\alpha^2}
\left(e^{\alpha L/D}-1\right)-\frac L\alpha.
$$

This increases monotonically with drift away from the target, so the constrained optimum is

$$
\boxed{\alpha_*=-\bar\alpha.}
$$

Expanding the exponential at zero drift yields

$$
\boxed{\tau_0=\lim_{\alpha\to0}\tau(L)=\frac{L^2}{2D}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [telegraph process](../../../stochastic-process.md#telegraph-process) has backward survival equations

$$
\boxed{\begin{aligned}
\partial_tQ^+&=s\partial_yQ^++\lambda(Q^--Q^+),\\
\partial_tQ^-&=-s\partial_yQ^-+\lambda(Q^+-Q^-).
\end{aligned}}
$$

Initially $Q^\pm(y,0)=1$. Only a left-moving trajectory reaches the target, while reflection reverses a right-moving velocity at the outer wall, so the hyperbolic boundary conditions are

$$
\boxed{Q^-(0,t)=0,
\qquad Q^+(L,t)=Q^-(L,t).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The backward equations for the two mean hitting times are

$$
\begin{aligned}
-1&=s(\tau^+)' +\lambda(\tau^--\tau^+),\\
-1&=-s(\tau^-)' +\lambda(\tau^+-\tau^-),
\end{aligned}
$$

with $\tau^-(0)=0$ and $\tau^+(L)=\tau^-(L)$. Their difference obeys

$$
\frac d{dy}(\tau^+-\tau^-)=-\frac2s,
$$

and the reflecting condition fixes $\tau^+-\tau^-=2(L-y)/s$. Integration then gives

$$
\boxed{\tau^-(y)=\frac ys
+\frac{2\lambda}{s^2}\left(Ly-\frac{y^2}{2}\right),}
$$

and

$$
\boxed{\tau^+(y)=\frac{2L-y}{s}
+\frac{2\lambda}{s^2}\left(Ly-\frac{y^2}{2}\right).}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

At the reflecting endpoint the two values coincide:

$$
\tau^+(L)=\tau^-(L)=\frac Ls+\frac{\lambda L^2}{s^2}.
$$

Under the [diffusion limit of the telegraph process](../../../stochastic-process.md#diffusion-limit-of-the-telegraph-process) $s,\lambda\to\infty$ with $s^2/(2\lambda)=D$,

$$
\boxed{\tau^\pm(L)\longrightarrow\frac{L^2}{2D}=\tau_0.}
$$

Rapid velocity reversals erase directional persistence. Their integrated velocity converges to Brownian motion with diffusivity $D$, so its first-passage statistic converges to the zero-drift result.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Choose $\Delta t$ with $\lambda\Delta t\ll1$ and $s\Delta t$ small relative to $L$ and the distance to the target. For each of many independent trajectories:

1. Set $x=y$, $v=s$, and $t=0$.  
2. Propose $x_{\rm new}=x+v\Delta t$.  
3. If $x_{\rm new}\leq0$, record the linearly interpolated target-crossing time and stop. If $x_{\rm new}\geq L$, reflect to $x_{\rm new}=2L-x_{\rm new}$ and set $v=-|v|$.  
4. Otherwise reverse $v$ with probability $1-e^{-\lambda\Delta t}$, set $x=x_{\rm new}$ and $t=t+\Delta t$, and repeat.

The sample mean of the recorded times estimates $\tau^+(y)$. Sampling a Poisson number of reversals and their ordered times inside each step removes the at-most-one-reversal approximation, but the stated Bernoulli scheme converges as $\Delta t\to0$.

## 2

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\mathbf e_i$ be the $i$th coordinate vector and take $p$ to be zero whenever any argument is negative. Right jumps $i\to i+1$, left jumps $i\to i-1$, and absorption from compartment $1$ give the [chemical master equation](../../../mathematical-biology.md#chemical-master-equation)

$$
\begin{aligned}
\partial_t p(\mathbf a,t)
={}&\sum_{i=1}^{m-1}k_i^+
\left[(a_i+1)p(\mathbf a+\mathbf e_i-\mathbf e_{i+1},t)
-a_ip(\mathbf a,t)\right]\\
&+\sum_{i=2}^{m}k_i^-
\left[(a_i+1)p(\mathbf a-\mathbf e_{i-1}+\mathbf e_i,t)
-a_ip(\mathbf a,t)\right]\\
&+k_1^-\left[(a_1+1)p(\mathbf a+\mathbf e_1,t)
-a_1p(\mathbf a,t)\right].
\end{aligned}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Multiplying the master equation by $a_i$, summing over every state, and shifting indices in each gain term gives, for $2\leq i\leq m-1$,

$$
\boxed{\frac{dM_i}{dt}
=k_{i-1}^+M_{i-1}-(k_i^++k_i^-)M_i+k_{i+1}^-M_{i+1}.}
$$

At the absorbing left edge and reflecting right edge the corresponding equations are

$$
\boxed{\frac{dM_1}{dt}=-(k_1^++k_1^-)M_1+k_2^-M_2,}
$$



$$
\boxed{\frac{dM_m}{dt}=k_{m-1}^+M_{m-1}-k_m^-M_m.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A centered nearest-neighbour discretization of drift--diffusion is obtained from

$$
\boxed{k_i^+=\frac D{h^2}+\frac{v(x_i)}{2h},
\qquad
k_i^-=\frac D{h^2}-\frac{v(x_i)}{2h}.}
$$

For sufficiently small $h$ these rates are nonnegative. Taylor expansion of the mean equations gives

$$
\partial_tc=D\partial_x^2c-\partial_x(vc).
$$

Absorption into the target to the left of the first compartment gives

$$
\boxed{c(0,t)=0,}
$$

while the absence of outward jumps at the right endpoint gives the [zero-flux boundary condition](../../../probability-theory.md#zero-flux-boundary-condition)

$$
\boxed{v(L)c(L,t)-D\partial_xc(L,t)=0.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation) corresponds to the [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion)

$$
\boxed{dX=v(X)dt+\sqrt{2D}\,dW,}
$$

absorbed at $0$ and reflected at $L$.

For $v(x)=x$, an Euler--Maruyama proposal is

$$
Y=X_n+X_n\Delta t+\sqrt{2D\Delta t}\,Z_n,
\qquad Z_n\sim N(0,1).
$$

If $Y\leq0$, kill the path. If $X_n>0$ and $Y>0$, an endpoint-only test can miss a crossing. Conditional on the endpoints, the local [Brownian bridge](../../../brownian-motion.md#brownian-bridge) crossing probability is

$$
\boxed{p_{\rm cross}=\exp\left(-\frac{X_nY}{D\Delta t}\right).}
$$

Kill the path with this probability; otherwise impose reflection at $L$ by replacing an overshoot $Y>L$ with $2L-Y$ and set $X_{n+1}=Y$. Repeated reflection handles very rare multiple overshoots, and the approximation converges as $\Delta t\to0$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Under the independence closure, the mean rightward flux across the bond $(i,i+1)$ is

$$
J_{i+1/2}=k_i^+M_i(1-M_{i+1})
-k_{i+1}^-M_{i+1}(1-M_i).
$$

The mean equation is the discrete conservation law $\dot M_i=J_{i-1/2}-J_{i+1/2}$. Substitution of the rates from part c and Taylor expansion show that the exclusion factors cancel from the symmetric diffusive contribution but remain in the biased contribution:

$$
J=-D\partial_xc+v(x)c(1-c).
$$

Therefore the mean-field [asymmetric simple exclusion process](../../../mathematical-biology.md#asymmetric-simple-exclusion-process) limit is

$$
\boxed{\partial_tc
=D\partial_x^2c-\partial_x[v(x)c(1-c)].}
$$

The factor $1-c$ is the probability that the destination site is vacant.

## 3

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use [stochastic mass-action propensities](../../../mathematical-biology.md#stochastic-chemical-kinetics)

$$
a_1=\frac{\alpha_1}{V}y(y-1),
\quad a_2=\frac{\alpha_2}{V}x(x-1),
\quad a_3=\frac{\alpha_3V}{\varepsilon},
\quad a_4=\frac{\alpha_4}{\varepsilon V}xy.
$$

Writing $E_x^rf(x,y)=f(x+r,y)$ and similarly for $E_y$, the fast and slow forward operators are

$$
\boxed{\mathcal L_0^*
=(E_y^{-1}-1)\alpha_3V
+(E_y^{+1}-1)\frac{\alpha_4xy}{V},}
$$



$$
\boxed{\mathcal L_1^*
=(E_x^{-1}E_y^{+2}-1)\frac{\alpha_1y(y-1)}V
+(E_x^{+1}-1)\frac{\alpha_2x(x-1)}V.}
$$

Each shift operator acts on everything to its right, including the propensity. Birth of $Y$ and consumption of $Y$ by $X+Y\to X$ are fast; $2Y\to X$ and $2X\to X$ are slow. The slow species is $X$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

At leading order, $\mathcal L_0^*[p_0(y\mid x)p_0(x,t)]=0$. For fixed $x$, the conditional stationary law therefore satisfies

$$
\boxed{0=\alpha_3V[p_0(y-1\mid x)-p_0(y\mid x)]
+\frac{\alpha_4x}{V}[(y+1)p_0(y+1\mid x)-yp_0(y\mid x)].}
$$

This is an [immigration--death process](../../../mathematical-biology.md#immigration-death-process), whose stationary distribution is Poisson with mean

$$
\boxed{q(x)=\langle Y\mid X=x\rangle
=\frac{\alpha_3V^2}{\alpha_4x}.}
$$

The mean is finite only for $x>0$. The assumption $X(0)\ne0$ and the pair-coalescence propensity $x(x-1)$ ensure that the slow process cannot remove its last $X$ molecule, so the reduced model remains in that domain.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Averaging the slow propensities over the conditional Poisson distribution uses $\mathbb E[Y(Y-1)\mid X=x]=q(x)^2$. Thus the effective birth and death rates of $X$ are

$$
\boxed{\lambda_1(x)=\frac{\alpha_1}{V}q(x)^2
=\frac{\alpha_1\alpha_3^2V^3}{\alpha_4^2x^2},}
$$



$$
\boxed{\lambda_2(x)=\frac{\alpha_2}{V}x(x-1).}
$$

Consequently

$$
\boxed{\partial_tp_0(x,t)
=([E_x^{-1}-1]\lambda_1(x)
+[E_x^{+1}-1]\lambda_2(x))p_0(x,t).}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Applying the reduced [Markov jump-process generator](../../../markov-process.md#markov-jump-process-generator) to $f(x)=x$ gives the exact moment equation

$$
\boxed{\frac{dm}{dt}
=\left\langle
\frac{\alpha_1\alpha_3^2V^3}{\alpha_4^2X^2}
-\frac{\alpha_2X(X-1)}V
\right\rangle.}
$$

Under the stated moment closure this becomes the same expression evaluated at $X=m$. Set $m=V\bar x$ and let $V\to\infty$ to obtain

$$
\frac{d\bar x}{dt}
=\frac{\alpha_1\alpha_3^2}{\alpha_4^2\bar x^2}
-\alpha_2\bar x^2.
$$

Its positive stable equilibrium is

$$
\boxed{\lim_{t\to\infty}\bar x(t)
=\left(\frac{\alpha_1\alpha_3^2}
{\alpha_2\alpha_4^2}\right)^{1/4}.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The stochastic quasi-steady-state simulation evolves only $X$:

1. At the current integer $x\geq1$, compute $q(x)=\alpha_3V^2/(\alpha_4x)$ and the averaged rates $\lambda_1(x)=\alpha_1q(x)^2/V$ and $\lambda_2(x)=\alpha_2x(x-1)/V$.  
2. Draw a waiting time $\Delta t\sim\operatorname{Exp}(\lambda_1+\lambda_2)$.  
3. Set $x\leftarrow x+1$ with probability $\lambda_1/(\lambda_1+\lambda_2)$; otherwise set $x\leftarrow x-1$.  
4. Advance time by $\Delta t$ and repeat.

This is a [Gillespie algorithm](../../../mathematical-biology.md#gillespie-algorithm) for the averaged slow master equation. It samples the fast conditional equilibrium analytically through its factorial moment and never simulates individual fast $Y$ births or deaths.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
