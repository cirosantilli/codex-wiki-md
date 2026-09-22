# Queueing theory

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Queueing_theory)

**Table of contents**

- [Scaling limit of a queue](#scaling-limit-of-a-queue)
  - [Heavy-traffic limit of a queue](#heavy-traffic-limit-of-a-queue)
  - [Moderate-deviation queue scaling](#moderate-deviation-queue-scaling)
  - [Many-source queue scaling](#many-source-queue-scaling)
  - [Large-buffer queue scaling](#large-buffer-queue-scaling)
    - [Cramér-Lundberg workload exponent](#cramer-lundberg-workload-exponent)
- [Geometric-arrival single-service queue](#geometric-arrival-single-service-queue)
- [General-service infinite-server queue](#general-service-infinite-server-queue)
  - [Clearance time after closing an infinite-server queue](#clearance-time-after-closing-an-infinite-server-queue)
- [Alternating arrival and service queue](#alternating-arrival-and-service-queue)
- [Queue (queueing theory)](#queue-queueing-theory)
  - [Burstiness of queue input](#burstiness-of-queue-input)
  - [Bufferless queue](#bufferless-queue)
    - [Poisson large-service overflow asymptotic](#poisson-large-service-overflow-asymptotic)
    - [Bufferless queue output](#bufferless-queue-output)
      - [Moderate deviation scales of a clipped Poisson aggregate](#moderate-deviation-scales-of-a-clipped-poisson-aggregate)
      - [Moderate deviations below a bufferless queue cap](#moderate-deviations-below-a-bufferless-queue-cap)
  - [Queue overflow](#queue-overflow)
  - [Buffer size of a queue](#buffer-size-of-a-queue)
  - [Service rate of a queue](#service-rate-of-a-queue)
  - [Queueing delay](#queueing-delay)
  - [Workload of a queue](#workload-of-a-queue)
    - [Stationary workload supremum](#stationary-workload-supremum)
    - [Linear workload rate for a local convex action](#linear-workload-rate-for-a-local-convex-action)
    - [Constant-rate burst path](#constant-rate-burst-path)
    - [Finite-buffer workload map](#finite-buffer-workload-map)
      - [Finite-memory continuity of a finite-buffer queue](#finite-memory-continuity-of-a-finite-buffer-queue)
      - [Finite-buffer workload rate truncation](#finite-buffer-workload-rate-truncation)
    - [Lindley recursion](#lindley-recursion)
      - [Slower-server tandem workload identity](#slower-server-tandem-workload-identity)
- [Heterogeneous two-server queue](#heterogeneous-two-server-queue)
- [Busy period](#busy-period)
  - [Busy-period branching equation](#busy-period-branching-equation)
- [Multiclass single-server queue](#multiclass-single-server-queue)
  - [Priority queue with a shared buffer](#priority-queue-with-a-shared-buffer)
    - [Effective-bandwidth admission region with a voice delay gate](#effective-bandwidth-admission-region-with-a-voice-delay-gate)
- [Service discipline](#service-discipline)
  - [Symmetric service discipline](#symmetric-service-discipline)
  - [Processor sharing](#processor-sharing)
  - [First come first served](#first-come-first-served)
- [Server utilization](#server-utilization)
  - [Finite-buffer server utilization](#finite-buffer-server-utilization)
- [Queue throughput](#queue-throughput)
- [Customer sojourn time](#customer-sojourn-time)
- [Service time](#service-time)
- [Quasireversibility](#quasireversibility)
- [M-M-s queue](#m-m-s-queue)
  - [Burke theorem for a multi-server queue](#burke-theorem-for-a-multi-server-queue)
- [Stochastic network](#stochastic-network)
  - [Sublinear path space for fluid queues](#sublinear-path-space-for-fluid-queues)
    - [Weighted cumulative-input topology for a slotted queue](#weighted-cumulative-input-topology-for-a-slotted-queue)
    - [Self-similar Gaussian workload rate](#self-similar-gaussian-workload-rate)
  - [Closed migration process](#closed-migration-process)
    - [Blocking probability in a finite-line sequential-service network](#blocking-probability-in-a-finite-line-sequential-service-network)
      - [Stationary flow conservation in a finite-line switchboard](#stationary-flow-conservation-in-a-finite-line-switchboard)
    - [Product-form stationary distribution of a closed migration process](#product-form-stationary-distribution-of-a-closed-migration-process)
  - [Product-form stationary distribution of a multiclass queueing network](#product-form-stationary-distribution-of-a-multiclass-queueing-network)
  - [Traffic equations for a multiclass queueing network](#traffic-equations-for-a-multiclass-queueing-network)
  - [Congestion control](#congestion-control)
    - [User-network decomposition of concave utility maximization](#user-network-decomposition-of-concave-utility-maximization)
    - [Resource congestion price](#resource-congestion-price)
      - [Route congestion price](#route-congestion-price)
    - [Multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics)
      - [Increasing-supply resource-price dynamics](#increasing-supply-resource-price-dynamics)
        - [Positive-price convergence for increasing resource supplies](#positive-price-convergence-for-increasing-resource-supplies)
        - [Boundary equilibria of multiplicative resource prices](#boundary-equilibria-of-multiplicative-resource-prices)
      - [Relative-entropy Lyapunov function for resource prices](#relative-entropy-lyapunov-function-for-resource-prices)
        - [Full-row-rank convergence of multiplicative resource prices](#full-row-rank-convergence-of-multiplicative-resource-prices)
    - [Boundary equilibrium of multiplicative price dynamics](#boundary-equilibrium-of-multiplicative-price-dynamics)
    - [Dual congestion potential](#dual-congestion-potential)
    - [Primal congestion potential](#primal-congestion-potential)
      - [Global convergence of primal congestion control](#global-convergence-of-primal-congestion-control)
        - [Square-root coordinates for primal congestion control](#square-root-coordinates-for-primal-congestion-control)
  - [Effective bandwidth](#effective-bandwidth)
    - [Poisson effective bandwidth](#poisson-effective-bandwidth)
    - [Bernoulli effective bandwidth](#bernoulli-effective-bandwidth)
    - [Exponential workload bound from cumulative arrival moments](#exponential-workload-bound-from-cumulative-arrival-moments)
    - [Continuous-time exponential workload bound](#continuous-time-exponential-workload-bound)
    - [Monotonicity and bounds of effective bandwidth](#monotonicity-and-bounds-of-effective-bandwidth)
    - [Workload Chernoff bound for independent increments](#workload-chernoff-bound-for-independent-increments)
    - [Mean and peak limits of effective bandwidth](#mean-and-peak-limits-of-effective-bandwidth)
    - [Gaussian effective bandwidth](#gaussian-effective-bandwidth)
      - [Exact Gaussian overflow constraint](#exact-gaussian-overflow-constraint)
        - [Zero-variance boundary of an overflow constraint](#zero-variance-boundary-of-an-overflow-constraint)
  - [Open migration process](#open-migration-process)
    - [Time reversal of an open migration process](#time-reversal-of-an-open-migration-process)
      - [Poisson migration stream without a return path](#poisson-migration-stream-without-a-return-path)
    - [Service-capacity allocation in an open migration process](#service-capacity-allocation-in-an-open-migration-process)
    - [Product-form stationary distribution of an open migration process](#product-form-stationary-distribution-of-an-open-migration-process)
    - [Traffic equation of an open migration process](#traffic-equation-of-an-open-migration-process)
  - [Flow-level network model](#flow-level-network-model)
    - [Balance function of a flow-level network](#balance-function-of-a-flow-level-network)
      - [Stationary law of a proportionally fair four-cycle](#stationary-law-of-a-proportionally-fair-four-cycle)
        - [Four-cycle partition function](#four-cycle-partition-function)
        - [Stability region for the reversible four-cycle flow network](#stability-region-for-the-reversible-four-cycle-flow-network)
    - [Linear flow network](#linear-flow-network)
      - [Stationary law of a linear flow network](#stationary-law-of-a-linear-flow-network)
        - [Local-count independence in a linear flow network](#local-count-independence-in-a-linear-flow-network)
      - [Proportionally fair allocation on a linear flow network](#proportionally-fair-allocation-on-a-linear-flow-network)
      - [Two-resource linear flow network](#two-resource-linear-flow-network)
        - [Stationary law of a two-resource linear flow network](#stationary-law-of-a-two-resource-linear-flow-network)
          - [Local-count independence with through-flow dependence](#local-count-independence-with-through-flow-dependence)
          - [Stability conditions for a two-resource linear flow network](#stability-conditions-for-a-two-resource-linear-flow-network)
        - [Proportionally fair allocation on a two-resource linear network](#proportionally-fair-allocation-on-a-two-resource-linear-network)
    - [Reversible four-cycle flow model](#reversible-four-cycle-flow-model)
  - [Fluid model](#fluid-model)
    - [Ratio time change for a homogeneous fluid model](#ratio-time-change-for-a-homogeneous-fluid-model)
    - [Finite-time draining of a fluid model](#finite-time-draining-of-a-fluid-model)
    - [Fluid limit](#fluid-limit)
      - [Kurtz fluid limit theorem](#kurtz-fluid-limit-theorem)
      - [Poisson concentration proof of a density-dependent fluid limit](#poisson-concentration-proof-of-a-density-dependent-fluid-limit)
  - [Random access network](#random-access-network)
    - [Exponential backoff](#exponential-backoff)
      - [Geometric-attempt exponential backoff](#geometric-attempt-exponential-backoff)
        - [Mean delay under independent exponential-backoff failures](#mean-delay-under-independent-exponential-backoff-failures)
      - [Binary exponential backoff](#binary-exponential-backoff)
    - [Throughput](#throughput)
    - [Carrier-sense multiple access](#carrier-sense-multiple-access)
    - [Interference graph](#interference-graph)
      - [Throughput region of an interference graph](#throughput-region-of-an-interference-graph)
    - [Slotted ALOHA](#slotted-aloha)
      - [Finite-population exclusion of permanent ALOHA collisions](#finite-population-exclusion-of-permanent-aloha-collisions)
      - [Backlog-aware ALOHA with arrival-adjusted attempt probabilities](#backlog-aware-aloha-with-arrival-adjusted-attempt-probabilities)
      - [Permanent collisions in constant-probability slotted ALOHA](#permanent-collisions-in-constant-probability-slotted-aloha)
        - [Collision-path coupling for slotted ALOHA](#collision-path-coupling-for-slotted-aloha)
      - [Fluid approximation of slotted ALOHA](#fluid-approximation-of-slotted-aloha)
        - [Stable fluid controller for slotted ALOHA](#stable-fluid-controller-for-slotted-aloha)
      - [ALOHA throughput bound](#aloha-throughput-bound)
  - [Wardrop equilibrium](#wardrop-equilibrium)
    - [Braess's paradox](#braess-s-paradox)
    - [Marginal external cost toll](#marginal-external-cost-toll)
      - [Optimal-flow calibrated congestion tolling](#optimal-flow-calibrated-congestion-tolling)
    - [Route-flow nonuniqueness at a Wardrop equilibrium](#route-flow-nonuniqueness-at-a-wardrop-equilibrium)
    - [Elastic-demand Wardrop equilibrium](#elastic-demand-wardrop-equilibrium)
      - [Boundary exclusion for elastic Wardrop demand](#boundary-exclusion-for-elastic-wardrop-demand)
      - [Inverse demand function](#inverse-demand-function)
        - [Elastic-demand utility with an interior reference](#elastic-demand-utility-with-an-interior-reference)
    - [Beckmann potential](#beckmann-potential)
    - [Source-sink route incidence matrix](#source-sink-route-incidence-matrix)
  - [Link-route incidence matrix](#link-route-incidence-matrix)
  - [Loss network](#loss-network)
    - [Rearrangeable triangular loss network](#rearrangeable-triangular-loss-network)
      - [Cut feasibility for a rearrangeable triangle](#cut-feasibility-for-a-rearrangeable-triangle)
    - [Alternative routing](#alternative-routing)
      - [Multiple Erlang fixed points under alternative routing](#multiple-erlang-fixed-points-under-alternative-routing)
        - [Fluid scaling proof of multiple Erlang fixed points](#fluid-scaling-proof-of-multiple-erlang-fixed-points)
        - [Alternative-routing triangle with three Erlang fixed points](#alternative-routing-triangle-with-three-erlang-fixed-points)
    - [Erlang loss formula](#erlang-loss-formula)
      - [Rational certificates for the Erlang loss recursion](#rational-certificates-for-the-erlang-loss-recursion)
      - [Monotonicity of the Erlang blocking probability](#monotonicity-of-the-erlang-blocking-probability)
      - [Proportional scaling limit of the Erlang loss formula](#proportional-scaling-limit-of-the-erlang-loss-formula)
      - [Carried load of an Erlang loss resource](#carried-load-of-an-erlang-loss-resource)
      - [Erlang fixed point approximation](#erlang-fixed-point-approximation)
        - [Convex potential for the Erlang fixed point](#convex-potential-for-the-erlang-fixed-point)
          - [Cyclic substitution for the Erlang fixed point](#cyclic-substitution-for-the-erlang-fixed-point)
        - [Reduced-load approximation](#reduced-load-approximation)
    - [Offered traffic](#offered-traffic)
    - [Fixed routing](#fixed-routing)
      - [Product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network)
        - [Blocking partition ratio for a loss network](#blocking-partition-ratio-for-a-loss-network)
        - [Entropy maximization for loss-network occupancy](#entropy-maximization-for-loss-network-occupancy)
          - [Poisson exponential tilting for a loss network](#poisson-exponential-tilting-for-a-loss-network)
        - [Insensitivity of loss networks](#insensitivity-of-loss-networks)
- [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages)
- [M/G/1 queue](#m-g-1-queue)
  - [M/D/1 queue](#m-d-1-queue)
  - [Embedded departure chain of an M-G-1 queue](#embedded-departure-chain-of-an-m-g-1-queue)
    - [Pollaczek-Khinchine formula](#pollaczek-khinchine-formula)
      - [Pollaczek-Khinchine mean formula](#pollaczek-khinchine-mean-formula)
- [Little's law](#little-s-law)

## Scaling limit of a queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

An asymptotic description obtained by increasing queue resources or input size, or by approaching critical load while rescaling time and workload. [Large-buffer queue scaling](#large-buffer-queue-scaling), [many-source queue scaling](#many-source-queue-scaling), [moderate-deviation queue scaling](#moderate-deviation-queue-scaling) and the [heavy-traffic limit of a queue](#heavy-traffic-limit-of-a-queue) preserve different relations between mean load, random fluctuations and storage.

### Heavy-traffic limit of a queue

↑ **Parent:** [Scaling limit of a queue](#scaling-limit-of-a-queue)

For fixed [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) arrivals of mean $\mu$ and positive finite [variance](variance.md) $\sigma^2$, put service at $\mu+\varepsilon d$. Rescaling net input by space $\varepsilon$ and time $\varepsilon^{-2}$ gives [Brownian motion](brownian-motion.md) with drift $-d$ by the [functional central limit theorem](convergence-of-random-variables.md#donsker-s-theorem). The continuous [Skorokhod reflection map on the half-line](stochastic-process.md#skorokhod-reflection-map-on-the-half-line) gives the displayed transient limit, with a correspondingly scaled initial workload. A stationary approximation additionally requires justification of limit interchange. When valid, the [stationary law of negatively drifted reflected Brownian motion](brownian-motion.md#stationary-law-of-negatively-drifted-reflected-brownian-motion) predicts $\mathbb P(Q_\varepsilon>b/\varepsilon)\approx e^{-2db/\sigma^2}$.

### Moderate-deviation queue scaling

↑ **Parent:** [Scaling limit of a queue](#scaling-limit-of-a-queue)

For a [bufferless queue](#bufferless-queue) with [Poisson](discrete-probability-distribution.md#poisson-distribution) mean input $L\lambda$, place the service margin at $C L^{(1+\beta)/2}$, $0<\beta<1$. It exceeds the ordinary square-root fluctuation scale but is sublinear in total input. The [Poisson moderate deviation principle](convergence-of-random-variables.md#poisson-moderate-deviation-principle) gives the displayed overflow exponent. This interpolates between a central-limit safety margin and a fixed per-source excess capacity.

### Many-source queue scaling

↑ **Parent:** [Scaling limit of a queue](#scaling-limit-of-a-queue)

Scale independent source count, service and buffer by the same factor $L$. For lookback horizon $n$, the source-average cumulative input has [rate function](convergence-of-random-variables.md#rate-function) $I_n$, and reaching buffer level $b$ requires input above $b+cn$. Optimizing this horizon gives the displayed exponent under uniform control of the infinite stationary supremum. For independent slots, $I_n(x)=nI_A(x/n)$; discrete time keeps $n$ an integer. Temporal dependence instead enters through the cumulative-input [cumulant-generating function](probability-theory.md#cumulant-generating-function).

### Large-buffer queue scaling

↑ **Parent:** [Scaling limit of a queue](#scaling-limit-of-a-queue)

Hold a stable input law and [service rate of a queue](#service-rate-of-a-queue) fixed while the [buffer size of a queue](#buffer-size-of-a-queue) grows. Under interior exponential-moment and root hypotheses, the [Cramér-Lundberg workload exponent](#cramer-lundberg-workload-exponent) gives an exponential tail linear in buffer size. A likely overflow accumulates during a lookback horizon proportional to the buffer size.

<h4 id="cramer-lundberg-workload-exponent">Cramér-Lundberg workload exponent</h4>

↑ **Parent:** [Large-buffer queue scaling](#large-buffer-queue-scaling)

For nondegenerate [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) arrivals with mean below $c$, suppose the positive root is interior to the [moment-generating function](probability-theory.md#moment-generating-function) domain. Then $\Lambda_A'(\theta_*)>c$. The [Fenchel–Young inequality](convex-optimization.md#fenchel-young-inequality) gives $tI_A(c+1/t)\ge\theta_*$ for every $t>0$, and equality occurs at $t=[\Lambda_A'(\theta_*)-c]^{-1}$. The [exponential workload bound from cumulative arrival moments](#exponential-workload-bound-from-cumulative-arrival-moments) gives the upper logarithmic tail bound for every $\theta<\theta_*$. A horizon of the indicated length times buffer size gives the matching lower bound by [Cramér's theorem](probability-theory.md#cramer-s-theorem). A positive interior root is an assumption; if arrivals never exceed capacity, positive workload cannot arise.

## Geometric-arrival single-service queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

Let the independent arrivals satisfy $\Pr(G_n=j)=qp^j$, with $p+q=1$. During a [busy period](#busy-period), each served customer produces $G_n$ further customers, so the total number served has the total-progeny law of a [Galton-Watson process](probability-and-statistics.md#galton-watson-process) with mean $p/q$. Its extinction probability solves $s=q/(1-ps)$ and is the smaller of $1$ and $q/p$. The queue is positive recurrent for $p<1/2$, null recurrent for $p=1/2$, and transient for $p>1/2$. In the positive recurrent case its [stationary distribution](markov-process.md#stationary-distribution) is $\pi_j=(1-p/q)(p/q)^j$.

## General-service infinite-server queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

Poisson arrivals of rate $\lambda$ receive independent service times distributed as $S$, with infinitely many servers so service starts on arrival. Starting empty, the occupancy at time $t$ is Poisson with mean $\lambda\int_0^t\mathbb P(S>u)\,du$, by independent thinning of the marked arrivals. If $\mathbb ES<\infty$, the equilibrium count is Poisson with mean $\lambda\mathbb ES$. Occupancy need not be a Markov process for a general service law; remaining service times carry additional state information.

### Clearance time after closing an infinite-server queue

↑ **Parent:** [General-service infinite-server queue](#general-service-infinite-server-queue)

Stop new arrivals at time $t$ in an initially empty [general-service infinite-server queue](#general-service-infinite-server-queue). The number remaining $v$ time units later is Poisson with mean $\lambda\int_v^{t+v}\mathbb P(S>u)\,du$. Thus the probability that clearance has not occurred is one minus the exponential of the negative of that mean. Letting $t\to\infty$ gives the displayed equilibrium formula, since $\int_v^\infty\mathbb P(S>u)\,du=\mathbb E(S-v)_+$. The clearance time is zero when no customers remain at closing.

## Alternating arrival and service queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

A [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) may alternate between an arrival phase $C$, with upward transitions at rate $\lambda$, and a service phase $W$, with downward transitions at rate $\mu$ when the level is positive. Switching rates $C\to W$ and $W\to C$ are $\alpha,\beta$. Its [stationary balance equations](markov-process.md#global-balance-for-a-continuous-time-markov-chain) give a geometric invariant tail with ratio $\theta=\lambda(\mu+\beta)/[\mu(\lambda+\alpha)]$. A stationary probability exists exactly when $\mu\alpha>\lambda\beta$, consistent with the stationary average service rate $\mu\alpha/(\alpha+\beta)$ exceeding the arrival rate $\lambda\beta/(\alpha+\beta)$.

## Queue (queueing theory)

↑ **Parent:** [Queueing theory](queueing-theory.md)

A queue consists of customers or jobs waiting for or receiving service. An arrival process adds customers and a service rule specifies which waiting customer is served next. A stochastic model of these events is studied in [queueing theory](queueing-theory.md); its queue length is the number of customers waiting or in service, according to the stated convention.

### Burstiness of queue input

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

The size and frequency of unusually large arrivals or sustained overload episodes. It depends on the time and threshold scales being examined, rather than just on the one-slot [variance](variance.md). A cap can leave smaller rare deviations unchanged while removing larger positive bursts.

### Bufferless queue

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

A [queue](#queue-queueing-theory) which retains no unfinished work between slots. Given nonnegative input $A$ and capacity $c$, its [bufferless queue output](#bufferless-queue-output) is $\min(A,c)$ and its lost work is $(A-c)^+$.

#### Poisson large-service overflow asymptotic

↑ **Parent:** [Bufferless queue](#bufferless-queue)

For fixed [Poisson](discrete-probability-distribution.md#poisson-distribution) mean $\lambda>0$ and capacity $c\to\infty$, set $m=\lfloor c\rfloor+1$. The optimized [Chernoff bound](probability-inequality.md#chernoff-bound) gives $\log\mathbb P(X\ge m)\le-I_P(m)$. The lower bound by $\mathbb P(X=m)$ and [Stirling's formula](real-analysis.md#stirling-formula) differs by only $O(\log m)$. Rounding $m$ to $c$ changes the cost by $O(\log c)$, proving the displayed formula and the leading scale $-c\log c$.

#### Bufferless queue output

↑ **Parent:** [Bufferless queue](#bufferless-queue)

The work served in one slot is capped at the [service rate of a queue](#service-rate-of-a-queue). The remainder is lost, so output is input minus its [positive part](function.md#positive-part-of-a-real-valued-function) above capacity. Every downstream threshold below the cap has exactly the same overflow event for input and output; thresholds at or above the cap cannot be exceeded by the output.

##### Moderate deviation scales of a clipped Poisson aggregate

↑ **Parent:** [Bufferless queue output](#bufferless-queue-output)

Clip [Poisson](discrete-probability-distribution.md#poisson-distribution) input of mean $L\lambda$ at $L\lambda+C L^{(1+\beta)/2}$. The [Poisson moderate deviation principle](convergence-of-random-variables.md#poisson-moderate-deviation-principle) and [contraction principle for large deviations](convergence-of-random-variables.md#contraction-principle-for-large-deviations) give the displayed output rate at the clipping scale. At smaller exponents the output retains the original rate by [moderate deviations below a bufferless queue cap](#moderate-deviations-below-a-bufferless-queue-cap). At larger positive-deviation scales every overflow event is eventually impossible because the requested threshold exceeds the cap.

##### Moderate deviations below a bufferless queue cap

↑ **Parent:** [Bufferless queue output](#bufferless-queue-output)

For [Poisson](discrete-probability-distribution.md#poisson-distribution) input and $u_L=L\lambda+C L^{(1+\beta)/2}$ with $C>0$, clipping occurs with logarithmic probability $-C^2L^\beta/(2\lambda)$. At any smaller exponent $0<\alpha<\beta$, this is superexponentially small at speed $L^\alpha$. Dividing the input and output difference by $L^{(1+\alpha)/2}$ therefore gives [exponential equivalence](convergence-of-random-variables.md#exponential-equivalence). More directly, for every threshold $r_L<u_L$, the events $\{\min(S_L,u_L)>r_L\}$ and $\{S_L>r_L\}$ are identical.

### Queue overflow

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

An arrival exceeds the available service and storage capacity, causing work to be lost or blocked. For a [bufferless queue](#bufferless-queue) with capacity $c$ per slot, overflow means input work strictly greater than $c$. Stationary [queue workload](#workload-of-a-queue) tails in an infinite-buffer comparison model are often used to estimate finite-buffer overflow probabilities.

### Buffer size of a queue

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

The maximum stored work or number of waiting jobs, according to the model's convention. A [bufferless queue](#bufferless-queue) has no room to retain excess input for a later slot.

### Service rate of a queue

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

The amount of work a [queue](#queue-queueing-theory) can serve per unit of time. In a slotted model the same units can describe work served per slot.

### Queueing delay

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

The [queueing delay](#queueing-delay) is the time between a customer's arrival and the start of its service, excluding its own [service time](#service-time). Under [first come first served](#first-come-first-served) with service rate $C$, its [queueing delay](#queueing-delay) is the [queue workload](#workload-of-a-queue) ahead of it divided by $C$. The [customer sojourn time](#customer-sojourn-time) also includes the customer's own service. In a preemptive [priority queue with a shared buffer](#priority-queue-with-a-shared-buffer), a voice customer's initial waiting time depends only on the voice [queue workload](#workload-of-a-queue) already present.

### Workload of a queue

↑ **Parent:** [Queue (queueing theory)](#queue-queueing-theory)

The [queue workload](#workload-of-a-queue) of a [queue](#queue-queueing-theory) is the total remaining service work of all present customers, including residual work in service. With a work-conserving server of rate $C$ and stationary input $A$, the stationary [queue workload](#workload-of-a-queue) is represented by

$$
W(0)=\sup_{t\geq0}\{A(-t,0]-Ct\}.
$$

This is the amount by which past offered work exceeds available service, maximized over possible starts of a busy period. It is the reflection of net input at zero. Under [first come first served](#first-come-first-served), an arriving infinitesimal customer waits $W/C$; a priority customer instead waits for the remaining work ahead of it under its [service discipline](#service-discipline).

#### Stationary workload supremum

↑ **Parent:** [Workload of a queue](#workload-of-a-queue)

For [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) arrivals with finite mean below service $c$, the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) makes the net cumulative input tend to minus infinity, so the supremum is finite [almost surely](convergence-of-random-variables.md#almost-sure-convergence). Applying the same formula to the past input gives a stationary solution of the [Lindley recursion](#lindley-recursion). This representation turns [queue workload](#workload-of-a-queue) overflow into an event involving some lookback horizon.

#### Linear workload rate for a local convex action

↑ **Parent:** [Workload of a queue](#workload-of-a-queue)

For a stable input with path action $I(a)=\int_{-\infty}^0g(\dot a_s)ds$, a workload x requires some interval of length t with average input near $C+x/t$. [Jensen inequality](real-analysis.md#jensen-s-inequality) bounds its cost below by $tg(C+x/t)$; taking the [supremum](real-analysis.md#supremum) workload and then the [infimum](real-analysis.md#infimum) over t yields the displayed lower bound. [Constant-rate burst paths](#constant-rate-burst-path) give the matching upper bound. At zero the typical-rate path has zero cost; negative workloads have infinite rate. If no finite-cost rate exceeds C, every positive workload has infinite rate.

#### Constant-rate burst path

↑ **Parent:** [Workload of a queue](#workload-of-a-queue)

Use arrival rate v during the last t time units and the normal stable rate mu before that, where $\mu<C$. The lookback net input increases from zero to x over the burst, then decreases because the earlier net drift is negative. Its infinite-buffer workload is x, as is the [finite-buffer workload map](#finite-buffer-workload-map) for capacity at least x. For a local convex path cost with density g and $g(\mu)=0$, its cost is $tg(v)=xg(v)/(v-C)$. These paths realize or approximate the optimal workload cost even if an optimizing duration is not attained.

#### Finite-buffer workload map

↑ **Parent:** [Workload of a queue](#workload-of-a-queue)

With lookback net input $z(s)=a(-s,0]-Cs$, the stable finite-buffer workload is $\sup_{t\geq0}\min(\sup_{0\leq s\leq t}z(s),B+\inf_{0\leq s\leq t}z(s))$. Since $z(0)=0$, it lies between zero and B, and is at most the infinite-buffer [supremum](real-analysis.md#supremum) $q(a)=\sup_{s\geq0}z(s)$. For a constant-rate burst which builds exactly x work from an empty queue, no upper reflection occurs when $x\leq B$ and both workloads equal x.

##### Finite-memory continuity of a finite-buffer queue

↑ **Parent:** [Finite-buffer workload map](#finite-buffer-workload-map)

Use the clipped [Lindley recursion](#lindley-recursion) $q_{t+1}=\min(B,\max(0,q_t+x_t-C))$ and the [weighted cumulative-input topology for a slotted queue](#weighted-cumulative-input-topology-for-a-slotted-queue). If cumulative past input $S_x(T)\leq\lambda T$ eventually with $\lambda<C$, choose a finite $T$ so $S_x(T)-CT<-B$. Starting with a full buffer at time $-T$, the queue must hit zero before the present, since otherwise its final workload is at most $B+S_x(T)-CT<0$. Monotonicity couples all initial workloads by that zero, establishing a finite memory horizon. The same horizon works for sufficiently close input $y$. Since $|x_{-k}-y_{-k}|\leq(2k-1)\|x-y\|$ and clipping is [Lipschitz continuous](real-analysis.md#lipschitz-continuity) with constant one, the two finite recursions started empty differ by at most $\sum_{k=1}^T(2k-1)\|x-y\|=T^2\|x-y\|$.

##### Finite-buffer workload rate truncation

↑ **Parent:** [Finite-buffer workload map](#finite-buffer-workload-map)

For the local convex action defining the [linear workload rate for a local convex action](#linear-workload-rate-for-a-local-convex-action), continuity and the [contraction principle for large deviations](convergence-of-random-variables.md#contraction-principle-for-large-deviations) give workload [rate functions](convergence-of-random-variables.md#rate-function). The pointwise bound $\bar q_B\leq q$ makes $\bar J_B(x)\geq\inf_{y\geq x}J(y)=J(x)$ on nonnegative workloads. Constant-rate burst paths produce the reverse bound for x at most B. Values outside the buffer interval are impossible. This statement concerns the rate at the workload value, rather than equality of exact finite-buffer and infinite-buffer stationary distributions.

#### Lindley recursion

↑ **Parent:** [Workload of a queue](#workload-of-a-queue)

For arrivals added before the slot's offered service, $Z_k$ is the arriving work minus that service. With independent identically distributed increments of negative mean, the stationary [queue workload](#workload-of-a-queue) has the law $\sup_{m\geq0}\sum_{j=1}^mZ_j$. Iterating the recursion from the past gives this [supremum](real-analysis.md#supremum); the strong law makes it finite. A different arrival/service ordering changes slot-boundary workload but requires its convention to be stated.

##### Slower-server tandem workload identity

↑ **Parent:** [Lindley recursion](#lindley-recursion)

Consider two work-conserving slotted [queues](#queue-queueing-theory) in tandem, with upstream service $c$ and downstream service $d<c$, where upstream departures can be served downstream in the same slot. Put $D_t=\min\{c,Q_{t-1}+a_t\}$. Then $Q_t=Q_{t-1}+a_t-D_t$ and $R_t=(R_{t-1}+D_t-d)^+$. If $R_{t-1}+D_t\geq d$, addition gives $(Q_{t-1}+R_{t-1}+a_t-d)^+$. Otherwise $D_t<d<c$, so the upstream queue empties and both sides of that identity are zero. Thus total workload obeys the [Lindley recursion](#lindley-recursion) with service $d$. Starting empty in the remote past yields the displayed identity whenever the upstream workload is finite. Both workloads, and hence their difference, are [continuous](calculus.md#continuous-function) in the [weighted cumulative-input topology for a slotted queue](#weighted-cumulative-input-topology-for-a-slotted-queue) under strictly subcritical mean input $\lambda<d<c$.

## Heterogeneous two-server queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

A queue with a [Poisson process](probability-theory.md#poisson-process) of arrivals and two independent [service times](#service-time) with [exponential distributions](continuous-probability-distribution.md#exponential-distribution) of different rates must distinguish the two possible single-customer states. If an arrival chooses either idle server with probability $1/2$, the [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) is [reversible](markov-process.md#reversible-markov-chain). Write $a,b$ for the states with only server one or two busy, and $n\geq2$ for total population. Its [detailed balance equations](markov-process.md#detailed-balance) give $\pi_a=\pi_0\nu/(2\mu_1)$, $\pi_b=\pi_0\nu/(2\mu_2)$ and $\pi_n=\pi_0\nu^2(\nu/\mu)^{n-2}/(2\mu_1\mu_2)$. These weights normalize exactly when $\nu<\mu$. In equilibrium, reversed upward transitions have total rate $\nu$ in every state, so [time reversal of a continuous-time Markov chain](markov-process.md#time-reversal-of-a-continuous-time-markov-chain) makes the departure stream a [Poisson process](probability-theory.md#poisson-process) of rate $\nu$. This output conclusion requires stationarity.

## Busy period

↑ **Parent:** [Queueing theory](queueing-theory.md)

A [busy period](#busy-period) is the interval from an arrival that finds the system empty until the next departure leaving it empty. It excludes the preceding idle waiting time. In a stable [M/G/1 queue](#m-g-1-queue) with arrival rate $\lambda$ and mean service time $m$, its mean is $m/(1-\lambda m)$.

### Busy-period branching equation

↑ **Parent:** [Busy period](#busy-period)

In an [M/G/1 queue](#m-g-1-queue), arrivals during the first service generate independent subtrees of work. Conditional on service time $S=s$, the number of descendants is Poisson with mean $\lambda s$. Thus $B\overset d=S+\sum_{j=1}^{N(S)}B_j$, with independent descendant [busy periods](#busy-period). Conditioning and the Poisson generating function give the displayed transform equation wherever its [moment-generating functions](probability-theory.md#moment-generating-function) are finite. Taking expectations yields $\mathbb EB=\mathbb ES+\lambda\mathbb ES\,\mathbb EB$ in the stable regime.

## Multiclass single-server queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

An ordered state $x=(c_1,\ldots,c_n)$ records the classes and positions of customers at a single server. Class-$r$ arrivals have rate $\alpha_r$ and exponential service parameter $\mu_r$. Under a [symmetric service discipline](#symmetric-service-discipline), its [stationary distribution](markov-process.md#stationary-distribution) is $(1-\rho)\prod_i(\alpha_{c_i}/\mu_{c_i})$, where $\rho=\sum_r\alpha_r/\mu_r<1$. If every $\mu_r=\mu$, class-independent insertion and service position rules need not be equal: [time reversal of a continuous-time Markov chain](markov-process.md#time-reversal-of-a-continuous-time-markov-chain) interchanges them and proves the same law. Aggregating words gives $(1-\rho)n!\prod_r[(\alpha_r/\mu_r)^{n_r}/n_r!]$ by the [multinomial coefficient](combinatorics.md#multinomial-coefficient). With class-dependent service rates, [first come first served](#first-come-first-served) need not have this product law.

### Priority queue with a shared buffer

↑ **Parent:** [Multiclass single-server queue](#multiclass-single-server-queue)

A two-class [queue](#queue-queueing-theory) has one total buffer but serves the high-priority class before the other. A preemptive-resume [service discipline](#service-discipline) interrupts low-priority work immediately and later resumes it without wasting completed work. Under [first come first served](#first-come-first-served) within the high-priority class, a new high-priority packet waits $V/C$ when $V$ is the high-priority workload immediately before its arrival. The total workload determines shared-buffer overflow, while $V$ determines the high-priority waiting time. An additional admission gate rejects high-priority packets when $V/C$ exceeds a prescribed delay limit. Finite packets require a fit test against the remaining buffer space, and nonpreemptive service adds residual low-priority service time.

#### Effective-bandwidth admission region with a voice delay gate

↑ **Parent:** [Priority queue with a shared buffer](#priority-queue-with-a-shared-buffer)

Assume [independent](random-variable.md#independent-random-variables) stationary [Compound Poisson process](stochastic-process.md#compound-poisson-process) inputs, preemptive-resume priority for voice, [first come first served](#first-come-first-served) within each class, capacity $C$, a shared buffer of $B$ units of work, packet sizes bounded by $s_{\max}<B$, and voice delay gate $D>0$. Write $B_0=B-s_{\max}$ and $K=CD$. For $n_v,n_d$ flows with per-flow [effective bandwidths](#effective-bandwidth) $a_v,a_d$, the [continuous-time exponential workload bound](#continuous-time-exponential-workload-bound) gives

$$
p_d\leq e^{-\theta_TB_0},\qquad
p_v\leq e^{-\theta_TB_0}+e^{-\theta_VK},
$$

provided $n_va_v(\theta_T)+n_da_d(\theta_T)\leq C$ and $n_va_v(\theta_V)\leq C$. To prove this, couple with the unthinned infinite-buffer aggregate and voice queues driven by the same offered packets. Dropping work reduces both the total and voice workloads under this [service discipline](#service-discipline). A buffer-fit failure implies total workload greater than $B_0$, and a voice-gate failure implies voice workload at least $K$. Apply the two bounds and a union bound; [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages) converts stationary prearrival probabilities to offered-packet loss fractions. For target losses $\ell_d,\ell_v$, choose $0<\eta_B<\min(\ell_d,\ell_v)$ and $\eta_V=\ell_v-\eta_B$, then set

$$
\theta_T=B_0^{-1}\log(1/\eta_B),\qquad
\theta_V=K^{-1}\log(1/\eta_V).
$$

The two [effective bandwidth](#effective-bandwidth) constraints, together with strict aggregate mean-load stability, define a sufficient integer admission region. Voice loss includes the shared-buffer term, even though data packets have lower service priority.

## Service discipline

↑ **Parent:** [Queueing theory](queueing-theory.md)

A service discipline specifies which customers receive the server's capacity and where newly arriving customers join the queue. [First come first served](#first-come-first-served) and [processor sharing](#processor-sharing) give different sample paths even when their equilibrium populations agree.

### Symmetric service discipline

↑ **Parent:** [Service discipline](#service-discipline)

In an ordered queue, let $\gamma_i(n)$ be the fraction of service capacity assigned to position $i$ when $n$ customers are present. A symmetric discipline inserts an arrival into position $i$ with probability $\gamma_i(n+1)$. The same position rule for service and insertion makes transitions satisfy [detailed balance](markov-process.md#detailed-balance) for the word weights $\prod_i\alpha_{c_i}/\mu_{c_i}$. It accommodates class-dependent exponential service rates; [processor sharing](#processor-sharing) is an example.

### Processor sharing

↑ **Parent:** [Service discipline](#service-discipline)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Processor_sharing)

A nonempty server divides its capacity equally among all customers present. With class-$r$ exponential service parameter $\mu_r$, population $n_r$, and total population $n$, the class departure rate is $\mu_r n_r/n$. The resulting class-count process is a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain).

### First come first served

↑ **Parent:** [Service discipline](#service-discipline)

A queue serves customers in arrival order. For multiple classes, retaining this order generally requires an ordered [multiclass single-server queue](#multiclass-single-server-queue) state, rather than only a vector of class counts.

## Server utilization

↑ **Parent:** [Queueing theory](queueing-theory.md)

The long-run fraction of time a work-conserving server is busy. Applying [Little's law](#little-s-law) to the server alone gives utilization equal to admitted [queue throughput](#queue-throughput) times mean [service time](#service-time). In a finite-buffer queue, the blocking probability must be included in that throughput.

### Finite-buffer server utilization

↑ **Parent:** [Server utilization](#server-utilization)

For a work-conserving single-server queue with independent Poisson arrivals, finite buffer and independent identically distributed admitted service times of mean $\mu$, [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages) give admitted rate $\lambda(1-P_n)$. [Little law](#little-s-law) for the server alone then gives the displayed busy fraction. The time parameter is the mean service duration, and need not be exponentially distributed.

## Queue throughput

↑ **Parent:** [Queueing theory](queueing-theory.md)

The long-run rate at which admitted customers complete service. In a stable queue without abandonment it equals the admitted arrival rate, which may be less than the offered rate because of blocking. [Little's law](#little-s-law) uses this actual rate for the chosen subsystem.

## Customer sojourn time

↑ **Parent:** [Queueing theory](queueing-theory.md)

The total time between admission to a selected queueing system and departure. It includes waiting and service if both are inside the chosen system, and only [service time](#service-time) if the selected system consists of the server alone. [Little's law](#little-s-law) relates its mean to mean population and admitted [queue throughput](#queue-throughput).

## Service time

↑ **Parent:** [Queueing theory](queueing-theory.md)

The time a customer occupies a server while receiving service. Its mean is a duration; its reciprocal is a service rate. An [exponential distribution](continuous-probability-distribution.md#exponential-distribution) is convenient for Markov queue models, but [Little's law](#little-s-law) can use a general finite mean.

## Quasireversibility

↑ **Parent:** [Queueing theory](queueing-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasireversibility)

In equilibrium, a queue is quasireversible when its present state is independent of subsequent arrival times and preceding departure times, for each customer class. For an [M-M-s queue](#m-m-s-queue), [detailed balance](markov-process.md#detailed-balance) and [time reversal of a continuous-time Markov chain](markov-process.md#time-reversal-of-a-continuous-time-markov-chain) show that past departures become future arrivals generated independently of the present state. This backward independence is useful in tandem calculations where downstream occupancy is determined by earlier departures.

## M-M-s queue

↑ **Parent:** [Queueing theory](queueing-theory.md)

Poisson arrivals of rate $\lambda$ and $s$ independent exponential servers of rate $\mu$ give a [birth-death chain](markov-process.md#birth-death-chain) with departure rate $\mu\min(n,s)$. The process is positive recurrent for $\lambda<s\mu$, null recurrent at equality, and transient above capacity.

### Burke theorem for a multi-server queue

↑ **Parent:** [M-M-s queue](#m-m-s-queue)

A stable equilibrium [M-M-s queue](#m-m-s-queue) has a [Poisson process](probability-theory.md#poisson-process) of departures with the same rate as its input. Its present population is also independent of past departures, a component of [quasireversibility](#quasireversibility). The [birth-death process](markov-process.md#birth-death-process) satisfies [detailed balance](markov-process.md#detailed-balance); reversed upward jumps have a constant arrival rate, so they are generated by an independent [Poisson process](probability-theory.md#poisson-process).

## Stochastic network

↑ **Parent:** [Queueing theory](queueing-theory.md)

A stochastic network combines resource constraints, routing, and random arrivals or service requirements. [Loss networks](#loss-network) reject requests that cannot acquire all required resources; [flow-level network models](#flow-level-network-model) let ongoing transfers share capacities.

### Sublinear path space for fluid queues

↑ **Parent:** [Stochastic network](#stochastic-network)

The useful infinite-horizon path space for a stable [queue](#queue-queueing-theory) is

$$
\mathcal C_0=\{f\in C([0,\infty)):f(0)=0,\ f(t)/(1+t)\to0\},\qquad
\|f\|_{\rm sl}=\sup_{t\geq0}|f(t)|/(1+t).
$$

For $\delta,\sigma>0$, the workload functional $R(f)=\sup_{t\geq0}(\sigma f(t)-\delta t)$ is finite and [continuous](calculus.md#continuous-function). Fix $f$, and choose $T\geq1$ so that $|\sigma f(t)|\leq\delta t/4$ for $t\geq T$. If $\|g-f\|_{\rm sl}<\delta/(4\sigma)$, then $\sigma g(t)-\delta t<0$ for $t\geq T$. Both suprema can thus be taken over $[0,T]$, where

$$
|R(g)-R(f)|\leq\sigma(1+T)\|g-f\|_{\rm sl}.
$$

Uniform convergence on bounded time intervals alone does not give this continuity: a pulse escaping to later times can produce a large workload while tending locally to zero.

#### Weighted cumulative-input topology for a slotted queue

↑ **Parent:** [Sublinear path space for fluid queues](#sublinear-path-space-for-fluid-queues)

For one-sided past inputs, let $A_n(a)=\sum_{j=0}^{n-1}a_{-j}$ and $A_0=0$. The displayed [metric](topological-analysis.md#metric) controls cumulative differences over every past window, including the latest arrival. On the affine class $A_n(a)/n\to\lambda<c$, the [queue workload](#workload-of-a-queue) $Q(a,c)=\sup_{n\geq0}(A_n(a)-cn)$ is locally [Lipschitz continuous](real-analysis.md#lipschitz-continuity). To prove this, choose $\varepsilon=(c-\lambda)/4$ and $N\geq1$ such that $A_n(a)/n\leq\lambda+\varepsilon$ for $n\geq N$. If $d_\#(a,b)<\varepsilon/2$, then $A_n(b)-cn\leq n(\lambda+2\varepsilon-c)<0$ for all such $n$. Both suprema reduce to $0\leq n<N$, and their difference is at most $(N+1)d_\#(a,b)$. Ignoring the latest coordinate makes this assertion false for a post-slot [workload of a queue](#workload-of-a-queue).

#### Self-similar Gaussian workload rate

↑ **Parent:** [Sublinear path space for fluid queues](#sublinear-path-space-for-fluid-queues)

Let a centered [Gaussian process](stochastic-process.md#gaussian-process) $Z$ satisfy $Z(a\,\cdot)\overset d=a^H Z$ with $0<H<1$, and suppose $Z/\sqrt L$ has a [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) in the [sublinear path space for fluid queues](#sublinear-path-space-for-fluid-queues), with speed $L$ and [good rate function](convergence-of-random-variables.md#good-rate-function) $I$. For $\delta,\sigma>0$, put $r=\sup_{t\geq0}(\sigma Z(t)-\delta t)$ and $\kappa=2(1-H)$. Self-similarity gives $Z(N\,\cdot)/N\overset d=Z/\sqrt{N^\kappa}$. Time substitution and the [contraction principle for large deviations](convergence-of-random-variables.md#contraction-principle-for-large-deviations) therefore give an LDP for $r/N$ with speed $N^\kappa$ and

$$
J(q)=\inf\{I(f):\sup_{t\geq0}(\sigma f(t)-\delta t)=q\}.
$$

The same family $r/(aN)$ has [rate function](convergence-of-random-variables.md#rate-function) $J(aq)$ by contraction, and $a^\kappa J(q)$ by replacing $N$ with $aN$ and expressing the speed again as $N^\kappa$. Uniqueness of a [rate function](convergence-of-random-variables.md#rate-function) gives $J(aq)=a^\kappa J(q)$, hence $J(q)=q^\kappa J(1)$ for $q>0$, with $J(0)=0$.

### Closed migration process

↑ **Parent:** [Stochastic network](#stochastic-network)

A closed migration process is a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) of populations moving between colonies with a conserved total number of individuals. A colony containing $k$ individuals has departure rate $\phi_j(k)$, with $\phi_j(0)=0$, and each departure chooses its next colony using a fixed routing [matrix](vector-space.md#matrix). Its colony populations can represent stages of a service system, including an idle stage.

// Target: probability-and-statistics.bigb

#### Blocking probability in a finite-line sequential-service network

↑ **Parent:** [Closed migration process](#closed-migration-process)

Represent $N$ telephone lines by a [closed migration process](#closed-migration-process) with free-line, operator and automated-service colonies. Accepted arrivals have rate $\nu$ when a free line exists, $c$ operators complete at rate $\lambda\min(k,c)$, and $i$ automated calls complete at rate $\mu i$. Define $D_c(k)=\prod_{h=1}^k\min(h,c)$ and

$$
H_c(n)=\sum_{i=0}^n\frac{(\nu/\lambda)^{n-i}(\nu/\mu)^i}{D_c(n-i)i!}.
$$

The [product-form stationary distribution of a closed migration process](#product-form-stationary-distribution-of-a-closed-migration-process) and [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages) give the displayed blocking probability. This extends a single-operator model without treating the independent operators as a server with rate $c\lambda$ when fewer than $c$ calls are present.

// Target: probability-and-statistics.bigb

##### Stationary flow conservation in a finite-line switchboard

↑ **Parent:** [Blocking probability in a finite-line sequential-service network](#blocking-probability-in-a-finite-line-sequential-service-network)

In a one-operator [closed migration process](#closed-migration-process) representing a finite-line switchboard, let $K$ count calls waiting for or receiving the operator's connection service and let $I$ count connected calls. At a [stationary distribution](markov-process.md#stationary-distribution), the expected drift of $K$ is $\nu\Pr\{K+I<N\}-\lambda\Pr\{K>0\}=0$, and that of $I$ is $\lambda\Pr\{K>0\}-\mu\mathbb E[I]=0$. [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages) identifies the full-state probability with $P_{\rm loss}$. Thus the accepted arrival rate, operator throughput and completed-call rate coincide. This is a useful independent check on the [product-form stationary distribution of a closed migration process](#product-form-stationary-distribution-of-a-closed-migration-process).

#### Product-form stationary distribution of a closed migration process

↑ **Parent:** [Closed migration process](#closed-migration-process)

For an irreducible [closed migration process](#closed-migration-process) with finite population $N$, positive departure rates and routing matrix $P$, choose positive traffic weights satisfying $\theta=\theta P$. On $\sum_jn_j=N$, its [stationary distribution](markov-process.md#stationary-distribution) has the displayed form. For a predecessor $m=n+e_j-e_k$, its weighted transition into $n$ is $\pi(n)(\theta_j/\theta_k)P_{jk}\phi_k(n_k)$. Summing over $j$ gives $\pi(n)\phi_k(n_k)$ by the traffic equation, and summing over $k$ proves [global balance for a continuous-time Markov chain](markov-process.md#global-balance-for-a-continuous-time-markov-chain). The distribution need not satisfy [detailed balance](markov-process.md#detailed-balance).

// Target: probability-and-statistics.bigb

### Product-form stationary distribution of a multiclass queueing network

↑ **Parent:** [Stochastic network](#stochastic-network)

Connect [multiclass single-server queues](#multiclass-single-server-queue) by Markovian routing. Each node must either have common exponential service parameters across its classes or use a [symmetric service discipline](#symmetric-service-discipline). If the [traffic equations for a multiclass queueing network](#traffic-equations-for-a-multiclass-queueing-network) give loads $\rho_j=\sum_r\lambda_{jr}/\mu_{jr}<1$, its equilibrium word law is the product of the individual queue laws. Queue populations are independent at a fixed equilibrium time. A proof reverses routing with $p_{ba}^*=\lambda_a p_{ab}/\lambda_b$, external arrivals with $\nu_a^*=\lambda_a p_{a0}$, and exits with $p_{a0}^*=\nu_a/\lambda_a$, and interchanges the insertion and service position rules. Weight ratios verify each reversed transition, and the traffic equations match total rates. This is a [quasireversibility](#quasireversibility) construction. A standard ordered-queue formulation is described in [Walton's paper on multiclass queueing networks, Section 2](https://arxiv.org/pdf/0809.2697).

### Traffic equations for a multiclass queueing network

↑ **Parent:** [Stochastic network](#stochastic-network)

For queue-class pairs $a$, external arrival rates $\nu_a$, and routing probabilities $p_{ab}$, the effective throughputs satisfy $\lambda_a=\nu_a+\sum_b\lambda_b p_{ba}$. In an open network with routing [spectral radius](analysis.md#spectral-radius) less than one, $\lambda=(I-P^T)^{-1}\nu$ is the unique nonnegative solution. Summing gives $\sum_a\lambda_a p_{a0}=\sum_a\nu_a$, balancing total entrances and exits.

### Congestion control

↑ **Parent:** [Stochastic network](#stochastic-network)

Congestion control adjusts user transmission rates in response to load signals from shared resources. A resource can compute its price from local aggregate load, while each user sums prices along its route. [Primal congestion potential](#primal-congestion-potential) and [dual congestion potential](#dual-congestion-potential) formulations explain equilibrium and stability for suitable monotone response functions.

#### User-network decomposition of concave utility maximization

↑ **Parent:** [Congestion control](#congestion-control)

Maximize a sum of increasing strictly concave utilities $U_r(x_r)$ subject to $Ax\leq C$, $x\geq0$. Suppose capacities are positive, every route is nonempty, and $U_r'(0)=\infty$. At its unique positive optimizer $x^*$, the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) give nonnegative [resource congestion prices](#resource-congestion-price) $p^*$ and [route congestion prices](#route-congestion-price) $y_r^*=U_r'(x_r^*)$. Choosing $\nu_r^*=x_r^*e^{y_r^*}$ makes each user maximize $U_r(\nu_r e^{-y_r^*})-y_r^*\nu_r e^{-y_r^*}$ at $\nu_r^*$. It also makes $x^*$ maximize the [entropy maximization for loss-network occupancy](#entropy-maximization-for-loss-network-occupancy) objective, since its gradient is $\log(\nu_r^*/x_r^*)=(A^Tp^*)_r$. Thus user and network optima implement the same system optimum.

#### Resource congestion price

↑ **Parent:** [Congestion control](#congestion-control)

A resource congestion price signals scarcity at a capacity-constrained link. Under [multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics), its increase indicates excess demand and its decrease indicates spare capacity. A route pays the sum of these prices, its [route congestion price](#route-congestion-price). A zero resource congestion price at an optimum satisfies [complementary slackness](mathematical-optimization.md#complementary-slackness) with possible spare capacity.

##### Route congestion price

↑ **Parent:** [Resource congestion price](#resource-congestion-price)

The total price seen by a route is the sum of [resource congestion prices](#resource-congestion-price) on its links. With [weighted logarithmic utility](convex-optimization.md#weighted-logarithmic-utility) $w_r\log x_r$, maximizing utility minus linear expenditure gives the demand $x_r=w_r/p_r$. This relation links user decisions to [multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics).

#### Multiplicative resource-price dynamics

↑ **Parent:** [Congestion control](#congestion-control)

For route prices $p=A^T\mu$, logarithmic users demand $x_r=w_r/p_r$, while resource prices adjust as

$$
\dot\mu_j=\kappa_j\mu_j[(Ax)_j-C_j].
$$

This model raises prices under excess demand and lowers them under spare capacity. Positive capacities and nonempty routes are standard well-definedness assumptions. Positive initial prices approach the dual optimum; zero prices are invariant and can create [boundary equilibria of multiplicative price dynamics](#boundary-equilibrium-of-multiplicative-price-dynamics) that overload a resource.

##### Increasing-supply resource-price dynamics

↑ **Parent:** [Multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics)

Routes with positive logarithmic utility weights choose rates inversely proportional to their total resource price. Each resource changes its price multiplicatively according to demand minus its increasing supply. For continuous strictly increasing $q_j$ with $q_j(0)=0$, the potential $V=\sum_r w_r\log(\sum_{j\in r}\mu_j)-\sum_j\int_0^{\mu_j}q_j(u)du$ is strictly concave and has nonnegative derivative along the dynamics. [Positive-price convergence for increasing resource supplies](#positive-price-convergence-for-increasing-resource-supplies) requires positivity on used resources; zero-price faces are invariant.

###### Positive-price convergence for increasing resource supplies

↑ **Parent:** [Increasing-supply resource-price dynamics](#increasing-supply-resource-price-dynamics)

For finite nonempty routes and positive weights, the potential of [increasing-supply resource-price dynamics](#increasing-supply-resource-price-dynamics) has a unique maximum. Increasing supplies give a linear penalty at large prices, so its superlevel sets are compact, and logarithmic route terms exclude zero route totals. Used resources have uniformly positive demand on a trapped set; a sufficiently small positive price therefore increases, giving a positive lower bound. The potential derivative is $\sum_j\kappa_j\mu_j(\partial_jV)^2$. It has finite integral and is uniformly continuous, so it tends to zero by [uniformly continuous integrable functions vanish at infinity](topological-analysis.md#uniformly-continuous-integrable-functions-vanish-at-infinity). Every limit point then satisfies the unique stationary equations. Unused resource prices decay to zero. Only continuity and strict increase of the supply functions are needed.

###### Boundary equilibria of multiplicative resource prices

↑ **Parent:** [Increasing-supply resource-price dynamics](#increasing-supply-resource-price-dynamics)

In [multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics), a zero price remains zero even if demand exceeds supply there. For one route using two resources, unit weight and supplies $q_j(u)=u$, both $(0,1)$ and $(1,0)$ are equilibria, while the unique positive equilibrium is $(1/\sqrt2,1/\sqrt2)$. Thus uniqueness on the positive price domain cannot be extended to every nonnegative price trajectory without an extra boundary rule.

##### Relative-entropy Lyapunov function for resource prices

↑ **Parent:** [Multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics)

For a complementary-slackness optimum $\mu^*$, define

$$
L(\mu)=\sum_j\kappa_j^{-1}[\mu_j-\mu_j^*-\mu_j^*\log(\mu_j/\mu_j^*)],
$$

interpreting a zero-reference summand as $\mu_j/\kappa_j$. This is a nonnegative generalized reverse-relative-entropy expression for positive resource prices. Along [multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics), with $p=A^T\mu$ and $g=Ax-C$,

$$
\dot L=-\sum_r\frac{w_r(p_r-p_r^*)^2}{p_rp_r^*}+\mu^Tg(\mu^*)\leq0.
$$

Its sublevel bounds keep all route prices away from zero and permit the [LaSalle invariance principle](dynamical-systems.md#lasalle-s-invariance-principle), including optima with some zero individual prices.

###### Full-row-rank convergence of multiplicative resource prices

↑ **Parent:** [Relative-entropy Lyapunov function for resource prices](#relative-entropy-lyapunov-function-for-resource-prices)

For [multiplicative resource-price dynamics](#multiplicative-resource-price-dynamics) with positive capacities, nonempty routes and strictly positive initial prices, full row rank of the [link-route incidence matrix](#link-route-incidence-matrix) makes

$$
V(\mu)=\sum_rw_r\log(A^T\mu)_r-C^T\mu
$$

strictly concave. There is a unique optimizing price vector, possibly on the boundary, and the [relative-entropy Lyapunov function for resource prices](#relative-entropy-lyapunov-function-for-resource-prices) proves convergence to it. Row-rank deficiency still gives unique optimal route prices and rates, but resource prices may depend on the initial state. Full column rank alone and unrestricted zero initial prices do not yield the same uniqueness theorem.

#### Boundary equilibrium of multiplicative price dynamics

↑ **Parent:** [Congestion control](#congestion-control)

In $\dot\mu_j=\kappa_j\mu_j(y_j-q_j(\mu_j))$, a zero price remains zero even if resource demand exceeds supply. Such a boundary equilibrium need not minimize the [dual congestion potential](#dual-congestion-potential); uniqueness of its positive minimizer does not imply uniqueness on the nonnegative orthant.

#### Dual congestion potential

↑ **Parent:** [Congestion control](#congestion-control)

For strictly increasing continuous supply functions $q_j$ with $q_j(0)=0$, this potential is strictly convex on prices with positive route-price sums. Its minimum is interior for every used resource and gives the unique positive-price equilibrium. Multiplicative price dynamics can also have [boundary equilibria of multiplicative price dynamics](#boundary-equilibrium-of-multiplicative-price-dynamics) if zero prices are permitted.

#### Primal congestion potential

↑ **Parent:** [Congestion control](#congestion-control)

This potential subtracts integrated resource prices from [weighted logarithmic utility](convex-optimization.md#weighted-logarithmic-utility). Continuous nonnegative nondecreasing prices make it strictly concave on positive rates. If every route meets a resource with a nonzero price function, its superlevel sets are compact and its maximizer is unique. The rate adjustment $\dot x_r=\kappa_rx_r\partial_rU$ increases it strictly away from equilibrium.

##### Global convergence of primal congestion control

↑ **Parent:** [Primal congestion potential](#primal-congestion-potential)

Assume finitely many nonempty routes, positive weights and adjustment rates, and continuous nonnegative nondecreasing resource prices. Each route must meet a resource whose price is positive somewhere. Then the [primal congestion potential](#primal-congestion-potential) has compact superlevel sets inside the positive orthant and a unique maximum. Along [gradient flow with diagonal mobility](analysis.md#gradient-flow-with-diagonal-mobility), $\dot U=\sum_r\kappa_rx_r(\partial_rU)^2$. The substitution $x_r=\kappa_rz_r^2/4$ makes the dynamics ordinary [gradient flow](analysis.md#gradient-flow) ascent for $V(z)=U((\kappa_rz_r^2/4)_r)$. This $V$ is [strictly concave](real-analysis.md#strictly-concave-function): the logarithmic terms are strictly concave, and each integrated price is convex and nondecreasing, composed with a convex quadratic load. Thus its continuous gradient is monotone decreasing, which proves uniqueness of trajectories even without differentiability of the prices. Compact trapping and the dissipation identity force every limit point to be the unique maximizer. If every price on some route vanishes identically, its rate instead grows linearly and there is no equilibrium.

###### Square-root coordinates for primal congestion control

↑ **Parent:** [Global convergence of primal congestion control](#global-convergence-of-primal-congestion-control)

For positive rates in [congestion control](#congestion-control), put $x_r=\kappa_rz_r^2/4$ and $V(z)=U(x(z))$, where $U$ is the [primal congestion potential](#primal-congestion-potential). The equation $\dot x_r=\kappa_rx_r\partial_rU$ becomes $\dot z_r=\partial_rV$. Positive logarithmic utility weights make $\sum_rw_r\log(\kappa_rz_r^2/4)$ strictly concave on the positive orthant. Each integrated nonnegative nondecreasing resource price is a convex nondecreasing function of its load; composing it with the convex quadratic load in $z$ preserves convexity. Hence $V$ is a [strictly concave function](real-analysis.md#strictly-concave-function), even for prices that are merely continuous. For two solutions, $\frac12\frac d{dt}\|z-\widetilde z\|^2=(z-\widetilde z)\cdot[\nabla V(z)-\nabla V(\widetilde z)]\leq0$. This proves uniqueness of the flow without assuming local Lipschitz continuity of the price functions.

### Effective bandwidth

↑ **Parent:** [Stochastic network](#stochastic-network)

Effective bandwidth describes the exponential-moment traffic rate at a specified time scale and tail parameter. Independent sources have additive effective bandwidths. The [Chernoff bound](probability-inequality.md#chernoff-bound) connects their sum to overflow bounds. For a single time unit, the small-parameter limit is the [expected value](probability-theory.md#expected-value) and the large-parameter limit is the [essential supremum](measure-theory.md#essential-supremum), with appropriate moment or extended-value conventions.

#### Poisson effective bandwidth

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

For independent [Poisson](discrete-probability-distribution.md#poisson-distribution) arrival counts of mean $\nu$ per slot, with one unit of work per arrival, the [cumulant-generating function](probability-theory.md#cumulant-generating-function) is $\nu(e^\theta-1)$. Its [effective bandwidth](#effective-bandwidth) is the displayed expression. If $c>\nu$, the equation $\nu(e^\theta-1)=c\theta$ has a unique positive root: strict [convexity](real-analysis.md#convex-function), negative initial derivative after subtracting $c\theta$, and divergence to infinity prove existence and uniqueness. Independent Poisson streams combine by replacing $\nu$ with the sum of their intensities.

#### Bernoulli effective bandwidth

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

Independent slots carry either zero work or $r>0$ units, the latter with probability $p$. Their [effective bandwidth](#effective-bandwidth) is the displayed expression, with small-parameter limit $pr$ and large-parameter limit $r$ when $0<p<1$. For $pr<c<r$, the positive root of $\log(1-p+pe^{\theta r})=c\theta$ determines the optimized exponential overflow bound. In the special case $r=2,c=1,p<1/2$, the stationary [queue workload](#workload-of-a-queue) is geometric with ratio $p/(1-p)$, and the root is $\theta_* =\log((1-p)/p)$, giving exactly $\mathbb P(Q\geq k)=e^{-\theta_*k}$ for integers $k\geq0$.

#### Exponential workload bound from cumulative arrival moments

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

Let a slotted [queue](#queue-queueing-theory) have stationary input, constant service $c$, and finite stationary [queue workload](#workload-of-a-queue) $Q=\sup_{n\geq0}(A_n-cn)$. Write $K_n(\theta)=\log\mathbb E e^{\theta A_n}$ for its past cumulative arrivals. The [union bound](probability-inequality.md#boole-s-inequality) and [Chernoff bound](probability-inequality.md#chernoff-bound) give the displayed inequality for $B>0$. It requires no temporal [independence](random-variable.md#independent-random-variables). If each $K_n(\theta)$ is finite and $K_n(\theta)/n\to\kappa(\theta)<c\theta$, the series is finite: its tail is bounded by a geometric series. Consequently $\limsup_{L\to\infty}L^{-1}\log\mathbb P(Q>Lb)\leq-\theta b$ for $b>0$. The condition is that the asymptotic [effective bandwidth](#effective-bandwidth) $\kappa(\theta)/\theta$ be less than service capacity.

#### Continuous-time exponential workload bound

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

For a nondecreasing process $A$ with [stationary increments](stochastic-process.md#stationary-increments) and [independent increments](stochastic-process.md#independent-increments), suppose $\mathbb E e^{\theta A(t)}=e^{t\Lambda(\theta)}$. If $\Lambda(\theta)\leq C\theta$, then $e^{\theta(A(t)-Ct)}$ is a nonnegative [supermartingale](martingale.md#supermartingale). Applying the [maximal inequality for a nonnegative supermartingale](martingale.md#maximal-inequality-for-a-nonnegative-supermartingale) up to time $T$ and then letting $T\to\infty$ gives

$$
\mathbb P\!\left(\sup_{t\geq0}(A(t)-Ct)\geq b\right)\leq e^{-\theta b}.
$$

The stationary workload of a stable [queue](#queue-queueing-theory) fed by $A$ has this supremum distribution, using the past input and [stationary increments](stochastic-process.md#stationary-increments) and [independent increments](stochastic-process.md#independent-increments). For [independent](random-variable.md#independent-random-variables) flows, the constraint is $\sum_j a_j(\theta)\leq C$, where $a_j(\theta)=\Lambda_j(\theta)/\theta$ is the long-time [effective bandwidth](#effective-bandwidth). The result bounds a continuous-time supremum directly; a one-time [Chernoff bound](probability-inequality.md#chernoff-bound) by itself does not do that.

#### Monotonicity and bounds of effective bandwidth

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

For $s>0$ in the finite [moment-generating function](probability-theory.md#moment-generating-function) domain and integrable $X$, [Jensen inequality](real-analysis.md#jensen-s-inequality) gives the lower bound and $X\le\operatorname{ess\,sup}X$ almost surely gives the upper bound. The [Holder inequality](functional-analysis.md#holder-inequality) makes $K(s)=\log\mathbb Ee^{sX}$ convex with $K(0)=0$. Thus $K(t)\le(t/s)K(s)$ for $0<t<s$, and the [effective bandwidth](#effective-bandwidth) is nondecreasing. It need not be strictly increasing: deterministic traffic gives a constant bandwidth. Infinite peaks or exponential moments require extended-value conventions.

#### Workload Chernoff bound for independent increments

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

For independent identically distributed traffic increments and constant service $C$, let $a(s)=\mathbb E[e^{s(X-C)}]$. If $a(s)<1$, apply the [Chernoff bound](probability-inequality.md#chernoff-bound) at each candidate workload window and sum a geometric series. This bounds the stationary random-walk supremum. It explains the [effective bandwidth](#effective-bandwidth) criterion $\alpha(s)<C$ and distinguishes a queue's infinite-horizon overflow event from a single-window traffic event.

#### Mean and peak limits of effective bandwidth

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

For nonnegative traffic with exponential moments near zero, its [effective bandwidth](#effective-bandwidth) has expansion $\mathbb EX+s\operatorname{Var}(X)/2+O(s^2)$. For bounded traffic with essential supremum $M$, it increases toward $M$: the exponential moment is at most $e^{sM}$, and any positive probability of $X>a$ gives $\alpha(s)\geq a+s^{-1}\log\mathbb P(X>a)$. Unbounded traffic has an infinite large-parameter limit when all positive exponential moments exist; a finite moment domain must be respected.

#### Gaussian effective bandwidth

↑ **Parent:** [Effective bandwidth](#effective-bandwidth)

For a [normal distribution](probability-theory.md#normal-distribution) $N(\lambda,\sigma^2)$, the logarithm of its [moment-generating function](probability-theory.md#moment-generating-function) is $s\lambda+s^2\sigma^2/2$. Dividing by $s>0$ gives its [effective bandwidth](#effective-bandwidth). Independent demands add these bandwidths. For total mean $m$ and positive total [variance](variance.md) $v$, optimizing a [Chernoff bound](probability-inequality.md#chernoff-bound) with target $e^{-\gamma}$, $\gamma>0$, yields the sufficient margin $C\geq m+\sqrt{2\gamma v}$.

##### Exact Gaussian overflow constraint

↑ **Parent:** [Gaussian effective bandwidth](#gaussian-effective-bandwidth)

For a [normal distribution](probability-theory.md#normal-distribution) with mean $m$, positive [variance](variance.md) $v$, and $\gamma>0$, the target $\mathbb P(X\geq C)\leq e^{-\gamma}$ is equivalent to the displayed constraint, where $\Phi$ is the [standard normal distribution function](probability-theory.md#standard-normal-distribution-function). This follows from $\mathbb P(X\geq C)=1-\Phi((C-m)/\sqrt v)$ and strict monotonicity of $\Phi$. Unlike the sufficient [Chernoff bound](probability-inequality.md#chernoff-bound) margin $\sqrt{2\gamma v}$, this constraint is necessary as well as sufficient. The exact quantile can be negative when $e^{-\gamma}>1/2$.

###### Zero-variance boundary of an overflow constraint

↑ **Parent:** [Exact Gaussian overflow constraint](#exact-gaussian-overflow-constraint)

If a random variable has [variance](variance.md) zero and mean $m$, it equals $m$ almost surely. For a target probability strictly between zero and one, $\mathbb P(X\geq C)$ meets the target exactly when $m<C$. Substituting zero variance into a positive-variance non-strict quantile constraint incorrectly includes $m=C$, where the overflow probability is one. The distinction comes from the atom at the threshold.

### Open migration process

↑ **Parent:** [Stochastic network](#stochastic-network)

An open migration process is a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) of colony populations with external [Poisson processes](probability-theory.md#poisson-process), state-dependent departure rates, and fixed probabilistic routing that eventually exits the system. Its [traffic equations of an open migration process](#traffic-equation-of-an-open-migration-process) determine the total arrival rates, and its equilibrium has a [product-form stationary distribution of an open migration process](#product-form-stationary-distribution-of-an-open-migration-process) when the normalizing sums are finite.

#### Time reversal of an open migration process

↑ **Parent:** [Open migration process](#open-migration-process)

For a stationary [open migration process](#open-migration-process) with local total departure rate $\phi_i(n_i)$ and traffic rates $\alpha_i$, adjacent product-weight ratios give the displayed reversed parameters. The [traffic equations of an open migration process](#traffic-equation-of-an-open-migration-process) make each reversed routing row sum to one, while total external arrival rates agree in the two directions. Thus the reversed process has the same local departure functions and is again an open migration process.

##### Poisson migration stream without a return path

↑ **Parent:** [Time reversal of an open migration process](#time-reversal-of-an-open-migration-process)

If no directed routing path returns from $k$ to $j$, the set of colonies reachable from $k$ has no outgoing edge to its complement. The complement is an autonomous [open migration process](#open-migration-process), and the marked $j\to k$ transition is an exit from it. In [time reversal of an open migration process](#time-reversal-of-an-open-migration-process), that exit is a state-independent Poisson immigration channel of rate $\alpha_jp_{jk}$. Reversing a stationary two-sided [Poisson process](probability-theory.md#poisson-process) preserves its law, proving the forward stream is Poisson. This argument does not assert Poisson internal streams for networks with feedback.

#### Service-capacity allocation in an open migration process

↑ **Parent:** [Open migration process](#open-migration-process)

For positive traffic rates in single-server colonies, a total service budget $F>\sum_j\alpha_j$ minimizes the stationary mean population when the spare rates $\phi_j-\alpha_j$ are proportional to $\sqrt{\alpha_j}$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) proves the optimum directly.

#### Product-form stationary distribution of an open migration process

↑ **Parent:** [Open migration process](#open-migration-process)

For an [open migration process](#open-migration-process), colony $j$ with population $k$ has total departure rate $\phi_j(k)$. Its stationary weight is $b_j(k)=\alpha_j^k/\prod_{h=1}^k\phi_j(h)$. The colony weights factor independently and normalize when $\sum_{k\geq0}b_j(k)<\infty$ for every colony. [Global balance for a continuous-time Markov chain](markov-process.md#global-balance-for-a-continuous-time-markov-chain) proves the formula even when routing is not reversible.

#### Traffic equation of an open migration process

↑ **Parent:** [Open migration process](#open-migration-process)

With row vectors, external arrival rates $\nu$ and transient routing [matrix](vector-space.md#matrix) $P$, the total arrival rates satisfy $\alpha=\nu+\alpha P=\nu(I-P)^{-1}$. These include all internal migrations and do not depend on colony service speeds.

### Flow-level network model

↑ **Parent:** [Stochastic network](#stochastic-network)

A flow-level model treats each document transfer as a flow whose rate depends on the current occupancy and resource capacities. With independent [Poisson processes](probability-theory.md#poisson-process) for arrivals and independent unit-mean [exponential distributions](continuous-probability-distribution.md#exponential-distribution) for sizes, a route's total completion rate equals its allocated aggregate service.

#### Balance function of a flow-level network

↑ **Parent:** [Flow-level network model](#flow-level-network-model)

A positive balance function $\Phi$ expresses each active route's aggregate service as this ratio. With independent Poisson arrivals and exponential document sizes, [detailed balance](markov-process.md#detailed-balance) yields stationary weights $\Phi(n)\prod_r\rho_r^{n_r}$, provided their sum is finite.

##### Stationary law of a proportionally fair four-cycle

↑ **Parent:** [Balance function of a flow-level network](#balance-function-of-a-flow-level-network)

The [proportionally fair allocation on a four-cycle](convex-optimization.md#proportionally-fair-allocation-on-a-four-cycle) has aggregate service $P/(P+Q)$ on each active odd route and $Q/(P+Q)$ on each active even route. With Poisson arrival rates $\nu_r$ and exponential document-size parameters $\mu_r$, the departure intensity is $\mu_rn_rx_r$. The adjacent ratios of the displayed [binomial coefficient](combinatorics.md#binomial-coefficient) weight cancel those intensities in [detailed balance](markov-process.md#detailed-balance), with $\rho_r=\nu_r/\mu_r$.

###### Four-cycle partition function

↑ **Parent:** [Stationary law of a proportionally fair four-cycle](#stationary-law-of-a-proportionally-fair-four-cycle)

For offered loads on consecutive routes $a,b,c,d$ of the reversible [proportionally fair allocation on a four-cycle](convex-optimization.md#proportionally-fair-allocation-on-a-four-cycle), the normalizing sum of the [stationary distribution](markov-process.md#stationary-distribution) is

$$
B=\frac{(1-a)(1-b)(1-c)(1-d)-abcd}{(1-a-b)(1-a-d)(1-c-b)(1-c-d)}.
$$

This formula applies in the [stability region for the reversible four-cycle flow network](#stability-region-for-the-reversible-four-cycle-flow-network). Grouping populations on opposite routes gives $\sum_{s,t}\binom{s+t}{s}h_s(a,c)h_t(b,d)$, where $h_s(a,c)=\sum_{i=0}^sa^ic^{s-i}$. For distinct opposite loads, substituting $h_s=(a^{s+1}-c^{s+1})/(a-c)$ and summing the four geometric generating series proves the formula; [continuity](calculus.md#continuous-function) covers coincident loads. If all four loads equal $z<1/2$, it reduces to $(1-2z+2z^2)/(1-2z)^3$.

###### Stability region for the reversible four-cycle flow network

↑ **Parent:** [Stationary law of a proportionally fair four-cycle](#stationary-law-of-a-proportionally-fair-four-cycle)

Group the normalizing sum by its odd and even flow counts. The coefficient sums are $h_p(\rho_1,\rho_3)=\sum_{i=0}^p\rho_1^i\rho_3^{p-i}$ and the analogous $h_q$ for even routes. If $a$ and $b$ are the two maximum loads, then $a^p\leq h_p\leq(p+1)a^p$ and similarly for $b$. The generating identity $\sum_{p,q}\binom{p+q}{p}a^pb^q=(1-a-b)^{-1}$ proves necessity and sufficiency of the displayed strict inequality. It is equivalent to strictly subunit offered load on each of the four resources.

#### Linear flow network

↑ **Parent:** [Flow-level network model](#flow-level-network-model)

A linear flow network has a through route using all resources and one local route for each individual resource. Under [proportional fairness](convex-optimization.md#proportional-fairness) with unit resource capacities, the per-flow through rate is $1/N$, where $N$ is the total number of flows. Its exponential-document model has a [balance function of a flow-level network](#balance-function-of-a-flow-level-network) given by $\binom{N}{n_0}$.

##### Stationary law of a linear flow network

↑ **Parent:** [Linear flow network](#linear-flow-network)

For the [proportionally fair allocation on a linear flow network](#proportionally-fair-allocation-on-a-linear-flow-network), independent Poisson flow arrivals at rates $\nu_r$ and exponential document sizes of rates $\mu_r$ give a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) with departures $\mu_rn_rx_r(n)$. Put $\rho_r=\nu_r/\mu_r$. Under $\rho_0+\rho_i<1$ for each local route, the normalizing constant is $Z=(1-\rho_0)^{I-1}/\prod_i(1-\rho_0-\rho_i)$. The [binomial coefficient](combinatorics.md#binomial-coefficient) weight has adjacent-state ratios equal to the aggregate service rates, proving [detailed balance](markov-process.md#detailed-balance). For more general network topologies, [proportional fairness](convex-optimization.md#proportional-fairness) need not give this reversible product form.

###### Local-count independence in a linear flow network

↑ **Parent:** [Stationary law of a linear flow network](#stationary-law-of-a-linear-flow-network)

Summing the [stationary law of a linear flow network](#stationary-law-of-a-linear-flow-network) over its through-flow count gives independent local [geometric distributions](discrete-probability-distribution.md#geometric-distribution) with ratios $q_i=\rho_i/(1-\rho_0)$. This gives the displayed means. The local counts are independent of one another in this marginal distribution; the through count is generally dependent on them. The [independence](random-variable.md#independent-random-variables) is a stationary distributional fact, not an assertion that their dynamics evolve independently.

##### Proportionally fair allocation on a linear flow network

↑ **Parent:** [Linear flow network](#linear-flow-network)

On unit-capacity links $1,\ldots,I$, route zero uses every link and route $i$ uses only link $i$. Let $N=\sum_{r=0}^I n_r$ and $M=\sum_{i=1}^I n_i$. Under [proportional fairness](convex-optimization.md#proportional-fairness), every active local route has $n_0x_0+n_ix_i=1$. Maximizing $n_0\log w_0+M\log(1-w_0)$ for $w_0=n_0x_0$ gives $w_0=n_0/N$ and the displayed per-flow rates on active routes. At the empty state departures vanish, and rates of absent flows may be set to zero.

##### Two-resource linear flow network

↑ **Parent:** [Linear flow network](#linear-flow-network)

A [two-resource linear flow network](#two-resource-linear-flow-network) has one local route on each of two resources and one through route using both. With unit capacities and [proportional fairness](convex-optimization.md#proportional-fairness), its exponential-document [flow-level network model](#flow-level-network-model) has the [stationary law of a two-resource linear flow network](#stationary-law-of-a-two-resource-linear-flow-network). The local counts are independent in equilibrium despite their dependence on the shared through-route count.

###### Stationary law of a two-resource linear flow network

↑ **Parent:** [Two-resource linear flow network](#two-resource-linear-flow-network)

For route offered loads $\rho_1,\rho_2,\rho_0$, the [balance function of a flow-level network](#balance-function-of-a-flow-level-network) $\Psi(a,b,c)=\binom{a+b+c}{c}$ gives the [stationary distribution](markov-process.md#stationary-distribution)

$$
\pi(a,b,c)=B\binom{a+b+c}{c}\rho_1^a\rho_2^b\rho_0^c.
$$

The [negative binomial series](real-analysis.md#negative-binomial-series) sums over $c$, and two geometric sums give $B=(1-\rho_0-\rho_1)(1-\rho_0-\rho_2)/(1-\rho_0)$ under the [stability conditions for a two-resource linear flow network](#stability-conditions-for-a-two-resource-linear-flow-network).

###### Local-count independence with through-flow dependence

↑ **Parent:** [Stationary law of a two-resource linear flow network](#stationary-law-of-a-two-resource-linear-flow-network)

In the [stationary law of a two-resource linear flow network](#stationary-law-of-a-two-resource-linear-flow-network), the local counts are independent geometric variables with parameters $q_i=\rho_i/(1-\rho_0)$. Conditional on local counts $a,b$, the through count has a [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) with mean $\rho_0(a+b+1)/(1-\rho_0)$. With positive loads, it is correlated with each local count, even though those two local counts are independent. Degenerate zero-load cases must be distinguished from the positive-load assertion.

###### Stability conditions for a two-resource linear flow network

↑ **Parent:** [Stationary law of a two-resource linear flow network](#stationary-law-of-a-two-resource-linear-flow-network)

The [stationary law of a two-resource linear flow network](#stationary-law-of-a-two-resource-linear-flow-network) is normalizable exactly when

$$
\rho_1+\rho_0<1,\qquad\rho_2+\rho_0<1.
$$

These are the strict offered-load constraints on the two unit-capacity resources. Summing first over the through-route count reduces normalization to two [geometric series](real-analysis.md#geometric-series), which diverge at equality. With positive arrival rates, the nonexplosive [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) is then positive recurrent.

###### Proportionally fair allocation on a two-resource linear network

↑ **Parent:** [Two-resource linear flow network](#two-resource-linear-flow-network)

For local counts $a,b$, through count $c$, and $N=a+b+c>0$, [proportional fairness](convex-optimization.md#proportional-fairness) gives aggregate through service $c/N$. Every active local route receives aggregate service $(a+b)/N$, divided equally among its active flows. Inactive routes receive zero aggregate service. This maximizes [weighted logarithmic utility](convex-optimization.md#weighted-logarithmic-utility) subject to both unit-capacity constraints.

#### Reversible four-cycle flow model

↑ **Parent:** [Flow-level network model](#flow-level-network-model)

The [proportionally fair allocation on a four-cycle](convex-optimization.md#proportionally-fair-allocation-on-a-four-cycle) produces a [reversible Markov chain](markov-process.md#reversible-markov-chain) with [stationary distribution](markov-process.md#stationary-distribution) proportional to $\binom{n_1+n_2+n_3+n_4}{n_1+n_3}\prod_r\rho_r^{n_r}$. This is normalizable exactly when every resource's offered load is strictly below capacity, equivalently $\max(\rho_1,\rho_3)+\max(\rho_2,\rho_4)<1$.

### Fluid model

↑ **Parent:** [Stochastic network](#stochastic-network)

A fluid model replaces discrete counts by continuous quantities whose evolution follows averaged large-scale drifts. A heuristic drift calculation motivates such a model; proving a [fluid limit](#fluid-limit) requires a separate convergence argument.

#### Ratio time change for a homogeneous fluid model

↑ **Parent:** [Fluid model](#fluid-model)

For a two-coordinate [fluid model](#fluid-model) with $\dot s=g(n/s)$, $\dot n=f(n/s)$ and $s>0$, set $\kappa=n/s$ and $du/dt=1/s$. Then $d\kappa/du=f(\kappa)-\kappa g(\kappa)$ and $d\log s/du=g(\kappa)$. A bounded ratio eventually confined where $g\leq-\eta<0$ makes $s$ decay exponentially in the new time. Since $dt/du=s$, the original fluid time has a finite terminal value and both coordinates tend to zero. This is a useful [finite-time draining of a fluid model](#finite-time-draining-of-a-fluid-model) argument; the singular origin is treated by a stopped trajectory.

#### Finite-time draining of a fluid model

↑ **Parent:** [Fluid model](#fluid-model)

A nonnegative [fluid model](#fluid-model) drains in finite time if all its coordinates approach zero at a finite terminal time. A ratio-based [ordinary differential equation](differential-equation.md#ordinary-differential-equation) can become undefined at that endpoint; an absorbing extension is an additional modeling convention.

#### Fluid limit

↑ **Parent:** [Fluid model](#fluid-model)

A fluid limit is a scaling limit of a [stochastic process](stochastic-process.md) obtained by scaling space and time so that random fluctuations vanish and a deterministic trajectory remains. It can justify a [fluid model](#fluid-model) when the required convergence conditions hold.

##### Kurtz fluid limit theorem

↑ **Parent:** [Fluid limit](#fluid-limit)

For a [density-dependent Markov jump process](markov-process.md#density-dependent-markov-jump-process) with finitely many jump vectors, bounded nonnegative rates and Lipschitz drift $F(x)=\sum_\ell\ell\beta_\ell(x)$, an initial state converging in probability to $x_0$ gives uniform convergence in probability on every finite horizon to the ODE $\dot x=F(x)$, $x(0)=x_0$. The compensated martingale has expected maximal squared size $O(N^{-1})$ by the [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality); [Gronwall's inequality](probability-and-statistics.md#gronwall-inequality) transfers that estimate to the solution error.

// Target: probability-and-statistics.bigb

##### Poisson concentration proof of a density-dependent fluid limit

↑ **Parent:** [Fluid limit](#fluid-limit)

If the rate functions are bounded and [Lipschitz](real-analysis.md#lipschitz-continuity) on an invariant compact state space, the [Poisson time-change representation of a Markov chain](markov-process.md#poisson-time-change-representation-of-a-markov-chain) has drift $F=\sum_jv_j\beta_j$. Each centered Poisson term is uniformly small after division by $n$. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) then bounds the distance to $\dot z=F(z)$ by the initial error and the centered counting error, multiplied by $e^{LT}$. A Poisson maximal concentration bound gives exponentially decreasing error probabilities for a fixed horizon and fixed error tolerance.

### Random access network

↑ **Parent:** [Stochastic network](#stochastic-network)

A random access network lets stations make transmission attempts independently using a shared medium. A collision can prevent all attempted packets from being delivered; [slotted ALOHA](#slotted-aloha) adjusts attempt probabilities using slot feedback.

#### Exponential backoff

↑ **Parent:** [Random access network](#random-access-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_backoff)

After failures, a transmitter increases its random retry window by a multiplicative factor, so its access behavior depends on its collision history. This reduces immediate repeated contention, but its stability and delay properties depend on the exact rule and traffic model.

##### Geometric-attempt exponential backoff

↑ **Parent:** [Exponential backoff](#exponential-backoff)

A packet with $k$ previous collisions attempts independently in each slot with probability $p_k=p_0 2^{-k}$. On failure it advances to stage $k+1$, and on success it leaves. The [Markov chain](markov-process.md#markov-chain) state records the number of packets at every stage, rather than only the total backlog. This memoryless-window model is related to [binary exponential backoff](#binary-exponential-backoff), but its geometric waiting times differ from uniform counters in finite retry windows.

// Target: probability-and-statistics.bigb

###### Mean delay under independent exponential-backoff failures

↑ **Parent:** [Geometric-attempt exponential backoff](#geometric-attempt-exponential-backoff)

For [geometric-attempt exponential backoff](#geometric-attempt-exponential-backoff), assume each attempted transmission fails independently with a fixed probability $q<1$. The probability of reaching stage $k$ is $q^k$, and its mean waiting time is $2^k/p_0$. The [Tonelli theorem](measure-theory.md#tonelli-theorem) gives $\mathbb ET=p_0^{-1}\sum_{k\ge0}(2q)^k$, finite exactly when $q<1/2$. The packet succeeds almost surely for every $q<1$, so almost-sure success does not guarantee finite mean delay. A fixed independent failure probability is a simplifying assumption, not a theorem about collisions in an interacting network.

// Target: probability-and-statistics.bigb

##### Binary exponential backoff

↑ **Parent:** [Exponential backoff](#exponential-backoff)

After $k$ collisions a packet chooses an independent counter uniformly from $\{0,\ldots,2^k-1\}$ and retries when it expires. The window doubles after a further collision. This is an example of [exponential backoff](#exponential-backoff) with a nonconstant retry rule, contrasting with constant-probability [slotted ALOHA](#slotted-aloha).

#### Throughput

↑ **Parent:** [Random access network](#random-access-network)

Throughput is the long-run rate of successful work. In an ideal stationary activation model with unit transmission speed, station $r$ has throughput equal to its stationary active fraction $\mathbb E[n_r]$.

#### Carrier-sense multiple access

↑ **Parent:** [Random access network](#random-access-network)

Carrier-sense multiple access lets a station attempt transmission only when interfering neighbors are inactive. An ideal continuous-time model gives inactive station $r$ an exponential attempt rate $e^{\theta_r}$ and unit-rate exponential transmission completions. [Detailed balance](markov-process.md#detailed-balance) then gives activation weights $e^{\theta\cdot n}$ on the [independent sets](graph-theory.md#independent-set-graph-theory) of the [interference graph](#interference-graph).

#### Interference graph

↑ **Parent:** [Random access network](#random-access-network)

An interference graph has one [graph vertex](graph.md#vertex-graph-theory) for each station and an [edge](graph-theory.md#edge-of-a-graph) for every pair that cannot transmit simultaneously. Feasible activation schedules are the graph's [independent sets](graph-theory.md#independent-set-graph-theory).

##### Throughput region of an interference graph

↑ **Parent:** [Interference graph](#interference-graph)

For feasible [independent set](graph-theory.md#independent-set-graph-theory) activation vectors $S$, the throughput region is their [convex hull](mathematical-optimization.md#convex-hull). Its downward closure is the same set because deleting active vertices preserves feasibility. Ideal [carrier-sense multiple access](#carrier-sense-multiple-access) can supply strict margins above every vector in its interior by adjusting attempt rates.

#### Slotted ALOHA

↑ **Parent:** [Random access network](#random-access-network)

Time is divided into slots, and a slot succeeds exactly when one station transmits. With backlog $N$ and independent attempt probability $p$, the success probability is $Np(1-p)^{N-1}$. [Fluid approximation of slotted ALOHA](#fluid-approximation-of-slotted-aloha) replaces the large-system binomial probabilities by Poisson probabilities.

##### Finite-population exclusion of permanent ALOHA collisions

↑ **Parent:** [Slotted ALOHA](#slotted-aloha)

If a finite-population [slotted ALOHA](#slotted-aloha) system has at most $M$ packets eligible to retry, uses independent retry probability $0<p<1$, and has conditional probability at least $\delta>0$ of no fresh attempts in any slot, then its conditional idle probability is at least $\delta(1-p)^M$. The probability that the next $k$ slots all collide is therefore at most $[1-\delta(1-p)^M]^k$. Letting $k\to\infty$ and taking a countable union over starting slots excludes eventual permanent collisions. Positive lower bounds on idle probability are essential: deterministic retries at probability one can create an absorbing collision state.

##### Backlog-aware ALOHA with arrival-adjusted attempt probabilities

↑ **Parent:** [Slotted ALOHA](#slotted-aloha)

In infinite-population [slotted ALOHA](#slotted-aloha), suppose new arrivals form an independent Poisson variable of mean $\eta$ per slot and attempt immediately. At backlog $b\ge1$, let old packets attempt independently with probability $p_b$. Their total attempted load tends to $1-\eta$, so the total offered attempts tend to one and the success probability tends to $e^{-1}$. For $0<\eta<e^{-1}$ the backlog has strictly negative drift outside a finite set, and [Foster theorem](markov-process.md#foster-s-theorem) proves a [positive recurrent Markov chain](markov-process.md#positive-recurrent-markov-chain). This mathematical benchmark requires exact backlog information; a practical feedback estimate needs its own analysis.

// Target: probability-and-statistics.bigb

##### Permanent collisions in constant-probability slotted ALOHA

↑ **Parent:** [Slotted ALOHA](#slotted-aloha)

With independent Poisson arrivals of any positive rate and a fixed retry probability $0<f\leq1$, the infinite-population [slotted ALOHA](#slotted-aloha) model eventually has collisions in every slot almost surely. For $f<1$, an [exponential-supermartingale escape bound](martingale.md#exponential-supermartingale-escape-bound) proves transience of the backlog chain. Bounded martingale increments then give backlog growth at the arrival rate, and the [Conditional Borel-Cantelli lemma](probability-theory.md#conditional-borel-cantelli-lemma) makes the exponentially unlikely noncollision slots finite in number. At $f=1$, two old packets suffice for permanent collisions. At $f=0$ the assertion is false.

###### Collision-path coupling for slotted ALOHA

↑ **Parent:** [Permanent collisions in constant-probability slotted ALOHA](#permanent-collisions-in-constant-probability-slotted-aloha)

In [slotted ALOHA](#slotted-aloha), let old packets retry independently with fixed probability $0<p<1$, and let independent [Poisson random variables](discrete-probability-distribution.md#poisson-distribution) of mean $\nu>0$ transmit once on arrival. Write $q=1-p$ and $r=e^{-\nu p}$. A hypothetical process which never removes a packet has backlog $b+A_t$, where $A_t$ is the cumulative arrival count over $t$ slots. Couple its attempts to those of the actual process until the first noncollision. Its one-slot noncollision probability at backlog $n$ is $h(n)=e^{-\nu}[(1+\nu)q^n+npq^{n-1}]$. The [union bound](probability-inequality.md#boole-s-inequality) and the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) give

$$
\varepsilon(b)=e^{-\nu}q^b\left[\frac{1+\nu+bp/q}{1-r}+\frac{p\nu r}{(1-r)^2}\right].
$$

Indeed $\mathbb E[q^{A_t}]=r^t$ and $\mathbb E[A_tq^{A_t}]=\nu tq r^t$. Thus $\varepsilon(b)\to0$. From every sufficiently large backlog, permanent collisions have probability at least $1/2$. Independent arrival batches reach that threshold almost surely; after each failed attempt the [Strong Markov property](markov-process.md#strong-markov-property) permits another attempt. The probability of $k$ consecutive failures is at most $2^{-k}$, proving almost-sure eventual permanent collisions without assuming in advance that the backlog escapes.

##### Fluid approximation of slotted ALOHA

↑ **Parent:** [Slotted ALOHA](#slotted-aloha)

When backlog $N$ and attempt-control scale $S$ are large with $N/S\approx\kappa$, idle and success probabilities approach $e^{-\kappa}$ and $\kappa e^{-\kappa}$. Expected update increments then motivate a [fluid model](#fluid-model) described by [ordinary differential equations](differential-equation.md#ordinary-differential-equation).

###### Stable fluid controller for slotted ALOHA

↑ **Parent:** [Fluid approximation of slotted ALOHA](#fluid-approximation-of-slotted-aloha)

This feedback family in [slotted ALOHA](#slotted-aloha) gives $g(\kappa)=A\{2/(e-2)-[e/(e-2)](1+\kappa)e^{-\kappa}\}$, which changes sign at contention ratio one. For $0\leq\nu<e^{-1}$, the ratio drift $h=\nu-\kappa e^{-\kappa}-\kappa g$ is strictly negative on $[1,\infty)$ and on some interval beginning below one. The [ratio time change for a homogeneous fluid model](#ratio-time-change-for-a-homogeneous-fluid-model) traps the ratio in a region where $g<0$ and proves finite-time draining. For $\nu>e^{-1}$, backlog drift is at least $\nu-e^{-1}>0$ regardless of this controller. These are statements about the interior [fluid model](#fluid-model), not a stand-alone theorem of stochastic stability.

##### ALOHA throughput bound

↑ **Parent:** [Slotted ALOHA](#slotted-aloha)

For $N\geq2$ backlogged stations, the largest one-slot success probability is $(1-1/N)^{N-1}$, attained at $p=1/N$. Its limit is $e^{-1}$; the exact finite-$N$ maximum is larger, and for $N=1$ it is one.

### Wardrop equilibrium

↑ **Parent:** [Stochastic network](#stochastic-network)

A Wardrop equilibrium assigns positive traffic only to routes with minimum delay for their source-sink pair. With fixed demands and continuous increasing link delays, it minimizes the [Beckmann potential](#beckmann-potential). Strictly increasing delays make link throughputs unique, while route flows can remain nonunique.

<h4 id="braess-s-paradox">Braess's paradox</h4>

↑ **Parent:** [Wardrop equilibrium](#wardrop-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Braess's_paradox)

Adding a link to a nonatomic traffic [flow network](graph-theory.md#flow-network) can increase the equilibrium travel delay. Extra routes change the incentives defining a [Wardrop equilibrium](#wardrop-equilibrium), so the new equilibrium need not retain an earlier good allocation. The system-optimal delay cannot worsen when the old allocation remains feasible; the paradox concerns selfish equilibrium.

#### Marginal external cost toll

↑ **Parent:** [Wardrop equilibrium](#wardrop-equilibrium)

For a differentiable link delay $D_j(y)$, the toll $T_j(y)=yD_j'(y)$ charges a user for the additional delay imposed on the other users. Its perceived link cost is the derivative of $yD_j(y)$. The resulting [Beckmann potential](#beckmann-potential) equals total travel delay. If total delay is [convex](real-analysis.md#convex-function), its [Wardrop equilibria](#wardrop-equilibrium) minimize that delay globally. Strict increase of $D_j$ alone does not imply this convexity; [optimal-flow calibrated congestion tolling](#optimal-flow-calibrated-congestion-tolling) avoids that extra requirement.

##### Optimal-flow calibrated congestion tolling

↑ **Parent:** [Marginal external cost toll](#marginal-external-cost-toll)

Let $y^*$ be a globally delay-minimizing feasible vector of link [throughputs](#throughput). For continuously differentiable strictly increasing delays, calibrated tolls

$$
T_j(u)=y_j^*D_j'(y_j^*)+\varepsilon_j(u-y_j^*)_+^2\qquad(\varepsilon_j\geq0)
$$

make the marginal social costs at $y^*$ equal the perceived route costs there. First-order route-exchange conditions make $y^*$ a tolled [Wardrop equilibrium](#wardrop-equilibrium). The nonnegative nondecreasing penalty vanishes at the optimum; choosing $\varepsilon_j>0$ makes the toll genuinely traffic-dependent. The perceived link delays remain strictly increasing, so their [Beckmann potential](#beckmann-potential) gives unique equilibrium link loads. Every tolled [Wardrop equilibrium](#wardrop-equilibrium) therefore has the globally optimal $y^*$, even when the total-delay objective is not [convex](real-analysis.md#convex-function).

#### Route-flow nonuniqueness at a Wardrop equilibrium

↑ **Parent:** [Wardrop equilibrium](#wardrop-equilibrium)

Strictly increasing link delays make [Wardrop equilibrium](#wardrop-equilibrium) link [throughputs](#throughput) unique, but route decompositions of those throughputs can differ. With unit demand through two successive stages of two parallel links each and link delay $D(u)=u$, the four-route vectors $(t,1/2-t,1/2-t,t)$ for $0\leq t\leq1/2$ all induce link loads $1/2$. All routes then have equal delay one.

#### Elastic-demand Wardrop equilibrium

↑ **Parent:** [Wardrop equilibrium](#wardrop-equilibrium)

In an elastic-demand Wardrop equilibrium, demand $f_s$ responds to the minimum route delay $\lambda_s$ through $f_s=B_s(\lambda_s)$. An [inverse demand function](#inverse-demand-function) supplies the utility term that must be subtracted from the [Beckmann potential](#beckmann-potential).

##### Boundary exclusion for elastic Wardrop demand

↑ **Parent:** [Elastic-demand Wardrop equilibrium](#elastic-demand-wardrop-equilibrium)

For nonnegative strictly increasing link delays and nonempty routes, let $M=B(0)$ and $L=\lim_{\lambda\to\infty}B(\lambda)$. The inverse demand tends to infinity as flow decreases to $L$, so increasing flow slightly there gains more utility than the bounded link-cost increment. At $M$ the inverse demand is zero, whereas a used route has positive delay, so reducing flow improves the objective. A minimizer consequently has $L<f<M$ and satisfies the ordinary interior [Wardrop equilibrium](#wardrop-equilibrium) conditions. Lower-semicontinuous endpoint extensions permit minimization on the compact demand interval even when utility diverges at $L$.

##### Inverse demand function

↑ **Parent:** [Elastic-demand Wardrop equilibrium](#elastic-demand-wardrop-equilibrium)

A strictly decreasing demand function has a decreasing inverse on its range. The utility primitive $\int P_s(u)\,du$ is a [concave function](real-analysis.md#concave-function). A positive interior reference value avoids assuming that an improper integral from zero is finite.

###### Elastic-demand utility with an interior reference

↑ **Parent:** [Inverse demand function](#inverse-demand-function)

An interior reference point defines the utility of a continuous strictly decreasing demand function without requiring integrability of its inverse at zero. The inverse demand is decreasing, so the utility is strictly [concave](real-analysis.md#concave-function). For example $B(\lambda)=(1+\lambda)^{-1/2}$ has inverse $f^{-2}-1$, whose integral from zero diverges. The interior-reference utility still has the required derivative and is finite at every interior demand.

#### Beckmann potential

↑ **Parent:** [Wardrop equilibrium](#wardrop-equilibrium)

The Beckmann potential integrates each link's delay function. Its [gradient](calculus.md#gradient) with respect to route flows is the corresponding vector of route delays, making [Wardrop equilibrium](#wardrop-equilibrium) a [convex optimization](convex-optimization.md) problem.

#### Source-sink route incidence matrix

↑ **Parent:** [Wardrop equilibrium](#wardrop-equilibrium)

This matrix has $H_{sr}=1$ when route $r$ serves source-sink pair $s$, and zero otherwise. Thus $Hx=f$ aggregates route flows into source-sink demands.

### Link-route incidence matrix

↑ **Parent:** [Stochastic network](#stochastic-network)

The link-route incidence matrix records how much resource $j$ is used by one call or flow on route $r$. For unit requirements $A_{jr}\in\{0,1\}$; the product $Ax$ gives resource throughputs from route flows.

### Loss network

↑ **Parent:** [Stochastic network](#stochastic-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loss_network)

A loss network admits a call only when all its required resources have enough free capacity. Rejected calls do not queue. Under [fixed routing](#fixed-routing) and independent [Poisson processes](probability-theory.md#poisson-process), its exact occupancy law has a [product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network).

#### Rearrangeable triangular loss network

↑ **Parent:** [Loss network](#loss-network)

Three nodes have integer link capacities $C_{12},C_{13},C_{23}$. Calls between a node pair use either its direct link or the two-link alternative. With unrestricted instantaneous rearrangement of existing calls, counts $n_{12},n_{13},n_{23}$ are feasible exactly when $n_{12}+n_{13}\leq C_{12}+C_{13}$, $n_{12}+n_{23}\leq C_{12}+C_{23}$ and $n_{13}+n_{23}\leq C_{13}+C_{23}$. Necessity follows by counting calls crossing each node cut. For sufficiency, the inequalities allow at most one count to exceed its direct-link capacity. Divert precisely that excess to the other two links; the same inequalities ensure capacity there. The counts thus have the same feasible set as a [fixed routing](#fixed-routing) [loss network](#loss-network) with one virtual resource at each node, capacity equal to the sum of its two incident physical-link capacities, and each call using its two endpoint resources. With independent [Poisson processes](probability-theory.md#poisson-process) for arrivals and independent routing-independent [exponential distributions](continuous-probability-distribution.md#exponential-distribution) for holding times, this gives the usual [product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network) and exact [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages) blocking probabilities.

##### Cut feasibility for a rearrangeable triangle

↑ **Parent:** [Rearrangeable triangular loss network](#rearrangeable-triangular-loss-network)

The three cyclic versions of this inequality are necessary and sufficient for routing unit calls on a triangle with complete instantaneous rearrangement. Necessity counts endpoint calls through a node cut. For sufficiency, at most one call count can exceed its direct-link capacity, since any two such excesses would violate their common endpoint cut. Route that one excess along the two other links; the two relevant cut inequalities guarantee room there. This gives an exact reduction to a [loss network](#loss-network) with a virtual resource at each node.

#### Alternative routing

↑ **Parent:** [Loss network](#loss-network)

Alternative routing lets a call try another resource path when its preferred route is blocked. Overflow onto longer paths can create feedback and multiple solutions of the [Erlang fixed point approximation](#erlang-fixed-point-approximation), even though an exact finite irreducible occupancy [Markov chain](markov-process.md#markov-chain) has a unique [stationary distribution](markov-process.md#stationary-distribution).

##### Multiple Erlang fixed points under alternative routing

↑ **Parent:** [Alternative routing](#alternative-routing)

A symmetric triangle with direct calls and two-link overflow routes has [Erlang fixed point approximation](#erlang-fixed-point-approximation) equation $B=E(\lambda[1+2B(1-B)],C)$. For $C=1000$ and $\lambda=950$, this has at least three solutions, certified by the [intermediate value theorem](calculus.md#intermediate-value-theorem) using signs at $B=0,0.01,0.1,0.4$.

###### Fluid scaling proof of multiple Erlang fixed points

↑ **Parent:** [Multiple Erlang fixed points under alternative routing](#multiple-erlang-fixed-points-under-alternative-routing)

Let $G_N(B)=E(20N[1+2B(1-B)],21N)-B$. The [proportional scaling limit of the Erlang loss formula](#proportional-scaling-limit-of-the-erlang-loss-formula) makes its limits at $B=1/100$ and $B=1/8$ respectively $-1/100$ and $7/520$. Since $G_N(0)>0$ and $G_N(1)<0$, sufficiently large $N$ give alternating signs at these four points. The [intermediate value theorem](calculus.md#intermediate-value-theorem) supplies three distinct zeros in the intervening intervals. These are multiple solutions of the [Erlang fixed point approximation](#erlang-fixed-point-approximation), not multiple stationary laws of an exact finite [irreducible Markov chain](markov-process.md#irreducible-markov-chain).

###### Alternative-routing triangle with three Erlang fixed points

↑ **Parent:** [Multiple Erlang fixed points under alternative routing](#multiple-erlang-fixed-points-under-alternative-routing)

On a three-node [loss network](#loss-network), each pair offers direct calls of load $v$ to its link of capacity $C$. If blocked, the call tries the two-link path through the remaining node. The symmetric [reduced-load approximation](#reduced-load-approximation) gives a link its direct load and two overflow contributions $vB(1-B)$, hence the displayed equation. For $C=1000$, $v=940$, its residual has alternating signs at $B=0,0.01,0.10,0.25$, giving at least three distinct roots. This multiplicity belongs to the [Erlang fixed point approximation](#erlang-fixed-point-approximation), not to the exact stationary law of a finite reachable [Markov chain](markov-process.md#markov-chain).

#### Erlang loss formula

↑ **Parent:** [Loss network](#loss-network)

For capacity $C$ and [offered traffic](#offered-traffic) $a$, the probability of a full single-resource loss system is $E(a,C)=(a^C/C!)/(\sum_{k=0}^Ca^k/k!)$. The stable recursion is $E(a,0)=1$, $E(a,k)=aE(a,k-1)/(k+aE(a,k-1))$.

##### Rational certificates for the Erlang loss recursion

↑ **Parent:** [Erlang loss formula](#erlang-loss-formula)

For rational [offered load](#offered-traffic), every step of the stable recursion for the [Erlang loss formula](#erlang-loss-formula) is rational. Comparing the final numerator and denominator with rational thresholds therefore certifies signs without floating-point uncertainty. Opposite certified signs of a continuous fixed-point residual imply a root by the [intermediate value theorem](calculus.md#intermediate-value-theorem); several alternating intervals can prove multiple [Erlang fixed points](#erlang-fixed-point-approximation) under [alternative routing](#alternative-routing).

##### Monotonicity of the Erlang blocking probability

↑ **Parent:** [Erlang loss formula](#erlang-loss-formula)

For positive integer capacity $C$ and [offered load](#offered-traffic) $a>0$, let $m_C(a)$ be the [carried load of an Erlang loss resource](#carried-load-of-an-erlang-loss-resource). Differentiating the [upper-truncated Poisson distribution](discrete-probability-distribution.md#upper-truncated-poisson-distribution) gives $m_C'(a)=\operatorname{Var}(N)/a>0$. Differentiating its probability at $C$ gives the displayed [derivative](calculus.md#derivative) of the [Erlang loss formula](#erlang-loss-formula); it is positive because $m_C(a)<C$. Thus blocking increases continuously from zero to one, and the carried load increases from zero to $C$. These properties justify the inverse blocking coordinates in the [convex potential for the Erlang fixed point](#convex-potential-for-the-erlang-fixed-point).

##### Proportional scaling limit of the Erlang loss formula

↑ **Parent:** [Erlang loss formula](#erlang-loss-formula)

Scale the offered load and capacity together. Reversing the denominator of the [Erlang loss formula](#erlang-loss-formula) gives

$$
E(N\nu,NC)^{-1}=\sum_{j=0}^{NC}\prod_{\ell=0}^{j-1}\frac{NC-\ell}{N\nu}.
$$

For each fixed $j$, the summand tends to $(C/\nu)^j$. If $\nu>C$, the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) applies with the summable [geometric series](real-analysis.md#geometric-series) bound $(C/\nu)^j$. Otherwise each fixed finite partial sum has limiting value at least its number of terms, so the reciprocal diverges. Taking reciprocals proves the formula, including the critical case $\nu=C$.

##### Carried load of an Erlang loss resource

↑ **Parent:** [Erlang loss formula](#erlang-loss-formula)

For offered load $a$ and capacity $C\geq1$, the carried load equals the mean occupancy:

$$
m_C(a)=a[1-E(a,C)].
$$

Differentiating the truncated-Poisson equilibrium weights gives $m_C'(a)=\operatorname{Var}_a(N)/a>0$ for $a>0$. The carried load increases from zero to $C$. This monotonicity supplies the strictly increasing term in the [convex potential for the Erlang fixed point](#convex-potential-for-the-erlang-fixed-point).

##### Erlang fixed point approximation

↑ **Parent:** [Erlang loss formula](#erlang-loss-formula)

The Erlang fixed point approximation treats resource blocking as independent and applies the [Erlang loss formula](#erlang-loss-formula) to traffic screened by other resources. Its self-consistency equations have a unique [fixed point](function.md#fixed-point) under [fixed routing](#fixed-routing), but can have several under [alternative routing](#alternative-routing).

###### Convex potential for the Erlang fixed point

↑ **Parent:** [Erlang fixed point approximation](#erlang-fixed-point-approximation)

Set $y_j=-\log(1-B_j)$ and let $e_C(a)=E(a,C)$. For positive integer capacities,

$$
U(z,C)=e^{-z}e_C^{-1}(1-e^{-z}),\qquad
F(y)=\sum_r\nu_r e^{-(A^Ty)_r}+\sum_j\int_0^{y_j}U(z,C_j)\,dz.
$$

The function $U$ is the [carried load of an Erlang loss resource](#carried-load-of-an-erlang-loss-resource) evaluated at its inverse blocking parametrization. It is continuous and strictly increasing from zero to $C$. Hence $F$ is a [coercive function](real-analysis.md#coercive-function) and a [strictly convex function](real-analysis.md#strictly-convex-function) on the nonnegative orthant. Its first-order conditions are the fixed-routing [Erlang fixed point](#erlang-fixed-point-approximation) equations, including zero prices at unused links.

###### Cyclic substitution for the Erlang fixed point

↑ **Parent:** [Convex potential for the Erlang fixed point](#convex-potential-for-the-erlang-fixed-point)

Update one link blocking probability at a time using the reduced load accepted by all other links, then cycle through the links. In logarithmic acceptance coordinates this is exact [coordinate descent](convex-optimization.md#coordinate-descent) for the [convex potential for the Erlang fixed point](#convex-potential-for-the-erlang-fixed-point). Potential values decrease within a compact sublevel set. Continuity of a whole-sweep update forces every limit point to minimize every coordinate, hence to equal the unique global minimizer. This proves convergence without requiring a simultaneous substitution scheme.

###### Reduced-load approximation

↑ **Parent:** [Erlang fixed point approximation](#erlang-fixed-point-approximation)

For unit resource requirements in a [loss network](#loss-network), the effective [offered traffic](#offered-traffic) to resource $j$ is $a_j=\sum_{r:j\in r}\alpha_r\prod_{k\in r\setminus\{j\}}(1-B_k)$, where $B_k$ are approximate resource blocking probabilities. The resource being modeled is excluded from its own screening product.

#### Offered traffic

↑ **Parent:** [Loss network](#loss-network)

For calls arriving at rate $\nu_r$ with mean holding time $1/\mu_r$, offered traffic is the dimensionless load $\alpha_r=\nu_r/\mu_r$, often measured in Erlangs. The [Erlang loss formula](#erlang-loss-formula) distinguishes this offered traffic from the mean traffic actually carried.

#### Fixed routing

↑ **Parent:** [Loss network](#loss-network)

Under fixed routing, each call type always requests the same collection of resources. The [link-route incidence matrix](#link-route-incidence-matrix) records those requirements. This differs from [alternative routing](#alternative-routing), in which a rejected direct request can try another route.

##### Product-form stationary distribution of a loss network

↑ **Parent:** [Fixed routing](#fixed-routing)

For a [loss network](#loss-network) with feasible occupancies $An\leq C$, its [stationary distribution](markov-process.md#stationary-distribution) is proportional to $\prod_r\alpha_r^{n_r}/n_r!$. It is the law of independent [Poisson random variables](discrete-probability-distribution.md#poisson-distribution) conditioned on the resource constraints. With exponential holding times, [detailed balance for a continuous-time Markov chain](markov-process.md#detailed-balance-for-a-continuous-time-markov-chain) proves the formula directly.

###### Blocking partition ratio for a loss network

↑ **Parent:** [Product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network)

Let $Z(C)$ sum the unnormalized occupancy weights $\prod_r\rho_r^{n_r}/n_r!$ over feasible counts. The states admitting another type-$r$ call are exactly those feasible under capacities $C-A_r$. [Poisson arrivals see time averages](#poisson-arrivals-see-time-averages) therefore gives the displayed blocking probability. Take $Z$ to be zero when the reduced capacities make its feasible set empty.

###### Entropy maximization for loss-network occupancy

↑ **Parent:** [Product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network)

For positive arrival rates and capacities with every route nonempty, maximizing $H_\nu(x)$ over $x\geq0$, $Ax\leq C$ has a unique positive optimizer $x^*$. The [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) give $x_r^*=\nu_r e^{-(A^Tz)_r}$ for nonnegative link prices with [complementary slackness](mathematical-optimization.md#complementary-slackness). Under proportional scaling by $N$, the [Stirling formula](real-analysis.md#stirling-formula) gives a uniform logarithmic weight approximation $\log w_N(n)=NH_\nu(n/N)+O(\log N)$. Strict [concavity](real-analysis.md#concave-function) and compactness give an objective gap away from $x^*$, while only polynomially many feasible states exist. Thus the [stationary distribution](markov-process.md#stationary-distribution) has $n/N\to x^*$ in probability, with exponentially small probabilities outside any fixed neighborhood of $x^*$. In particular $\mathbb E[n]=Nx^*+o(N)$.

###### Poisson exponential tilting for a loss network

↑ **Parent:** [Entropy maximization for loss-network occupancy](#entropy-maximization-for-loss-network-occupancy)

Substituting the optimizer relation $\nu_r=x_r^*e^{(A^Tz)_r}$ into the [product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network) proves the displayed exact identity. The independent [Poisson random variables](discrete-probability-distribution.md#poisson-distribution) give a reference law centered at the optimized occupancies, while the constraint and exponential factor account for saturated resources. An unconstrained [Gaussian approximation](convergence-of-random-variables.md#normal-approximation) can miss these boundary effects.

###### Insensitivity of loss networks

↑ **Parent:** [Product-form stationary distribution of a loss network](#product-form-stationary-distribution-of-a-loss-network)

For the standard [fixed routing](#fixed-routing) [loss network](#loss-network) with independent [Poisson processes](probability-theory.md#poisson-process), the stationary occupancy law depends on independent holding-time distributions only through their means. The occupancy process alone need not be a [Markov process](markov-process.md) when those holding times lack the [memoryless property](continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution).

## Poisson arrivals see time averages

↑ **Parent:** [Queueing theory](queueing-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_arrivals_see_time_averages)

The Poisson arrivals see time averages property says that an external [Poisson process](probability-theory.md#poisson-process) independent of a stationary system sees the system-state distribution at its arrival times. Thus the fraction of arrivals that accept a state-dependent admission rule $p(n)$ is $\sum_n\pi_np(n)$.

<h2 id="m-g-1-queue">M/G/1 queue</h2>

↑ **Parent:** [Queueing theory](queueing-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/M/G/1_queue)

An $M/G/1$ queue has Poisson arrivals, [independent identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) service times, and one server. If service has mean $m$ and $\lambda m<1$, its mean busy period is

$$
\frac{m}{1-\lambda m}.
$$

This follows by decomposing the busy period into the first service and the busy-period descendants of arrivals during that service.

<h3 id="m-d-1-queue">M/D/1 queue</h3>

↑ **Parent:** [M/G/1 queue](#m-g-1-queue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/M/D/1_queue)

An [M/D/1 queue](#m-d-1-queue) has a [Poisson process](probability-theory.md#poisson-process) of arrivals, a deterministic service time $\tau$, and one work-conserving server. With arrival rate $\lambda$ and $\lambda\tau<1$, its equilibrium idle probability is $1-\lambda\tau$: the stationary completed work per unit time is $\lambda\tau$. Its output generally need not be a [Poisson process](probability-theory.md#poisson-process).

### Embedded departure chain of an M-G-1 queue

↑ **Parent:** [M/G/1 queue](#m-g-1-queue)

Let $Q_n$ be the number left immediately after departure $n$, and let $A_n$ be the arrivals during the next service. Then

$$
Q_{n+1}=Q_n-\mathbf1_{\{Q_n>0\}}+A_n.
$$

Conditional on service duration $S$, $A_n$ is Poisson with parameter $\lambda S$, so

$$
\mathbb EA_n=\lambda\mathbb ES,
\qquad
\mathbb EA_n^2=\lambda\mathbb ES+\lambda^2\mathbb ES^2.
$$

#### Pollaczek-Khinchine formula

↑ **Parent:** [Embedded departure chain of an M-G-1 queue](#embedded-departure-chain-of-an-m-g-1-queue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pollaczek–Khinchine_formula)

For a stable first-come first-served [M/G/1 queue](#m-g-1-queue), write $\rho=\lambda\mathbb ES<1$ and $\widetilde S(s)=\mathbb E e^{-sS}$. The stationary waiting-time [Laplace transform](analysis.md#laplace-transform) is

$$
\widetilde W_q(s)=\frac{(1-\rho)s}{s-\lambda+\lambda\widetilde S(s)}.
$$

With finite second service moment, differentiating at zero gives the [Pollaczek-Khinchine mean formula](#pollaczek-khinchine-mean-formula). These are the transform and mean forms of the same queueing identity.

##### Pollaczek-Khinchine mean formula

↑ **Parent:** [Pollaczek-Khinchine formula](#pollaczek-khinchine-formula)

For a stable $M/G/1$ queue with traffic intensity $\rho=\lambda\mathbb ES<1$, the mean waiting time before service is

$$
W_q=\frac{\lambda\mathbb ES^2}{2(1-\rho)}.
$$

Equivalently, the mean number in the system is

$$
L=\rho+\frac{\lambda^2\mathbb ES^2}{2(1-\rho)}.
$$

<h2 id="little-s-law">Little's law</h2>

↑ **Parent:** [Queueing theory](queueing-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Little's_law)

In a stable regenerative queue,

$$
L=\lambda W,
$$

where $L$ is mean population, $\lambda$ is throughput, and $W$ is mean sojourn time. Renewal reward proves it by identifying the area under the population path with the sum of customer sojourn times.

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (4)

- [FIFO queue](computer-science.md#fifo-queue)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#2/a/solution)
- [Queue (queueing theory)](#queue-queueing-theory)
