<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the [slotted ALOHA](../../../../../slotted-aloha.md) model, a station retains one packet until it successfully transmits. Conditional on $(S_t,N_t)=(S,N)$, take fresh independent trials with a [Bernoulli distribution](../../../../../bernoulli-distribution.md) of parameter $1/S$ for the $N$ backlogged stations. Let arrivals be independent across slots and independent of these trials, with [Poisson distribution](../../../../../poisson-distribution.md) of mean $\nu$. New arrivals join the next slot's backlog. An idle slot serves nobody, exactly one attempt serves one packet, and a collision serves nobody. Consequently the backlog changes by arrivals minus the success indicator.

Under these [independence](../../../../../independent-random-variables.md) assumptions, **$(S_t,N_t)$ is a time-homogeneous [Markov chain](../../../../../markov-chain.md)**: the feedback [probabilities](../../../../../probability.md) and the independent arrival law depend only on its current state. Merely specifying Poisson arrival marginals would not suffice. For example, take $S_t=1$, $a=b=c=0$, $N_0=0$, and arrivals $Y_0=H$, $Y_1=K$, $Y_2=H$ for [independent random variables](../../../../../independent-random-variables.md) $H,K$ with [Poisson distributions](../../../../../poisson-distribution.md). Histories with $(N_1,N_2)=(0,2)$ and $(2,2)$ both have current backlog two, but the next backlog is respectively two and four. The usual model therefore includes fresh arrivals as an assumption.

Write $p_0=(1-1/S)^N$ and $p_1=(N/S)(1-1/S)^{N-1}$. Set $p_1=0$ for $N=0$, and use their exact [binomial distribution](../../../../../binomial-distribution.md) [probabilities](../../../../../probability.md) at $S=1$. Away from the clipping boundary, the conditional drifts are

$$
\mathbb E[\Delta N\mid S,N]=\nu-p_1,\qquad
\mathbb E[\Delta S\mid S,N]=ap_0+bp_1+c(1-p_0-p_1).
$$

Near $S=1$, the latter must use $\max(1,S+d)-S$ for each update $d$, rather than $d$ itself.

When both coordinates are large with $N/S\to\kappa$, the [Poisson limit theorem](../../../../../poisson-limit-theorem.md) approximates the attempt count, which has a [binomial distribution](../../../../../binomial-distribution.md), by a [Poisson distribution](../../../../../poisson-distribution.md) of mean $\kappa$. Thus $p_0\to e^{-\kappa}$ and $p_1\to\kappa e^{-\kappa}$. Rescaling state by $K$ and slot time by $K$ motivates the [fluid approximation of slotted ALOHA](../../../../../fluid-approximation-of-slotted-aloha.md)

$$
\dot s=g(\kappa)=(a-c)e^{-\kappa}+(b-c)\kappa e^{-\kappa}+c,\qquad
\dot n=f(\kappa)=\nu-\kappa e^{-\kappa},\qquad\kappa=n/s.
$$

This is an interior [fluid approximation of slotted ALOHA](../../../../../fluid-approximation-of-slotted-aloha.md), not the exact conditional drift at a clipped boundary.

Here is one explicit set of sufficient conditions, independent of the arrival rate within the subcritical range:

$$
\boxed{a=b=-A,\qquad c=\frac{2A}{e-2},\qquad A\geq1,\qquad0\leq\nu<e^{-1}}.
$$

Put $c_0=2/(e-2)$. Then

$$
g(\kappa)=A\{c_0-(1+c_0)(1+\kappa)e^{-\kappa}\},\quad
g(1)=0,\quad g'(\kappa)=A(1+c_0)\kappa e^{-\kappa}>0\ (\kappa>0).
$$

Hence $g$ is negative below one and positive above one: the controller decreases the attempt denominator when offered contention is too small, and increases it when contention is too large.

Use the [ratio time change for a homogeneous fluid model](../../../../../ratio-time-change-for-a-homogeneous-fluid-model.md), $du/dt=1/s$. The equations become

$$
\frac{d\kappa}{du}=h(\kappa):=f(\kappa)-\kappa g(\kappa),\qquad
\frac{d\log s}{du}=g(\kappa).
$$

For $\kappa\geq1$,

$$
h'(\kappa)=e^{-\kappa}(\kappa-1)-g(\kappa)-A(1+c_0)\kappa^2e^{-\kappa}<0,
$$

since $g(\kappa)\geq0$ and $A(1+c_0)>1$. Also $h(1)=\nu-e^{-1}<0$. Therefore $h$ is negative on $[1,\infty)$, and by continuity on $[\bar\kappa,\infty)$ for some $\bar\kappa<1$. Its value at zero is $\nu\geq0$, so nonnegative backlog is preserved.

The ratio remains bounded by $K=\max(\kappa(0),1)$ and eventually enters $[0,\bar\kappa]$: on the compact interval $[\bar\kappa,K]$, its [derivative](../../../../../derivative.md) is bounded above by a strictly negative number. Once inside it cannot cross upward. The bounded ratio and smooth coefficients make the transformed equations exist for all $u\geq0$. In this region $g(\kappa)\leq g(\bar\kappa)<0$, so $s(u)$ decreases at least exponentially in $u$. The original time satisfies $t(u)=\int_0^u s(v)\,dv$ and has a finite limit $T$; boundedness of $\kappa$ gives $n(u)=\kappa(u)s(u)\to0$ as well. Thus **every nonnegative interior fluid trajectory drains to the origin in finite fluid time**. At the origin the ratio equation is undefined; the usual stopped fluid trajectory is held there afterward. A state with $s=0<n$ enters the interior under the continuous limiting boundary drift $\dot s=c>0$; the same argument then applies.

This proof supplies sufficient conditions, not a characterization of every stabilizing triplet. It also does not assert the [positive recurrent Markov chain](../../../../../positive-recurrent-markov-chain.md) property of the original stochastic chain solely from the heuristic ODE.

If $\nu>e^{-1}$, the [ALOHA throughput bound](../../../../../aloha-throughput-bound.md) gives

$$
\boxed{\dot n\geq\nu-e^{-1}>0,\qquad n(t)\geq n(0)+(\nu-e^{-1})t}.
$$

No choice of the three feedback increments can make this fluid backlog drain, since $\max_{\kappa\geq0}\kappa e^{-\kappa}=e^{-1}$. For the displayed controller, the supercritical fluid trajectory is global and grows instead of draining. At $\nu=e^{-1}$ the ray $n=s>0$ consists of stationary fluid states, explaining why the strict load inequality matters.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
