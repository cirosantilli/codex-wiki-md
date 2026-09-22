# Continuous-time Markov chain

↑ **Parent:** [Markov chain](markov-chain.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous-time_Markov_chain)

A continuous-time Markov chain waits an exponential time of rate $q_i$ in state $i$ and then jumps according to probabilities $p_{ij}=q_{ij}/q_i$.

**Table of contents**

- [Nonexplosion of a continuous-time Markov chain](#nonexplosion-of-a-continuous-time-markov-chain)
- [Markov jump process](#markov-jump-process)
  - [Symmetric stochastic attrition process](#symmetric-stochastic-attrition-process)
    - [Squared-population near-invariant for stochastic attrition](#squared-population-near-invariant-for-stochastic-attrition)
      - [Exponential concentration of terminal stochastic attrition survivors](#exponential-concentration-of-terminal-stochastic-attrition-survivors)
  - [Single marked exponential jump process](#single-marked-exponential-jump-process)
  - [Lévy kernel of a Markov jump process](#levy-kernel-of-a-markov-jump-process)
    - [Centered finite-rate jump kernel gives square martingales](#centered-finite-rate-jump-kernel-gives-square-martingales)
  - [Jump measure of a Markov jump process](#jump-measure-of-a-markov-jump-process)
    - [Predictable compensator of a jump measure](#predictable-compensator-of-a-jump-measure)
    - [Compensated jump-measure local martingale](#compensated-jump-measure-local-martingale)
  - [Density-dependent Markov jump process](#density-dependent-markov-jump-process)
    - [Cyclic imitation chain](#cyclic-imitation-chain)
      - [Product decay in a cyclic imitation chain](#product-decay-in-a-cyclic-imitation-chain)
    - [Martingale decomposition of a density-dependent jump process](#martingale-decomposition-of-a-density-dependent-jump-process)
- [Destination-dependent reset chain](#destination-dependent-reset-chain)
- [Hitting probabilities for a velocity-switching Markov ladder](#hitting-probabilities-for-a-velocity-switching-markov-ladder)
- [Nonexplosive continuous-time Markov chain](#nonexplosive-continuous-time-markov-chain)
  - [Absorption-or-escape dichotomy for a chain with killing](#absorption-or-escape-dichotomy-for-a-chain-with-killing)
- [Equilibrium distribution of a continuous-time Markov chain](#equilibrium-distribution-of-a-continuous-time-markov-chain)
- [Transition intensity matrix](#transition-intensity-matrix)
- [Ergodic theorem for a finite continuous-time Markov chain](#ergodic-theorem-for-a-finite-continuous-time-markov-chain)
- [Nonexplosive Markov chain](#nonexplosive-markov-chain)
- [Global balance for a continuous-time Markov chain](#global-balance-for-a-continuous-time-markov-chain)
- [Poisson time-change representation of a Markov chain](#poisson-time-change-representation-of-a-markov-chain)
- [Interchange process](#interchange-process)
  - [Aldous spectral gap theorem](#aldous-spectral-gap-theorem)
- [Time reversal of a continuous-time Markov chain](#time-reversal-of-a-continuous-time-markov-chain)
- [Kingman's coalescent](#kingman-s-coalescent)
  - [Mutation count on a neutral coalescent tree](#mutation-count-on-a-neutral-coalescent-tree)
    - [Moments of the mutation count on a neutral coalescent tree](#moments-of-the-mutation-count-on-a-neutral-coalescent-tree)
    - [Geometric mutation count in a coalescent epoch](#geometric-mutation-count-in-a-coalescent-epoch)
    - [Independent mutation counts in coalescent epochs](#independent-mutation-counts-in-coalescent-epochs)
  - [Total branch length of a neutral coalescent](#total-branch-length-of-a-neutral-coalescent)
  - [Kingman's infinite coalescent](#kingman-s-infinite-coalescent)
    - [Coming down from infinity of the Kingman coalescent](#coming-down-from-infinity-of-the-kingman-coalescent)
- [Entry count of a continuous-time Markov chain](#entry-count-of-a-continuous-time-markov-chain)
- [Occupation time of a continuous-time Markov chain](#occupation-time-of-a-continuous-time-markov-chain)
  - [Occupation time at an interior state of a variable-rate symmetric walk](#occupation-time-at-an-interior-state-of-a-variable-rate-symmetric-walk)
  - [Expected finite-horizon occupation time](#expected-finite-horizon-occupation-time)
- [Holding time](#holding-time)
  - [Mean holding time from a transition intensity matrix](#mean-holding-time-from-a-transition-intensity-matrix)
    - [Confidence interval for an inverse rate](#confidence-interval-for-an-inverse-rate)
- [Master equation](#master-equation)
  - [Entropy production rate of a Markov chain](#entropy-production-rate-of-a-markov-chain)
- [Continuous-time random walk](#continuous-time-random-walk)
  - [Coalescing random walks](#coalescing-random-walks)
- [Martingale problem for a continuous-time Markov chain](#martingale-problem-for-a-continuous-time-markov-chain)
- [Transition-rate matrix](#transition-rate-matrix)
- [Transition semigroup of a continuous-time Markov chain](#transition-semigroup-of-a-continuous-time-markov-chain)
  - [Poisson-sampled continuous-time Markov chain](#poisson-sampled-continuous-time-markov-chain)
  - [Kolmogorov equations](#kolmogorov-equations)
- [Markov reward model](#markov-reward-model)
- [Markov jump-process generator](#markov-jump-process-generator)
  - [Exponential martingale from a jump generator](#exponential-martingale-from-a-jump-generator)
  - [Forward operator of a Markov jump process](#forward-operator-of-a-markov-jump-process)
- [Holding-time reversal along a fixed CTMC jump path](#holding-time-reversal-along-a-fixed-ctmc-jump-path)
- [Recurrence equivalence for a CTMC and its fixed-time skeleton](#recurrence-equivalence-for-a-ctmc-and-its-fixed-time-skeleton)
- [Jump chain](#jump-chain)
  - [Reflected nearest-neighbour random walk](#reflected-nearest-neighbour-random-walk)
  - [Invariant-measure transfer between a jump chain and a CTMC](#invariant-measure-transfer-between-a-jump-chain-and-a-ctmc)
    - [Slow holding rates destroy positive recurrence](#slow-holding-rates-destroy-positive-recurrence)
    - [Fast holding rates create continuous-time positive recurrence](#fast-holding-rates-create-continuous-time-positive-recurrence)
  - [Nonexplosion from recurrent visits to a slow state](#nonexplosion-from-recurrent-visits-to-a-slow-state)
  - [Irreducibility and recurrence pass between a CTMC and its jump chain](#irreducibility-and-recurrence-pass-between-a-ctmc-and-its-jump-chain)
- [Explosion of a continuous-time Markov chain](#explosion-of-a-continuous-time-markov-chain)
  - [Nonexplosion under uniformly bounded jump rates](#nonexplosion-under-uniformly-bounded-jump-rates)
  - [Explosion by summable holding times](#explosion-by-summable-holding-times)
  - [Explosion of an upward-biased walk with geometrically increasing rates](#explosion-of-an-upward-biased-walk-with-geometrically-increasing-rates)
- [Invariant distribution of a continuous-time Markov chain](#invariant-distribution-of-a-continuous-time-markov-chain)
  - [Nonuniqueness of invariant distributions of a finite Markov chain](#nonuniqueness-of-invariant-distributions-of-a-finite-markov-chain)
  - [Invariant distribution of an explosive chain](#invariant-distribution-of-an-explosive-chain)
- [Batch-birth linear-death process](#batch-birth-linear-death-process)
  - [Moments of a batch-birth linear-death process](#moments-of-a-batch-birth-linear-death-process)
- [Birth-death process](#birth-death-process)
  - [Birth process](#birth-process)
    - [Exponential martingale of a pure birth process](#exponential-martingale-of-a-pure-birth-process)
    - [Logistic cell-division process](#logistic-cell-division-process)
    - [Nonexplosion criterion for a pure birth process](#nonexplosion-criterion-for-a-pure-birth-process)
    - [Linear birth process with immigration](#linear-birth-process-with-immigration)
      - [Linear birth process with catastrophes](#linear-birth-process-with-catastrophes)
  - [Yule process](#yule-process)
    - [Mean population of a Yule process](#mean-population-of-a-yule-process)
    - [Conditional Yule birth times](#conditional-yule-birth-times)
  - [Extinction probability of a linear birth-death process](#extinction-probability-of-a-linear-birth-death-process)
  - [Detailed balance for a birth-death process](#detailed-balance-for-a-birth-death-process)
  - [Birth-death master equation](#birth-death-master-equation)
    - [First-moment equation of a birth-death process](#first-moment-equation-of-a-birth-death-process)
    - [Moment equations of a linear birth-death process](#moment-equations-of-a-linear-birth-death-process)
    - [Factorial moment](#factorial-moment)
      - [Factorial-moment inversion](#factorial-moment-inversion)
      - [Poisson factorial moments](#poisson-factorial-moments)
        - [Factorial-moment criterion for Poisson convergence](#factorial-moment-criterion-for-poisson-convergence)
  - [Poisson moment closure for a birth-death process](#poisson-moment-closure-for-a-birth-death-process)
  - [Diffusion approximation of a birth-death process](#diffusion-approximation-of-a-birth-death-process)
    - [Linear noise approximation](#linear-noise-approximation)
      - [Chemical diffusion matrix](#chemical-diffusion-matrix)
      - [Normalized stationary fluctuation-dissipation relation for a reaction network](#normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network)
        - [Feedback attenuation of gene-expression noise](#feedback-attenuation-of-gene-expression-noise)
      - [Ornstein-Uhlenbeck fluctuation limit at a stable population equilibrium](#ornstein-uhlenbeck-fluctuation-limit-at-a-stable-population-equilibrium)
    - [Mean drift from a Fokker--Planck equation](#mean-drift-from-a-fokker-planck-equation)
  - [Birth-death recurrence classification](#birth-death-recurrence-classification)
  - [M/M/1 queue](#m-m-1-queue)
    - [Stationary workload of an exponential-payload queue](#stationary-workload-of-an-exponential-payload-queue)
    - [M-M-1 queue with state-dependent admission](#m-m-1-queue-with-state-dependent-admission)
    - [Positive recurrence of an M-M-1 queue](#positive-recurrence-of-an-m-m-1-queue)
    - [Stationary distribution of an M-M-1 queue](#stationary-distribution-of-an-m-m-1-queue)
    - [Burke's theorem](#burke-s-theorem)
    - [M-M-1 queue with Bernoulli feedback](#m-m-1-queue-with-bernoulli-feedback)
      - [Poisson output theorem for a feedback queue](#poisson-output-theorem-for-a-feedback-queue)
    - [Mean busy period of an M-M-1 queue](#mean-busy-period-of-an-m-m-1-queue)
  - [M/M/∞ queue](#m-m-∞-queue)
    - [Stationary distribution of an M-M-infinity queue](#stationary-distribution-of-an-m-m-infinity-queue)
    - [Burke theorem for an M-M-infinity queue](#burke-theorem-for-an-m-m-infinity-queue)
    - [Transient distribution of an M-M-infinity queue](#transient-distribution-of-an-m-m-infinity-queue)
    - [Mean busy period of an M-M-infinity queue](#mean-busy-period-of-an-m-m-infinity-queue)
  - [M-M-s-K queue](#m-m-s-k-queue)
    - [Stationary distribution of an M-M-s-K queue](#stationary-distribution-of-an-m-m-s-k-queue)

## Nonexplosion of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A [continuous-time Markov chain](continuous-time-markov-chain.md) is nonexplosive if it makes only finitely many jumps on every bounded time interval. A uniformly bounded total jump intensity permits domination by a [Poisson process](poisson-process.md). More generally, if a population process stays in a finite random set of states on each finite interval and every individual state has finite exit rate, localizing to fixed finite sets gives the same conclusion. In an [open migration process](queueing-theory.md#open-migration-process), external Poisson immigration bounds the total population while internal moves preserve it and exits reduce it, giving this localization.

## Markov jump process

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A Markov jump process is a nonexplosive, piecewise-constant continuous-time Markov process. Transition rates $q(x,y)$ give exponential holding time of rate $\sum_{y\ne x}q(x,y)$ and next-state probabilities proportional to these rates. Being Markov relative to a specified filtration requires the conditional future law given that filtration to depend only on the present state.

// Target: probability-and-statistics.bigb

### Symmetric stochastic attrition process

↑ **Parent:** [Markov jump process](#markov-jump-process)

This finite-state [Markov jump process](#markov-jump-process) models two opposing populations, each suffering losses at a rate proportional to the surviving opposing population. Both coordinate axes are absorbing. Its embedded [jump chain](#jump-chain) removes one individual at each step, with probabilities $b/(a+b)$ and $a/(a+b)$. The corresponding deterministic equations $\dot a=-\kappa b$, $\dot b=-\kappa a$ conserve $a^2-b^2$; finite stochastic populations satisfy a near-invariant instead.

#### Squared-population near-invariant for stochastic attrition

↑ **Parent:** [Symmetric stochastic attrition process](#symmetric-stochastic-attrition-process)

In the [jump chain](#jump-chain) of the [symmetric stochastic attrition process](#symmetric-stochastic-attrition-process), the two possible increments of $D$ are $-2A+1$ and $2B-1$. Their mean is the displayed quantity, bounded by one in absolute value. Subtracting these conditional means produces a [martingale](martingale.md). If both initial populations are at most $N$, it has at most $2N$ nonzero increments, each bounded by $4N$. Thus [Azuma-Hoeffding inequality](martingale.md#azuma-s-inequality) controls changes of order $N^2$ with exponentially small probability of order $e^{-cN}$.

##### Exponential concentration of terminal stochastic attrition survivors

↑ **Parent:** [Squared-population near-invariant for stochastic attrition](#squared-population-near-invariant-for-stochastic-attrition)

Start the [symmetric stochastic attrition process](#symmetric-stochastic-attrition-process) at $(N,\lfloor\alpha N\rfloor)$, with $0<\alpha<1$, and let $X^N$ be the final first-population size divided by $N$. The bound holds for all sufficiently large $N$, depending on $\alpha,\delta>0$. At absorption, one coordinate is zero. If the first survives, the terminal squared difference is $N^2(X^N)^2$; if it is extinguished, that difference is nonpositive. In either case the indicated deviation forces an error of at least $\sqrt{1-\alpha^2}\,\delta N^2$ from the limiting squared invariant. The initial rounding error and total conditional drift are only $O(N)$. Apply [Azuma-Hoeffding inequality](martingale.md#azuma-s-inequality) to the centered [squared-population near-invariant for stochastic attrition](#squared-population-near-invariant-for-stochastic-attrition), using its $2N$ increments bounded by $4N$, to obtain the displayed exponent.

### Single marked exponential jump process

↑ **Parent:** [Markov jump process](#markov-jump-process)

Let $T$ be a rate-one [exponential random variable](continuous-probability-distribution.md#exponential-distribution) independent of a [uniform random variable](continuous-probability-distribution.md#uniform-random-variable) $U$ on $(0,1)$. In its natural [filtration](stochastic-process.md#filtration-probability-theory), this [Markov jump process](#markov-jump-process) jumps once from zero to its mark and then stays there. Its destination rate kernel is $q(x,dy)=\mathbf1_{\{x=0\}}\mathbf1_{(0,1)}(y)dy$. For a Borel mark set $B$, the [martingale](martingale.md) $\mathbf1_{\{T\leq t,U\in B\}}-|B|(t\wedge T)$ follows directly from the memoryless residual lifetime. Information about the future mark or lifetime must not be inserted into the initial filtration.

<h3 id="levy-kernel-of-a-markov-jump-process">Lévy kernel of a Markov jump process</h3>

↑ **Parent:** [Markov jump process](#markov-jump-process)

A kernel specifying the jump rate from state $x$ for each displacement $z$. With the displacement convention the [infinitesimal generator](stochastic-process.md#infinitesimal-generator-stochastic-processes) is $L\varphi(x)=\int(\varphi(x+z)-\varphi(x))K(x,dz)$. The destination convention instead records a rate measure on the new state, translating each displacement by $x$. For finite total rate, that total is the exponential holding rate and the normalized measure is the next-jump distribution.

#### Centered finite-rate jump kernel gives square martingales

↑ **Parent:** [Lévy kernel of a Markov jump process](#levy-kernel-of-a-markov-jump-process)

With the displacement convention for a [Lévy kernel of a Markov jump process](#levy-kernel-of-a-markov-jump-process), suppose its total rate is bounded, its first moment is zero and its second moment $v$ is bounded by $V$. The bounded rate prevents explosion. The compensated displacement integral is a square-integrable [martingale](martingale.md) with $\mathbb EX_t^2\le Vt$. The displayed process is the sum of $2\int X_{s-}dX_s$ and the compensated sum of squared jumps. The first term is square [integrable](measure-theory.md#integrability) since $4\mathbb E\int_0^tX_{s-}^2v(X_{s-})ds\le2V^2t^2$; the second is [integrable](measure-theory.md#integrability) because its expected total jump-square sum is at most $Vt$. Consequently the square compensation is a true [martingale](martingale.md), without a fourth-moment assumption.

### Jump measure of a Markov jump process

↑ **Parent:** [Markov jump process](#markov-jump-process)

For a [Markov jump process](#markov-jump-process) with off-diagonal rate kernel $q(x,dy)$, the jump measure records the jump time and the destination state. Relative to a filtration for which the process has the Markov jump property, its predictable compensator is the displayed rate measure, up to explosion. The corresponding generator is $Qf(x)=\int[f(y)-f(x)]q(x,dy)$. An enlarged filtration revealing future jumps need not preserve this compensator, so the filtration condition is essential.

#### Predictable compensator of a jump measure

↑ **Parent:** [Jump measure of a Markov jump process](#jump-measure-of-a-markov-jump-process)

The [predictable](martingale.md#predictable-process) random measure $\nu$ matching the expected integrals of the jump measure $N$ against every nonnegative [predictable](martingale.md#predictable-process) integrand. For displacement marks of a [Markov jump process](#markov-jump-process), $\nu(ds,dy)=K(X_{s-},dy)ds$. Multiplying the integrand by an event known before an interval proves that the compensated integral has conditionally centered increments; expected absolute [integrability](measure-theory.md#integrability) makes it a true [martingale](martingale.md). Squared-integrand [integrability](measure-theory.md#integrability) gives the square-integrable compensation isometry.

#### Compensated jump-measure local martingale

↑ **Parent:** [Jump measure of a Markov jump process](#jump-measure-of-a-markov-jump-process)

A predictable mark-dependent integrand $H(t,y)$ gives a true [martingale](martingale.md) $\int_0^t\int H(s,y)(\mu-\nu)(ds,dy)$ whenever $\mathbb E\int_0^t\int|H|d\nu<\infty$ on every finite horizon. Local versions follow when this expected integrability holds after localization. The compensator identity applied to predictable indicators from the past proves that every increment has conditional expectation zero. Choosing $H(s,y)=f(y)-f(X_{s-})$ gives the generator martingale $f(X_t)-f(X_0)-\int_0^tQf(X_s)ds$ under the same local integrability conditions.

### Density-dependent Markov jump process

↑ **Parent:** [Markov jump process](#markov-jump-process)

With scale $N$, such a process has finitely many possible jump vectors $\ell/N$ occurring at rates $N\beta_\ell(x)$ depending on the current scaled state. Its drift is $\sum_\ell\ell\beta_\ell(x)$, while the predictable covariance rate of its martingale fluctuations is $N^{-1}\sum_\ell\ell\ell^T\beta_\ell(x)$.

// Target: probability-and-statistics.bigb

#### Cyclic imitation chain

↑ **Parent:** [Density-dependent Markov jump process](#density-dependent-markov-jump-process)

In a population of $N$ playing [rock paper scissors](game-theory.md#rock-paper-scissors), let losers copy winners. With pair-selection events of rate $(N-1)/2$, the proportion process has jumps $(e_1-e_3)/N$, $(e_2-e_1)/N$, $(e_3-e_2)/N$ at rates $Nx_1x_3$, $Nx_2x_1$, $Nx_3x_2$. Its [fluid limit](queueing-theory.md#fluid-limit) obeys $\dot x_i=x_i(x_{i-1}-x_{i+1})$, with indices interpreted cyclically. The [product of numbers](arithmetic.md#product-of-numbers) $x_1x_2x_3$ is conserved in this [ordinary differential equation](differential-equation.md#ordinary-differential-equation), whereas the finite chain eventually reaches a monochromatic absorbing state.

##### Product decay in a cyclic imitation chain

↑ **Parent:** [Cyclic imitation chain](#cyclic-imitation-chain)

For the [cyclic imitation chain](#cyclic-imitation-chain), its [infinitesimal generator](stochastic-process.md#infinitesimal-generator-stochastic-processes) satisfies $\mathcal L_N(x_1x_2x_3)=-3x_1x_2x_3/N$. Therefore $\mathbb E[X_1^N(t)X_2^N(t)X_3^N(t)]=e^{-3t/N}\mathbb E[X_1^N(0)X_2^N(0)X_3^N(0)]$. While all three types remain, the [product of numbers](arithmetic.md#product-of-numbers) is at least $(N-2)/N^3$ for $N\geq3$, so this identity proves that one type is lost almost surely. The remaining pair has a fixed winner, which eventually occupies the whole population. The conserved product in the deterministic [fluid limit](queueing-theory.md#fluid-limit) therefore describes fixed finite horizons, not the chain's infinite-time behavior.

#### Martingale decomposition of a density-dependent jump process

↑ **Parent:** [Density-dependent Markov jump process](#density-dependent-markov-jump-process)

With jumps $\ell/N$ at rates $N\beta_\ell(z)$, compensate each jump count by its integrated rate. The drift is $F(z)=\sum_\ell\ell\beta_\ell(z)$ and the [predictable quadratic variation](stochastic-calculus.md#predictable-quadratic-variation) matrix of the [martingale](martingale.md) term is $N^{-1}\int_0^t\sum_\ell\ell\ell^{\mathsf T}\beta_\ell(Z_s^N)ds$. On a compact region with bounded rates this bracket is of order $1/N$. A Lipschitz drift and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) transfer martingale concentration to the [fluid limit](queueing-theory.md#fluid-limit).

## Destination-dependent reset chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For jump rates $q_{ij}=r_j$ when $i\ne j$, let $R=\sum_jr_j>0$. The positive-rate states form the unique closed communicating class; every zero-rate state is an open singleton. The stationary law is $\pi_i=r_i/R$, with detailed balance $\pi_iq_{ij}=r_ir_j/R$. When at least two rates are positive, the embedded jump-chain law is proportional to $r_i(R-r_i)$. With only one positive rate, that state is absorbing and the genuine sequence of jump times stops there; an extended discrete chain can use an absorbing self-loop.

## Hitting probabilities for a velocity-switching Markov ladder

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

On nonnegative levels, a chain moves right at rate $\lambda$ in state $C$, left at rate $\mu$ in state $W$, and switches $C\to W$ at rate $\alpha$ and $W\to C$ at rate $\beta$. The minimal nonnegative solution for hitting $W_0$ is identically one when $\mu\alpha\ge\lambda\beta$. When $\mu\alpha<\lambda\beta$, it is $h_{W_i}=\vartheta^i$ and $h_{C_i}=b\vartheta^i$, where $b=\alpha(\mu+\beta)/[\beta(\lambda+\alpha)]<1$. These cases give recurrence and transience respectively.

## Nonexplosive continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A continuous-time [Markov chain](markov-chain.md) with finite holding rates is nonexplosive when its jump times have no finite accumulation almost surely. It then remains in its specified state space at every finite time, rather than being lost to a cemetery state after infinitely many jumps. Bounded rates are sufficient for nonexplosion, but finite rates at individual states alone are not.

### Absorption-or-escape dichotomy for a chain with killing

↑ **Parent:** [Nonexplosive continuous-time Markov chain](#nonexplosive-continuous-time-markov-chain)

For a [nonexplosive continuous-time Markov chain](#nonexplosive-continuous-time-markov-chain) on the nonnegative integers, suppose zero is absorbing and each positive state has positive rate to zero. On every finite positive set the conditional chance of absorption at the next jump has a positive minimum. By the [Strong Markov property](markov-chain.md#strong-markov-property), the chance of surviving $r$ departures from that set is bounded by $(1-\delta)^r$. Without absorption only finitely many such departures occur, and finite positive holding rates prohibit staying forever at a positive state. Thus eventually the path stays outside each finite set: it escapes to infinity. This conclusion needs no upward skip-free assumption.

## Equilibrium distribution of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

An equilibrium probability row vector is invariant under every time transition matrix, and satisfies $\pi Q=0$ when generator sums are defined. A finite irreducible chain has a unique such distribution and all transition rows converge to it. With absorbing states, every probability mixture on the closed absorbing states is an equilibrium, and limiting rows are determined by absorption probabilities. For a jump chain with stationary weights $\alpha_i$ and positive holding rates $\lambda_i$, the corresponding time-stationary weights are proportional to $\alpha_i/\lambda_i$.

## Transition intensity matrix

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For a finite-state [continuous-time Markov chain](continuous-time-markov-chain.md), a transition intensity matrix has nonnegative off-diagonal rates $q_{rs}$ and $q_{rr}=-\sum_{s\ne r}q_{rs}$. Every row sums to zero. In the time-homogeneous case its [transition probability matrix](#transition-semigroup-of-a-continuous-time-markov-chain) is the [matrix exponential](linear-operator-theory.md#matrix-exponential) $P(t)=e^{tQ}$. An [absorbing state](markov-chain.md#absorbing-state) has a zero row.

## Ergodic theorem for a finite continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For a finite [irreducible Markov chain](markov-chain.md#irreducible-markov-chain) in continuous time, time averages converge almost surely to averages under its unique [stationary distribution](markov-chain.md#stationary-distribution), from any initial state. Applying this to an activation indicator yields the corresponding [throughput](queueing-theory.md#throughput).

## Nonexplosive Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A [continuous-time Markov chain](continuous-time-markov-chain.md) is nonexplosive when it makes only finitely many jumps in every finite time interval, almost surely. Uniformly bounded total jump rates suffice. Another useful criterion bounds the states visited over each finite interval by a random finite set on which rates are bounded.

## Global balance for a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

Global balance equates total stationary incoming and outgoing [transition intensities](survival-analysis.md#transition-intensity) at each state. [Detailed balance for a continuous-time Markov chain](markov-chain.md#detailed-balance-for-a-continuous-time-markov-chain) is sufficient but stronger: it equates each pair separately.

## Poisson time-change representation of a Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A jump process with event types $k$, increments $\nu_k$, and rates $a_k(X)$ can be represented as $X(t)=X(0)+\sum_k\nu_k P_k(\int_0^t a_k(X(s-))\,ds)$, with independent unit-rate [Poisson processes](poisson-process.md). This represents the [Markov jump-process generator](#markov-jump-process-generator) through time-changed counts.

## Interchange process

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

Place one distinct label at each vertex of a finite connected weighted [graph](graph.md). At rate $c_{uv}=c_{vu}\geq0$, interchange the labels at $u$ and $v$. This [continuous-time Markov chain](continuous-time-markov-chain.md) has a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) as its [stationary distribution](markov-chain.md#stationary-distribution). The position of one label is the [random walk](random-walk.md) with the same rates.

### Aldous spectral gap theorem

↑ **Parent:** [Interchange process](#interchange-process)

On a finite connected weighted [graph](graph.md), the [interchange process](#interchange-process) and the single-label [random walk](random-walk.md) with the same symmetric rates have equal [spectral gaps](linear-operator-theory.md#spectral-gap). This is a substantial theorem, not just the elementary inclusion of the single-label [spectrum](linear-operator-theory.md#spectrum-functional-analysis) in the full [spectrum](linear-operator-theory.md#spectrum-functional-analysis). A proof is given in [Proof of Aldous' spectral gap conjecture](https://arxiv.org/abs/0906.1238), Theorem 1.1.

## Time reversal of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For an equilibrium chain with strictly positive stationary probabilities, reversed jump rates are $q^*_{ij}=\pi_jq_{ji}/\pi_i$. Under [detailed balance](markov-chain.md#detailed-balance) they equal the original rates, making the stationary path law reversible. Holding times and jump directions reverse together; this is more than symmetry of one-time distributions.

<h2 id="kingman-s-coalescent">Kingman's coalescent</h2>

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A partition-valued [Markov chain](markov-chain.md) in which every unordered pair of current blocks merges at rate one. On $n$ initial singleton blocks, the holding time with $j$ blocks is exponential with rate $\binom j2$. Restrictions to subsets of labels have the same law.

### Mutation count on a neutral coalescent tree

↑ **Parent:** [Kingman's coalescent](#kingman-s-coalescent)

In [Kingman's coalescent](#kingman-s-coalescent), the epoch with $j$ ancestral lineages lasts $T_j\sim\operatorname{Exp}(\binom j2)$, independently across epochs. If each lineage carries an independent [Poisson process](poisson-process.md) of [mutations](genetics.md#mutation) with rate $\theta/2$, its epoch mutation count satisfies $Y_j\mid T_j\sim\operatorname{Poisson}(j\theta T_j/2)$. The total mutation count is $S=\sum_{j=2}^nY_j$. Under the [infinite sites mutation model](population-genetics.md#infinite-sites-mutation-model), this also counts [segregating sites](population-genetics.md#segregating-site); without that assumption it still counts mutation events, which need not correspond one-to-one to observed polymorphisms.

#### Moments of the mutation count on a neutral coalescent tree

↑ **Parent:** [Mutation count on a neutral coalescent tree](#mutation-count-on-a-neutral-coalescent-tree)

The [independent mutation counts in coalescent epochs](#independent-mutation-counts-in-coalescent-epochs) have the [geometric mutation count in a coalescent epoch](#geometric-mutation-count-in-a-coalescent-epoch) laws. Summing their [expectations](expected-value.md) and [variances](variance.md) gives the displayed formulas, where $H_m=\sum_{i=1}^m1/i$ and $H_m^{(2)}=\sum_{i=1}^m1/i^2$. The extra quadratic term records randomness of the ancestral tree, beyond the conditional [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) variance.

#### Geometric mutation count in a coalescent epoch

↑ **Parent:** [Mutation count on a neutral coalescent tree](#mutation-count-on-a-neutral-coalescent-tree)

Integrating the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) [probability generating function](probability-distribution.md#probability-generating-function) over the [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of the epoch length gives

$$
\mathbb E[s^{Y_j}]=\frac{j-1}{j-1+\theta(1-s)}.
$$

Thus $Y_j$ has a [geometric distribution](discrete-probability-distribution.md#geometric-distribution) on $\{0,1,\ldots\}$, with [expectation](expected-value.md) $\theta/(j-1)$ and [variance](variance.md) $\theta/(j-1)+\theta^2/(j-1)^2$. The support convention matters: the count includes zero mutations.

#### Independent mutation counts in coalescent epochs

↑ **Parent:** [Mutation count on a neutral coalescent tree](#mutation-count-on-a-neutral-coalescent-tree)

The epoch lengths in [Kingman's coalescent](#kingman-s-coalescent) are [independent random variables](random-variable.md#independent-random-variables). Conditional on these lengths, [mutation](genetics.md#mutation) counts on disjoint tree pieces are independent [Poisson random variables](discrete-probability-distribution.md#poisson-distribution). Their conditional laws depend only on the corresponding epoch length, so integrating the product of conditional laws against the independent epoch laws leaves independent unconditional epoch mutation counts. This justifies adding their [variances](variance.md), rather than assuming independence from conditional independence alone.

### Total branch length of a neutral coalescent

↑ **Parent:** [Kingman's coalescent](#kingman-s-coalescent)

In coalescent units, independent waiting times satisfy $T_j\sim\operatorname{Exp}(j(j-1)/2)$, and total branch length is $L=\sum_{j=2}^n jT_j$. Therefore $EL=2\sum_{i=1}^{n-1}1/i$. The variables $jT_j/2$ are independent exponentials with rates $j-1$, so $W=L/2$ has the same distribution as the maximum of $n-1$ independent unit exponentials, with density $(n-1)e^{-w}(1-e^{-w})^{n-2}$. The last identity follows either from its Laplace transform or from the independent spacings of exponential order statistics.

<h3 id="kingman-s-infinite-coalescent">Kingman's infinite coalescent</h3>

↑ **Parent:** [Kingman's coalescent](#kingman-s-coalescent)

The consistent partition process on $\mathbb N$ whose finite restrictions are [Kingman's coalescent](#kingman-s-coalescent). It starts with infinitely many singleton blocks.

#### Coming down from infinity of the Kingman coalescent

↑ **Parent:** [Kingman's infinite coalescent](#kingman-s-infinite-coalescent)

For $t>0$, the number $B_t$ of blocks is finite almost surely. On a finite restriction, the expected time to reach $m$ blocks is at most $\sum_{j>m}2/[j(j-1)]=2/m$. [Markov inequality](probability-inequality.md#markov-s-inequality), followed by increasing the restriction, gives $\mathbb P(B_t>m)\leq2/(mt)$. Let $m\to\infty$, then use rational times and monotonicity to obtain the assertion simultaneously for every $t>0$.

## Entry count of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

The entry count $N_s(t)$ counts jumps of a [continuous-time Markov chain](continuous-time-markov-chain.md) into state $s$ by time $t$, excluding initial occupation. It is a [counting process](stochastic-process.md#counting-process). For homogeneous [transition intensities](survival-analysis.md#transition-intensity), its mean has derivative $\sum_{i\ne s}p_{ri}(t)q_{is}$ conditional on initial state $r$, so its [expected value](expected-value.md) is the sum of incoming rates times the expected [occupation times of a continuous-time Markov chain](#occupation-time-of-a-continuous-time-markov-chain). This density is an expected count rate, not necessarily a normalized [probability density function](continuous-probability-distribution.md#probability-density-function).

## Occupation time of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

The occupation time records the duration spent in a state of a [continuous-time Markov chain](continuous-time-markov-chain.md). Conditional on $Z(0)=r$, its [expected value](expected-value.md) is $\int_0^t p_{rs}(u)\,du$, where $p_{rs}$ is the [transition probability](markov-chain.md#transition-probability).

### Occupation time at an interior state of a variable-rate symmetric walk

↑ **Parent:** [Occupation time of a continuous-time Markov chain](#occupation-time-of-a-continuous-time-markov-chain)

For a [continuous-time Markov chain](continuous-time-markov-chain.md) with absorbing endpoints $0,N$ and rates $q_{j,j\pm1}=\lambda_j/2$, the jump chain is a [simple symmetric random walk](random-walk.md#simple-symmetric-random-walk). On leaving $i$, absorption before returning has probability $p_i=\tfrac12(1/i+1/(N-i))$, by [gambler's ruin](markov-chain.md#gambler-s-ruin) on each side. The [geometric return count before absorption](discrete-probability-distribution.md#geometric-return-count-before-absorption) and independent rate-$\lambda_i$ [holding times](#holding-time) give $\mathbb E_iI=1/(p_i\lambda_i)$. The rates at other states affect elapsed excursion times but not their return probabilities.

### Expected finite-horizon occupation time

↑ **Parent:** [Occupation time of a continuous-time Markov chain](#occupation-time-of-a-continuous-time-markov-chain)

For a finite-state homogeneous [continuous-time Markov chain](continuous-time-markov-chain.md) with [generator matrix](coding-theory.md#generator-matrix) $Q$, integrate the indicator of occupying state $j$ over $[0,T]$. Interchanging the bounded time integral and [expected value](expected-value.md) gives the displayed integral of [transition probabilities](markov-chain.md#transition-probability). It counts all visits, not only the first [holding time](#holding-time). Summing over states gives $T$. A zero [eigenvalue](linear-operator-theory.md#eigenvalue) of $Q$ does not cause a problem for this integral, although it prevents casually writing it with an [inverse matrix](matrix-inverse.md) $Q^{-1}$.

## Holding time

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

The holding time of a [continuous-time Markov chain](continuous-time-markov-chain.md) is the time spent in its current state before the next jump. In state $i$ it has an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate equal to the total outgoing rate $q_i$.

### Mean holding time from a transition intensity matrix

↑ **Parent:** [Holding time](#holding-time)

A state's [holding time](#holding-time) in a time-homogeneous [continuous-time Markov chain](continuous-time-markov-chain.md) is exponentially distributed with rate $-q_{rr}>0$. Its mean is $-1/q_{rr}$; the [probability](probability-theory.md#probability) that its next jump is to state $s$ is $q_{rs}/(-q_{rr})$. An absorbing state has infinite holding time.

#### Confidence interval for an inverse rate

↑ **Parent:** [Mean holding time from a transition intensity matrix](#mean-holding-time-from-a-transition-intensity-matrix)

For an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) with positive rate $\lambda$, the mean is $1/\lambda$. A [confidence interval](statistical-inference.md#confidence-interval) for the rate transforms to one for the mean by reversing and inverting its endpoints. The monotonic transformation preserves the coverage event; it does not give a [prediction interval](statistical-inference.md#prediction-interval) for one realized [holding time](#holding-time).

## Master equation

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Master_equation)

For transition rate $w_{ij}$ from state $i$ to state $j$, the master equation is

$$
\dot P_i=\sum_j(w_{ji}P_j-w_{ij}P_i).
$$

### Entropy production rate of a Markov chain

↑ **Parent:** [Master equation](#master-equation)

For edge current $J_{ij}=w_{ij}P_i-w_{ji}P_j$, the total entropy production rate is

$$
\dot S_{\rm tot}=\frac12\sum_{i,j}J_{ij}
\log\frac{w_{ij}P_i}{w_{ji}P_j}\geq0.
$$

It vanishes precisely when every occupied edge satisfies detailed balance.

## Continuous-time random walk

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous-time_random_walk)

A continuous-time random walk waits a random time at each site before jumping. Constant outgoing rates produce an exponential residence time, while the relative transition rates determine the destination of the next jump.

### Coalescing random walks

↑ **Parent:** [Continuous-time random walk](#continuous-time-random-walk)

Particles perform independent [continuous-time random walks](#continuous-time-random-walk) until they meet, after which they share one path. A finite initial particle set remains finite and its cardinality cannot increase. They arise as the common ancestors of sites in a [voter model](stochastic-process.md#voter-model). On the [square lattice](graph.md#square-lattice) every pair eventually coalesces, because the difference walk is [recurrent Markov chain](markov-chain.md#recurrent-markov-chain).

## Martingale problem for a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A finite-state process has generator $Q$ exactly when, for every function $f$ on the state space,

$$
f(X_t)-f(X_0)-\int_0^t(Qf)(X_s)\,ds
$$

is a martingale with respect to the process filtration.

## Transition-rate matrix

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transition-rate_matrix)

A Q-matrix has nonnegative off-diagonal entries and row sums zero. Its diagonal entry is the negative total rate out of the state.

## Transition semigroup of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For a time-homogeneous [continuous-time Markov chain](continuous-time-markov-chain.md), $P_{ij}(t)=\mathbb P_i(X_t=j)$ and the [matrices](vector-space.md#matrix) satisfy $P(s+t)=P(s)P(t)$, the [Chapman-Kolmogorov equation](markov-process.md#chapman-kolmogorov-equation). On a finite [state space](dynamical-systems.md#state-space) with [Q-matrix](#transition-rate-matrix) $Q$, the [matrix exponential](linear-operator-theory.md#matrix-exponential) gives $P(t)=e^{tQ}$.

The distinction from a discrete-time [transition matrix](markov-chain.md#stochastic-matrix) is the elapsed-time parameter: $P(t)$ describes where the process is after $t$ time units, allowing any number of intervening jumps. Each $P(t)$ is a [stochastic matrix](markov-chain.md#stochastic-matrix), with $P(0)=I$. A [Q-matrix](#transition-rate-matrix) instead records instantaneous rates and has row sums zero. Sampling at a fixed spacing $\Delta$ yields a [Discrete-time Markov chain](markov-chain.md#discrete-time-markov-chain) with [transition matrix](markov-chain.md#stochastic-matrix) $P(\Delta)$. See [Hao Wu's MIT lecture 21, transition semigroups](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/245cbb8888672b1b902c308fd6e2468f_MIT18_445S15_lecture21.pdf) and [lecture 22, infinitesimal rates](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/f6b1c125c2b471928e960a1d2c8ea6b5_MIT18_445S15_lecture22.pdf).

### Poisson-sampled continuous-time Markov chain

↑ **Parent:** [Transition semigroup of a continuous-time Markov chain](#transition-semigroup-of-a-continuous-time-markov-chain)

Sample a finite-state [continuous-time Markov chain](continuous-time-markov-chain.md) with generator $Q$ at the independent arrival times of a rate-$\lambda$ [Poisson process](poisson-process.md). The sampled states form a discrete-time Markov chain with transition matrix

$$
P_\lambda
=\int_0^\infty\lambda e^{-\lambda t}e^{tQ}\,dt
=\lambda(\lambda I-Q)^{-1}.
$$

Its invariant distributions are exactly those of the continuous-time chain.

### Kolmogorov equations

↑ **Parent:** [Transition semigroup of a continuous-time Markov chain](#transition-semigroup-of-a-continuous-time-markov-chain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov_equations)

For a finite-state [continuous-time Markov chain](continuous-time-markov-chain.md) with [Q-matrix](#transition-rate-matrix) $Q$, the backward and forward equations are $P'(t)=QP(t)$ and $P'(t)=P(t)Q$, respectively.

## Markov reward model

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Markov_reward_model)

A Markov reward model attaches a reward rate to each state and integrates it over the time spent there.

## Markov jump-process generator

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For transition rates $q_{nm}$, the generator acts on a function $f$ by

$$
(Lf)(n)=\sum_{m\ne n}q_{nm}\bigl(f(m)-f(n)\bigr).
$$

Whenever the expectations are finite,

$$
\frac d{dt}\mathbb E[f(N_t)]=\mathbb E[(Lf)(N_t)].
$$

Choosing polynomial functions $f$ gives differential equations for the moments.

### Exponential martingale from a jump generator

↑ **Parent:** [Markov jump-process generator](#markov-jump-process-generator)

For a positive function $g$ in the domain of a [Markov jump-process generator](#markov-jump-process-generator), the generator martingale for $g(X_t)$ and [semimartingale integration by parts](stochastic-calculus.md#semimartingale-integration-by-parts) give the displayed [local martingale](martingale.md#local-martingale). Suitable finite-horizon deterministic bounds on $g$ and $Lg/g$ make it a true [martingale](martingale.md). For a [single marked exponential jump process](#single-marked-exponential-jump-process), take $g(x)=e^{\theta x}$. Then the exponent's compensating process is $r_\theta(t\wedge T)$, where $r_\theta=(e^\theta-1)/\theta-1$ for $\theta\ne0$ and $r_0=0$; it is continuous adapted and hence [predictable](martingale.md#predictable-process).

### Forward operator of a Markov jump process

↑ **Parent:** [Markov jump-process generator](#markov-jump-process-generator)

For jumps $x\mapsto x+\nu_r$ of rates $a_r(x)$, the forward operator acts on a probability mass function by

$$
(L^*p)(x)=\sum_r\left[a_r(x-\nu_r)p(x-\nu_r)-a_r(x)p(x)\right].
$$

It is adjoint to the [Markov jump-process generator](#markov-jump-process-generator) $Lf(x)=\sum_ra_r(x)[f(x+\nu_r)-f(x)]$.

## Holding-time reversal along a fixed CTMC jump path

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

Conditioned on a finite jump path $i_0,\ldots,i_n$, the holding times are independent exponentials with the corresponding rates. Multiplying the probability of occupying $i_n$ at time $t$ by $q_{i_n}$ turns its simplex density into a product symmetric under reversal of the time portions and the state sequence.

## Recurrence equivalence for a CTMC and its fixed-time skeleton

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For $h>0$, the fixed-time skeleton has matrix $P(h)$. If $q_i$ is the holding rate, then for $nh\leq t\leq(n+1)h$,

$$
e^{-q_ih}p_{ii}(nh)\leq p_{ii}(t)
\leq e^{q_ih}p_{ii}((n+1)h).
$$

Thus $\int_0^\infty p_{ii}(t)dt$ diverges exactly when $\sum_np_{ii}(nh)$ does, proving recurrence equivalence for an irreducible chain.

## Jump chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

The jump chain records the successive states visited by a continuous-time Markov chain while discarding its holding times.

### Reflected nearest-neighbour random walk

↑ **Parent:** [Jump chain](#jump-chain)

On $\mathbb N$, let the chain jump from every $i\geq1$ to $i+1$ with probability $p$ and to $i-1$ with probability $1-p$, and jump from zero to one. It is recurrent exactly when $p\leq1/2$; at $p=1/2$ it is null recurrent.

### Invariant-measure transfer between a jump chain and a CTMC

↑ **Parent:** [Jump chain](#jump-chain)

For holding rates $q_i$, a measure $\pi$ satisfies $\pi Q=0$ exactly when $\mu_i=q_i\pi_i$ is invariant for the jump chain. Thus $\pi_i=\mu_i/q_i$ when normalization is possible.

#### Slow holding rates destroy positive recurrence

↑ **Parent:** [Invariant-measure transfer between a jump chain and a CTMC](#invariant-measure-transfer-between-a-jump-chain-and-a-ctmc)

Even when the jump chain has invariant probability $\mu$, the continuous-time invariant measure $\mu_i/q_i$ may have infinite mass if holding rates become too small, producing infinite mean return time.

#### Fast holding rates create continuous-time positive recurrence

↑ **Parent:** [Invariant-measure transfer between a jump chain and a CTMC](#invariant-measure-transfer-between-a-jump-chain-and-a-ctmc)

A recurrent jump chain with infinite invariant measure $\mu$ can yield a positive-recurrent continuous-time chain when $\sum_i\mu_i/q_i<\infty$.

### Nonexplosion from recurrent visits to a slow state

↑ **Parent:** [Jump chain](#jump-chain)

If the jump chain visits a state of finite holding rate infinitely often, the sum of its independent positive holding times at that state diverges almost surely, preventing explosion.

### Irreducibility and recurrence pass between a CTMC and its jump chain

↑ **Parent:** [Jump chain](#jump-chain)

For a [continuous-time Markov chain](continuous-time-markov-chain.md) whose jump times tend to infinity, the chain and its [jump chain](#jump-chain) have the same directed paths of positive-probability jumps. They are therefore [irreducible](markov-chain.md#irreducible-markov-chain) simultaneously, and a state is [recurrent](markov-chain.md#recurrent-state) for one exactly when it is recurrent for the other: the event of returning after departure depends only on the sequence of visited states.

## Explosion of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

Explosion occurs when infinitely many jumps take place in finite time.

Explosion is determined by whether the successive holding times of the [continuous-time Markov chain](continuous-time-markov-chain.md) have a finite sum.

### Nonexplosion under uniformly bounded jump rates

↑ **Parent:** [Explosion of a continuous-time Markov chain](#explosion-of-a-continuous-time-markov-chain)

If every holding rate of a [continuous-time Markov chain](continuous-time-markov-chain.md) is at most $C<\infty$, its holding times can be coupled as $E_n/q_{Y_n}\geq E_n/C$, where the $E_n$ are independent rate-one [exponential random variables](continuous-probability-distribution.md#exponential-distribution). The [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) gives $\sum_nE_n=\infty$ almost surely, so the jump times tend to infinity and the chain cannot [explode](#explosion-of-a-continuous-time-markov-chain).

### Explosion by summable holding times

↑ **Parent:** [Explosion of a continuous-time Markov chain](#explosion-of-a-continuous-time-markov-chain)

Conditional on a jump path $(Y_n)$, if $\sum_n1/q_{Y_n}<\infty$, then the sum of exponential holding times has finite expectation and is finite almost surely.

### Explosion of an upward-biased walk with geometrically increasing rates

↑ **Parent:** [Explosion of a continuous-time Markov chain](#explosion-of-a-continuous-time-markov-chain)

Suppose a transient nearest-neighbour jump chain on $\mathbb N$ has uniformly bounded expected visits to each state and the holding rate at $i$ grows geometrically. Then

$$
\mathbb E\sum_n\frac1{q_{Y_n}}
=\sum_i\frac{\mathbb E V_i}{q_i}<\infty,
$$

so the continuous-time chain explodes almost surely.

## Invariant distribution of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For a finite-state chain with transition semigroup $P(t)=e^{tQ}$, a probability row vector $\pi$ is invariant when $\pi P(t)=\pi$ for every $t\geq0$. Equivalently,

$$
\pi Q=0.
$$

### Nonuniqueness of invariant distributions of a finite Markov chain

↑ **Parent:** [Invariant distribution of a continuous-time Markov chain](#invariant-distribution-of-a-continuous-time-markov-chain)

Every closed communicating class of a finite Markov chain has its own invariant probability distribution. All invariant distributions are convex combinations of those class distributions. In particular, a finite irreducible chain has a unique invariant distribution, while a reducible chain may have many.

### Invariant distribution of an explosive chain

↑ **Parent:** [Invariant distribution of a continuous-time Markov chain](#invariant-distribution-of-a-continuous-time-markov-chain)

An explosive chain can have a summable solution of $\pi Q=0$ despite being transient. Nonexplosion is needed for the usual equivalence between invariant distributions and positive recurrence.

## Batch-birth linear-death process

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A batch-birth linear-death process has transitions

$$
n\longrightarrow n+k\quad\hbox{at rate }\lambda,
\qquad
n\longrightarrow n-1\quad\hbox{at rate }\beta n.
$$

Writing $P_n(t)=\mathbb P(N_t=n)$ and taking $P_j=0$ for $j<0$, its master equation is

$$
\dot P_n=\lambda P_{n-k}+\beta(n+1)P_{n+1}-(\lambda+\beta n)P_n.
$$

### Moments of a batch-birth linear-death process

↑ **Parent:** [Batch-birth linear-death process](#batch-birth-linear-death-process)

For $m=\mathbb E N$ and $v=\operatorname{var}N$, the Markov jump-process generator applied to $n$ and $n^2$ gives

$$
m'=k\lambda-\beta m,
\qquad
v'=k^2\lambda+\beta m-2\beta v.
$$

Consequently

$$
m\longrightarrow\frac{k\lambda}{\beta},
\qquad
v\longrightarrow\frac{k(k+1)\lambda}{2\beta}.
$$

## Birth-death process

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birth–death_process)

A birth-death process moves only between neighbouring nonnegative integer states, with state-dependent birth and death rates.

### Birth process

↑ **Parent:** [Birth-death process](#birth-death-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birth_process)

A pure birth process on $\mathbb N_0$ jumps only from $n$ to $n+1$, at a strictly positive rate $\lambda_n$. Its successive holding times are independent exponential variables of rates $\lambda_n$.

#### Exponential martingale of a pure birth process

↑ **Parent:** [Birth process](#birth-process)

For a [pure birth process](#birth-process) with fixed initial state and finite statewise rates, the jump-count compensator gives $dM=(e^\theta-1)M_{-}[dN-\lambda(X_{-})dt]$, so $M$ is a [local martingale](martingale.md#local-martingale) up to explosion. If $\lambda\le C$, a rate-$C$ Poisson candidate clock with accepted jumps of probability $\lambda(X_{-})/C$ prevents explosion and dominates the jump count. Its finite exponential moments dominate every stopped $M$ on each finite horizon, upgrading the local martingale to a true martingale. A random initial state requires $\mathbb E e^{\theta X_0}<\infty$; uniformly bounded rates do not supply this missing initial integrability.

#### Logistic cell-division process

↑ **Parent:** [Birth process](#birth-process)

For a carrying capacity $N$, each of $k$ cells splits into two at rate $1-k/N$, so the population increases by one at the displayed total rate and is absorbed at $N$. Starting from population density $p\in(0,1)$, its normalized density converges on finite horizons to $p e^t/(1-p+p e^t)$ by the [Kurtz fluid limit theorem](queueing-theory.md#kurtz-fluid-limit-theorem).

// Target: analysis.bigb

#### Nonexplosion criterion for a pure birth process

↑ **Parent:** [Birth process](#birth-process)

A pure birth process is nonexplosive exactly when

$$
\sum_{n=0}^{\infty}\frac1{\lambda_n}=\infty.
$$

Its explosion time is the sum of independent exponential holding times. If the displayed series converges, that sum has finite expectation. If it diverges, the Laplace transform of the sum is

$$
\prod_n\frac{\lambda_n}{\lambda_n+s}=0,
$$

forcing the sum to be infinite almost surely.

#### Linear birth process with immigration

↑ **Parent:** [Birth process](#birth-process)

The pure birth process with rates $\lambda_n=\alpha n+\beta$, where $\alpha,\beta>0$, combines linear reproduction with immigration. Starting from zero, its mean satisfies

$$
m'(t)=\alpha m(t)+\beta,
\qquad
m(0)=0,
$$

and hence

$$
\mathbb EN(t)=\frac{\beta}{\alpha}(e^{\alpha t}-1).
$$

##### Linear birth process with catastrophes

↑ **Parent:** [Linear birth process with immigration](#linear-birth-process-with-immigration)

Add independent rate-$\mu$ resets to zero to a [linear birth process with immigration](#linear-birth-process-with-immigration). The resulting irreducible [continuous-time Markov chain](continuous-time-markov-chain.md) is nonexplosive by domination of births and finiteness of Poisson reset counts. When $\mu=\lambda$, an excursion from one reaches $n$ with probability $2/(n+1)$, so its [jump chain](#jump-chain) is recurrent with infinite expected jump count. The elapsed return-cycle time instead has mean

$$
\lambda^{-1}+\sum_{n\ge1}\frac{2}{\lambda(n+1)(n+2)}=2/\lambda.
$$

Thus the continuous-time chain is positive recurrent while its jump chain is null recurrent. Its stationary probabilities are $\pi_0=1/2$ and $\pi_n=1/[(n+1)(n+2)]$ for $n\ge1$.

### Yule process

↑ **Parent:** [Birth-death process](#birth-death-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Yule_process)

The Yule process is the pure birth process with rate $n\lambda$ in population state $n$. Starting from one individual, it is nonexplosive because the independent holding times have divergent total almost surely.

#### Mean population of a Yule process

↑ **Parent:** [Yule process](#yule-process)

For the Yule process starting from one individual, the generator applied to $f(n)=n$ gives

$$
\frac d{dt}\mathbb E X_t=\lambda\mathbb E X_t,
\qquad \mathbb E X_0=1,
$$

and hence $\mathbb E X_t=e^{\lambda t}$.

#### Conditional Yule birth times

↑ **Parent:** [Yule process](#yule-process)

Given $X_t=n+1$, the $n$ birth times in a Yule process have the law of the order statistics of independent variables with density

$$
f(x)=\frac{\lambda e^{\lambda x}}{e^{\lambda t}-1},
\qquad0\leq x\leq t.
$$

This follows by dividing the joint holding-time density by  
$\mathbb P(X_t=n+1)=e^{-\lambda t}(1-e^{-\lambda t})^n$.

### Extinction probability of a linear birth-death process

↑ **Parent:** [Birth-death process](#birth-death-process)

For individual birth and death rates $\lambda,\mu$ and one initial individual, the finite-time extinction probability satisfies

$$
h'=(h-1)(\lambda h-\mu),\qquad h(0)=0.
$$

When $\lambda\ne\mu$,

$$
h(t)=\frac{\mu(1-e^{-(\lambda-\mu)t})}
{\lambda-\mu e^{-(\lambda-\mu)t}}.
$$

### Detailed balance for a birth-death process

↑ **Parent:** [Birth-death process](#birth-death-process)

For birth rates $b_i$ and death rates $d_i$, a reversible measure satisfies

$$
\pi_i b_i=\pi_{i+1}d_{i+1}.
$$

Thus $\pi_{i+1}/\pi_i=b_i/d_{i+1}$, and it is an invariant distribution when the resulting measure is summable and the chain is nonexplosive.

### Birth-death master equation

↑ **Parent:** [Birth-death process](#birth-death-process)

For birth rates $b_n$, death rates $d_n$, and state probabilities $P_n$,

$$
\dot P_n=b_{n-1}P_{n-1}+d_{n+1}P_{n+1}-(b_n+d_n)P_n.
$$

#### First-moment equation of a birth-death process

↑ **Parent:** [Birth-death master equation](#birth-death-master-equation)

Since births and deaths change the state by $+1$ and $-1$,

$$
\frac d{dt}\mathbb{E} N_t=\mathbb{E}[b_{N_t}-d_{N_t}].
$$

#### Moment equations of a linear birth-death process

↑ **Parent:** [Birth-death master equation](#birth-death-master-equation)

For per-capita birth and death rates $B$ and $D$, the rates are $b_n=Bn$ and $d_n=Dn$. If $\mu=\mathbb EN_t$ and $\sigma^2=\operatorname{var}N_t$, then

$$
\mu'=(B-D)\mu,
\qquad
(\sigma^2)'=2(B-D)\sigma^2+(B+D)\mu.
$$

The [expected value](expected-value.md) sees only the net growth rate $B-D$, whereas the [variance](variance.md) also sees the total event rate $B+D$.

#### Factorial moment

↑ **Parent:** [Birth-death master equation](#birth-death-master-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Factorial_moment)

The $r$th falling factorial moment is $\mathbb{E}[(N)_r]$, where $(N)_r=N(N-1)\cdots(N-r+1)$.

##### Factorial-moment inversion

↑ **Parent:** [Factorial moment](#factorial-moment)

For a nonnegative integer-valued [random variable](random-variable.md), the displayed inversion is valid when $\mathbb E(X)_s s^k/s!\to0$. Indeed the gap between consecutive [Jordan-Bonferroni exact-occurrence inequalities](combinatorics.md#jordan-bonferroni-exact-occurrence-inequalities) is $\mathbb E(X)_{k+m+1}/[k!(m+1)!]$, which tends to zero under this hypothesis. No exchange of an infinite signed sum with an [expectation](expected-value.md) is needed.

##### Poisson factorial moments

↑ **Parent:** [Factorial moment](#factorial-moment)

If $N$ is Poisson with mean $\lambda$, then $\mathbb{E}[(N)_r]=\lambda^r$; in particular, $\mathbb{E}N=\lambda$ and $\mathbb{E}[N(N-1)]=\lambda^2$.

###### Factorial-moment criterion for Poisson convergence

↑ **Parent:** [Poisson factorial moments](#poisson-factorial-moments)

If nonnegative integer-valued [random variables](random-variable.md) $X_n$ have all fixed [factorial moments](#factorial-moment) converging to $\lambda^k$, then their [convergence in distribution](convergence-of-random-variables.md#convergence-in-distribution) is to the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with mean $\lambda$. The first-moment bound gives [uniform tightness](probability-space.md#uniform-tightness), and bounds on higher moments give [uniform integrability](convergence-of-random-variables.md#uniform-integrability) of each fixed lower moment. Every subsequential limit therefore has the indicated [factorial moments](#factorial-moment). For such a limit $X$ and $t\geq0$, the nonnegative binomial expansion and the [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) give $\mathbb E(1+t)^X=\sum_{k\geq0}t^k\lambda^k/k!=e^{\lambda t}$. This identifies its [moment-generating function](probability-distribution.md#moment-generating-function) as that of the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution), uniquely determining the limit.

### Poisson moment closure for a birth-death process

↑ **Parent:** [Birth-death process](#birth-death-process)

Approximating the population law by a Poisson law replaces its first two factorial moments by $\lambda$ and $\lambda^2$, closing a quadratic first-moment equation as a Riccati equation for $\lambda$.

### Diffusion approximation of a birth-death process

↑ **Parent:** [Birth-death process](#birth-death-process)

For unit jumps with birth and death rates $b(x),d(x)$, the Fokker--Planck drift and diffusion in the convention

$$
\partial_tP=-\partial_x(uP)+\partial_x^2(DP)
$$

are $u=b-d$ and $D=(b+d)/2$.

#### Linear noise approximation

↑ **Parent:** [Diffusion approximation of a birth-death process](#diffusion-approximation-of-a-birth-death-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_noise_approximation)

Near a stable deterministic equilibrium, replace the drift by its linearization and the diffusion coefficient by its equilibrium value. The resulting Ornstein-Uhlenbeck approximation has a stationary [normal distribution](probability-distribution.md#normal-distribution).

##### Chemical diffusion matrix

↑ **Parent:** [Linear noise approximation](#linear-noise-approximation)

A reaction's [stoichiometric vector](mathematical-biology.md#stoichiometric-vector) outer product multiplied by its [reaction propensity function](mathematical-biology.md#reaction-propensity-function) is its contribution to the infinitesimal state-increment covariance. Summing over channels gives $B$. Its normalized form $D$ divides by the two mean copy numbers. The [Fokker-Planck equation](probability-theory.md#fokker-planck-equation) writes the associated second-derivative term with $B/2$; the covariance evolution and normalized stationary Lyapunov equation instead use $B$ and $D$ themselves. A simultaneous unit loss of two species contributes positive cross noise even when their long-time stationary covariance is negative.

##### Normalized stationary fluctuation-dissipation relation for a reaction network

↑ **Parent:** [Linear noise approximation](#linear-noise-approximation)

Let $A$ be the drift Jacobian at a stable mean-field equilibrium, $S=\operatorname{diag}(\mu_i)$, and $B=\sum_ra_r\nu_r\nu_r^{\mathsf T}$ the reaction noise matrix. For normalized fluctuations, put $M=-S^{-1}AS$, $D=S^{-1}BS^{-1}$, and $\eta_{ij}=\operatorname{Cov}(X_i,X_j)/(\mu_i\mu_j)$. Stationarity of the linear-noise covariance gives the displayed [Continuous Lyapunov equation](control-theory.md#continuous-lyapunov-equation). It applies to driven reaction networks without requiring thermal equilibrium. A mode with zero restoring eigenvalue and nonzero noise has no stationary covariance.

// Target: mathematical-biology.bigb

###### Feedback attenuation of gene-expression noise

↑ **Parent:** [Normalized stationary fluctuation-dissipation relation for a reaction network](#normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network)

For RNA birth/death rates $\lambda_1,\beta_1x_1$ and protein rates $\lambda_2x_1f(x_2),\beta_2x_2$, linearize at stationary means $m_1,m_2$. Put $H=1-\partial\log f/\partial\log x_2=1+h$. The relative-fluctuation drift is $\begin{pmatrix}-\beta_1&0\\\beta_2&-\beta_2H\end{pmatrix}$ and the diffusion matrix is $\operatorname{diag}(2\beta_1/m_1,2\beta_2/m_2)$. The stationary covariance equation gives the displayed normalized protein variance. Its extrinsic part factors as $H^{-2}[\beta_2H/(\beta_1+\beta_2H)]m_1^{-1}$: static susceptibility squared times a time-averaging factor times environmental noise. Faster response alone weakens averaging; feedback reduces susceptibility and thereby lowers noise. The formula is exact for affine rates when $H=1$, and is a [linear noise approximation](#linear-noise-approximation) for nonlinear feedback.

##### Ornstein-Uhlenbeck fluctuation limit at a stable population equilibrium

↑ **Parent:** [Linear noise approximation](#linear-noise-approximation)

For a unit-jump population chain with one-step probabilities $\alpha k/n$ and $\beta k^2/n^2$, its equilibrium density is $u_0=\alpha/\beta$. Speed time by $n$ and center and scale the population as $(k-nu_0)/\sqrt n$. The accelerated conditional drift is $-\alpha x-\beta x^2/\sqrt n$, and the second moment is $2\alpha^2/\beta+3\alpha x/\sqrt n+\beta x^2/n$. Their compact-set limits give the displayed [Ornstein-Uhlenbeck process](gaussian-process.md#ornstein-uhlenbeck-process). If $2\alpha^2<\beta$, the invalid-probability threshold stays a fixed positive density distance above equilibrium. Before that threshold, the generator of $x^2$ is at most one because its drift contribution is nonpositive. The stopped [Lyapunov function](dynamical-systems.md#lyapunov-function) bound proves [compact containment](convergence-of-random-variables.md#compact-containment) and makes the probability of hitting that threshold on a fixed accelerated horizon tend to zero. This supplies the global hypotheses of the [diffusion approximation theorem](stochastic-calculus.md#diffusion-approximation-theorem).

<h4 id="mean-drift-from-a-fokker-planck-equation">Mean drift from a Fokker--Planck equation</h4>

↑ **Parent:** [Diffusion approximation of a birth-death process](#diffusion-approximation-of-a-birth-death-process)

If boundary fluxes decay sufficiently fast, two integrations by parts give

$$
\frac d{dt}\mathbb{E} X_t=\mathbb{E}[u(X_t)],
$$

while the diffusion term contributes zero to the first moment.

### Birth-death recurrence classification

↑ **Parent:** [Birth-death process](#birth-death-process)

For constant birth rate $\lambda$ and death rate $\delta$ away from zero, the chain is transient when $\lambda>\delta$, null recurrent when $\lambda=\delta$, and positive recurrent when $\lambda<\delta$.

<h3 id="m-m-1-queue">M/M/1 queue</h3>

↑ **Parent:** [Birth-death process](#birth-death-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/M/M/1_queue)

The queue length in an $M/M/1$ queue is a birth-death process with constant arrival rate $\lambda$ and service rate $\mu$ while nonempty.

#### Stationary workload of an exponential-payload queue

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)

With packet arrival rate lambda, independent exponential payloads of mean one and byte-service rate C, let $\rho=\lambda/C<1$. The number N of unfinished packets has law $(1-\rho)\rho^n$. Conditional on N=n, the remaining payloads are n independent unit-mean exponentials, including the in-service residual by memorylessness. Summing their [Laplace transforms](integral-transform.md#laplace-transform) gives $\mathbb E e^{-sW}=(1-\rho)(1+s)/(1+s-\rho)$. Thus W has mass $1-\rho$ at zero and, conditional on positivity, is exponential with rate $1-\rho$. The probability of at least r headers is instead $\rho^r$ for integer r.

#### M-M-1 queue with state-dependent admission

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)

If potential arrivals form a Poisson process of rate $\lambda$ and an arrival seeing $n$ customers joins with probability $p(n)$, the queue length is a [birth-death process](#birth-death-process) with birth rate $b_n=\lambda p(n)$ and death rate $d_n=\mu$ for $n\geq1$. Its stationary ratios, when normalizable, are

$$
\frac{\pi_{n+1}}{\pi_n}=\frac{\lambda p(n)}\mu.
$$

#### Positive recurrence of an M-M-1 queue

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)

An $M/M/1$ queue is positive recurrent exactly when its traffic intensity $\rho=\lambda/\mu$ is below one.

#### Stationary distribution of an M-M-1 queue

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)

When $\rho<1$, the equilibrium queue length has distribution $\pi_n=(1-\rho)\rho^n$ and mean $\rho/(1-\rho)$.

<h4 id="burke-s-theorem">Burke's theorem</h4>

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burke's_theorem)

At equilibrium, the departure process of a stable $M/M/1$ queue is Poisson with the same rate as the arrival process.

#### M-M-1 queue with Bernoulli feedback

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)

If a served customer returns with probability $p$, thinning service completions gives effective external departure rate $\mu(1-p)$ for the queue-length process.

##### Poisson output theorem for a feedback queue

↑ **Parent:** [M-M-1 queue with Bernoulli feedback](#m-m-1-queue-with-bernoulli-feedback)

In equilibrium, a Bernoulli-feedback $M/M/1$ queue has the same queue-length process as an ordinary queue with service rate $\mu(1-p)$, so its external departures form a Poisson process of rate $\lambda$.

#### Mean busy period of an M-M-1 queue

↑ **Parent:** [M/M/1 queue](#m-m-1-queue)

Starting with one customer, the mean busy period of an $M/M/1$ queue is

$$
\mathbb EB=\frac1{\mu-\lambda}
$$

when $\lambda<\mu$. It is infinite when $\lambda\geq\mu$.

<h3 id="m-m-∞-queue">M/M/∞ queue</h3>

↑ **Parent:** [Birth-death process](#birth-death-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/M/M/∞_queue)

An $M/M/\infty$ queue has [Poisson](poisson-process.md) arrivals of rate $\lambda$, [independent](random-variable.md#independent-random-variables) exponential service times of rate $\mu$, and infinitely many servers. Its occupancy is a [birth-death process](#birth-death-process) with birth rate $\lambda$ and death rate $n\mu$ in state $n$.

#### Stationary distribution of an M-M-infinity queue

↑ **Parent:** [M/M/∞ queue](#m-m-∞-queue)

For every $\lambda,\mu>0$, an $M/M/\infty$ queue is positive recurrent and has the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with mean $\rho=\lambda/\mu$ as its unique stationary distribution:

$$
\pi_n=e^{-\rho}\frac{\rho^n}{n!}.
$$

#### Burke theorem for an M-M-infinity queue

↑ **Parent:** [M/M/∞ queue](#m-m-∞-queue)

In stationarity, the departure process of an $M/M/\infty$ queue is a [Poisson process](poisson-process.md) of rate $\lambda$. By time reversibility, the departures before any fixed time are independent of the occupancy at that time.

#### Transient distribution of an M-M-infinity queue

↑ **Parent:** [M/M/∞ queue](#m-m-∞-queue)

If $X_0=n$ and $p_t=e^{-\mu t}$, then

$$
X_t\overset{d}{=}
\operatorname{Binomial}(n,p_t)
+\operatorname{Poisson}\!\left(\frac\lambda\mu(1-p_t)\right),
$$

with independent summands. The binomial term counts surviving initial customers; [Poisson thinning](poisson-process.md#poisson-thinning) gives the surviving later arrivals.

#### Mean busy period of an M-M-infinity queue

↑ **Parent:** [M/M/∞ queue](#m-m-∞-queue)

Writing $\rho=\lambda/\mu$, the stationary empty probability is $e^{-\rho}$. Alternating idle periods of mean $1/\lambda$ with busy periods and applying the renewal-reward theorem gives

$$
\mathbb EB=\frac{e^\rho-1}{\lambda}.
$$

### M-M-s-K queue

↑ **Parent:** [Birth-death process](#birth-death-process)

An $M/M/s/K$ queue has arrivals forming a [Poisson process](poisson-process.md) of rate $\lambda$, $s$ servers with independent service times having an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate $\mu$, and total system capacity $K\geq s$. Its occupancy is the finite [birth-death process](#birth-death-process) on $\{0,\ldots,K\}$ with

$$
b_n=\lambda\mathbf1_{\{n<K\}},
\qquad
d_n=\mu\min(n,s).
$$

#### Stationary distribution of an M-M-s-K queue

↑ **Parent:** [M-M-s-K queue](#m-m-s-k-queue)

Put $\rho=\lambda/\mu$. The unique stationary distribution of an $M/M/s/K$ queue is

$$
\pi_n=\frac1Z
\begin{cases}
\rho^n/n!,&0\leq n\leq s,\\
\rho^n/(s!s^{n-s}),&s<n\leq K,
\end{cases}
$$

where $Z$ is the sum of the displayed weights. Adjacent terms satisfy [detailed balance for a birth-death process](#detailed-balance-for-a-birth-death-process), so the queue is reversible in equilibrium.

## ↑ Ancestors (7)

1. [Markov chain](markov-chain.md)
2. [Markov process](markov-process.md)
3. [Probability theory](probability-theory.md)
4. [Probability and statistics](probability-and-statistics.md)
5. [Area of mathematics](mathematics.md#area-of-mathematics)
6. [Mathematics](mathematics.md)
7. [Codex Wiki](README.md)

## ← Incoming links (109)

- [Alternating arrival and service queue](queueing-theory.md#alternating-arrival-and-service-queue)
- [Chemical master equation](mathematical-biology.md#chemical-master-equation)
- [Closed migration process](queueing-theory.md#closed-migration-process)
- [Detailed balance for a continuous-time Markov chain](markov-chain.md#detailed-balance-for-a-continuous-time-markov-chain)
- [Entry count of a continuous-time Markov chain](#entry-count-of-a-continuous-time-markov-chain)
- [Expected finite-horizon occupation time](#expected-finite-horizon-occupation-time)
- [Explosion of a continuous-time Markov chain](#explosion-of-a-continuous-time-markov-chain)
- [First-passage-time density](markov-chain.md#first-passage-time-density)
- [Geometric return count before absorption](discrete-probability-distribution.md#geometric-return-count-before-absorption)
- [Heterogeneous two-server queue](queueing-theory.md#heterogeneous-two-server-queue)
- [Holding time](#holding-time)
- [Interchange process](#interchange-process)
- [Irreducibility and recurrence pass between a CTMC and its jump chain](#irreducibility-and-recurrence-pass-between-a-ctmc-and-its-jump-chain)
- [Jukes-Cantor model](genetics.md#jukes-cantor-model)
- [Kolmogorov equations](#kolmogorov-equations)
- [Linear birth process with catastrophes](#linear-birth-process-with-catastrophes)
- [Markov chain](markov-chain.md)
- [Markov process](markov-process.md)
- [Mean holding time from a transition intensity matrix](#mean-holding-time-from-a-transition-intensity-matrix)
- [Nonexplosion of a continuous-time Markov chain](#nonexplosion-of-a-continuous-time-markov-chain)
- [Nonexplosion under uniformly bounded jump rates](#nonexplosion-under-uniformly-bounded-jump-rates)
- [Nonexplosive Markov chain](#nonexplosive-markov-chain)
- [Nucleotide substitution model](biology.md#nucleotide-substitution-model)
- [Occupation time at an interior state of a variable-rate symmetric walk](#occupation-time-at-an-interior-state-of-a-variable-rate-symmetric-walk)
- [Occupation time of a continuous-time Markov chain](#occupation-time-of-a-continuous-time-markov-chain)
- [Open migration process](queueing-theory.md#open-migration-process)
- [Optical pumping versus relaxation](atomic-physics.md#optical-pumping-versus-relaxation)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37.md#5/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-74.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#26i/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#26i/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#26i/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#26i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#25i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-40.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#27j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#27j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#26j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#27i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#26i/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#26i/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#26i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#26i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207.md#3/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#27k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#25k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#3/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#3/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#28k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#28k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#28k/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#27k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#28k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#27k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#27k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#28j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#27j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-207.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-207.md#2/b/solution)
- [Solution](past-exam-of-the-plant-sciences-course-of-the-university-of-cambridge/2025/paper-plm3.md#2/solution)
- [Solution](past-exam-of-the-plant-sciences-course-of-the-university-of-cambridge/2025/paper-plm3.md#3/solution)
- [Poisson-sampled continuous-time Markov chain](#poisson-sampled-continuous-time-markov-chain)
- [Processor sharing](queueing-theory.md#processor-sharing)
- [Random transposition shuffle](markov-chain.md#random-transposition-shuffle)
- [Regime-switching Merton equations](utility-function.md#regime-switching-merton-equations)
- [SIRS Markov chain](mathematical-biology.md#sirs-markov-chain)
- [Stability conditions for a two-resource linear flow network](queueing-theory.md#stability-conditions-for-a-two-resource-linear-flow-network)
- [Stationary law of a linear flow network](queueing-theory.md#stationary-law-of-a-linear-flow-network)
- [Stochastic chemical kinetics](mathematical-biology.md#stochastic-chemical-kinetics)
- [Stochastic epidemic model](mathematical-biology.md#stochastic-epidemic-model)
- [Stochastic SIR model](mathematical-biology.md#stochastic-sir-model)
- [Three-state irreversible disease model](survival-analysis.md#three-state-irreversible-disease-model)
- [Three-sublevel optical pumping model](atomic-physics.md#three-sublevel-optical-pumping-model)
- [Transition intensity matrix](#transition-intensity-matrix)
- [Transition semigroup of a continuous-time Markov chain](#transition-semigroup-of-a-continuous-time-markov-chain)
- [Two-state ion-channel gating](membrane-potential.md#two-state-ion-channel-gating)
