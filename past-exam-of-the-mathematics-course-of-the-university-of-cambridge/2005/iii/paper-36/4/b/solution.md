<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The capacity and quality targets alone do not determine flow counts: the per-flow traffic statistics must also be supplied. The following explicit model gives a computable sufficient region, with genuine upper bounds on both loss fractions.

Measure [queue workload](../../../../../../workload-of-a-queue.md) and buffer size in bits. Denote capacity by $C$, shared buffer size by $B$, voice delay limit by $D$, target voice loss by $\ell_v$, and target data loss by $\ell_d$, with $0<\ell_v,\ell_d<1$. Let there be $n_v$ voice flows and $n_d$ data flows. Model each class-$j$ flow, $j\in\{v,d\}$, by a stationary [Compound Poisson process](../../../../../../compound-poisson-process.md) with packet rate $\nu_j$ and positive [independent](../../../../../../independent-random-variables.md) packet sizes $S_j$, and assume [independence](../../../../../../independent-random-variables.md) across flows and marks. Use a work-conserving preemptive-resume [priority queue with a shared buffer](../../../../../../priority-queue-with-a-shared-buffer.md), with voice priority and [first come first served](../../../../../../first-come-first-served.md) within each class. This preemptive or fluid approximation makes the predicted voice waiting time exactly $V/C$, where $V$ is the remaining voice [queue workload](../../../../../../workload-of-a-queue.md) just before arrival. Assume packet sizes are bounded by a known $s_{\max}<B$ and interpret the buffer gate as a packet-fit test; rejecting packets which do not fit is the packet version of the full-buffer rule.

For one flow the [Compound Poisson process](../../../../../../compound-poisson-process.md) formula gives

$$
\Lambda_j(\theta)=\nu_j(\mathbb E e^{\theta S_j}-1),\qquad
\boxed{a_j(\theta)=\frac{\nu_j(\mathbb E e^{\theta S_j}-1)}{\theta}.}
$$

For fixed-size packets of size $s_j$, substitute $e^{\theta s_j}$. Estimate the packet rate and size law from measurements or a declared traffic contract. Also require the strict stability inequality

$$
n_v\nu_v\mathbb E S_v+n_d\nu_d\mathbb E S_d<C.
$$

Define $B_0=B-s_{\max}>0$ and $K=CD$. Couple the switch with an unthinned infinite-buffer aggregate [queue](../../../../../../queue-queueing-theory.md) and an unthinned infinite-buffer voice-only [queue](../../../../../../queue-queueing-theory.md), both driven by the same offered packets and both served at rate $C$. Under the preemptive [service discipline](../../../../../../service-discipline.md), dropping arrivals can only decrease both the total [queue workload](../../../../../../workload-of-a-queue.md) and the voice [queue workload](../../../../../../workload-of-a-queue.md). Thus total switch [queue workload](../../../../../../workload-of-a-queue.md) $Q$ and voice [queue workload](../../../../../../workload-of-a-queue.md) $V$ satisfy $Q\leq W_T$ and $V\leq W_V$ in the stationary coupling. A packet-fit loss implies $Q>B-S_j\geq B_0$, and a voice-delay rejection implies $V\geq K$.

Apply the [continuous-time exponential workload bound](../../../../../../continuous-time-exponential-workload-bound.md) to the two comparison [queues](../../../../../../queue-queueing-theory.md). For any positive $\theta_T,\theta_V$ satisfying

$$
n_v a_v(\theta_T)+n_d a_d(\theta_T)\leq C,\qquad
n_v a_v(\theta_V)\leq C,
$$

the stationary loss-event [probabilities](../../../../../../probability.md) obey

$$
\boxed{p_d\leq e^{-\theta_T B_0},\qquad
p_v\leq e^{-\theta_T B_0}+e^{-\theta_V K}.}
$$

The second inequality is a [union bound](../../../../../../boole-s-inequality.md): voice can be lost either at the shared buffer or at its delay gate. Data congestion therefore contributes to voice loss despite its lower service priority. [Poisson arrivals see time averages](../../../../../../poisson-arrivals-see-time-averages.md) applies to each offered packet stream, whose future arrivals are [independent](../../../../../../independent-random-variables.md) of the prearrival state; the stationary event bounds are consequently bounds on the offered-packet loss fractions. Voice packets that are admitted have [queueing delay](../../../../../../queueing-delay.md) below $D$, because later voice packets join behind them and data work cannot delay them in this model.

To turn the bounds into flow counts, allocate loss budgets

$$
0<\eta_B<\min(\ell_d,\ell_v),\qquad
\eta_V=\ell_v-\eta_B,\qquad
\theta_T=\frac{\log(1/\eta_B)}{B_0},\quad
\theta_V=\frac{\log(1/\eta_V)}{CD}.
$$

For example, $\eta_B=\min(\ell_d,\ell_v/2)$ and $\eta_V=\ell_v-\eta_B$ also work; equality with $\ell_d$ is harmless. The required sufficient [effective-bandwidth admission region with a voice delay gate](../../../../../../effective-bandwidth-admission-region-with-a-voice-delay-gate.md) is

$$
\boxed{\begin{gathered}
n_v a_v(\theta_V)\leq C,\\
n_v a_v(\theta_T)+n_d a_d(\theta_T)\leq C,\\
n_v\nu_v\mathbb E S_v+n_d\nu_d\mathbb E S_d<C,\qquad
n_v,n_d\in\mathbb Z_{\geq0}.
\end{gathered}}
$$

It ensures $p_d\leq\ell_d$ and $p_v\leq\ell_v$. A simple enumeration is

$$
0\leq n_v\leq\left\lfloor\frac C{a_v(\theta_V)}\right\rfloor,\qquad
0\leq n_d\leq
\left\lfloor\frac{C-n_v a_v(\theta_T)}{a_d(\theta_T)}\right\rfloor,
$$

discarding negative bounds and pairs failing strict mean-load stability. The formulas assume positive-rate nonzero-size flows. Optimize a chosen revenue or flow-count objective over these integer pairs. Searching over the budget split $\eta_B$ can enlarge the sufficient region. For a bit-fluid buffer gate with no packet-fit issue, $B_0$ can be replaced by $B$.

Real nonpreemptive packet service needs an additional residual-service allowance or an explicit priority [queue workload](../../../../../../workload-of-a-queue.md) analysis: a voice packet may have to wait for the data packet already in service. Burst-correlated voice sources also require richer descriptors, such as measured finite-time [effective bandwidths](../../../../../../effective-bandwidth.md) $\alpha_j(\theta,t)$ or a Markov-modulated source model. For such inputs, additivity still holds for [independent](../../../../../../independent-random-variables.md) flows, but the independent-increment supermartingale bound is not automatic; use a valid sample-path [large deviation principle](../../../../../../large-deviation-principle.md) or a model-specific overflow bound, with prefactors or a safety margin when using asymptotics. If packet arrivals do not form a [Poisson process](../../../../../../poisson-process.md), loss fractions must be assessed at arrival epochs rather than inferred solely from time-average [queue workload](../../../../../../workload-of-a-queue.md) [probabilities](../../../../../../probability.md). These qualifications explain both how to calculate an admission region from specified traffic statistics and why the five switch/QoS parameters by themselves cannot supply a numerical answer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
