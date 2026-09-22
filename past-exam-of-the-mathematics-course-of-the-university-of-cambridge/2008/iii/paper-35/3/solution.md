<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [random access network](../../../../../random-access-network.md) shares one communication channel among an unbounded collection of possible transmitters. Each packet occupies one slot; exactly one attempt succeeds, an idle slot carries nothing, and a collision delivers none of its attempted packets. Assume perfect slot synchronization, immediate idle/success/collision feedback, no channel errors, and independent random choices by packets. The important quantities are [throughput](../../../../../throughput.md), the size of the retransmission backlog, and delay. A good one-slot success probability alone does not establish stability of the backlog.

For a precise infinite-population [slotted ALOHA](../../../../../slotted-aloha.md) model, let $A_t$ be independent [Poisson random variables](../../../../../poisson-distribution.md) of mean $\eta>0$, representing new packets which attempt immediately in slot $t$. Let $B_t$ be the backlog before those arrivals. Each old packet independently retries with a constant probability $p\in(0,1)$, so conditional on $B_t=b$, its retry count is $K_t\sim\operatorname{Binomial}(b,p)$, independent of $A_t$. If $D_t=\mathbf1_{\{A_t+K_t=1\}}$ records a successful slot, then

$$
\boxed{B_{t+1}=B_t+A_t-D_t.}
$$

This includes a new packet in the backlog precisely when it has not succeeded; an old packet is removed precisely when it succeeds. The total backlog is a [Markov chain](../../../../../markov-chain.md) in this constant-probability model. Its idle and success probabilities are

$$
\begin{aligned}
I(b)&=e^{-\eta}(1-p)^b,\\
S(b)&=e^{-\eta}\left[\eta(1-p)^b+bp(1-p)^{b-1}\right],\\
\mathbb E[B_{t+1}-B_t\mid B_t=b]&=\eta-S(b),
\end{aligned}
$$

with the second term in $S(0)$ interpreted as zero. A success may be either one new packet and no old attempt, or one old attempt and no new packet.

The [fluid approximation of slotted ALOHA](../../../../../fluid-approximation-of-slotted-aloha.md) replaces the binomial retry count by a Poisson count when there are many packets with small retry probability. If $g=\eta+bp$ is total attempt intensity, the approximate success probability is $ge^{-g}$. Differentiation gives

$$
\frac{d}{dg}(ge^{-g})=(1-g)e^{-g},\qquad \boxed{\max_{g\ge0}ge^{-g}=e^{-1}\text{ at }g=1.}
$$

This is the limiting [ALOHA throughput bound](../../../../../aloha-throughput-bound.md), not an exact upper bound for every finite packet population: one isolated packet which certainly transmits succeeds with probability one. In a [fluid model](../../../../../fluid-model.md), when $0<\eta<e^{-1}$ the equation $\eta=ge^{-g}$ has two roots. The root below one is locally stable for constant $p$, while the root above one is unstable, because the drift derivative is $-p(1-g)e^{-g}$. These approximations explain a low-backlog operating region and a congestion threshold; they do not imply a stationary law for the infinite-population chain.

Indeed, for fixed $p>0$, the exact success probability $S(b)$ tends to zero as $b\to\infty$, so the exact drift tends to $\eta>0$. One can prove instability, rather than relying only on this positive drift. Fix $\theta>0$ and use $V(b)=e^{-\theta b}$. Since $D_t$ is zero or one,

$$
\frac{\mathbb E[V(B_{t+1})\mid B_t=b]}{V(b)}=\mathbb E[e^{-\theta(A_t-D_t)}]\le\exp\{\eta(e^{-\theta}-1)\}+(e^\theta-1)S(b).
$$

The first term is strictly less than one and the second tends to zero. Hence $V(B_{t\wedge\tau})$ is a nonnegative [supermartingale](../../../../../supermartingale.md) outside a sufficiently large finite set, where $\tau$ is the first entrance into that set, say $\{0,\ldots,b_0\}$. The [optional sampling theorem for a supermartingale](../../../../../optional-sampling-theorem-for-a-supermartingale.md), first at bounded stopping times, gives

$$
\mathbb P_b(\tau<\infty)\le e^{-\theta(b-b_0)}<1,\qquad b>b_0.
$$

This is an [exponential-supermartingale escape bound](../../../../../exponential-supermartingale-escape-bound.md). The chain is irreducible: a no-arrival slot with exactly one old retry can reduce any positive state by one, and Poisson arrivals can reach arbitrarily high states. Therefore the escape probability proves transience and excludes a [positive recurrent Markov chain](../../../../../positive-recurrent-markov-chain.md), for every $\eta>0$ and fixed $0<p<1$. A locally stable fluid operating point can consequently coexist with eventual stochastic congestion. At $p=1$, once at least two packets are backlogged, they collide forever, so constant unit retry probability also fails.

A state-dependent retry rule removes this fixed-$p$ congestion mechanism. As an ideal benchmark with exact backlog information and known arrival intensity $0<\eta<e^{-1}$, use

$$
p_b=\frac{1-\eta}{b},\qquad b\ge1.
$$

This is [backlog-aware ALOHA with arrival-adjusted attempt probabilities](../../../../../backlog-aware-aloha-with-arrival-adjusted-attempt-probabilities.md). Its total attempt intensity approaches one: the mean old-attempt count is $1-\eta$ and the new-attempt count has mean $\eta$. Substitution in the exact success formula yields

$$
S(b)\longrightarrow e^{-\eta}e^{-(1-\eta)}[\eta+(1-\eta)]=e^{-1}.
$$

Thus the drift tends to $\eta-e^{-1}<0$. For the [Lyapunov function](../../../../../lyapunov-function.md) $L(b)=b$, the drift is bounded above by a negative constant outside a finite set, and the expected one-step backlog is finite at every state. [Foster theorem](../../../../../foster-s-theorem.md) therefore gives positive recurrence. This proves a genuine stochastic stability result for this specified, informed controller. Real transmitters generally observe feedback rather than the exact backlog; estimating the backlog and using a probability of order its reciprocal motivates adaptive ALOHA, but an estimate's dynamics must be included in the state and analyzed before claiming the same stability result.

A different nonconstant rule uses a packet's own collision history. In [geometric-attempt exponential backoff](../../../../../geometric-attempt-exponential-backoff.md), a packet at stage $k$ attempts with probability $p_k=p_0 2^{-k}$, where $0<p_0<1$. A collision advances every attempted packet by one stage, a success removes its packet, and new arrivals enter stage zero. For definiteness, in this version arrivals join at the end of a slot and first become eligible in the next slot. The full [Markov chain](../../../../../markov-chain.md) state is the sequence $(N_0,N_1,\ldots)$ of stage populations; the total backlog alone is insufficient. Conditional on that state,

$$
I(N)=\prod_{k\ge0}(1-p_k)^{N_k},\qquad S(N)=I(N)\sum_{k\ge0}\frac{N_kp_k}{1-p_k}.
$$

These formulas follow from independent attempts and selecting which one packet succeeds. They reduce approximately to $S\simeq Ge^{-G}$ for many small probabilities with $G=\sum_kN_kp_k$. The retry probabilities decrease after failure, preventing repeated aggressive attempts by the same packets. [Binary exponential backoff](../../../../../binary-exponential-backoff.md) instead chooses uniform random counters from expanding finite windows; that counter model requires residual counters as well as collision stages in its state and is not identical to geometric waiting.

Backoff also exposes a distinction between eventual delivery and acceptable delay. In the simplifying model where each attempt independently fails with a fixed probability $q<1$, the probability of reaching stage $k$ is $q^k$ and its mean waiting time is $1/p_k=2^k/p_0$. The [mean delay under independent exponential-backoff failures](../../../../../mean-delay-under-independent-exponential-backoff-failures.md) is therefore

$$
\mathbb ET=\frac1{p_0}\sum_{k\ge0}(2q)^k,\qquad \boxed{\mathbb ET<\infty\iff q<1/2.}
$$

Although a packet succeeds almost surely whenever $q<1$, its mean delay can be infinite. In an actual [random access network](../../../../../random-access-network.md), failures are correlated with the other stage populations, so this fixed-$q$ calculation is a diagnostic approximation, not a proof of network stability. These models show why random-access analysis must track the retry rule, feedback information and full state, and assess [throughput](../../../../../throughput.md), stability and delay separately.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
