# Paper 356

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_356.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_356.pdf)

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
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
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

## 1

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $w_{ij}$ be the transition rate from $i$ to $j$ and define the probability current $J_{ij}=w_{ij}P_i-w_{ji}P_j=-J_{ji}$. The [master equation](../../../markov-process.md#master-equation) is $\dot P_i=-\sum_jJ_{ij}$. Differentiating the Shannon entropy $S_{\rm sys}=-\sum_iP_i\log P_i$ and symmetrizing gives

$$
\dot S_{\rm sys}=\frac12\sum_{i,j}J_{ij}\log\frac{P_i}{P_j}.
$$

Adding the entropy flow to the environment produces the nonnegative [entropy production rate of a Markov chain](../../../markov-process.md#entropy-production-rate-of-a-markov-chain)

$$
\boxed{\dot S_{\rm tot}=\frac12\sum_{i,j}J_{ij}
\log\frac{w_{ij}P_i}{w_{ji}P_j}\geq0.}
$$

The paper's displayed $\sum P\log P$ is the negative of the thermodynamic system entropy, so its derivative has the opposite sign before the environmental contribution is added.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the two-state chain,

$$
\boxed{\dot P_1=-\alpha P_1+\beta P_2,
\qquad \dot P_2=\alpha P_1-\beta P_2,}
$$

with $P_1+P_2=1$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Eliminating $P_2=1-P_1$ gives $\dot P_1=\beta-(\alpha+\beta)P_1$. Therefore

$$
P_1(t)=\frac\beta{\alpha+\beta}
+\left(p-\frac\beta{\alpha+\beta}\right)e^{-(\alpha+\beta)t}.
$$

With $r=\alpha p-\beta(1-p)$,

$$
\boxed{P_1=\frac{\beta+re^{-(\alpha+\beta)t}}{\alpha+\beta},
\qquad P_2=\frac{\alpha-re^{-(\alpha+\beta)t}}{\alpha+\beta}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The only independent current is

$$
J(t)=\alpha P_1-\beta P_2=re^{-(\alpha+\beta)t}.
$$

Hence the total transient entropy production is

$$
\boxed{\dot S_{\rm tot}=J(t)\log\frac{\alpha P_1(t)}{\beta P_2(t)}\geq0.}
$$

Its relaxational part may be written

$$
\dot S_{\rm rel}=J\log\frac{P_1P_2^{\rm ss}}{P_2P_1^{\rm ss}},
\qquad
(P_1^{\rm ss},P_2^{\rm ss})=\frac1{\alpha+\beta}(\beta,\alpha),
$$

while the steady or housekeeping entropy production is zero. Both the current and total production vanish as $t\to\infty$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

At stationarity,

$$
\alpha P_1^{\rm ss}=\frac{\alpha\beta}{\alpha+\beta}
=\beta P_2^{\rm ss}.
$$

**Thus every edge current vanishes and the two-state system satisfies [detailed balance](../../../markov-process.md#detailed-balance). A network containing only one undirected edge cannot sustain a stationary cycle current.**

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

With indices understood cyclically,

$$
\boxed{\dot P_i=\beta P_{i+1}+\alpha P_{i-1}-(\alpha+\beta)P_i.}
$$

The circulant generator has eigenvalues $0$ and $-3\phi\pm i\sqrt3\psi$, where $\phi=(\alpha+\beta)/2$ and $\psi=(\alpha-\beta)/2$. Expanding the initial vector $(1,0,0)$ in its three Fourier eigenvectors gives

$$
\boxed{P_1=\frac13[1+2e^{-3\phi t}\cos(\sqrt3\psi t)],}
$$



$$
\boxed{P_2=\frac13[1-2e^{-3\phi t}\cos(\sqrt3\psi t-\pi/3)],}
$$



$$
\boxed{P_3=\frac13[1-2e^{-3\phi t}\cos(\sqrt3\psi t+\pi/3)].}
$$

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

For the oriented edge $i\to j=i+1\pmod3$, $J_i=\alpha P_i-\beta P_j$. Substitution in the Markov-chain entropy production gives

$$
\dot S_{\rm tot}=\sum_iJ_i\log\frac{\alpha P_i}{\beta P_j}.
$$

Since $\sum_iJ_i=\alpha-\beta$,

$$
\boxed{\dot S_{\rm tot}=(\alpha-\beta)\log\frac\alpha\beta
+\sum_i[\alpha P_i-\beta P_j]\log\frac{P_i}{P_j}.}
$$

The second term is relaxational and vanishes for the uniform stationary distribution. The steady entropy exported to the environment is therefore

$$
\boxed{\dot S_{\rm neq}=(\alpha-\beta)\log(\alpha/\beta)\geq0.}
$$

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

At stationarity $P_i=1/3$, but the cycle current is $J_i=(\alpha-\beta)/3$. Therefore the chain is out of detailed balance exactly when

$$
\boxed{\alpha\ne\beta.}
$$

The nonzero cycle affinity $3\log(\alpha/\beta)$ sustains the stationary current and positive housekeeping entropy production.

## 2

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Equation (1) is [Underdamped Langevin dynamics](../../../stochastic-calculus.md#underdamped-langevin-dynamics) for a unit-mass particle in potential $U$, coupled to a heat bath of temperature $T$. The coefficient $\gamma>0$ is viscous friction, and the noise amplitude is fixed by the [Fluctuation-dissipation theorem](../../../quantum-field-theory.md#fluctuation-dissipation-theorem). Its [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation) is

$$
\boxed{\partial_tf=-v\partial_xf
+\partial_v[(U'(x)+\gamma v)f]
+\gamma k_BT\partial_v^2f.}
$$

For $\gamma\gg1$, velocity relaxes rapidly, so formally

$$
V_tdt\simeq-\frac{U'(X_t)}\gamma dt
+\sqrt{\frac{2k_BT}{\gamma}}dW_t.
$$

Thus the [overdamped Langevin dynamics](../../../stochastic-calculus.md#overdamped-langevin-dynamics) is

$$
dX_t=-\phi'(X_t)dt+\sqrt{2D}\,dW_t,
\qquad D=\frac{k_BT}\gamma,
\qquad \phi=\frac U\gamma,
$$

and its density obeys

$$
\boxed{\partial_tp=\partial_x[D\partial_xp+\phi'(x)p].}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $0\leq F_0<1$, stationary points satisfy $\cos x=F_0$. There is one minimum $m_k=2\pi-\arccos F_0+2\pi k$ and one maximum $M_k=\arccos F_0+2\pi k$ per period. The potential is a sinusoidal washboard tilted downward to the right by $2\pi F_0$ per period.

Periodization partitions the real line into translated cells, so

$$
\int_{M_0}^{M_1}\widehat p(x,t)dx=\int_{\mathbb R}p(x,t)dx=1.
$$

Translation by $2\pi$ merely reindexes the sum, proving periodic boundary conditions; summing the Fokker--Planck equation proves that $\widehat p$ obeys it.

At stationarity the current $J_0=-D\widehat p_s'-\phi'\widehat p_s$ is constant. Solving this first-order equation and imposing periodicity gives

$$
\boxed{\widehat p_s(x)=\frac{J_0u(x)}{D(1-e^{-2\pi F_0/D})},
\qquad
u(x)=e^{-\phi(x)/D}\int_x^{x+2\pi}e^{\phi(y)/D}dy.}
$$

Here $J_0$ is the stationary probability crossing any point per unit time. Normalization determines it:

$$
\boxed{J_0=\frac{D(1-e^{-2\pi F_0/D})}
{\int_{M_0}^{M_1}u(x)dx}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Each net crossing of a periodic cell advances the unwrapped particle by $2\pi$. The stationary mean velocity is therefore

$$
\boxed{v_s=2\pi J_0
=\frac{2\pi D(1-e^{-2\pi F_0/D})}
{\int_{M_0}^{M_1}u(x)dx}.}
$$

For $F_0>0$ the numerator is positive, so motion is on average toward increasing $x$, down the tilted potential.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

In the low-temperature regime, the particle rapidly equilibrates near a minimum and only rarely crosses a neighboring maximum. Applying [Laplace's method](../../../analysis.md#laplace-s-method) to the exact current formula gives the [Kramers escape rates](../../../stochastic-calculus.md#kramers-escape-rate)

$$
k_+=\frac{\sqrt{|\phi''(m_0)\phi''(M_1)|}}{2\pi}e^{-\Delta\phi_+/D},
\qquad
k_-=\frac{\sqrt{|\phi''(m_0)\phi''(M_0)|}}{2\pi}e^{-\Delta\phi_-/D}.
$$

Each right or left escape changes position by $2\pi$, hence

$$
\boxed{v_s\simeq2\pi(k_+-k_-).}
$$

The reduced [continuous-time random walk](../../../markov-process.md#continuous-time-random-walk) on minima has off-diagonal transition rates

$$
\boxed{W(k|l)=k_+\delta_{k,l+1}+k_-\delta_{k,l-1},}
$$

and diagonal generator entry $W(l|l)=-(k_++k_-)$. Its residence time in each well is exponentially distributed with rate $k_++k_-$, and the next jump is right with probability $k_+/(k_++k_-)$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

An exact [Gillespie algorithm](../../../mathematical-biology.md#gillespie-algorithm) for one particle is:

- Set the current well $k$ and time $t=0$.
- If $k$ is absorbing, stop.
- Set $a=k_++k_-$ and draw $\Delta t=-\log U_1/a$.
- Move to $k+1$ if $U_2<k_+/a$, and otherwise to $k-1$.
- Set $t\leftarrow t+\Delta t$ and repeat, stopping if the jump crosses an absorbing end.

For $N\ll K$, simulate particle identities independently and maintain a priority queue of their next event times. For $N\gg K$, store occupation numbers $n_k$ and use aggregate event rates $n_kk_+$ and $n_kk_-$ for each well; one population-level Gillespie event then decrements one $n_k$ and increments its neighbor. This replaces work proportional to particle number by work proportional to the number of occupied wells.

## 3

↑ **Parent:** [Paper 356](paper-356.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The pair $(X_t,V_t)$ is a hybrid-state process: position is continuous and velocity is discrete. It is Markov because its future law is fixed by the present position and velocity. Position $X_t$ alone is generally non-Markovian, since its future displacement depends on the hidden persistent velocity.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The two transport equations are

$$
\partial_tp_+=-s\partial_xp_+-\lambda_+p_++\lambda_-p_-,
$$



$$
\partial_tp_-=s\partial_xp_-+\lambda_+p_+-\lambda_-p_-.
$$

For $p=p_++p_-$ and $j=s(p_+-p_-)$ they become

$$
p_t=-j_x,
\qquad
j_t=-s^2p_x+2sb c'(x)p-2\lambda_0j.
$$

Eliminating $j$ gives the closed [chemotactic telegraph equation](../../../mathematical-biology.md#chemotactic-telegraph-equation)

$$
\boxed{p_{tt}+2\lambda_0p_t=s^2p_{xx}
-2sb\,\partial_x[c'(x)p].}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Take $\lambda_0\to\infty$ with

$$
\boxed{D=\frac{s^2}{2\lambda_0},
\qquad \chi=\frac{sb}{\lambda_0}}
$$

fixed, so $s$ and $b$ scale as $\sqrt{\lambda_0}$. The rapidly relaxing flux satisfies $j\simeq-Dp_x+\chi c'p$, and therefore

$$
\boxed{p_t=\partial_x(Dp_x-\chi pc').}
$$

Zero stationary flux gives $p_s(x)\propto e^{\chi c(x)/D}$. A stationary probability density on $\mathbb R$ exists exactly when this exponential is integrable, in addition to the positivity condition $|c'|<\lambda_0/b$. The limiting process is

$$
\boxed{dX_t=\chi c'(X_t)dt+\sqrt{2D}\,dW_t.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The even pair potential $u$ represents repulsion: because it decreases for positive separation, the force $-u'(x_i-x_j)$ pushes particles apart. Marginalizing the $N$-particle [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation) gives

$$
\boxed{\partial_tp(x_1)=D\partial_{x_1}^2p
-\partial_{x_1}[\chi c'(x_1)p]
+\frac{N-1}{N}\partial_{x_1}
\int u'(x_1-x_2)P_2(x_1,x_2)dx_2.}
$$

Under the [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation), propagation of chaos gives $P_2(x_1,x_2)\simeq p(x_1)p(x_2)$. Taking $N\to\infty$ yields the closed nonlocal equation

$$
\boxed{\partial_tp=\partial_x\left[
D\partial_xp-\chi c'p+p\,\partial_x(u*p)
\right].}
$$

The convolution term is the collective repulsive drift generated by the population density.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
