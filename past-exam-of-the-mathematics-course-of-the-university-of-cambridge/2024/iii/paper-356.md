# Paper 356

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_356.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_356.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)

## 1

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write the [molecular copy numbers](../../../mathematical-biology.md#molecular-copy-number) as $\mathbf x=(x_1,x_2,x_3,x_4)$ and use the [power-law reaction propensity](../../../mathematical-biology.md#power-law-reaction-propensity) convention of the paper. The seven propensities and [stoichiometric vectors](../../../mathematical-biology.md#stoichiometric-vector) are

$$
\begin{array}{c|c|c}
r&a_r(\mathbf x)&\nu_r\\ \hline
1&\alpha_1x_1^2/V&(-2,0,0,0)\\
2&\alpha_2x_1&(0,1,0,0)\\
3&\alpha_3x_2^2/V&(0,-1,0,0)\\
4&\alpha_4V&(0,0,1,0)\\
5&\alpha_5x_3x_4/V&(0,0,-1,-1)\\
6&\alpha_6x_2&(0,0,0,1)\\
7&\alpha_7x_2x_4/V&(0,-1,0,0).
\end{array}
$$

A channel is assigned zero propensity whenever its update would leave the [nonnegative integer](../../../arithmetic.md#natural-number) lattice.

The [Gillespie algorithm](../../../mathematical-biology.md#gillespie-algorithm) starts from $\mathbf x=(5,0,0,0)$ and $t=0$. At the current state compute $a_0=\sum_{r=1}^7a_r$. If $a_0=0$, terminate the path. Otherwise draw [independent random variables](../../../random-variable.md#independent-random-variables) $U_1,U_2$ from the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$, set the next waiting time to

$$
\tau=-\frac{\log U_1}{a_0},
$$

and choose the least index $r$ satisfying

$$
\sum_{j=1}^ra_j\geq U_2a_0.
$$

Then update $t\leftarrow t+\tau$ and $\mathbf x\leftarrow\mathbf x+\nu_r$, and repeat. The minimum of the seven competing reaction clocks has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $a_0$, while reaction $r$ wins with probability $a_r/a_0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a function $h$ on the copy-number state space, define the shift operator

$$
(E_i^kh)(x_1,\ldots,x_i,\ldots,x_4)
=h(x_1,\ldots,x_i+k,\ldots,x_4).
$$

With the propensities from part (a), the [forward operator of a Markov jump process](../../../markov-process.md#forward-operator-of-a-markov-jump-process) is

$$
\boxed{\begin{aligned}
\mathcal L^*p={}&(E_1^2-1)(a_1p)
+(E_2^{-1}-1)(a_2p)
+(E_2^1-1)(a_3p)\\
&+(E_3^{-1}-1)(a_4p)
+(E_3^1E_4^1-1)(a_5p)
+(E_4^{-1}-1)(a_6p)
+(E_2^1-1)(a_7p).
\end{aligned}}
$$

Equivalently, the [chemical master equation](../../../mathematical-biology.md#chemical-master-equation) has the gain-minus-loss form

$$
(\mathcal L^*p)(\mathbf x)
=\sum_{r=1}^7
\left[a_r(\mathbf x-\nu_r)p(\mathbf x-\nu_r)
-a_r(\mathbf x)p(\mathbf x)\right],
$$

where terms outside the state space vanish.

The adjoint [Markov jump-process generator](../../../markov-process.md#markov-jump-process-generator) acts on observables:

$$
\boxed{(\mathcal Lf)(\mathbf x)
=\sum_{r=1}^7a_r(\mathbf x)
\left[f(\mathbf x+\nu_r)-f(\mathbf x)\right].}
$$

Indeed, shifting the summation index in the gain terms gives $\langle f,\mathcal L^*p\rangle=\langle\mathcal Lf,p\rangle$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Only reaction 1 changes $X_1$. Starting from five molecules, its successive states are $5\to3\to1$, with rates $5^2=25$ and $3^2=9$; state one is then absorbing for this channel. Thus

$$
\mathbb P(X_1(t)=5)=e^{-25t}.
$$

The probability of still being at three is the [convolution](../../../fourier-analysis.md#convolution) of the first waiting time with an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) and survival of the second:

$$
\mathbb P(X_1(t)=3)
=\int_0^t25e^{-25s}e^{-9(t-s)}\,ds
=\frac{25}{16}\left(e^{-9t}-e^{-25t}\right).
$$

Applying the [law of total probability](../../../probability-theory.md#law-of-total-probability) to the three possible states gives

$$
\boxed{g(t)=1-\frac{25}{16}e^{-9t}
+\frac9{16}e^{-25t}.}
$$

It has $g(0)=0$ and tends to one as both reaction waiting times elapse.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

For any observable $f$, the [Markov jump-process generator](../../../markov-process.md#markov-jump-process-generator) identity gives

$$
\frac d{dt}\langle f\rangle=\langle\mathcal Lf\rangle.
$$

Set $m(t)=\langle x_2\rangle$ and $s(t)=\langle x_2^2\rangle$. With $\alpha_7=0$, reaction 2 changes $x_2$ by $+1$ and reaction 3 changes it by $-1$. Therefore

$$
\boxed{\dot m=\alpha_2\langle x_1\rangle-\alpha_3\langle x_2^2\rangle}
$$

and, using $(x_2+1)^2-x_2^2=2x_2+1$ and $(x_2-1)^2-x_2^2=-2x_2+1$,

$$
\boxed{\dot s
=\alpha_2\left(2\langle x_1x_2\rangle+\langle x_1\rangle\right)
-2\alpha_3\langle x_2^3\rangle
+\alpha_3\langle x_2^2\rangle.}
$$

The equation for the second [moment](../../../probability-theory.md#moment) contains the third, whose equation contains the fourth, and so on. This is an infinite [moment hierarchy](../../../mathematical-biology.md#moment-hierarchy).

Reaction 1 eventually leaves the odd initial copy number at $x_1^*=1$. Put

$$
\mu=\langle x_2^*\rangle,\qquad
q=\frac{\alpha_2}{\alpha_3}.
$$

The stationary first-moment equation gives

$$
\langle(x_2^*)^2\rangle=q.
$$

The stationary second-moment equation then gives

$$
\langle(x_2^*)^3\rangle=q(\mu+1).
$$

Under the prescribed [central-moment closure](../../../mathematical-biology.md#central-moment-closure),

$$
0=\left\langle(x_2^*-\mu)^3\right\rangle
=\langle(x_2^*)^3\rangle
-3\mu\langle(x_2^*)^2\rangle+2\mu^3.
$$

Substitution yields the requested [polynomial equation](../../../polynomial.md#polynomial-equation)

$$
\boxed{2\mu^3-2\frac{\alpha_2}{\alpha_3}\mu
+\frac{\alpha_2}{\alpha_3}=0.}
$$

This cubic comes from the closure approximation; it is not an exact equation for the stationary mean.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

Reaction 4 creates $X_3$, reaction 5 removes one $X_3$ and one $X_4$, and reaction 6 creates $X_4$; reaction 7 leaves $X_4$ unchanged. The exact first-moment equations are therefore

$$
\frac d{dt}\langle x_3\rangle
=\alpha_4-\alpha_5\langle x_3x_4\rangle,
\qquad
\frac d{dt}\langle x_4\rangle
=\alpha_6\langle x_2\rangle
-\alpha_5\langle x_3x_4\rangle.
$$

At the assumed unique [stationary distribution](../../../markov-process.md#stationary-distribution), both left-hand sides vanish. Eliminating the common mixed moment gives

$$
\alpha_4=\alpha_6\langle x_2^*\rangle,
\qquad
\boxed{\langle x_2^*\rangle=\frac{\alpha_4}{\alpha_6}.}
$$

**No [moment closure](../../../mathematical-biology.md#moment-closure) or independence assumption is involved.**

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The odd $X_1$ copy number decreases by two until it reaches one, so $\langle x_1(t)\rangle\to1$. The exact $X_2$ first-moment equation is

$$
\dot m_2
=\alpha_2\langle x_1\rangle
-\alpha_3\langle x_2^2\rangle
-\alpha_7\langle x_2x_4\rangle.
$$

Because copy numbers are [nonnegative integers](../../../arithmetic.md#natural-number), $x_2^2\geq x_2$, and the last mixed moment is nonnegative. Hence

$$
\dot m_2+\alpha_3m_2
\leq\alpha_2\langle x_1\rangle.
$$

The [integrating factor](../../../differential-equation.md#integrating-factor) $e^{\alpha_3t}$, together with $\langle x_1(t)\rangle\to1$, gives the comparison bound

$$
\limsup_{t\to\infty}m_2(t)
\leq\frac{\alpha_2}{\alpha_3}.
$$

Subtracting the exact $X_4$ first-moment equation from the $X_3$ equation cancels reaction 5:

$$
\frac d{dt}\left(\langle x_3\rangle-\langle x_4\rangle\right)
=\alpha_4-\alpha_6m_2(t).
$$

The assumed inequality is precisely

$$
\alpha_4-\alpha_6\frac{\alpha_2}{\alpha_3}>0.
$$

Choose a positive $\varepsilon$ smaller than this gap divided by $\alpha_6$. The [limit superior](../../../real-analysis.md#limit-superior) bound implies that, for all sufficiently large $t$,

$$
\frac d{dt}\left(\langle x_3\rangle-\langle x_4\rangle\right)
\geq
\alpha_4-\alpha_6\left(\frac{\alpha_2}{\alpha_3}+\varepsilon\right)>0.
$$

Thus $\langle x_3\rangle-\langle x_4\rangle$ grows at least linearly. Since $\langle x_4\rangle\geq0$,

$$
\boxed{\lim_{t\to\infty}\langle x_3(t)\rangle=\infty,}
$$

so the required species index is $\boxed{i=3}$.

## 2

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The two-dimensional [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation) is

$$
\boxed{
\partial_t p
=-a_1\partial_xp-\partial_y(a_2p)
+\partial_{xx}p+\frac12\partial_{yy}(\sigma^2p)
=-\nabla\mathbin\cdot\mathbf J,
}
$$

with [Fokker-Planck probability current](../../../probability-theory.md#fokker-planck-probability-current)

$$
\boxed{
\mathbf J=
\left(
a_1p-\partial_xp,\,
a_2p-\frac12\partial_y(\sigma^2p)
\right).
}
$$

The point initial condition is

$$
p(x,y,0)=\delta(x)\delta(y),
$$

where $\delta$ is the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function). The [reflecting boundary condition for a diffusion](../../../probability-theory.md#reflecting-boundary-condition-for-a-diffusion) is

$$
\boxed{\mathbf J\mathbin\cdot\mathbf n=0
\quad\hbox{on }\partial\Omega,}
$$

with $\mathbf n$ the outward unit normal. This zero-flux condition conserves the integral of the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) over the square.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\xi_{1,n},\xi_{2,n}$ be [independent random variables](../../../random-variable.md#independent-random-variables) with the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). The unconstrained [Milstein method](../../../stochastic-calculus.md#milstein-method) step is

$$
\widetilde X_{n+1}
=X_n+a_1\Delta t+\sqrt{2\Delta t}\,\xi_{1,n},
$$



$$
\widetilde Y_{n+1}
=Y_n+a_2(X_n,Y_n)\Delta t
+\sigma(Y_n)\sqrt{\Delta t}\,\xi_{2,n}
+\frac12\sigma(Y_n)\sigma'(Y_n)\Delta t
\left(\xi_{2,n}^2-1\right).
$$

The $X$ noise is additive, so its Milstein correction vanishes. The diagonal, independent noise fields commute, so no cross iterated stochastic integral is required.

Implement each [reflecting boundary condition for a diffusion](../../../probability-theory.md#reflecting-boundary-condition-for-a-diffusion) by folding the proposed coordinate back into $[-1,1]$. One formula that also handles multiple overshoots is

$$
R(z)=1-\left|\big((z+1)\bmod4\big)-2\right|.
$$

The complete update is

$$
\boxed{X_{n+1}=R(\widetilde X_{n+1}),\qquad
Y_{n+1}=R(\widetilde Y_{n+1}).}
$$

Under the usual smoothness assumptions, the Milstein discretization has [strong order of convergence](../../../stochastic-calculus.md#strong-convergence-of-a-stochastic-numerical-method) one and [weak order of convergence](../../../stochastic-calculus.md#weak-convergence-of-a-stochastic-numerical-method) one. The reflection enforces the boundary pathwise.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The adsorption mechanism is uniform along the two vertical sides, and $X$ evolves independently of $Y$. Consequently the [mean first-passage time](../../../markov-process.md#mean-first-passage-time) depends only on the initial $x$-coordinate. Its [Kolmogorov backward equation](../../../stochastic-calculus.md#kolmogorov-backward-equation) for $a_1=1$ is

$$
\tau''(x)+\tau'(x)=-1,\qquad -1<x<1.
$$

The forward [partially absorbing boundary condition for a diffusion](../../../probability-theory.md#partially-absorbing-boundary-condition-for-a-diffusion) is $\mathbf J\mathbin\cdot\mathbf n=\kappa p$. The boundary term in the adjoint relation is

$$
\int_{\partial\Omega}
\left(\tau\,\mathbf J\mathbin\cdot\mathbf n
+p\,\partial_n\tau\right)ds,
$$

because the $X$ diffusion coefficient is one. It vanishes for every admissible $p$ precisely when

$$
\partial_n\tau=-\kappa\tau.
$$

For $\kappa=1$, the two [Robin boundary conditions](../../../differential-equation.md#robin-boundary-condition) are therefore

$$
\tau'(-1)=\tau(-1),\qquad
\tau'(1)=-\tau(1).
$$

The general solution of the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) is

$$
\tau(x)=-x+C+De^{-x}.
$$

The right condition gives $C=2$, and the left gives $D=-2/e$. At the prescribed initial position,

$$
\boxed{\tau=\tau(0)=2-\frac2e.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

With an [absorbing boundary condition for a diffusion](../../../probability-theory.md#absorbing-boundary-condition-for-a-diffusion) on each vertical side, the [splitting probability](../../../markov-process.md#splitting-probability) $u(x)$ of hitting the left side before the right is harmonic for the [Kolmogorov backward equation](../../../stochastic-calculus.md#kolmogorov-backward-equation):

$$
u''+a_1u'=0,\qquad
u(-1)=1,\quad u(1)=0.
$$

For $a_1\neq0$,

$$
u(x)=\frac{e^{-a_1x}-e^{-a_1}}
{e^{a_1}-e^{-a_1}}.
$$

The particle starts at $x=0$, so

$$
\boxed{
g(a_1)=u(0)
=\frac{1-e^{-a_1}}{e^{a_1}-e^{-a_1}}
=\frac1{1+e^{a_1}}.
}
$$

The continuous limit at zero is $g(0)=1/2$, as required by reflection symmetry. A large positive drift drives the particle toward the right and gives $g(a_1)\to0$; a large negative drift drives it toward the left and gives $g(a_1)\to1$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
