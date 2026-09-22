<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [slotted ALOHA](../../../../../slotted-aloha.md) model with one outstanding packet per active station and a collision channel: a slot with exactly one attempt succeeds, whereas an idle slot or a slot with two or more attempts delivers nothing. Let $Y_t$ be independent [Poisson random variables](../../../../../poisson-distribution.md) of mean $\nu$, independent also of the transmission choices. Arrivals join after the current slot's attempts. Given $(S_t,N_t)=(S,N)$, the attempt count has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $N$ and $1/S$. Consequently, for $N\geq1$,

$$
p_0(N,S)=(1-1/S)^N,\qquad
p_1(N,S)=\frac NS(1-1/S)^{N-1},\qquad p_*=1-p_0-p_1.
$$

For $N=0$, set $p_0=1$ and $p_1=0$. The equation $N_{t+1}=N_t+Y_t-\mathbf1_{\{Z_t=1\}}$ adds arrivals and removes precisely one packet following a successful slot. The estimate $S_t\geq1$ controls the common transmission probability and updates using the idle, success, or collision feedback. The [conditional distribution](../../../../../conditional-distribution.md) of the next state depends only on $(S_t,N_t)$, so this pair is a [Markov chain](../../../../../markov-chain.md).

Away from the reflecting floor in $S$, its one-step [conditional expectations](../../../../../conditional-expectation.md) are

$$
\mathbb E[\Delta N\mid S,N]=\nu-p_1,
\qquad\mathbb E[\Delta S\mid S,N]=ap_0+bp_1+cp_*.
$$

When $N$ and $S$ are large with $N/S\approx\kappa$, the [Poisson limit theorem](../../../../../poisson-limit-theorem.md) gives $p_0\approx e^{-\kappa}$ and $p_1\approx\kappa e^{-\kappa}$. Treating these approximate drifts as derivatives motivates the [fluid approximation of slotted ALOHA](../../../../../fluid-approximation-of-slotted-aloha.md):

$$
\boxed{\dot s=(a-c)e^{-\kappa}+(b-c)\kappa e^{-\kappa}+c,\qquad
\dot n=\nu-\kappa e^{-\kappa},\qquad\kappa=n/s.}
$$

The floor at $S=1$ is negligible in this interior scaling. This calculation motivates the [ordinary differential equations](../../../../../ordinary-differential-equation.md); it is not a proof of a stochastic [fluid limit](../../../../../fluid-limit.md).

For $(a,b,c)=(2-e,0,1)$, put

$$
g(\kappa)=1-(e-1+\kappa)e^{-\kappa},\qquad
h(\kappa)=\nu-\kappa e^{-\kappa}.
$$

Then $g'(\kappa)=(e-2+\kappa)e^{-\kappa}>0$ and $g(1)=0$. On the domain $s>0$, introduce time $\tau$ by $d\tau/dt=1/s$. Differentiating $\kappa=n/s$ gives

$$
\frac{d\kappa}{d\tau}=\nu-r(\kappa),\qquad
\frac{ds}{d\tau}=s\,g(\kappa),\qquad
\frac{dt}{d\tau}=s,
$$

where $r(\kappa)=\kappa[1-(e-2+\kappa)e^{-\kappa}]$.

The function $r$ is strictly increasing from zero to infinity, and $r(1)=e^{-1}$. To check the monotonicity explicitly,

$$
r'(\kappa)=1-e^{-\kappa}\bigl[e-2+(4-e)\kappa-\kappa^2\bigr]>0.
$$

Indeed, with $d=3-e\in(0,1)$,

$$
1+\kappa-\bigl[e-2+(4-e)\kappa-\kappa^2\bigr]
=\kappa^2-d\kappa+d>0,
$$

because its discriminant is $d^2-4d<0$; and $e^\kappa\geq1+\kappa$. Thus the scalar [ordinary differential equation](../../../../../ordinary-differential-equation.md) for $\kappa$ points toward the unique value $\kappa_*$ satisfying $r(\kappa_*)=\nu$. Every trajectory with $s(0)>0$, $n(0)\geq0$ has bounded $\kappa$ and $\kappa(\tau)\to\kappa_*$. Positivity of $s$ follows from $s(\tau)=s(0)\exp(\int_0^\tau g(\kappa(u))\,du)$.

If $0\leq\nu<e^{-1}$, then $\kappa_*<1$ and $g(\kappa_*)<0$. Thus $s(\tau)$ decays exponentially for large $\tau$, and

$$
T=\int_0^\infty s(\tau)\,d\tau<\infty,\qquad
\boxed{(s(t),n(t))\longrightarrow(0,0)\quad\text{as }t\uparrow T.}
$$

This is [finite-time draining of a fluid model](../../../../../finite-time-draining-of-a-fluid-model.md). The unmodified equations have $n/s$ undefined at the origin, so the statement that trajectories converge to the origin needs this endpoint interpretation; continuing with an absorbing zero trajectory is an additional fluid-model convention, not a solution of the displayed equations at the origin.

If $\nu>e^{-1}$, then $\kappa_*>1$ and $g(\kappa_*)>0$. Now $s(\tau)$ grows exponentially, physical time tends to infinity, and

$$
\boxed{\frac{s(t)}t\to g(\kappa_*),\qquad
\frac{n(t)}t\to\kappa_*g(\kappa_*)>0.}
$$

In particular the trajectory escapes to infinity. Even without the ratio analysis, $\dot n\geq\nu-e^{-1}>0$, since $\max_{\kappa\geq0}\kappa e^{-\kappa}=e^{-1}$.

For the actual [Markov chain](../../../../../markov-chain.md), it is essential not to replace the finite-$N$ success probability by $e^{-1}$: a single backlogged packet can succeed with probability one. Instead, for $N\geq2$, maximizing over $S\geq1$ gives the [ALOHA throughput bound](../../../../../aloha-throughput-bound.md)

$$
p_1(N,S)\leq\left(1-\frac1N\right)^{N-1}\longrightarrow e^{-1}.
$$

If $\nu>e^{-1}$, choose $K_0$ and $r_0<\nu$ so that $p_1(N,S)\leq r_0$ for all $N>K_0$, uniformly in $S$. For sufficiently small $\theta>0$,

$$
q_\theta:=\exp\bigl(\nu(e^{-\theta}-1)\bigr)
\bigl[1+r_0(e^\theta-1)\bigr]<1,
$$

because its derivative at zero is $r_0-\nu<0$. Independence of arrivals and attempts gives

$$
\mathbb E[e^{-\theta\Delta N}\mid S,N]
=\exp\bigl(\nu(e^{-\theta}-1)\bigr)
\bigl[1+p_1(N,S)(e^\theta-1)\bigr]\leq q_\theta
$$

whenever $N>K_0$. For any integer $K\geq K_0$, stop at the [stopping time](../../../../../stopping-time.md) $\sigma_K=\inf\{t:N_t\leq K\}$. The stopped process $e^{-\theta N_{t\wedge\sigma_K}}$ is a nonnegative [supermartingale](../../../../../supermartingale.md). The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md), first at bounded times and then by a limit, yields the [exponential-supermartingale escape bound](../../../../../exponential-supermartingale-escape-bound.md)

$$
\boxed{\mathbb P_{S,N}(\sigma_K<\infty)\leq e^{-\theta(N-K)}\qquad(N>K).}
$$

From every state with $N\leq K$, a [Poisson distribution](../../../../../poisson-distribution.md) arrival burst has a uniformly positive probability of sending the next backlog to at least $K+m$, for any fixed $m>0$. From there the probability of never revisiting $N\leq K$ is at least $1-e^{-\theta m}$. By the [Markov property](../../../../../markov-property.md) at successive visits, the probability of infinitely many visits to this strip is zero: each visit has a uniform positive chance of being the last. This holds for every integer $K\geq K_0$, so

$$
\boxed{N_t\to\infty\quad\text{almost surely when }\nu>e^{-1}.}
$$

Therefore **the [Markov chain](../../../../../markov-chain.md) is transient for every finite choice of $a,b,c$**. The proof is uniform in $S$ and does not infer stochastic transience merely from the approximate [ordinary differential equations](../../../../../ordinary-differential-equation.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
