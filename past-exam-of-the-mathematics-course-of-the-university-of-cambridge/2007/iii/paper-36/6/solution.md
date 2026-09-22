<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Markov jump process](../../../../../markov-jump-process.md) relative to $(\mathcal F_t)$ is an adapted [càdlàg](../../../../../cadlag.md) process with piecewise-constant paths and finitely many jumps on each bounded time interval, whose conditional future law given $\mathcal F_t$ depends only on its current state. For a time-homogeneous process on a countable state space, write $q(x,y)\ge0$ for its transition rates and $q(x)=\sum_{y\ne x}q(x,y)<\infty$. In state $x$, the holding time is exponential of rate $q(x)$ and the next state is $y$ with probability $q(x,y)/q(x)$; a zero rate makes the state absorbing. The generator is $\mathcal Af(x)=\sum_{y\ne x}q(x,y)(f(y)-f(x))$. Nonexplosion is included here so that the process is defined at every finite time.

Here is a finite-jump, bounded-rate form of the [Kurtz fluid limit theorem](../../../../../kurtz-fluid-limit-theorem.md). For each $N$, let $Z^N$ be a chain on a countable state space $E_N\subseteq\mathbb R^d$ with jumps $\ell/N$ at rates $N\beta_\ell(z)$, with $\ell$ in a fixed finite subset $\mathcal J\subset\mathbb R^d$. Assume the nonnegative $\beta_\ell$ are uniformly bounded, admissible jumps remain in the state space, and

$$
F(z)=\sum_{\ell\in\mathcal J}\ell\beta_\ell(z)
$$

is globally Lipschitz with constant $L$. Suppose $Z_0^N\to z_0$ in probability, and let $z$ solve $\dot z=F(z)$, $z(0)=z_0$. Then for every finite $T$,

$$
\boxed{\sup_{0\le t\le T}|Z_t^N-z(t)|\longrightarrow0\quad\text{in probability}.}
$$

Bounded total jump rates ensure nonexplosion; the globally Lipschitz drift gives a unique global ODE solution. These explicit hypotheses suffice for the population example, without needing a more general local version of the theorem.

To prove the result, compensate the jumps of this [density-dependent Markov jump process](../../../../../density-dependent-markov-jump-process.md). The drift and the coordinate [martingales](../../../../../martingale-split.md) satisfy

$$
Z_t^N=Z_0^N+\int_0^tF(Z_s^N)\,ds+M_t^N,\qquad\langle M^{N,i}\rangle_t=\frac1N\int_0^t\sum_\ell\ell_i^2\beta_\ell(Z_s^N)\,ds.
$$

Here $\langle M^{N,i}\rangle$ is [predictable quadratic variation](../../../../../predictable-quadratic-variation.md), not the sum of realized squared jumps. The compensation identity follows because each possible increment $\ell/N$ has intensity $N\beta_\ell$, and its squared coordinate increment contributes $\ell_i^2\beta_\ell/N$ per unit time. Bounded rates and jump sizes make these [martingales](../../../../../martingale-split.md) square-integrable.

We use the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) in the explicit form $\mathbb E\sup_{s\le T}|M_s|^2\le4\mathbb E|M_T|^2$ for a scalar square-integrable [martingale](../../../../../martingale-split.md) starting at zero. Applying it coordinatewise and setting $K=\sup_z\sum_\ell|\ell|^2\beta_\ell(z)<\infty$ gives

$$
\mathbb E\sup_{s\le T}|M_s^N|^2\le\sum_i\mathbb E\sup_{s\le T}|M_s^{N,i}|^2\le\frac{4KT}{N}.
$$

Subtract the ODE integral equation. Lipschitz continuity and [Gronwall's inequality](../../../../../gronwall-inequality.md) yield

$$
\sup_{s\le T}|Z_s^N-z(s)|\le e^{LT}\left(|Z_0^N-z_0|+\sup_{s\le T}|M_s^N|\right).
$$

The first term tends to zero in probability by hypothesis, and the second by its maximal second-moment estimate. More quantitatively, for $\delta>0$,

$$
\mathbb P\left(\sup_{s\le T}|Z_s^N-z(s)|>\delta\right)\le\mathbb P\left(|Z_0^N-z_0|>\tfrac12\delta e^{-LT}\right)+\frac{16KT e^{2LT}}{N\delta^2}.
$$

This proves the stated uniform finite-horizon [fluid limit](../../../../../fluid-limit.md).

For the cells, division replaces one cell by two and increases population by one. At population $k\le N$, the total rate is the sum of the $k$ identical cell rates, namely

$$
q_N(k,k+1)=k(1-k/N).
$$

The state $N$ is absorbing. Set $Z_t^N=\xi_t/N$; its jump is $1/N$ with rate $N\beta(z)$, where $\beta(z)=z(1-z)$ on $[0,1]$. Extending this function by zero outside $[0,1]$ makes it bounded, nonnegative and globally Lipschitz, with Lipschitz constant one. Starting from $Z_0^N=p$, or from $\lfloor pN\rfloor/N$ when integer rounding is necessary, the limiting ODE is the [logistic differential equation](../../../../../logistic-differential-equation.md)

$$
\dot z=z(1-z),\qquad z(0)=p.
$$

Separation of variables, or differentiating $z/(1-z)$, gives its solution. The [logistic cell-division process](../../../../../logistic-cell-division-process.md) therefore satisfies

$$
\boxed{z(t)=\frac{pe^t}{1-p+pe^t},\qquad\sup_{s\le T}\left|\frac{\xi_s}{N}-\frac{pe^s}{1-p+pe^s}\right|\longrightarrow0\ \text{in probability for every finite }T.}
$$

Here $K\le1/4$, so the maximal [martingale](../../../../../martingale-split.md) second moment is at most $T/N$. With exact initial density $p$, the preceding pathwise bound even gives $\mathbb E\sup_{s\le T}|Z_s^N-z(s)|^2\le Te^{2T}/N$. With integer rounding, the bound $\mathbb E\sup_{s\le T}|Z_s^N-z(s)|^2\le2e^{2T}(T/N+1/N^2)$ follows from $|Z_0^N-p|\le1/N$ and $(a+b)^2\le2a^2+2b^2$. Thus the deterministic logistic curve approximates the density with fluctuations of order $N^{-1/2}$ on fixed time intervals. The convergence statement is on finite horizons; it does not interchange the limits $t\to\infty$ and $N\to\infty$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
