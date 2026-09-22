# Paper 2

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_2.pdf)

**Table of contents**

- [1B](#1b)
  - [Solution](#1b/solution)
- [2B](#2b)
  - [Solution](#2b/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6B](#6b)
  - [i](#6b/i)
    - [Solution](#6b/i/solution)
  - [ii](#6b/ii)
    - [Solution](#6b/ii/solution)
  - [iii](#6b/iii)
    - [Solution](#6b/iii/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
- [8B](#8b)
  - [i](#8b/i)
    - [Solution](#8b/i/solution)
  - [ii](#8b/ii)
    - [Solution](#8b/ii/solution)
  - [iii](#8b/iii)
    - [Solution](#8b/iii/solution)
  - [iv](#8b/iv)
    - [Solution](#8b/iv/solution)
- [9F](#9f)
  - [Solution](#9f/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12F](#12f)
  - [Solution](#12f/solution)

## 1B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1b/solution">Solution</h3>

↑ **Parent:** [1B](#1b)

With $\tau=1/t$, the [chain rule](../../../calculus.md#chain-rule) gives $d/dt=-\tau^2d/d\tau$. Since $u=v/\tau$,

$$
\frac{du}{dt}=v-\tau v',\qquad \frac{d^2u}{dt^2}=\tau^3v''.
$$

Substituting into the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) and multiplying by $\tau>0$ leaves $v''+\lambda^2v=0$, the [harmonic oscillator equation](../../../classical-mechanics.md#simple-harmonic-motion). Its two independent real solutions are $\cos(\lambda\tau)$ and $\sin(\lambda\tau)$. Undoing the [change of variables](../../../calculus.md#change-of-variables-formula) gives

$$
\boxed{u(t)=t\left[A\cos\frac\lambda t+B\sin\frac\lambda t\right],\qquad t>0.}
$$

The constants $A,B$ are arbitrary real numbers. The [reciprocal-coordinate reduction of a beam-type equation](../../../differential-equation.md#reciprocal-coordinate-reduction-of-a-beam-type-equation) works on the entire positive half-line, where the coordinate transformation is invertible.

## 2B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2b/solution">Solution</h3>

↑ **Parent:** [2B](#2b)

For continuously differentiable coefficients on a simply connected domain, the exactness condition is **$P_y=Q_x$**. Locally the same condition suffices without a global topological assumption. An [exact first-order ordinary differential equation](../../../differential-equation.md#exact-first-order-ordinary-differential-equation) has a potential $F$ with $F_x=P$ and $F_y=Q$, so $dF/dx=P+Qy'=0$ along a solution. Thus its [implicit solution](../../../differential-equation.md#implicit-solution) is $F(x,y)=C$. One local construction, on a rectangle about $(x_0,y_0)$, is

$$
F(x,y)=\int_{x_0}^xP(s,y_0)\,ds+\int_{y_0}^yQ(x,t)\,dt.
$$

The equality of cross derivatives verifies both required derivatives; on a simply connected domain one may use the corresponding path-independent integral of the [exact differential form](../../../differential-form.md#exact-differential-form).

Here $P=4x+3y$, $Q=3x+3y^2$ and $P_y=Q_x=3$. Integrating $P$ with respect to $x$ gives $F=2x^2+3xy+K(y)$. Matching $F_y=Q$ gives $K'=3y^2$, so take $K=y^3$. The initial value sets $C=F(1,2)=16$. Therefore

$$
\boxed{2x^2+3xy+y^3=16.}
$$

This is the requested explicit relation between the coordinates. Since $F_y(1,2)=15\ne0$, the [implicit function theorem](../../../calculus.md#implicit-function-theorem) gives a unique local graph through the initial point, with slope $-10/15=-2/3$.

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

Let the independent unit-step vectors be $V_j=(\cos\Theta_j,\sin\Theta_j)$. The [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) of each angle gives $\mathbb E[V_j]=0$, while $|V_j|^2=1$. With $S_n=\sum_{j=1}^nV_j$, expand the [squared Euclidean norm](../../../functional-analysis.md#squared-euclidean-norm):

$$
\mathbb E|S_n|^2=\sum_{j=1}^n\mathbb E|V_j|^2+2\sum_{i<j}\mathbb E[V_i\cdot V_j].
$$

By [independence](../../../random-variable.md#independent-random-variables), each cross term equals $\mathbb E[V_i]\cdot\mathbb E[V_j]=0$. Hence

$$
\boxed{\mathbb E|S_n|^2=n.}
$$

This [mean-square displacement of an isotropic planar random walk](../../../markov-process.md#mean-square-displacement-of-an-isotropic-planar-random-walk) grows linearly even though the [expected value](../../../probability-theory.md#expected-value) of the displacement vector remains zero.

## 4F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

Write the countable supports as $D_i$ and the marginal masses as $p_i(x_i)$. [Independence](../../../random-variable.md#independent-random-variables) gives joint mass $\prod_ip_i(x_i)$. Assuming finite [expected values](../../../probability-theory.md#expected-value), absolute integrability is justified by [Tonelli theorem](../../../measure-theory.md#tonelli-theorem):

$$
\mathbb E\left[\prod_i|X_i|\right]=\sum_{x_1\in D_1,\ldots,x_n\in D_n}\prod_i|x_i|p_i(x_i)=\prod_i\mathbb E|X_i|<\infty.
$$

Consequently [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) permits factorization of the signed sum, proving the [expectation of a product of independent random variables](../../../probability-theory.md#expectation-of-a-product-of-independent-random-variables):

$$
\boxed{\mathbb E\left[\prod_iX_i\right]=\prod_i\mathbb E[X_i].}
$$

The second claim holds as a general assertion with the additional hypothesis that **the positive variables are integer-valued**. For a nonnegative integer-valued $Z$, the pointwise identity $Z=\sum_{m\ge0}\mathbf1_{\{Z>m\}}$ and [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) give the [tail-sum formula](../../../probability-theory.md#tail-sum-formula)

$$
\mathbb E[Z]=\sum_{m=0}^\infty\mathbb P(Z>m).
$$

If each $X_i$ is integer-valued, their product is too. Apply this identity to each factor and to the product, then use [independence](../../../random-variable.md#independent-random-variables):

$$
\boxed{\prod_i\sum_{m\ge0}\mathbb P(X_i>m)=\prod_i\mathbb E[X_i]=\mathbb E\left[\prod_iX_i\right]=\sum_{m\ge0}\mathbb P\left(\prod_iX_i>m\right).}
$$

Under the literal broader meaning of a [discrete random variable](../../../random-variable.md#discrete-random-variable), the second claim is false. Two independent constants $X_1=X_2=3/2$ are positive and discrete, but the left side is $2\cdot2=4$ and the right side is $3$. More generally the integer-indexed tail sum of a positive real-valued variable is $\mathbb E\lceil Z\rceil$, not $\mathbb E Z$. This is the [integer-valued hypothesis in the tail-sum formula](../../../probability-theory.md#integer-valued-hypothesis-in-the-tail-sum-formula).

## 5B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

For $c\ne0$ and on an interval where $x\ne0$, the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) substitution gives

$$
y'=\frac{x''}{cx}-\frac{x'^2}{cx^2},\qquad cy^2=\frac{x'^2}{cx^2}.
$$

The quadratic terms cancel. Multiplying by $cx$ gives the [linearization of a Riccati equation](../../../analysis.md#linearization-of-a-riccati-equation):

$$
\boxed{x''+a(t)x'+cb(t)x=0.}
$$

Multiplying $x$ by a nonzero constant leaves $y$ unchanged. If $c=0$, that substitution is undefined, but the original equation is already a first-order [linear ordinary differential equation](../../../differential-equation.md#linear-ordinary-differential-equation), solvable by an [integrating factor](../../../differential-equation.md#integrating-factor).

For the particular equation, $c=1$ and the linear equation is $x''+x'/t-\lambda^2x/t^2=0$. Use the PDF's logarithmic coordinate $\tau=\log t$ and write $X(\tau)=x(e^\tau)$. The [chain rule](../../../calculus.md#chain-rule) gives $x'=X'/t$ and $x''=(X''-X')/t^2$, leaving $X''-\lambda^2X=0$. Thus $x=A t^\lambda+B t^{-\lambda}$, as also follows from the [Euler-Cauchy equation](../../../differential-equation.md#euler-cauchy-equation). Recovering the [Riccati equation](../../../analysis.md#riccati-equation) solution yields

$$
y(t)=\frac\lambda t\frac{A t^{2\lambda}-B}{A t^{2\lambda}+B}.
$$

The initial value imposes $A=-3B$; choose $A=3,B=-1$. Therefore

$$
\boxed{y(t)=\frac\lambda t\frac{3t^{2\lambda}+1}{3t^{2\lambda}-1},\qquad t_*=3^{-1/(2\lambda)}.}
$$

The denominator vanishes only at $t_*>0$, and its numerator is then nonzero. This is a simple pole: $y(t)\sim1/(t-t_*)$. The maximal interval containing $t=1$ is $(t_*,\infty)$; the same expression on $(0,t_*)$ is a separate solution branch. These are [poles of a Riccati solution from zeros of its linearizing solution](../../../analysis.md#poles-of-a-riccati-solution-from-zeros-of-its-linearizing-solution).

## 6B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6b/i">i</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/i/solution">Solution</h4>

↑ **Parent:** [I](#6b/i)

Linearize about rest and a flat surface. An appropriate small-amplitude scaling has $|\zeta|/h\ll1$ and $|u|/\sqrt{gh}\ll1$, with gradients on fixed common length/time scales. Products such as $(\zeta u)_x$ and $uu_x$ are then higher order. The [linearized shallow water equations](../../../physics.md#linearized-shallow-water-equations) become

$$
\zeta_t+hu_x=0,\qquad u_t+g\zeta_x=0.
$$

Differentiate the first with respect to time and substitute the second:

$$
\boxed{\zeta_{tt}=gh\,\zeta_{xx},\qquad c=\sqrt{gh}.}
$$

The [shallow-water dispersion relation](../../../physics.md#shallow-water-dispersion-relation) therefore has a constant wave speed. In these equations $g$ is gravitational [acceleration](../../../classical-mechanics.md#acceleration), despite the source's label “gravitational constant”; $gh$ has units of speed squared.

<h3 id="6b/ii">ii</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6b/ii)

In the characteristic coordinates, the [chain rule](../../../calculus.md#chain-rule) gives $\partial_x=\partial_\xi+\partial_\eta$ and $\partial_t=c(\partial_\xi-\partial_\eta)$. Hence

$$
\zeta_{tt}-c^2\zeta_{xx}=-4c^2\zeta_{\xi\eta}=0.
$$

Integrating this mixed derivative gives $\zeta=F(\xi)+G(\eta)$, a sum of oppositely traveling profiles. The initial data require $F+G=u_0$ and $c(F'-G')=v_0$, so

$$
F'=\frac12\left(u_0'+\frac{v_0}c\right),\qquad G'=\frac12\left(u_0'-\frac{v_0}c\right).
$$

Integrating the profiles and matching their total additive constant gives the [D'Alembert formula with initial velocity](../../../wave-equation.md#d-alembert-formula-with-initial-velocity):

$$
\boxed{\zeta(x,t)=\frac{u_0(x+ct)+u_0(x-ct)}2+\frac1{2c}\int_{x-ct}^{x+ct}v_0(s)\,ds.}
$$

Here $u_0$ names the initial surface displacement, rather than the water velocity $u$ appearing in the original [shallow water equations](../../../physics.md#shallow-water-equations). The formula verifies both initial conditions directly.

<h3 id="6b/iii">iii</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6b/iii)

With zero initial time derivative, the integral term in the [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula) vanishes. The [Heaviside step function](../../../analysis.md#heaviside-step-function) representation gives

$$
\boxed{\zeta(x,t)=\frac12\big[H(x+ct+1)-H(x+ct-1)+H(x-ct+1)-H(x-ct-1)\big].}
$$

The [rectangular pulse splitting under the wave equation](../../../wave-equation.md#rectangular-pulse-splitting-under-the-wave-equation) consists of **two width-two pulses of height $1/2$, moving left and right at speed $c$**. At $t=0$ they coincide and add to the initial height-one pulse. Before $ct=1$ the overlapping interval has height one; after $ct=1$ the two pulses are separated. Values exactly at the fronts depend on the chosen $H(0)$ convention. Away from the fronts the equation holds classically, and across the fronts it holds as a [weak solution](../../../partial-differential-equation.md#weak-solution) of the [wave equation](../../../wave-equation.md).

## 7B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

Substitute $y_2=vy_1$ and use $y_1''+py_1'+qy_1=0$ to cancel the terms proportional to $v$. The remaining [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) is

$$
\boxed{y_1v''+(2y_1'+py_1)v'=0.}
$$

On an interval where $y_1\ne0$, divide through and put $w=v'$:

$$
w'+\left(2\frac{y_1'}{y_1}+p\right)w=0,\qquad w=C\frac{e^{-\int p(x)\,dx}}{y_1(x)^2}.
$$

Thus [reduction of order](../../../differential-equation.md#reduction-of-order) gives

$$
\boxed{y_2(x)=y_1(x)\int^x\frac{e^{-\int^s p(r)\,dr}}{y_1(s)^2}\,ds.}
$$

A nonzero multiplicative constant gives an independent solution; adding a constant inside the integral adds a multiple of $y_1$. The [Wronskian](../../../differential-equation.md#wronskian) is proportional to $e^{-\int p}$ and is nonzero on the interval. The undivided equation remains meaningful at a zero of $y_1$, but this integral representation then needs continuation rather than direct division.

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

Inspection gives $y_1=x$ in the degree-one [Legendre differential equation](../../../differential-equation.md#legendre-differential-equation). After division by $1-x^2$, $p=-2x/(1-x^2)$ and $e^{-\int p}=1/(1-x^2)$. On either side of zero, [reduction of order](../../../differential-equation.md#reduction-of-order) therefore gives

$$
v'=\frac1{x^2(1-x^2)}=\frac1{x^2}+\frac1{1-x^2},\qquad v=-\frac1x+\operatorname{arctanh}x.
$$

A second solution is $y_2=x\operatorname{arctanh}x-1$. Although $v$ is singular at zero, the product $vy_1$ has a smooth continuation throughout $(-1,1)$. This illustrates [reduction of order across a zero of the known solution](../../../differential-equation.md#reduction-of-order-across-a-zero-of-the-known-solution). Since $y_1(0)=0$, $y_1'(0)=1$, $y_2(0)=-1$ and $y_2'(0)=0$, the required coefficients are $1,-1$. Hence

$$
\boxed{y(x)=1+x-x\operatorname{arctanh}x=1+x-\frac x2\log\frac{1+x}{1-x},\qquad -1<x<1.}
$$

The [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) has regular coefficients near zero, so the resulting initial-value solution is unique and the removable singularity in the intermediate representation causes no ambiguity.

## 8B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8b/i">i</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/i/solution">Solution</h4>

↑ **Parent:** [I](#8b/i)

Differentiate the [mechanical energy](../../../classical-mechanics.md#mechanical-energy) and use the [damped pendulum](../../../classical-mechanics.md#damped-pendulum) equation:

$$
\boxed{\frac{dE}{dt}=\dot\theta(\ddot\theta+\sin\theta)=-c\dot\theta^2\leq0.}
$$

The [energy dissipation of a damped pendulum](../../../classical-mechanics.md#energy-dissipation-of-a-damped-pendulum) makes $E$ nonincreasing, rather than strictly decreasing at every instant: its derivative vanishes at turning points. It is constant along an equilibrium trajectory. Along every nonstationary trajectory it strictly decreases over any nonzero time interval, because a vanishing integral of $c\dot\theta^2$ over an interval would force an equilibrium there and hence everywhere by uniqueness.

<h3 id="8b/ii">ii</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8b/ii)

The [small-angle approximation](../../../geometry-and-topology.md#small-angle-approximation) replaces $\sin\theta$ by $\theta$, giving the [damped harmonic oscillator](../../../analysis.md#damped-harmonic-oscillator) equation $\ddot\theta+c\dot\theta+\theta=0$. Its [characteristic roots](../../../differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) satisfy $r^2+cr+1=0$.

For **$0<c<2$**, put $\nu=\sqrt{1-c^2/4}$; the motion is underdamped:

$$
\boxed{\theta(t)\simeq e^{-ct/2}[A\cos(\nu t)+B\sin(\nu t)].}
$$

It oscillates with decaying amplitude. For **$c=2$**, the repeated root gives [critical damping](../../../wave-equation.md#critical-damping):

$$
\boxed{\theta(t)\simeq(A+Bt)e^{-t}.}
$$

For **$c>2$**, the motion is overdamped:

$$
\boxed{\theta(t)\simeq A e^{(-c+\sqrt{c^2-4})t/2}+B e^{(-c-\sqrt{c^2-4})t/2}.}
$$

Both real exponents are negative, so there is no oscillatory factor. The two constants are arbitrary in each case; these approximations require the displacement to remain small.

<h3 id="8b/iii">iii</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8b/iii)

The [phase plane](../../../dynamical-systems.md#phase-plane) system is $\dot x=y$, $\dot y=-cy-\sin x$. Its [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are **$(k\pi,0)$ for every integer $k$**. At such a point the [Jacobian matrix](../../../calculus.md#jacobian-matrix) and characteristic equation are

$$
J=\begin{pmatrix}0&1\\-(-1)^k&-c\end{pmatrix},\qquad r^2+cr+(-1)^k=0.
$$

For even $k$, the [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is a **[stable focus](../../../dynamical-systems.md#stable-spiral) for $0<c<2$**, with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $-c/2\pm i\sqrt{1-c^2/4}$; it is a **[stable node](../../../dynamical-systems.md#stable-node) for $c>2$**, with two distinct negative real [eigenvalues](../../../linear-operator-theory.md#eigenvalue). The excluded value $c=2$ gives the repeated critical case.

For odd $k$, the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $(-c\pm\sqrt{c^2+4})/2$. One is positive and one negative, so each is a **[saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium) for every $c>0$**. These classifications follow from the [linearization of a dynamical system](../../../algebra.md#linearization-of-a-dynamical-system), since all the relevant [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have nonzero real part for $c>0$. The even equilibria remain hyperbolic at $c=2$ too, although their [linearization](../../../algebra.md#linearization) then has a repeated eigenvalue; that critical case is excluded from the requested classification.

<h3 id="8b/iv">iv</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#8b/iv)

For $c=1$, the even equilibria are **[stable foci](../../../dynamical-systems.md#stable-spiral)** with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $(-1\pm i\sqrt3)/2$, and the odd equilibria are **[saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium)** with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $r_\pm=(-1\pm\sqrt5)/2$. The local saddle directions are $y=r_\pm[x-(2j+1)\pi]$.

<a id="8b/iv/image-phase-portrait-of-a-pendulum-with-unit-damping-showing-spiral-sinks-and-the-stable-and-unstable-saddle-branches"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2-pendulum-phase.png)

**[Figure 1](#8b/iv/image-phase-portrait-of-a-pendulum-with-unit-damping-showing-spiral-sinks-and-the-stable-and-unstable-saddle-branches). Phase portrait of a pendulum with unit damping, showing spiral sinks and the stable and unstable saddle branches**.

The [phase portrait](../../../dynamical-systems.md#phase-portrait) shows clockwise spiraling into each even equilibrium: on its right-hand horizontal axis, the flow initially points down. The stable [separatrices](../../../dynamical-systems.md#separatrix) of the saddles divide attraction basins on the unwrapped angle axis, while the unstable branches flow into neighboring sinks. Initial conditions with enough [mechanical energy](../../../classical-mechanics.md#mechanical-energy) can cross one or more potential crests before being captured. The curves repeat under $x\mapsto x+2\pi$. They are trajectories, not conservative energy contours: [energy dissipation of a damped pendulum](../../../classical-mechanics.md#energy-dissipation-of-a-damped-pendulum) rules out nonconstant periodic orbits.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/solution">Solution</h3>

↑ **Parent:** [9F](#9f)

A [probability space](../../../probability-theory.md#probability-space) consists of a sample space $\Omega$, a [sigma-algebra](../../../measure-theory.md#sigma-algebra) $\mathcal F$ of events, and a [probability measure](../../../probability-theory.md#probability-measure) $\mathbb P$ satisfying:

- $\mathbb P(A)\geq0$ for every $A\in\mathcal F$.
- $\mathbb P(\Omega)=1$.
- For pairwise disjoint events, $\mathbb P(\bigcup_{j\ge1}A_j)=\sum_{j\ge1}\mathbb P(A_j)$.

For arbitrary events, **[Boole's inequality](../../../probability-inequality.md#boole-s-inequality) is $\mathbb P(\bigcup_jA_j)\leq\sum_j\mathbb P(A_j)$**. To prove it, replace each $A_j$ by $D_j=A_j\setminus\bigcup_{i<j}A_i$. The $D_j$ are disjoint, have the same union, and satisfy $D_j\subseteq A_j$. Countable additivity and monotonicity give $\mathbb P(\bigcup_jA_j)=\sum_j\mathbb P(D_j)\leq\sum_j\mathbb P(A_j)$. Finite unions are included by taking subsequent events empty.

Let $H_i$ be the $i$th heads event. For every $m$, the event of infinitely many heads lies inside $\bigcup_{i\ge m}H_i$. By the [union bound](../../../probability-inequality.md#boole-s-inequality), its probability is at most $\sum_{i\ge m}p_i$, which tends to zero. Thus **the probability of infinitely many heads is $0$**. This is the [First Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-first-lemma), and requires no [independence](../../../random-variable.md#independent-random-variables) of the coin tosses.

For the dice experiment there are $4$ ordered outcomes giving a sum of $5$ and $6$ giving $7$, out of $36$. Each trial therefore has $p_5=1/9$, $p_7=1/6$ and irrelevant-outcome probability $13/18$. By [independence](../../../random-variable.md#independent-random-variables) between trials, summing over the number of initial irrelevant outcomes gives

$$
\boxed{\mathbb P(5\text{ before }7)=\sum_{k\ge0}\left(\frac{13}{18}\right)^k\frac19=\frac{p_5}{p_5+p_7}=\frac25.}
$$

The geometric series also shows that one of the two relevant sums eventually appears almost surely. Equivalently, [first-step analysis](../../../analysis.md#first-step-analysis) gives $p=p_5+(13/18)p$.

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

For $\lambda\geq0$, a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has mass $\mathbb P(X=k)=e^{-\lambda}\lambda^k/k!$ for $k=0,1,\ldots$; at $\lambda=0$ it is concentrated at zero. Its [moment-generating function](../../../probability-theory.md#moment-generating-function) is

$$
\boxed{M_X(s)=\sum_{k\ge0}e^{sk}e^{-\lambda}\frac{\lambda^k}{k!}=\exp[\lambda(e^s-1)],\qquad s\in\mathbb R.}
$$

For independent $X,Y$, the [moment-generating function](../../../probability-theory.md#moment-generating-function) of their sum is the product, $\exp[(\lambda+\mu)(e^s-1)]$. Uniqueness of the [moment-generating function](../../../probability-theory.md#moment-generating-function) near zero therefore gives **$X+Y\sim\operatorname{Poisson}(\lambda+\mu)$**. Repeating the argument gives **$S_n=\sum_{i=1}^nX_i\sim\operatorname{Poisson}(n)$** when every parameter is one.

The displayed sequence is $a_n=\mathbb P(S_n\leq n)$. The classical [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) states that independent identically distributed variables with finite mean $m$ and nonzero finite [variance](../../../variance.md) $\sigma^2$ have standardized sum $(S_n-nm)/(\sigma\sqrt n)$ converging in distribution to the standard [normal distribution](../../../probability-theory.md#normal-distribution). Here $m=\sigma^2=1$, so

$$
\boxed{a_n=\mathbb P\left(\frac{S_n-n}{\sqrt n}\leq0\right)\longrightarrow\Phi(0)=\frac12.}
$$

Convergence of the distribution functions at the continuity point zero justifies the last step. This is the [Poisson cumulative probability at its growing mean](../../../discrete-probability-distribution.md#poisson-cumulative-probability-at-its-growing-mean).

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

Assume $\mathbb E|g(X)|<\infty$, or use nonnegative $g$ with extended expectations. Let $p_{ij}=\mathbb P(X=x_i,Y=y_j)$ and $p_j=\mathbb P(Y=y_j)$. For $p_j>0$, the discrete [conditional expectation](../../../measure-theory.md#conditional-expectation) is $\mathbb E[g(X)\mid Y=y_j]=\sum_i g(x_i)p_{ij}/p_j$. Therefore [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem), or [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) in the nonnegative case, gives the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation):

$$
\boxed{\mathbb E[\mathbb E[g(X)\mid Y]]=\sum_{j:p_j>0}\sum_i g(x_i)p_{ij}=\sum_i g(x_i)\mathbb P(X=x_i)=\mathbb E[g(X)].}
$$

Values of a [conditional expectation](../../../measure-theory.md#conditional-expectation) on zero-probability conditioning events do not affect the sum. An unrestricted signed $g$ whose expectation is undefined is outside this assertion.

Write $M(x)=\mathbb E[N(x)]$. The waiting time for two increments larger than $1/2$ dominates $N(x)$ for $0\leq x\leq1$ and has mean $4$, so $M$ is finite. Conditioning on the first increment, one step is always consumed; if that increment is below $x$, the remaining independent sequence has the original law. Thus [first-step analysis](../../../analysis.md#first-step-analysis) and the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) give

$$
M(x)=1+\int_0^xM(x-u)\,du=1+\int_0^xM(s)\,ds.
$$

This first makes $M$ continuous and then gives $M'=M$, with $M(0)=1$. Hence the [uniform-sum crossing time below one](../../../probability-theory.md#uniform-sum-crossing-time-below-one) has

$$
\boxed{\mathbb E[N(x)]=e^x,\qquad 0\leq x\leq1.}
$$

An independent explanation uses the [tail-sum formula](../../../probability-theory.md#tail-sum-formula): $\mathbb P(N(x)>n)=\mathbb P(U_1+\cdots+U_n\leq x)=x^n/n!$ for $x\leq1$, since this region is an $n$-dimensional simplex inside the unit cube. Summing from $n=0$ gives $e^x$. In particular the strict-crossing convention gives $N(0)=1$ almost surely and $\mathbb E N(1)=e$.

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

An [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\lambda>0$ has density $f_X(x)=\lambda e^{-\lambda x}$ for $x\geq0$ and zero for $x<0$, with survival probability $\mathbb P(X>x)=e^{-\lambda x}$. For $s,t\geq0$, its [memoryless property](../../../continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution) follows from

$$
\boxed{\mathbb P(X>s+t\mid X>s)=\frac{e^{-\lambda(s+t)}}{e^{-\lambda s}}=e^{-\lambda t}=\mathbb P(X>t).}
$$

For the minimum, [independence](../../../random-variable.md#independent-random-variables) gives $\mathbb P(Z>z)=\mathbb P(X>z)\mathbb P(Y>z)=e^{-2\lambda z}$. Hence

$$
\boxed{f_Z(z)=2\lambda e^{-2\lambda z}\quad(z\geq0),\qquad \mathbb P(X>Y)=\frac12.}
$$

The density is zero for negative $z$. The comparison probability follows from identical continuous laws and zero tie probability; directly it is $\int_0^\infty\lambda e^{-2\lambda y}dy=1/2$. These are [competing exponential clocks](../../../continuous-probability-distribution.md#competing-exponential-clocks).

For the last density, substitute $y=s^2$ into the normalizing integral to obtain $C=2\int_0^\infty e^{-s^2}ds=\sqrt\pi$, the [Gaussian integral](../../../calculus.md#gaussian-integral). Equivalently, each variable has a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $1/2$ and rate one. [Independence](../../../random-variable.md#independent-random-variables) permits [convolution](../../../fourier-analysis.md#convolution) of the densities. For $z>0$,

$$
f_{G_1+G_2}(z)=\frac{e^{-z}}{C^2}\int_0^z\frac{dy}{\sqrt{y(z-y)}}.
$$

Putting $y=z\sin^2\theta$ turns the integral into $2\int_0^{\pi/2}d\theta=\pi$. Consequently

$$
\boxed{f_{G_1+G_2}(z)=e^{-z}\quad(z\geq0),\qquad G_1+G_2\sim\operatorname{Exp}(1).}
$$

This is also the [additivity of independent gamma distributions with a common rate](../../../continuous-probability-distribution.md#additivity-of-independent-gamma-distributions-with-a-common-rate): their shapes add to one. Density values at the single endpoint zero are immaterial.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
