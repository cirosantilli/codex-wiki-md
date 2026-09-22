# Game theory

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Game_theory)

Game theory studies strategic interaction among decision makers.

**Table of contents**

- [Prisoner's dilemma](#prisoner-s-dilemma)
  - [Iterated prisoner's dilemma](#iterated-prisoner-s-dilemma)
    - [Reactive strategy (game theory)](#reactive-strategy-game-theory)
      - [Always defect](#always-defect)
      - [Always cooperate](#always-cooperate)
      - [Tit for tat](#tit-for-tat)
        - [Tit for tat invasion of a reactive resident](#tit-for-tat-invasion-of-a-reactive-resident)
          - [Finite-horizon invasion threshold of Tit for tat against unconditional defection](#finite-horizon-invasion-threshold-of-tit-for-tat-against-unconditional-defection)
        - [Neutrality between Tit for tat and unconditional cooperation](#neutrality-between-tit-for-tat-and-unconditional-cooperation)
      - [Long-run payoff of reactive strategies](#long-run-payoff-of-reactive-strategies)
- [Evolutionary game theory](#evolutionary-game-theory)
  - [Replicator equation](#replicator-equation)
- [Repeated game](#repeated-game)
- [Payoff](#payoff)
- [Costly turnout game](#costly-turnout-game)
  - [Turnout equilibria with two supporters and one opponent](#turnout-equilibria-with-two-supporters-and-one-opponent)
  - [Pivotal voting probability](#pivotal-voting-probability)
- [Nonatomic congestion game](#nonatomic-congestion-game)
- [Congestion game](#congestion-game)
- [Evolutionarily stable strategy](#evolutionarily-stable-strategy)
  - [Selection gradient](#selection-gradient)
  - [Hawk-Dove game](#hawk-dove-game)
  - [Two-condition criterion for evolutionary stability](#two-condition-criterion-for-evolutionary-stability)
- [Security level payoff](#security-level-payoff)
- [Nash bargaining problem](#nash-bargaining-problem)
  - [Negotiation set in two-person bargaining](#negotiation-set-in-two-person-bargaining)
  - [Joint dominance of payoff vectors](#joint-dominance-of-payoff-vectors)
  - [Bargaining individual rationality](#bargaining-individual-rationality)
  - [Bargaining independence of irrelevant alternatives](#bargaining-independence-of-irrelevant-alternatives)
  - [Positive affine invariance in bargaining](#positive-affine-invariance-in-bargaining)
  - [Bargaining symmetry](#bargaining-symmetry)
  - [Nash bargaining solution](#nash-bargaining-solution)
    - [Maximin bargaining solution](#maximin-bargaining-solution)
    - [Supporting triangle for Nash bargaining](#supporting-triangle-for-nash-bargaining)
    - [Nash product](#nash-product)
  - [Disagreement point](#disagreement-point)
- [Cooperative game theory](#cooperative-game-theory)
  - [Transferable utility game](#transferable-utility-game)
    - [Coverage coalitional game](#coverage-coalitional-game)
      - [Shapley value of a coverage game](#shapley-value-of-a-coverage-game)
      - [Core of a coverage game](#core-of-a-coverage-game)
    - [Bankruptcy game](#bankruptcy-game)
    - [Superadditive coalitional game](#superadditive-coalitional-game)
    - [Glove game](#glove-game)
      - [Core of a glove game](#core-of-a-glove-game)
    - [Characteristic function of a coalitional game](#characteristic-function-of-a-coalitional-game)
    - [Dual coalitional game](#dual-coalitional-game)
    - [Nucleolus](#nucleolus)
      - [Prenucleolus](#prenucleolus)
    - [Imputation in a coalitional game](#imputation-in-a-coalitional-game)
    - [Marginal contribution](#marginal-contribution)
    - [Coalition (game theory)](#coalition-game-theory)
      - [Excess of a coalition](#excess-of-a-coalition)
    - [Convex cooperative game](#convex-cooperative-game)
      - [Shapley population monotonicity in a convex game](#shapley-population-monotonicity-in-a-convex-game)
      - [Shapley value belongs to the core of a convex game](#shapley-value-belongs-to-the-core-of-a-convex-game)
    - [Core (game theory)](#core-game-theory)
      - [Core of the miners game](#core-of-the-miners-game)
    - [Shapley value](#shapley-value)
      - [Shapley limit in a buyer-heavy exchange market](#shapley-limit-in-a-buyer-heavy-exchange-market)
      - [Balanced contributions of Shapley values](#balanced-contributions-of-shapley-values)
      - [Shapley wages in an entrepreneur-worker game](#shapley-wages-in-an-entrepreneur-worker-game)
      - [Shapley self-duality](#shapley-self-duality)
      - [Marginal contribution vector](#marginal-contribution-vector)
    - [Weighted voting game](#weighted-voting-game)
    - [Simple cooperative game](#simple-cooperative-game)
- [Payoff-equivalent strategies](#payoff-equivalent-strategies)
- [Normal-form game](#normal-form-game)
- [Subgame perfect equilibrium](#subgame-perfect-equilibrium)
- [Stackelberg competition](#stackelberg-competition)
  - [Stackelberg equilibrium](#stackelberg-equilibrium)
- [Contest theory](#contest-theory)
  - [Sequential elimination all-pay contest](#sequential-elimination-all-pay-contest)
    - [Backward-induction threshold in an elimination all-pay contest](#backward-induction-threshold-in-an-elimination-all-pay-contest)
      - [Vanishing-discount limit of an elimination all-pay contest](#vanishing-discount-limit-of-an-elimination-all-pay-contest)
        - [Ranked winning probabilities in an undiscounted elimination contest](#ranked-winning-probabilities-in-an-undiscounted-elimination-contest)
    - [Discounted continuation value in an elimination contest](#discounted-continuation-value-in-an-elimination-contest)
      - [Effective prize in a sequential contest](#effective-prize-in-a-sequential-contest)
  - [Sequential private-value all-pay contest](#sequential-private-value-all-pay-contest)
    - [Ex ante follower advantage in a sequential all-pay contest](#ex-ante-follower-advantage-in-a-sequential-all-pay-contest)
    - [Leader optimization in a sequential private-value all-pay contest](#leader-optimization-in-a-sequential-private-value-all-pay-contest)
      - [Best-response selection at a flat leader objective](#best-response-selection-at-a-flat-leader-objective)
      - [Median-density threshold for the leader in an all-pay contest](#median-density-threshold-for-the-leader-in-an-all-pay-contest)
  - [Proportional allocation contest](#proportional-allocation-contest)
    - [Proportional contest with outside effort](#proportional-contest-with-outside-effort)
      - [Active-set threshold for a proportional contest with outside effort](#active-set-threshold-for-a-proportional-contest-with-outside-effort)
      - [Total-effort formula for a proportional contest with outside effort](#total-effort-formula-for-a-proportional-contest-with-outside-effort)
    - [Quadratic-cost two-player proportional contest](#quadratic-cost-two-player-proportional-contest)
  - [Simultaneous all-pay contests](#simultaneous-all-pay-contests)
    - [Two-of-three all-pay participation equilibrium](#two-of-three-all-pay-participation-equilibrium)
      - [Marginal-equivalent equilibria in additive contests](#marginal-equivalent-equilibria-in-additive-contests)
    - [All-pay indifference equation with random entry](#all-pay-indifference-equation-with-random-entry)
  - [Rank-order contest](#rank-order-contest)
    - [All-pay effort identity](#all-pay-effort-identity)
      - [Expected effort in a rank-order contest](#expected-effort-in-a-rank-order-contest)
        - [Uniform-value multi-prize all-pay effort formula](#uniform-value-multi-prize-all-pay-effort-formula)
          - [Discrete prize-count optimization for a power-valued contest](#discrete-prize-count-optimization-for-a-power-valued-contest)
    - [Rank-order expected prize allocation](#rank-order-expected-prize-allocation)
  - [Prize allocation rule](#prize-allocation-rule)
    - [Winning probability](#winning-probability)
- [Bayesian game](#bayesian-game)
  - [Bayesian Nash equilibrium](#bayesian-nash-equilibrium)
- [Mechanism design](#mechanism-design)
  - [Expected seller revenue](#expected-seller-revenue)
  - [Posted price](#posted-price)
  - [Mechanism (mechanism design)](#mechanism-mechanism-design)
  - [Single-parameter mechanism](#single-parameter-mechanism)
    - [Virtual valuation](#virtual-valuation)
      - [Virtual surplus](#virtual-surplus)
      - [Virtual-surplus revenue identity](#virtual-surplus-revenue-identity)
        - [Revenue-optimal public-project auction](#revenue-optimal-public-project-auction)
      - [Regular distribution (economics)](#regular-distribution-economics)
  - [Direct revelation mechanism](#direct-revelation-mechanism)
    - [Revelation principle](#revelation-principle)
    - [Vickrey-Clarke-Groves mechanism](#vickrey-clarke-groves-mechanism)
  - [Incentive compatibility](#incentive-compatibility)
    - [Dominant-strategy incentive compatibility](#dominant-strategy-incentive-compatibility)
      - [Critical-value payment](#critical-value-payment)
    - [Bayesian incentive compatibility](#bayesian-incentive-compatibility)
  - [Individual rationality](#individual-rationality)
    - [Ex post individual rationality](#ex-post-individual-rationality)
    - [Interim individual rationality](#interim-individual-rationality)
  - [Auction](#auction)
    - [Vickrey auction](#vickrey-auction)
    - [Lowest-price auction](#lowest-price-auction)
      - [Uniform lowest-price auction equilibrium](#uniform-lowest-price-auction-equilibrium)
    - [Reserve price](#reserve-price)
    - [English auction](#english-auction)
    - [Least unique bid auction](#least-unique-bid-auction)
      - [Two-bid three-player least unique bid auction](#two-bid-three-player-least-unique-bid-auction)
    - [All-pay auction](#all-pay-auction)
      - [Two-player complete-information all-pay equilibrium](#two-player-complete-information-all-pay-equilibrium)
    - [First-price sealed-bid auction](#first-price-sealed-bid-auction)
      - [No dominant positive-value bid in a first-price auction](#no-dominant-positive-value-bid-in-a-first-price-auction)
      - [Uniform private-value first-price bidding equilibrium](#uniform-private-value-first-price-bidding-equilibrium)
    - [Interim payment identity](#interim-payment-identity)
      - [Revenue equivalence](#revenue-equivalence)
    - [Private-value auction](#private-value-auction)
      - [Unit-demand valuation](#unit-demand-valuation)
      - [Independent private values model](#independent-private-values-model)
        - [Symmetric independent private values model](#symmetric-independent-private-values-model)
        - [Revenue comparison for two uniform private values](#revenue-comparison-for-two-uniform-private-values)
  - [Strategyproofness](#strategyproofness)
    - [Rank-raising monotonicity lemma](#rank-raising-monotonicity-lemma)
    - [Gibbard-Satterthwaite theorem](#gibbard-satterthwaite-theorem)
      - [Binary social ordering from strategyproof choice](#binary-social-ordering-from-strategyproof-choice)
        - [Two-voter dictatorship from binary choice](#two-voter-dictatorship-from-binary-choice)
      - [Top-bottom decisiveness lemma](#top-bottom-decisiveness-lemma)
  - [Social choice theory](#social-choice-theory)
    - [Condorcet winner](#condorcet-winner)
      - [Weak Condorcet winner](#weak-condorcet-winner)
    - [Single-peaked preferences](#single-peaked-preferences)
      - [Median voter rule](#median-voter-rule)
    - [Social choice function](#social-choice-function)
      - [Two-alternative majority rule](#two-alternative-majority-rule)
      - [Dictatorship in social choice](#dictatorship-in-social-choice)
        - [Dictator in social choice](#dictator-in-social-choice)
- [Pure strategy](#pure-strategy)
  - [Strict dominance](#strict-dominance)
- [Finite game](#finite-game)
  - [Symmetric finite game](#symmetric-finite-game)
- [Mixed strategy](#mixed-strategy)
  - [Support of a mixed strategy](#support-of-a-mixed-strategy)
  - [Strategy support](#strategy-support)
- [Bimatrix game](#bimatrix-game)
  - [Matching pennies](#matching-pennies)
  - [Lottery over joint action profiles](#lottery-over-joint-action-profiles)
  - [Support enumeration for a bimatrix game](#support-enumeration-for-a-bimatrix-game)
  - [Symmetric bimatrix game](#symmetric-bimatrix-game)
  - [Nondegeneracy of a bimatrix game](#nondegeneracy-of-a-bimatrix-game)
  - [Nash equilibrium](#nash-equilibrium)
    - [Ranked university application game](#ranked-university-application-game)
    - [Symmetric Nash equilibrium](#symmetric-nash-equilibrium)
    - [Equilibrium oddness theorem](#equilibrium-oddness-theorem)
    - [Symmetric equilibrium](#symmetric-equilibrium)
      - [Symmetric equilibrium parity](#symmetric-equilibrium-parity)
      - [Symmetric Nash gain map](#symmetric-nash-gain-map)
        - [Gain-map proof of symmetric equilibrium](#gain-map-proof-of-symmetric-equilibrium)
    - [Complementarity construction of a symmetric Nash equilibrium](#complementarity-construction-of-a-symmetric-nash-equilibrium)
    - [Lemke-Howson algorithm](#lemke-howson-algorithm)
      - [Complementary pivoting](#complementary-pivoting)
    - [Nash's theorem](#nash-s-theorem)
      - [Brouwer gain-map proof of bimatrix equilibrium](#brouwer-gain-map-proof-of-bimatrix-equilibrium)
    - [Brouwer proof of Nash equilibrium for a two-by-two game](#brouwer-proof-of-nash-equilibrium-for-a-two-by-two-game)
- [Best response](#best-response)
  - [Dominant strategy](#dominant-strategy)
    - [Strictly dominant strategy](#strictly-dominant-strategy)
- [Zero-sum game](#zero-sum-game)
  - [Rock paper scissors](#rock-paper-scissors)
  - [Value of a zero-sum game](#value-of-a-zero-sum-game)
  - [Cost-weighted finite search game](#cost-weighted-finite-search-game)
  - [Matrix game](#matrix-game)
    - [Positive-payoff linear programming for a matrix game](#positive-payoff-linear-programming-for-a-matrix-game)
    - [Payoff matrix](#payoff-matrix)
    - [Matrix-game optimization problem](#matrix-game-optimization-problem)
    - [Mixed-strategy optimality certificate for a matrix game](#mixed-strategy-optimality-certificate-for-a-matrix-game)
    - [Symmetric inverse formula for a matrix-game equilibrium](#symmetric-inverse-formula-for-a-matrix-game-equilibrium)
      - [Three-card threshold-sum zero-sum game](#three-card-threshold-sum-zero-sum-game)
  - [Minimax theorem](#minimax-theorem)
  - [Optimal mixed strategy](#optimal-mixed-strategy)
  - [Antisymmetric zero-sum game](#antisymmetric-zero-sum-game)
    - [Support certificate for an antisymmetric matrix game](#support-certificate-for-an-antisymmetric-matrix-game)
    - [Consecutive-number antisymmetric game](#consecutive-number-antisymmetric-game)
- [Dominated strategy](#dominated-strategy)
  - [Dominated strategy elimination](#dominated-strategy-elimination)
  - [Weakly dominated strategy](#weakly-dominated-strategy)
    - [Equilibrium preservation under iterated weak dominance](#equilibrium-preservation-under-iterated-weak-dominance)
    - [Weak domination does not exclude equilibrium strategies](#weak-domination-does-not-exclude-equilibrium-strategies)

<h2 id="prisoner-s-dilemma">Prisoner's dilemma</h2>

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prisoner's_dilemma)

The [prisoner's dilemma](#prisoner-s-dilemma) has cooperation and defection actions, with mutual cooperation reward $R$, mutual defection [payoff](#payoff) $P$, unilateral temptation $T$ and exploited-cooperator [payoff](#payoff) $S$. Defection dominates in the one-shot game. The extra inequality $2R\ge T+S$ expresses cooperative efficiency against alternating asymmetric outcomes; it is a further assumption, not implied by the basic ordering.

<h3 id="iterated-prisoner-s-dilemma">Iterated prisoner's dilemma</h3>

↑ **Parent:** [Prisoner's dilemma](#prisoner-s-dilemma)

The [iterated prisoner's dilemma](#iterated-prisoner-s-dilemma) is a [repeated game](#repeated-game) whose stage [payoffs](#payoff) are the [prisoner's dilemma](#prisoner-s-dilemma). Historical dependence, initial memories and the [payoff](#payoff) time convention affect whether a cooperative rule resists or invades other strategies.

#### Reactive strategy (game theory)

↑ **Parent:** [Iterated prisoner's dilemma](#iterated-prisoner-s-dilemma)

A [reactive strategy](#reactive-strategy-game-theory) cooperates with [probability](probability-theory.md#probability) $p$ after the opponent cooperated and [probability](probability-theory.md#probability) $q$ after the opponent defected. It ignores its own previous action. [Independent](random-variable.md#independent-random-variables) behavioural randomization gives a four-state joint-action [Markov chain](markov-process.md#markov-chain). The reduced marginal recurrences depend on the prescribed initial action distribution.

##### Always defect

↑ **Parent:** [Reactive strategy (game theory)](#reactive-strategy-game-theory)

[Always defect](#always-defect) chooses defection independently of the opponent's actions.

##### Always cooperate

↑ **Parent:** [Reactive strategy (game theory)](#reactive-strategy-game-theory)

[Always cooperate](#always-cooperate) chooses cooperation independently of the opponent's actions.

##### Tit for tat

↑ **Parent:** [Reactive strategy (game theory)](#reactive-strategy-game-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tit_for_tat)

[Tit for tat](#tit-for-tat) cooperates initially and then repeats the opponent's previous action. Two such players cooperate forever without mistakes under this initial convention. It retaliates against defection and returns to cooperation after the opponent cooperates.

###### Tit for tat invasion of a reactive resident

↑ **Parent:** [Tit for tat](#tit-for-tat)

For a reactive resident $(p,q)$ with $|p-q|<1$, let $z=q/(1-p+q)$ and $g(z)=Rz^2+(S+T)z(1-z)+P(1-z)^2$. Its self-payoff and both ordered cross-payoffs against [Tit for tat](#tit-for-tat) equal $g(z)$. At introduced [Tit for tat](#tit-for-tat) frequency $\epsilon$, its fitness difference is therefore the displayed expression. If $2R\ge S+T$, it is positive for $z<1$ because $R-g(z)=(1-z)[R-P+(R+P-S-T)z]$. Fully cooperative reached histories tie; the deterministic opposite-response strategy needs a separate cycle calculation. Initial advantage is order frequency rather than a positive invasion exponent at zero.

###### Finite-horizon invasion threshold of Tit for tat against unconditional defection

↑ **Parent:** [Tit for tat invasion of a reactive resident](#tit-for-tat-invasion-of-a-reactive-resident)

In an $L$-round [iterated prisoner's dilemma](#iterated-prisoner-s-dilemma), [Tit for tat](#tit-for-tat) against [always defect](#always-defect) gets $S$ once and $P$ thereafter; the defector gets $T$ once and $P$ thereafter. Their self-payoffs are $R,P$. At introduced frequency $\epsilon$, subtracting mixed-population [payoffs](#payoff) gives $\epsilon[(R-P)-(T+S-2P)/L]-(P-S)/L$. The displayed positive threshold applies when its denominator is positive and the threshold is less than one. Taking $L\to\infty$ first removes this finite entry cost, so the horizon and rare-mutant [limits](calculus.md#limit-of-a-function) cannot be casually interchanged.

###### Neutrality between Tit for tat and unconditional cooperation

↑ **Parent:** [Tit for tat](#tit-for-tat)

Under cooperative initial memories, matches involving only [Tit for tat](#tit-for-tat) and [always cooperate](#always-cooperate) contain only cooperation, so all four [payoffs](#payoff) equal $R$. The [two-condition criterion for evolutionary stability](#two-condition-criterion-for-evolutionary-stability) has both differences zero. Thus [Tit for tat](#tit-for-tat) is not an [evolutionarily stable strategy](#evolutionarily-stable-strategy) against a strategy space containing unconditional cooperation, even if it is a [Nash equilibrium](#nash-equilibrium). This counterexample is valid for finite horizons and discounting as well as infinite averages.

##### Long-run payoff of reactive strategies

↑ **Parent:** [Reactive strategy (game theory)](#reactive-strategy-game-theory)

With initially [independent](random-variable.md#independent-random-variables) actions, same-round [independence](random-variable.md#independent-random-variables) is preserved by reactive updates: each next action uses the other [independent](random-variable.md#independent-random-variables) previous action and fresh [independent](random-variable.md#independent-random-variables) randomization. Marginal cooperation follows $x'=q_1+(p_1-q_1)y$, $y'=q_2+(p_2-q_2)x$. If the product of response slopes has [modulus](complex-analysis.md#modulus) below one, these recurrences converge and the joint distribution is their product. Averaging $R,S,T,P$ over that distribution gives the long-time [payoffs](#payoff). At deterministic response slopes of [modulus](complex-analysis.md#modulus) one, initial-memory-specific cycles must instead be averaged directly.

## Evolutionary game theory

↑ **Parent:** [Game theory](game-theory.md)

[Evolutionary game theory](#evolutionary-game-theory) models changes in strategy frequencies when reproductive success or imitation depends on a game's [payoff](#payoff). An [evolutionarily stable strategy](#evolutionarily-stable-strategy) is an invasion criterion; a [replicator equation](#replicator-equation) is a particular deterministic frequency dynamic.

### Replicator equation

↑ **Parent:** [Evolutionary game theory](#evolutionary-game-theory)

In a symmetric [matrix](vector-space.md#matrix) game, a strategy frequency grows in proportion to its excess [payoff](#payoff) above the current [mean](probability-theory.md#expected-value). Summing the displayed equations gives zero, preserving the [probability simplex](algebraic-topology.md#probability-simplex). For two strategies and [payoff](#payoff) difference $\Delta w(x)$, it reduces to $\dot x=x(1-x)\Delta w(x)$.

## Repeated game

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Repeated_game)

A [repeated game](#repeated-game) plays a stage game over several rounds, allowing actions to depend on earlier observations. Its [payoff](#payoff) convention must specify a finite horizon, a discount factor or a long-time average; these need not have identical invasion properties.

## Payoff

↑ **Parent:** [Game theory](game-theory.md)

A payoff is the numerical outcome assigned to a player for a profile of [pure strategies](#pure-strategy). In a finite [zero-sum game](#zero-sum-game), one player's payoff is the negative of the other's. For [mixed strategies](#mixed-strategy), the expected payoff is the probability-weighted average of the entries of the [payoff matrix](#payoff-matrix).

## Costly turnout game

↑ **Parent:** [Game theory](game-theory.md)

Each voter chooses whether to incur a voting cost. The collective result changes each voter's payoff, and abstention can be optimal when other voters are likely to determine the outcome. The payoff difference between voting and abstaining is the benefit of being pivotal, weighted by the pivotal probability, minus the turnout cost.

// Target: mathematical-optimization.bigb

### Turnout equilibria with two supporters and one opponent

↑ **Parent:** [Costly turnout game](#costly-turnout-game)

Suppose turnout costs $3c>0$, each supporter gains $4c$ on passage, and the opponent loses $8c$. The symmetric-supporter [Nash equilibria](#nash-equilibrium) $(\alpha,\beta,\gamma)$ are $(0,1/4,1/4)$ and $(1,3/4,3/4)$. Allowing different supporter probabilities adds $(1/4,0,3/8)$ and $(1/4,3/8,0)$. These follow by comparing the [pivotal voting probabilities](#pivotal-voting-probability) with the turnout cost; no player benefits by changing their mixed strategy.

// Target: mathematical-optimization.bigb

### Pivotal voting probability

↑ **Parent:** [Costly turnout game](#costly-turnout-game)

A voter is pivotal when changing only that voter's participation changes the election result. For an opponent facing two independent supporters with participation probabilities $\beta,\gamma$, under a rule requiring strictly more votes in favour, the opponent is pivotal when exactly one supporter votes. This probability is $\beta(1-\gamma)+(1-\beta)\gamma$.

// Target: mathematical-optimization.bigb

## Nonatomic congestion game

↑ **Parent:** [Game theory](game-theory.md)

In a nonatomic congestion game, a divisible population chooses resources whose costs depend on aggregate usage. Each individual has negligible size, so changing their choice does not alter those costs. For traffic on a [flow network](graph-theory.md#flow-network), strategies are routes and an equilibrium is a [Wardrop equilibrium](queueing-theory.md#wardrop-equilibrium): every route with positive flow has minimum delay for its source-sink pair. This differs from a finite-player [congestion game](#congestion-game), where a deviation changes the load used to evaluate the deviator's new cost. Continuous nondecreasing link delays give a [Beckmann potential](queueing-theory.md#beckmann-potential) whose minimizers are exactly the traffic equilibria.

## Congestion game

↑ **Parent:** [Game theory](game-theory.md)

Players select sets of resources, and each resource's cost depends on its total number of users. Each player's cost is the sum of the costs of their selected resources. A unilateral deviation changes resource loads, so a finite-player [Nash equilibrium](#nash-equilibrium) compares costs after that change, not at the old loads. For cost functions $c_e$, the potential $\sum_e\sum_{j=1}^{n_e}c_e(j)$ changes by exactly the deviator's cost change. A minimizer of this potential in a [finite game](#finite-game) is therefore a pure [Nash equilibrium](#nash-equilibrium).

## Evolutionarily stable strategy

↑ **Parent:** [Game theory](game-theory.md)

A resident strategy is evolutionarily stable if every distinct mutant earns lower expected fitness when introduced at sufficiently small positive frequency. The upper bound on the frequency may depend on the mutant. In a finite symmetric matrix game, $e(x,y)=x^TAy$ is the expected payoff, with the second argument representing the population strategy. Affineness in this argument yields the [two-condition criterion for evolutionary stability](#two-condition-criterion-for-evolutionary-stability). Every evolutionarily stable strategy is a symmetric [Nash equilibrium](#nash-equilibrium), but a tied best response must also be strictly outperformed against its own mutant population. The [Hawk-Dove game](#hawk-dove-game) supplies an interior stable mixture despite equality of all payoffs against the resident mixture.

### Selection gradient

↑ **Parent:** [Evolutionarily stable strategy](#evolutionarily-stable-strategy)

For a differentiable rare-mutant invasion fitness $f(y,x)$ against resident trait $x$, the [selection gradient](#selection-gradient) gives the first-order growth advantage of a nearby mutant. A zero gradient is a candidate interior evolutionary singularity. Strict local uninvadability follows from negative mutant-fitness curvature; evolutionary approach additionally requires the gradient to point toward the candidate. Boundary traits require one-sided tests. A gradient alone does not prove global evolutionary stability.

### Hawk-Dove game

↑ **Parent:** [Evolutionarily stable strategy](#evolutionarily-stable-strategy)

Hawk fights for a resource of value $V$, while Dove retreats from Hawk and shares with another Dove. Hawk–Hawk competition incurs damage cost $D$. The expected payoff difference between Hawk probabilities $p,r$ against population probability $q$ is $(p-r)(V-Dq)/2$. For positive $V,D$, pure Hawk is an [evolutionarily stable strategy](#evolutionarily-stable-strategy) when $V>D$. At $V=D$, it remains stable because a mutant $p<1$ loses $V(1-p)^2/2$ against its own population. When $0<V<D$, the stable mixture has Hawk probability $p^*=V/D$: all first-condition payoffs tie, and its second-condition advantage is $D(p-p^*)^2/2>0$. For nonpositive resource values, pure Dove is stable if $V<0$ or if $V=0<D$. At $V=D=0$ all payoffs vanish and there is no evolutionarily stable strategy.

### Two-condition criterion for evolutionary stability

↑ **Parent:** [Evolutionarily stable strategy](#evolutionarily-stable-strategy)

For mixed-strategy expected payoffs put $A_y=e(x^*,x^*)-e(y,x^*)$ and $B_y=e(x^*,y)-e(y,y)$. The invasion payoff difference is exactly $(1-\epsilon)A_y+\epsilon B_y$. Positivity for all sufficiently small positive $\epsilon$ forces $A_y\geq0$ by taking the limit. When $A_y=0$, it forces $B_y>0$. Conversely $A_y>0$ makes the difference positive for sufficiently small frequency, and $A_y=0,B_y>0$ makes it positive for every positive frequency. Apply this separately to every distinct mutant. This proves the equivalence with an [evolutionarily stable strategy](#evolutionarily-stable-strategy); affineness in population composition is essential to the formula.

## Security level payoff

↑ **Parent:** [Game theory](game-theory.md)

A player maximizes the worst payoff it can receive against the other player's actions. Allowing the opponent to mix does not lower the worst payoff beyond a pure action, since the payoff is linear in that mixture. A [security level payoff](#security-level-payoff) is an individual guarantee, not generally a [Nash equilibrium](#nash-equilibrium) payoff.

## Nash bargaining problem

↑ **Parent:** [Game theory](game-theory.md)

The essential two-person bargaining domain consists of a [compact convex set](mathematical-optimization.md#compact-convex-set) of feasible utility vectors $F$, a [disagreement point](#disagreement-point) $d\in F$, and at least one feasible vector strictly exceeding $d$ coordinatewise. The [Nash bargaining solution](#nash-bargaining-solution) selects a jointly feasible improvement using a rule characterized by [Pareto efficiency](mathematical-optimization.md#pareto-efficiency), [bargaining symmetry](#bargaining-symmetry), [positive affine invariance in bargaining](#positive-affine-invariance-in-bargaining) and [bargaining independence of irrelevant alternatives](#bargaining-independence-of-irrelevant-alternatives).

### Negotiation set in two-person bargaining

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

For a [compact convex set](mathematical-optimization.md#compact-convex-set) of feasible [payoff](#payoff) [vectors](vector-space.md#vector) $F$ and a specified [disagreement point](#disagreement-point) $d$, the [negotiation set](#negotiation-set-in-two-person-bargaining) is its individually rational [Pareto frontier](mathematical-optimization.md#pareto-frontier). It is the set of efficient agreements each player prefers at least weakly to disagreement. In a [maximin bargaining solution](#maximin-bargaining-solution), $d$ is the [vector](vector-space.md#vector) of the two [security level payoffs](#security-level-payoff). This usage is distinct from objection-and-counterobjection bargaining sets in coalitional-game theory.

### Joint dominance of payoff vectors

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

A feasible [payoff](#payoff) [vector](vector-space.md#vector) $u'$ jointly dominates $u$ if every coordinate is at least as large and at least one is strictly larger. A [Pareto optimal](mathematical-optimization.md#pareto-efficiency) [vector](vector-space.md#vector) has no feasible joint dominator. Strict increase of every coordinate is not required. This compares each player's own utilities, not the numerical size of utilities across different players.

### Bargaining individual rationality

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

A payoff is individually rational for a [Nash bargaining problem](#nash-bargaining-problem) when neither player receives less than its [disagreement point](#disagreement-point) payoff. Essentiality permits strict improvement for both. Maximizing a positive [Nash product](#nash-product) therefore selects a strictly individually rational payoff.

### Bargaining independence of irrelevant alternatives

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

If an admissible smaller feasible set with the same [disagreement point](#disagreement-point) contains the original chosen vector, deleting the other outcomes must leave the choice unchanged. The [Nash bargaining solution](#nash-bargaining-solution) satisfies this axiom because its unique product maximizer remains feasible.

### Positive affine invariance in bargaining

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

Transforming each utility by an independent positive affine map must transform the chosen payoff by the same map. The [Nash product](#nash-product) changes only by a positive factor, so the [Nash bargaining solution](#nash-bargaining-solution) has this invariance.

### Bargaining symmetry

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

When the feasible payoff set and [disagreement point](#disagreement-point) are invariant under interchange of players, the solution must give both players the same payoff.

### Nash bargaining solution

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

For an essential [Nash bargaining problem](#nash-bargaining-problem), maximizing the [Nash product](#nash-product) gives a unique vector: on positive gains its logarithm is a [strictly concave function](real-analysis.md#strictly-concave-function). The rule satisfies the four bargaining axioms, and the [supporting triangle for Nash bargaining](#supporting-triangle-for-nash-bargaining) proves their converse characterization. The nonessential case requires additional conventions, since a zero product may have many maximizers.

#### Maximin bargaining solution

↑ **Parent:** [Nash bargaining solution](#nash-bargaining-solution)

For a finite two-person game, let $d_i$ be player $i$'s [security level payoff](#security-level-payoff), obtained by maximizing its minimum expected [payoff](#payoff) against the other player's actions. Apply the [Nash bargaining solution](#nash-bargaining-solution) to the convexified feasible [payoff](#payoff) region with this [disagreement point](#disagreement-point). This is the [maximin bargaining solution](#maximin-bargaining-solution). “Maximin” specifies the disagreement guarantees; the arbitration [objective function](mathematical-optimization.md#objective-function) remains the [Nash product](#nash-product), not the minimum of two numerically incomparable utilities.

#### Supporting triangle for Nash bargaining

↑ **Parent:** [Nash bargaining solution](#nash-bargaining-solution)

Normalize a positive [Nash product](#nash-product) maximizer and the [disagreement point](#disagreement-point) to $(1,1)$ and zero. The first-order product inequality along every feasible segment places the transformed set in $z_1+z_2\leq2$. Compactness allows a symmetric containing triangle with finite lower coordinate bounds. [Bargaining symmetry](#bargaining-symmetry) and [Pareto efficiency](mathematical-optimization.md#pareto-efficiency) choose $(1,1)$ in that triangle; [bargaining independence of irrelevant alternatives](#bargaining-independence-of-irrelevant-alternatives) transfers this choice to the original normalized set. [Positive affine invariance in bargaining](#positive-affine-invariance-in-bargaining) then proves the full characterization.

#### Nash product

↑ **Parent:** [Nash bargaining solution](#nash-bargaining-solution)

The product of the two players' gains over the [disagreement point](#disagreement-point) is maximized over the individually rational feasible set in the [Nash bargaining solution](#nash-bargaining-solution). Positive affine changes of utility multiply this product by a positive constant and leave the selected payoff correspondence unchanged after transforming coordinates.

### Disagreement point

↑ **Parent:** [Nash bargaining problem](#nash-bargaining-problem)

The disagreement point specifies each player's payoff if bargaining fails. It supplies the baseline from which the [Nash product](#nash-product) measures gains. In a game-based example it may be set to the vector of [security level payoffs](#security-level-payoff); this choice must be recomputed when the underlying payoff matrices change.

## Cooperative game theory

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cooperative_game_theory)

Cooperative game theory studies what groups of players can achieve together and how their joint value can be allocated. A [transferable utility game](#transferable-utility-game) assigns a real value to each [coalition](#coalition-game-theory). The [core of a cooperative game](#core-game-theory) asks which allocations no [coalition](#coalition-game-theory) can improve upon; the [Shapley value](#shapley-value) averages [marginal contributions](#marginal-contribution) across player orderings.

### Transferable utility game

↑ **Parent:** [Cooperative game theory](#cooperative-game-theory)

A finite transferable utility game gives each [coalition](#coalition-game-theory) $S\subseteq N$ a real value $v(S)$ that its members can distribute among themselves. The usual normalization is $v(\varnothing)=0$. An efficient payoff vector $x$ satisfies $\sum_{i\in N}x_i=v(N)$. [Simple cooperative games](#simple-cooperative-game) model winning [coalitions](#coalition-game-theory) with values zero and one; [convex cooperative games](#convex-cooperative-game) model increasing [marginal contributions](#marginal-contribution).

#### Coverage coalitional game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

Players hold finite sets of resources, and their coalition value is the number of distinct resources they collectively cover. The value is generally subadditive rather than superadditive: overlapping resources are counted only once. It is a [superadditive coalitional game](#superadditive-coalitional-game) exactly when the players' resource sets are pairwise disjoint.

##### Shapley value of a coverage game

↑ **Parent:** [Coverage coalitional game](#coverage-coalitional-game)

Decompose a [coverage coalitional game](#coverage-coalitional-game) into one-resource games and use additivity of the [Shapley value](#shapley-value). A player contributes a resource precisely when it is the earliest player in a random ordering among those holding that resource. Each holder has probability the reciprocal of the number of holders of being earliest. Summing these contributions proves the formula, regardless of overlaps or emptiness of the core.

##### Core of a coverage game

↑ **Parent:** [Coverage coalitional game](#coverage-coalitional-game)

A [coverage coalitional game](#coverage-coalitional-game) has a nonempty [core of a cooperative game](#core-game-theory) exactly when all resource sets are pairwise disjoint. Singleton coalition constraints require $x_i\geq|B_i|$, while efficiency requires $\sum_i x_i=|\bigcup_iB_i|$. Any overlap makes these inequalities inconsistent. When there is no overlap, the allocation $x_i=|B_i|$ is the unique core allocation and gives every coalition its value exactly.

#### Bankruptcy game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

With nonnegative claims $c_i$ and an estate $0\leq a\leq\sum_i c_i$, a coalition's guaranteed worth is the estate left after all outside claims are met, or zero if those claims exhaust it. Writing the total deficit $d=\sum_i c_i-a$ gives $v(S)=(\sum_{i\in S}c_i-d)_+$. For disjoint coalitions, $(p+q-d)_+\geq(p-d)_++(q-d)_+$, so this is a [superadditive coalitional game](#superadditive-coalitional-game). Its [core of a cooperative game](#core-game-theory) consists exactly of efficient allocations with $0\leq x_i\leq c_i$: the upper bounds are equivalent to the complementary-coalition constraints, and the lower bounds together with efficiency imply every other coalition constraint.

#### Superadditive coalitional game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

The [characteristic function of a coalitional game](#characteristic-function-of-a-coalitional-game) is superadditive when disjoint coalitions can attain at least the sum of their separate values by joining. This follows when their separate strategies can be played together without interference. Superadditivity is an additional property of an abstract [transferable utility game](#transferable-utility-game), not a consequence of merely assigning values to subsets: $v(\{1\})=v(\{2\})=v(\{1,2\})=1$ is a normalized counterexample.

#### Glove game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

Players each own one object of one of two complementary types. A matched pair sells for $\omega>0$, and objects of one type alone have no value. The [characteristic function of a coalitional game](#characteristic-function-of-a-coalitional-game) is therefore the displayed matching count times pair price. The [core of a glove game](#core-of-a-glove-game) pays the scarce type the entire pair value and the abundant type zero; if type counts are equal, a common split between the two types can vary continuously.

##### Core of a glove game

↑ **Parent:** [Glove game](#glove-game)

If there are fewer left owners than right owners, deleting any right owner leaves the grand-coalition value unchanged. The complement's core constraint and efficiency force that owner's payoff to be zero. Mixed-pair inequalities then require every left owner to receive at least $\omega$, and efficiency makes all these payoffs exactly $\omega$. Reverse the types when right owners are scarce. If both counts equal $k$, sum all $k^2$ mixed-pair inequalities. Their total is exactly $k$ times the grand-coalition payoff, so each pair sum is $\omega$. Hence all left owners receive a common $\theta\in[0,\omega]$ and all right owners $\omega-\theta$. Such allocations meet every coalition constraint because $\theta u+(\omega-\theta)v\geq\omega\min(u,v)$. This proves the complete [core](#core-game-theory) description.

#### Characteristic function of a coalitional game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

The characteristic function assigns every [coalition](#coalition-game-theory) its total attainable transferable payoff, with $v(\varnothing)=0$. It determines the efficiency condition of an [imputation](#imputation-in-a-coalitional-game) and all constraints of the [core of a cooperative game](#core-game-theory). For the [glove game](#glove-game), $v(S)=\omega\min(|S\cap L|,|S\cap R|)$; for miners requiring $r$ people to carry one lump, $v(S)=\lfloor|S|/r\rfloor$. This game-theoretic function is distinct from the [characteristic function](probability-theory.md#characteristic-function) of a probability distribution.

#### Dual coalitional game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

Duality assigns a [coalition](#coalition-game-theory) the grand-coalition value less the value of its complement. For a normalized [transferable utility game](#transferable-utility-game), the dual is normalized and taking the dual twice recovers the original game. A player's dual [marginal contribution](#marginal-contribution) at predecessor set $S$ equals its original contribution at the complementary predecessor set in $N\setminus\{i\}$. This preserves the [Shapley value](#shapley-value).

#### Nucleolus

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

When the [imputation](#imputation-in-a-coalitional-game) set is nonempty, the [nucleolus](#nucleolus) is the unique [imputation](#imputation-in-a-coalitional-game) lexicographically minimizing the vector of [excesses of a coalition](#excess-of-a-coalition) sorted decreasingly. It minimizes the largest complaint first, then subsequent complaints among ties. It can be computed through successive [linear programs](mathematical-optimization.md#linear-programming) that minimize the current maximum excess and retain constraints fixed by prior stages. Its uniqueness is the standard [nucleolus](#nucleolus) theorem. If the [core of a cooperative game](#core-game-theory) is nonempty, the [nucleolus](#nucleolus) belongs to it; an empty core does not preclude a [nucleolus](#nucleolus).

##### Prenucleolus

↑ **Parent:** [Nucleolus](#nucleolus)

The [prenucleolus](#prenucleolus) uses the same sorted [excesses of a coalition](#excess-of-a-coalition) but minimizes over all efficient payoff vectors, without imposing individual rationality. It can differ from the [nucleolus](#nucleolus) when [coalition](#coalition-game-theory) values are not superadditive. Any computation must state which domain is used rather than silently relaxing [imputation](#imputation-in-a-coalitional-game) inequalities.

#### Imputation in a coalitional game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

An [imputation](#imputation-in-a-coalitional-game) is an efficient, individually rational allocation in a [transferable utility game](#transferable-utility-game). Its total is the grand-coalition value and each player receives at least its singleton value. The set is nonempty exactly when $v(N)\geq\sum_i v(\{i\})$, and is then compact. This individual-rationality condition distinguishes the [nucleolus](#nucleolus) from the [prenucleolus](#prenucleolus).

#### Marginal contribution

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

A player's [marginal contribution](#marginal-contribution) to a [coalition](#coalition-game-theory) is the increase in its value when that player joins. In a [convex cooperative game](#convex-cooperative-game), [marginal contributions](#marginal-contribution) increase with the preceding [coalition](#coalition-game-theory). Averaging contributions across player orderings gives the [Shapley value](#shapley-value).

#### Coalition (game theory)

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

A [coalition](#coalition-game-theory) is a subset of the players in a [transferable utility game](#transferable-utility-game), considered as a group that can act together. The game assigns it value $v(S)$. The [core of a cooperative game](#core-game-theory) constrains the total payoff assigned to every [coalition](#coalition-game-theory), while a [marginal contribution](#marginal-contribution) measures the value gained by adding one player.

##### Excess of a coalition

↑ **Parent:** [Coalition (game theory)](#coalition-game-theory)

The excess measures a [coalition](#coalition-game-theory)'s complaint against an allocation: a positive excess means its own attainable value exceeds its assigned total. The [core of a cooperative game](#core-game-theory) requires every excess to be nonpositive at an efficient allocation. The [nucleolus](#nucleolus) lexicographically minimizes the decreasingly sorted excess vector over [imputations](#imputation-in-a-coalitional-game).

#### Convex cooperative game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

A transferable utility game is convex when its coalition-value function is [supermodular](function.md#supermodular-set-function). Equivalently a player's [marginal contribution](#marginal-contribution) cannot decrease when the preceding [coalition](#coalition-game-theory) grows. The implication follows by applying the displayed inequality to $A\cup\{i\}$ and $B$ with $A\subseteq B$, $i\notin B$; the reverse implication follows by adding successive marginal inequalities. This property concerns [coalition](#coalition-game-theory) values, not geometrical convexity of a strategy space.

##### Shapley population monotonicity in a convex game

↑ **Parent:** [Convex cooperative game](#convex-cooperative-game)

Choose a uniform random ordering of $N$ and restrict it to $T$. The restriction is uniform, and each player's predecessor set in $T$ is contained in their predecessor set in $N$. Increasing [marginal contributions](#marginal-contribution) in a [convex cooperative game](#convex-cooperative-game) make the full-population contribution at least the restricted contribution. Averaging proves the displayed [Shapley value](#shapley-value) inequality. Summing over $i\in T$ and using efficiency in the restricted game proves every [core](#core-game-theory) inequality.

##### Shapley value belongs to the core of a convex game

↑ **Parent:** [Convex cooperative game](#convex-cooperative-game)

Increasing [marginal contributions](#marginal-contribution) imply $m_i^\pi\ge v((S\cap P_i)\cup\{i\})-v(S\cap P_i)$ for $i\in S$. Summing telescopes to $\sum_{i\in S}m_i^\pi\ge v(S)$, while efficiency follows by telescoping over the full ordering. Hence every [marginal contribution vector](#marginal-contribution-vector) is in the [core of a cooperative game](#core-game-theory). The [core](#core-game-theory) is a [convex set](mathematical-optimization.md#convex-set), so their average, the [Shapley value](#shapley-value), is in it too. This gives an elementary proof of nonemptiness and stability for a [convex cooperative game](#convex-cooperative-game).

#### Core (game theory)

↑ **Parent:** [Transferable utility game](#transferable-utility-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Core_(game_theory))

The [core](#core-game-theory) consists of efficient payoff vectors for which each [coalition](#coalition-game-theory) receives at least its own attainable value. Thus no [coalition](#coalition-game-theory) can improve every member's payoff by leaving. It is a [convex set](mathematical-optimization.md#convex-set) defined by linear constraints, but can be empty. Every [convex cooperative game](#convex-cooperative-game) has a nonempty [core](#core-game-theory) because each [marginal contribution vector](#marginal-contribution-vector) belongs to it.

##### Core of the miners game

↑ **Parent:** [Core (game theory)](#core-game-theory)

For $r\geq2$, the [core](#core-game-theory) is zero when $n<r$, the nonnegative unit simplex when $n=r$, the single allocation $x_i=1/r$ when $n\geq2r$ is divisible by $r$, and empty for all other $n\geq r$. To prove the obstruction, every $r$-person [coalition](#coalition-game-theory) requires payoff at least one. Summing these constraints counts each player $\binom{n-1}{r-1}$ times and gives $r\lfloor n/r\rfloor/n\geq1$, impossible when $r\nmid n$. For a divisible $n$, all such coalition sums must equal one. Comparing coalitions with the same $r-1$ members makes all individual payoffs equal when $n>r$. The uniform allocation satisfies every coalition constraint because $|S|/r\geq\lfloor|S|/r\rfloor$. At $n=r$ all proper coalition values are zero, giving the whole simplex instead.

#### Shapley value

↑ **Parent:** [Transferable utility game](#transferable-utility-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shapley_value)

The [Shapley value](#shapley-value) averages each player's [marginal contribution](#marginal-contribution) over uniformly random player orderings. Exactly $|S|!(n-|S|-1)!$ orderings have $S$ immediately before player $i$, giving the formula. The values sum to $v(N)$ by telescoping each ordering. In a [simple cooperative game](#simple-cooperative-game) this is the [probability](probability-theory.md#probability) of being pivotal. For a [convex cooperative game](#convex-cooperative-game), [Shapley value belongs to the core of a convex game](#shapley-value-belongs-to-the-core-of-a-convex-game) guarantees a stable allocation as well.

##### Shapley limit in a buyer-heavy exchange market

↑ **Parent:** [Shapley value](#shapley-value)

For $k$ unit sellers and $3k$ unit buyers with unit surplus per trade, a coalition's value is the smaller of its seller and buyer counts. Give each player an independent uniform arrival time. Conditional on a specified seller arriving at time $t$, the previous buyers and other sellers have independent binomial counts $B\sim\operatorname{Bin}(3k,t)$ and $S\sim\operatorname{Bin}(k-1,t)$. The seller contributes one exactly when $B>S$. For fixed positive $t$ this probability tends to one; a Chebyshev bound and a split near $t=0$ also give an explicit uniform integral estimate. Averaging gives seller [Shapley value](#shapley-value) tending to one. Efficiency and role symmetry give $s_k+3b_k=1$, hence the buyer value tends to zero.

##### Balanced contributions of Shapley values

↑ **Parent:** [Shapley value](#shapley-value)

For a [coalitional game](#transferable-utility-game), restriction to the remaining players preserves coalition values. Remove player $j$ from a uniformly random ordering when comparing player $i$'s [Shapley value](#shapley-value). The marginal contribution changes only when $j$ precedes $i$. If $S$ is the set of other predecessors, the change is $v(S\cup\{i,j\})-v(S\cup\{i\})-v(S\cup\{j\})+v(S)$, with coefficient $(|S|+1)!(n-|S|-2)!/n!$. The same expression and coefficient arise after interchanging $i,j$, proving balanced contributions.

##### Shapley wages in an entrepreneur-worker game

↑ **Parent:** [Shapley value](#shapley-value)

An entrepreneur is indispensable and a [coalition](#coalition-game-theory) containing the entrepreneur and $k$ of $n$ workers earns $p(k)$; a [coalition](#coalition-game-theory) without the entrepreneur earns zero. A worker's [marginal contribution](#marginal-contribution) is nonzero only when the entrepreneur precedes them. The [probability](probability-theory.md#probability) that the entrepreneur and exactly $k$ other workers precede that worker is $(k+1)/(n(n+1))$, giving the displayed common [Shapley value](#shapley-value) wage. The entrepreneur receives $p(n)-nw$. Convex nondecreasing $p$ makes all [marginal contributions](#marginal-contribution) increase with predecessor sets, so the whole [Shapley value](#shapley-value) allocation belongs to the [core](#core-game-theory).

##### Shapley self-duality

↑ **Parent:** [Shapley value](#shapley-value)

Complementing predecessor sets within $N\setminus\{i\}$ preserves their [Shapley value](#shapley-value) weights, since the factorials $|S|!$ and $(n-|S|-1)!$ interchange. For the [dual coalitional game](#dual-coalitional-game), the corresponding [marginal contribution](#marginal-contribution) equals the original contribution at that complementary set. Hence the values coincide. The same bijection gives $\phi_i(v)=\sum_S w(S)(v(N\setminus S)-v(S))$.

##### Marginal contribution vector

↑ **Parent:** [Shapley value](#shapley-value)

For a player ordering $\pi$, $P_i$ is the set before player $i$, and the displayed entries form its [marginal contribution](#marginal-contribution) vector. Their sum is $v(N)-v(\varnothing)$. The [Shapley value](#shapley-value) is the average of these vectors. In a [convex cooperative game](#convex-cooperative-game), increasing [marginal contributions](#marginal-contribution) make each such vector satisfy every [coalition](#coalition-game-theory) constraint of the [core of a cooperative game](#core-game-theory).

#### Weighted voting game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

A weighted voting game assigns player weights and a threshold, and declares [coalitions](#coalition-game-theory) winning when their total weight passes that threshold. The strict $>t$ convention is equivalent to quota $t+1$ for integer weights; another common convention writes a weak inequality directly. Nontrivial examples are [simple cooperative games](#simple-cooperative-game). Having nonnegative weights does not guarantee a [convex cooperative game](#convex-cooperative-game): two-of-three majority supplies a counterexample.

#### Simple cooperative game

↑ **Parent:** [Transferable utility game](#transferable-utility-game)

A simple cooperative game is a monotone [transferable utility game](#transferable-utility-game) in which each [coalition](#coalition-game-theory) either loses, with value zero, or wins, with value one. In the usual nontrivial convention the empty [coalition](#coalition-game-theory) loses and the grand [coalition](#coalition-game-theory) wins. The [Shapley value](#shapley-value) is then the [probability](probability-theory.md#probability) that a player changes a losing [coalition](#coalition-game-theory) into a winning one when players enter in uniformly random order.

## Payoff-equivalent strategies

↑ **Parent:** [Game theory](game-theory.md)

Two strategies are payoff-equivalent for a player when they give that player the same payoff against every strategy of the opponents. If every player's payoff is also unchanged, replacing one by the other preserves the game outcomes entirely. This is distinct from [weakly dominated strategies](#weakly-dominated-strategy), whose definition requires a strict comparison somewhere.

## Normal-form game

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal-form_game)

A normal-form game specifies each player's strategy set and their payoff for every strategy profile. In a finite two-player game these data form a [bimatrix game](#bimatrix-game); if the two payoffs always sum to zero, one [payoff matrix](#payoff-matrix) describes the [matrix game](#matrix-game). The representation specifies choices and incentives, without a temporal order of observed moves.

## Subgame perfect equilibrium

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subgame_perfect_equilibrium)

A strategy profile that is a [Nash equilibrium](#nash-equilibrium) in every subgame, including those outside the realized play path. In finite sequential games, [backward induction](foundations-of-mathematics.md#backward-induction) constructs such profiles by solving continuation games before earlier decisions. When a stage is an [all-pay contest](#all-pay-auction), its solution can involve [mixed strategies](#mixed-strategy).

## Stackelberg competition

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stackelberg_competition)

A sequential model in [game theory](game-theory.md) in which a leader commits to an action before a follower observes it and chooses a [best response](#best-response). The leader anticipates the follower's response when optimizing. With private follower information, the leader maximizes its expected payoff over follower types. The resulting solution is a [Stackelberg equilibrium](#stackelberg-equilibrium).

### Stackelberg equilibrium

↑ **Parent:** [Stackelberg competition](#stackelberg-competition)

A solution of [Stackelberg competition](#stackelberg-competition) in which the follower chooses a [best response](#best-response) after each observed leader action and the leader optimizes given those responses. Indifference may require a specified response or leader-selection convention; it cannot be silently treated as a strict inequality. In a [sequential private-value all-pay contest](#sequential-private-value-all-pay-contest), the leader's objective is $vF(b)-b$.

## Contest theory

↑ **Parent:** [Game theory](game-theory.md)

Contest theory studies how [prize allocation rules](#prize-allocation-rule) and effort costs influence strategic effort investment, participation, and the resulting [Nash equilibria](#nash-equilibrium) or [Bayesian Nash equilibria](#bayesian-nash-equilibrium). Unlike a sale in which only the winner pays, an [all-pay auction](#all-pay-auction) charges every participant for its effort.

### Sequential elimination all-pay contest

↑ **Parent:** [Contest theory](#contest-theory)

A finite sequence of [all-pay contests](#all-pay-auction) in which each stage awards one prize and its winner leaves. Losing players remain eligible for later stages. A player can receive at most one prize, while its effort costs are incurred whenever it participates. [Subgame perfect equilibrium](#subgame-perfect-equilibrium) accounts for both the immediate prize and the value of remaining eligible.

#### Backward-induction threshold in an elimination all-pay contest

↑ **Parent:** [Sequential elimination all-pay contest](#sequential-elimination-all-pay-contest)

With ordered values $v_1>\cdots>v_k$ and $r<k$ prizes remaining, define $C_r=(1-\delta)\sum_{j=2}^{r}\delta^{j-2}v_j+\delta^{r-1}v_{r+1}$. In the recursively constructed discounted [subgame perfect equilibrium](#subgame-perfect-equilibrium), it is the second active player's effective prize and the effort-support upper endpoint. The highest player's utility is $v_1-C_r$. The coefficients form a convex combination, so $C_r\geq v_{r+1}$, allowing lower-player deviations to be bounded.

##### Vanishing-discount limit of an elimination all-pay contest

↑ **Parent:** [Backward-induction threshold in an elimination all-pay contest](#backward-induction-threshold-in-an-elimination-all-pay-contest)

As $\delta\uparrow1$, both active players' effective prizes in every nonfinal subgame tend to the marginal valuation $v_{r+1}$. The [two-player complete-information all-pay equilibrium](#two-player-complete-information-all-pay-equilibrium) then gives each a winning probability $1/2$. In the final stage, actual valuations determine the asymmetric winning probabilities. Taking this limit from discounted equilibria specifies the continuation selection instead of independently choosing an undiscounted game equilibrium.

###### Ranked winning probabilities in an undiscounted elimination contest

↑ **Parent:** [Vanishing-discount limit of an elimination all-pay contest](#vanishing-discount-limit-of-an-elimination-all-pay-contest)

For $m<n$ prizes and ordered distinct valuations, the discounted-equilibrium limit gives $x_1=1-2^{-m}v_{m+1}/v_1$ and $x_i=1-2^{-(m-i+2)}v_{m+1}/v_i$ for $2\leq i\leq m$. A player must lose its successive fair nonfinal contests and then the asymmetric final contest to receive no prize. The marginal player's probability is $m-\sum_{i=1}^m x_i$, and lower players have probability zero.

#### Discounted continuation value in an elimination contest

↑ **Parent:** [Sequential elimination all-pay contest](#sequential-elimination-all-pay-contest)

If $J_i(S,r)$ is a player's net expected utility with remaining players $S$ and $r$ prizes, losing the current stage to player $j$ gives baseline $\delta J_i(S\setminus\{j\},r-1)$. This baseline includes later prize values and later effort costs. Subtracting it from the immediate prize value gives an [effective prize in a sequential contest](#effective-prize-in-a-sequential-contest). Discounting must be applied to utilities, rather than to winning probabilities.

##### Effective prize in a sequential contest

↑ **Parent:** [Discounted continuation value in an elimination contest](#discounted-continuation-value-in-an-elimination-contest)

Relative to losing against a particular rival, the gain from winning now is the current value minus discounted continuation utility. In an elimination contest this is $A_i=v_i-\delta J_i(S\setminus\{j\},r-1)$. When the relevant losing baseline is fixed, current effort incentives reduce to a [two-player complete-information all-pay equilibrium](#two-player-complete-information-all-pay-equilibrium). In general, the baseline can depend on which rival wins; that dependence must be verified before using a single effective prize.

### Sequential private-value all-pay contest

↑ **Parent:** [Contest theory](#contest-theory)

Two players pay their invested efforts regardless of outcome. A leader invests first, and a follower observes that effort before deciding. With ties favoring the follower and unit costs, a follower of value $u$ matches leader effort $b$ when $u>b$, and otherwise declines. For a continuous follower [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $F$, the leader wins with probability $F(b)$ and has payoff $vF(b)-b$.

#### Ex ante follower advantage in a sequential all-pay contest

↑ **Parent:** [Sequential private-value all-pay contest](#sequential-private-value-all-pay-contest)

Every optimal leader bid satisfies $b(v)\leq v$, because bidding zero guarantees payoff zero and winning probability is at most one. Hence $F(b(v))\leq F(v)$. With identically distributed independent continuous valuations, the [probability integral transform](probability-theory.md#probability-integral-transform) gives $\mathbb E F(V)=1/2$. The leader's unconditional winning probability is therefore at most $1/2$, even when some high leader types have a conditional advantage. This argument does not depend on selecting a unique optimum.

#### Leader optimization in a sequential private-value all-pay contest

↑ **Parent:** [Sequential private-value all-pay contest](#sequential-private-value-all-pay-contest)

With follower distribution $F$, a leader of value $v$ chooses $b\in\arg\max_{0\leq b\leq1}\{vF(b)-b\}$. If $F$ is a [concave function](real-analysis.md#concave-function), the objective is concave and an interior optimum satisfies $vF'(b)=1$. Endpoint derivatives handle zero or maximal effort. Zero effort guarantees nonnegative payoff, so every optimum satisfies $b\leq vF(b)\leq v$.

##### Best-response selection at a flat leader objective

↑ **Parent:** [Leader optimization in a sequential private-value all-pay contest](#leader-optimization-in-a-sequential-private-value-all-pay-contest)

If a concave leader objective $vF(b)-b$ is constant over an interval, all efforts there are [best responses](#best-response), but they can have different winning probabilities. A flat positive-density interval of $F$ produces this at the type $v=1/F'$. Thus strict threshold statements must distinguish strict concavity from a selection such as the smallest maximizing effort. For an atom-free type distribution, the specified threshold type has zero ex ante probability.

##### Median-density threshold for the leader in an all-pay contest

↑ **Parent:** [Leader optimization in a sequential private-value all-pay contest](#leader-optimization-in-a-sequential-private-value-all-pay-contest)

For increasing concave $F$, write $q=F^{-1}(1/2)$. Under the smallest-maximizer convention, the leader wins with probability greater than $1/2$ exactly when $v>1/F'(q)$. The sign of $vF'(q)-1$ places the maximizer before or after $q$. At equality, concavity alone permits a flat interval of optima; strict concavity or an explicit selection is needed for the strict comparison at that type.

### Proportional allocation contest

↑ **Parent:** [Contest theory](#contest-theory)

For positive total effort, a proportional allocation contest awards player $i$ the prize with [probability](probability-theory.md#probability) $b_i/\sum_j b_j$, or gives it that proportion of a divisible prize. A convention is needed at zero total effort. This allocation is different from the discontinuous highest-effort rule of an [all-pay auction](#all-pay-auction).

#### Proportional contest with outside effort

↑ **Parent:** [Proportional allocation contest](#proportional-allocation-contest)

An [all-pay contest](#all-pay-auction) with allocations $x_i=b_i/(\sum_jb_j+\delta)$ includes fixed outside effort $\delta\geq0$. A player with unit effort cost has payoff $v_ix_i-b_i$. The outside effort represents an ineligible fixed competitor and may leave some prize probability unallocated to eligible players. At equilibrium, a player is active exactly when its value exceeds total eligible effort plus outside effort.

##### Active-set threshold for a proportional contest with outside effort

↑ **Parent:** [Proportional contest with outside effort](#proportional-contest-with-outside-effort)

For ordered positive valuations, rank $j$ is active exactly when $\delta<v_j(2-j+\sum_{i<j}v_j/v_i)$. These ranks form a prefix, and the number active is the largest qualifying rank, or zero if none qualifies. This follows by evaluating the decreasing equilibrium equation $\sum_i(1-S/v_i)_+-1+\delta/S=0$ at $S=v_j$. Strict inequality excludes zero-effort boundary players.

##### Total-effort formula for a proportional contest with outside effort

↑ **Parent:** [Proportional contest with outside effort](#proportional-contest-with-outside-effort)

With $k>0$ active players of [harmonic mean](arithmetic.md#harmonic-mean) valuation $\bar v_k$, unit-cost [Nash equilibrium](#nash-equilibrium) effort satisfies $R+\delta=\frac{\bar v_k}{2k}[(k-1)+\sqrt{(k-1)^2+4k\delta/\bar v_k}]$. Sum the active-player first-order equations $b_i=(R+\delta)(1-(R+\delta)/v_i)$ to obtain the quadratic. If $\delta$ is at least the largest valuation, no one is active and $R=0$. With no outside effort, at least two players must be active.

#### Quadratic-cost two-player proportional contest

↑ **Parent:** [Proportional allocation contest](#proportional-allocation-contest)

With values $v_i>0$ and effort costs $b_i^2$, the unique pure [Nash equilibrium](#nash-equilibrium) has the efforts displayed above. Interior [first-order conditions](mathematical-optimization.md#first-order-optimality-condition) give $v_i b_j/(b_1+b_2)^2=2b_i$, hence $b_1/b_2=\sqrt{v_1/v_2}$ and $(b_1+b_2)^2=\sqrt{v_1v_2}/2$. Against a positive rival effort, each payoff is a [strictly concave function](real-analysis.md#strictly-concave-function), so these conditions identify global [best responses](#best-response). On the axes, lowering a positive uncontested effort or adding a sufficiently small effort at the zero tie rules out equilibrium.

### Simultaneous all-pay contests

↑ **Parent:** [Contest theory](#contest-theory)

Players choose efforts in several [all-pay contests](#all-pay-auction) at the same time. With additive [quasilinear utility](utility-function.md#quasilinear-utility) and no shared effort budget, a player's expected payoff is the sum of its per-contest payoffs. An entry restriction couples the choices of contests even though the subsequent effort optimization is separable.

#### Two-of-three all-pay participation equilibrium

↑ **Parent:** [Simultaneous all-pay contests](#simultaneous-all-pay-contests)

Consider $n\geq2$ identical players, prizes $w_j>0$, unit effort costs, and exactly two entries per player. The symmetric equilibrium omission probabilities $q_j$ sum to one. The common per-contest payoff is $u=(\sum_j w_j^{-1/(n-1)})^{-(n-1)}$, and the unconditional rival distribution on $0\leq b\leq w_j-u$ is $G_j(b)=((b+u)/w_j)^{1/(n-1)}$. Conditional on entry, its [distribution function](probability-theory.md#cumulative-distribution-function) is $(G_j(b)-q_j)/(1-q_j)$. Choosing the omitted contest according to $q$ and sampling the two active efforts independently gives a [symmetric equilibrium](#symmetric-equilibrium) with expected payoff $2u$. These formulas determine the marginal laws; they do not determine the dependence between a player's two efforts.

##### Marginal-equivalent equilibria in additive contests

↑ **Parent:** [Two-of-three all-pay participation equilibrium](#two-of-three-all-pay-participation-equilibrium)

If contest rewards and costs add, a fixed deviation's expected payoff depends on each rival's per-contest [marginal distributions](probability-theory.md#marginal-distribution), rather than on dependence between that rival's efforts across contests. Replacing the conditional independent sampling of two active efforts by another [copula](probability-theory.md#copula-probability-theory) with the same conditional marginals therefore preserves every deviation payoff. Consequently it preserves the [Nash equilibrium](#nash-equilibrium), even when the new joint strategy distribution is different. This explains why unique participation probabilities and bid marginals need not imply a unique full [mixed strategy](#mixed-strategy).

#### All-pay indifference equation with random entry

↑ **Parent:** [Simultaneous all-pay contests](#simultaneous-all-pay-contests)

For a prize of value $w$, let $G(b)$ be the probability that a rival is absent or enters with effort at most $b$. When rivals act independently and have no atoms at positive efforts, effort $b>0$ wins with probability $G(b)^{n-1}$. If a player mixes over an interval of [best responses](#best-response), its payoff on that interval is constant, so $G(b)=((b+u)/w)^{1/(n-1)}$. If the absence probability is $q$ and the active [effort support](probability-theory.md#effort-support) starts at zero, then $u=wq^{n-1}$.

### Rank-order contest

↑ **Parent:** [Contest theory](#contest-theory)

A rank-order contest awards a sequence of prizes according to the ranks of efforts, while every player incurs its own effort cost. With an [independent private values model](#independent-private-values-model), an increasing symmetric bidding function orders efforts in the same way as valuations.

#### All-pay effort identity

↑ **Parent:** [Rank-order contest](#rank-order-contest)

Suppose values are nonnegative, the [rank-order expected prize allocation](#rank-order-expected-prize-allocation) $a$ is increasing and differentiable, and $a(\underline v)=0$. With unit effort cost and zero effort at the lowest type, the symmetric equilibrium effort is $b(v)=v a(v)-\int_{\underline v}^v a(t)dt$. A true type $v$ imitating type $z$ receives utility $v a(z)-b(z)$, whose derivative in $z$ is $(v-z)a'(z)$. It increases up to $v$ and decreases afterwards, proving the [best response](#best-response) property. This is the [interim payment identity](#interim-payment-identity) specialized to an [all-pay contest](#all-pay-auction).

##### Expected effort in a rank-order contest

↑ **Parent:** [All-pay effort identity](#all-pay-effort-identity)

Let $V_{[1]}\geq\cdots\geq V_{[n]}$ be descending [order statistics](probability-theory.md#order-statistic), with $w_n=0$ and nonnegative decreasing prizes. Decompose the prize vector into awards of $w_k-w_{k+1}$ to each of the best $k$ players. The corresponding truthful multi-unit auction charges each winner the next value $V_{[k+1]}$. Its total payment is $k(w_k-w_{k+1})V_{[k+1]}$. [Revenue equivalence](#revenue-equivalence) transfers the expected payment to the [all-pay contest](#all-pay-auction), because the interim allocations and lowest-type utilities coincide. Summing the layers proves the formula.

###### Uniform-value multi-prize all-pay effort formula

↑ **Parent:** [Expected effort in a rank-order contest](#expected-effort-in-a-rank-order-contest)

With $n$ independent uniform types, $m<n$ equal prizes of scale $w(m/n)$ and unit effort costs, a symmetric [Bayesian Nash equilibrium](#bayesian-nash-equilibrium) has total expected effort $R_m=m(n-m)w(m/n)/(n+1)$. The [all-pay effort identity](#all-pay-effort-identity) yields $b(v)=w(m/n)\int_0^v t q_m'(t)dt$. The allocation derivative is a [Beta distribution](probability-theory.md#beta-distribution) density with parameters $n-m,m$, so integration gives the formula.

###### Discrete prize-count optimization for a power-valued contest

↑ **Parent:** [Uniform-value multi-prize all-pay effort formula](#uniform-value-multi-prize-all-pay-effort-formula)

For prize scale $w(x)=x^{-\alpha}$, total effort is proportional to $h(x)=x^{1-\alpha}(1-x)$ on the feasible grid $x=m/n$. If $\alpha\geq1$, one prize is optimal. For $0<\alpha<1$, $h$ increases up to $x_*=(1-\alpha)/(2-\alpha)$ and then decreases, so the optimal feasible integer is among $\lfloor nx_*\rfloor$ and $\lfloor nx_*\rfloor+1$. Remove infeasible candidates and compare their objective values. No definition at $x=0$ is needed.

#### Rank-order expected prize allocation

↑ **Parent:** [Rank-order contest](#rank-order-contest)

For $n$ players with independent valuations having a continuous [distribution function](probability-theory.md#cumulative-distribution-function) $F$, a type $v$ occupies rank $k$ when exactly $k-1$ rivals have higher values. Multiplying this [binomial distribution](discrete-probability-distribution.md#binomial-distribution) by the rank prize $w_k$ and summing gives $a(v)$. Ties occur only on [zero-probability events](probability-theory.md#zero-probability-event) when the valuation law is atomless.

### Prize allocation rule

↑ **Parent:** [Contest theory](#contest-theory)

A prize allocation rule assigns winning probabilities or divisible prize shares to a profile of efforts. In an [all-pay auction](#all-pay-auction), the greatest effort wins; a [proportional allocation contest](#proportional-allocation-contest) instead assigns shares continuously according to relative effort. The rule is essential data of a contest model.

#### Winning probability

↑ **Parent:** [Prize allocation rule](#prize-allocation-rule)

A winning probability is the [probability](probability-theory.md#probability) that a specified participant receives the prize, conditional on the submitted efforts and the allocation rule's randomization.

## Bayesian game

↑ **Parent:** [Game theory](game-theory.md)

A Bayesian game gives players private information about their types, a probability model for that information, and strategies depending on the player's own type. A [private-value auction](#private-value-auction) with uncertain other valuations is a Bayesian game.

### Bayesian Nash equilibrium

↑ **Parent:** [Bayesian game](#bayesian-game)

A Bayesian Nash equilibrium consists of type-dependent strategies such that every type maximizes its conditional expected payoff given the other players' strategies and the type distribution. It is a [Nash equilibrium](#nash-equilibrium) in the strategic description whose actions are whole contingent strategy functions. Auction incentive comparisons can test a deviation by imitating another type's equilibrium bid.

## Mechanism design

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mechanism_design)

Mechanism design chooses allocation and payment rules while accounting for how agents' information and incentives affect their reports. [Social choice theory](#social-choice-theory) studies collective choice from preferences, while [auction](#auction) design also uses monetary transfers.

### Expected seller revenue

↑ **Parent:** [Mechanism design](#mechanism-design)

The expectation of the seller's total receipts over the buyers' valuation types and any randomization in the sales mechanism. In an [auction](#auction) it is the sum of the bidders' expected payments; with a [posted price](#posted-price) it is price times sale probability. It does not subtract selling costs or the seller's opportunity cost of retaining the item, so it is revenue rather than profit.

### Posted price

↑ **Parent:** [Mechanism design](#mechanism-design)

A seller commits to a fixed price and sells if at least one buyer accepts. With two independent valuations having common cumulative distribution $F$, the sale probability is $1-F(p)^2$ and expected revenue is $p(1-F(p)^2)$. The winner's selection among multiple willing buyers does not affect this revenue.

### Mechanism (mechanism design)

↑ **Parent:** [Mechanism design](#mechanism-design)

A mechanism specifies participants' available messages, an allocation rule, and any payment rule. [Mechanism design](#mechanism-design) chooses these rules to achieve an objective while respecting participants' [incentive compatibility](#incentive-compatibility) and [individual rationality](#individual-rationality).

### Single-parameter mechanism

↑ **Parent:** [Mechanism design](#mechanism-design)

In a single-parameter mechanism, player $i$ has one private scalar value $v_i$, receives an allocation amount $x_i$, and has [quasilinear utility](utility-function.md#quasilinear-utility) $v_i x_i-p_i$. The allocation-payment relation is governed by [incentive compatibility](#incentive-compatibility) and the [interim payment identity](#interim-payment-identity).

#### Virtual valuation

↑ **Parent:** [Single-parameter mechanism](#single-parameter-mechanism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virtual_valuation)

For an absolutely continuous valuation distribution with density $f(v)>0$, its virtual valuation is $v-(1-F(v))/f(v)$. The [virtual-surplus revenue identity](#virtual-surplus-revenue-identity) converts expected incentive-compatible payments into expected allocations weighted by virtual valuations. A [regular prior](#regular-distribution-economics) makes this quantity nondecreasing.

##### Virtual surplus

↑ **Parent:** [Virtual valuation](#virtual-valuation)

Virtual surplus weights allocation amounts by the corresponding [virtual valuations](#virtual-valuation). Under the hypotheses of the [virtual-surplus revenue identity](#virtual-surplus-revenue-identity), maximizing it subject to implementability and feasibility yields a revenue-optimal mechanism when lowest-type utilities can be normalized to zero.

##### Virtual-surplus revenue identity

↑ **Parent:** [Virtual valuation](#virtual-valuation)

For an [independent private values model](#independent-private-values-model), let $X_i(v)$ and $P_i(v)$ be interim allocation and payment. The [interim payment identity](#interim-payment-identity) gives $P_i(v)=vX_i(v)-U_i(\underline v_i)-\int_{\underline v_i}^vX_i(t)dt$. Applying [Fubini's theorem](measure-theory.md#fubini-s-theorem) to reverse the order of integration yields $\mathbb E\int_{\underline v_i}^{V_i}X_i(t)dt=\int X_i(t)(1-F_i(t))dt$. Subtracting this term from $\int vX_i(v)f_i(v)dv$ proves the identity. [Interim individual rationality](#interim-individual-rationality) bounds the lowest-type utilities below by zero.

###### Revenue-optimal public-project auction

↑ **Parent:** [Virtual-surplus revenue identity](#virtual-surplus-revenue-identity)

In a public-project [single-parameter mechanism](#single-parameter-mechanism), all players receive the same binary allocation. For independent [regular priors](#regular-distribution-economics) and voluntary participation with zero outside utility, maximizing [virtual surplus](#virtual-surplus) means providing the project exactly when $\sum_i\phi_i(v_i)\geq0$. The allocation is monotone in each value, so [critical-value payments](#critical-value-payment) implement it with [dominant-strategy incentive compatibility](#dominant-strategy-incentive-compatibility) and [ex post individual rationality](#ex-post-individual-rationality). For independent uniform values on $[0,1]$, the condition is $\sum_i v_i\geq n/2$, with winning payment $\max\{0,n/2-\sum_{j\ne i}v_j\}$.

##### Regular distribution (economics)

↑ **Parent:** [Virtual valuation](#virtual-valuation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_distribution_(economics))

A valuation distribution is regular when its [virtual valuation](#virtual-valuation) is a [nondecreasing function](calculus.md#nondecreasing-function) of value. This is an auction-theory condition, not the unrelated regularity notions used elsewhere in mathematics.

### Direct revelation mechanism

↑ **Parent:** [Mechanism design](#mechanism-design)

A direct revelation mechanism asks agents to report their types directly, then computes allocation and payments from those reports. Being direct does not itself imply [strategyproofness](#strategyproofness); the allocation and payment rules must supply the incentive guarantee.

#### Revelation principle

↑ **Parent:** [Direct revelation mechanism](#direct-revelation-mechanism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Revelation_principle)

An equilibrium outcome of a [mechanism](#mechanism-mechanism-design) can be reproduced by asking for types and then sending the messages prescribed by the original equilibrium strategies. Truthful reports are then a [Bayesian Nash equilibrium](#bayesian-nash-equilibrium): a profitable false report would induce a profitable original deviation. This reduces optimization over indirect mechanisms to [direct revelation mechanisms](#direct-revelation-mechanism) with [Bayesian incentive compatibility](#bayesian-incentive-compatibility), under the same information and participation assumptions.

#### Vickrey-Clarke-Groves mechanism

↑ **Parent:** [Direct revelation mechanism](#direct-revelation-mechanism)

The pivot form chooses a reported-welfare-maximizing allocation and charges each agent the maximum welfare achievable by the others without that agent minus the others' welfare in the chosen allocation. With [quasilinear utility](utility-function.md#quasilinear-utility), truthful reporting is a dominant strategy because the first term in the payment depends only on other reports. For two identical items and three unit-demand bidders, each winner pays the lowest reported valuation and the loser pays zero.

### Incentive compatibility

↑ **Parent:** [Mechanism design](#mechanism-design)

Incentive compatibility makes the prescribed truthful or type-dependent strategy optimal under the specified solution concept. Dominant-strategy incentive compatibility holds for every other report profile; Bayesian incentive compatibility compares expected utilities over the other agents' types.

#### Dominant-strategy incentive compatibility

↑ **Parent:** [Incentive compatibility](#incentive-compatibility)

Dominant-strategy incentive compatibility means truthful reporting maximizes a player's utility for every fixed profile of the other reports. It is the monetary-mechanism version of [strategyproofness](#strategyproofness) and implies [Bayesian incentive compatibility](#bayesian-incentive-compatibility) under any independent prior.

##### Critical-value payment

↑ **Parent:** [Dominant-strategy incentive compatibility](#dominant-strategy-incentive-compatibility)

A monotone binary allocation is made truthful by charging its winning threshold, truncated below at the lowest allowed value, and charging zero to losers. The displayed integral formula sets the lowest type's utility to zero. To check it, hold the other reports fixed: a type above the threshold benefits from winning at that price, while a type below it benefits from losing. At a threshold, either deterministic tie choice is compatible with indifference.

#### Bayesian incentive compatibility

↑ **Parent:** [Incentive compatibility](#incentive-compatibility)

Truthful reporting is Bayesian incentive compatible when every type maximizes its expected utility over the other players' types by reporting truthfully. In an [independent private values model](#independent-private-values-model), the displayed inequality uses the same interim allocation and payment functions for every possible true type.

### Individual rationality

↑ **Parent:** [Mechanism design](#mechanism-design)

Individual rationality means participation yields at least the outside-option utility, normalized here to zero. A risk-neutral zero-value bidder with nonnegative payments and no positive-valued allocation must have zero expected payment and utility if participation is individually rational.

#### Ex post individual rationality

↑ **Parent:** [Individual rationality](#individual-rationality)

Ex post individual rationality requires nonnegative participation utility at every realized profile of types. A truthful threshold allocation with its [critical-value payment](#critical-value-payment) satisfies this condition for nonnegative valuations.

#### Interim individual rationality

↑ **Parent:** [Individual rationality](#individual-rationality)

Interim individual rationality requires a nonnegative expected participation utility for each private type, averaging over the other types with the player's conditional beliefs. It differs from requiring nonnegative utility at each realized profile, which is [ex post individual rationality](#ex-post-individual-rationality).

### Auction

↑ **Parent:** [Mechanism design](#mechanism-design)

An auction allocates goods using submitted messages and a specified payment rule. [Private-value auctions](#private-value-auction) model each bidder's valuation as its own private information. Equilibrium bids depend on the allocation and payment rules, not only on valuations.

#### Vickrey auction

↑ **Parent:** [Auction](#auction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vickrey_auction)

A single-item [auction](#auction) in which the highest bidder wins and pays the highest competing bid. Under private values and [quasilinear utility](utility-function.md#quasilinear-utility), bidding one's valuation is a [dominant strategy](#dominant-strategy): if the competing maximum is below one's value, winning at that price is best; if it is above one's value, losing is best; equality gives zero utility either way. Thus truthful bidding is an ex post [Nash equilibrium](#nash-equilibrium).

#### Lowest-price auction

↑ **Parent:** [Auction](#auction)

The highest bidder wins a single item but pays the lowest submitted bid, while losers pay nothing. This differs from a [lowest unique bid auction](#least-unique-bid-auction). With at least two bidders using increasing strategies, the winning bidder pays the smallest opponent bid.

// Target: mathematical-optimization.bigb

##### Uniform lowest-price auction equilibrium

↑ **Parent:** [Lowest-price auction](#lowest-price-auction)

For $n\geq2$ risk-neutral bidders with independent [uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$, the [lowest-price auction](#lowest-price-auction) has a symmetric [Bayesian Nash equilibrium](#bayesian-nash-equilibrium) $b(v)=(n-1)v$. A deviation bidding $(n-1)z$, with $0\leq z\leq1$, wins with probability $z^{n-1}$ and has expected payment $(n-1)z^n/n$. Its expected profit is $vz^{n-1}-(n-1)z^n/n$, whose derivative is $(n-1)z^{n-2}(v-z)$, proving optimality at $z=v$. Bids above $n-1$ give the same outcome as $z=1$. The seller receives $(n-1)$ times the minimum of $n$ independent uniform valuations, with expected revenue $(n-1)/(n+1)$.

// Target: mathematical-optimization.bigb

#### Reserve price

↑ **Parent:** [Auction](#auction)

A reserve price is the seller's minimum acceptable price. In an [English auction](#english-auction) it changes both the sale rule and the payment rule: the highest valuation must exceed the reserve and the winner pays at least the reserve. Mechanisms with different reserves generally have different allocation probabilities, so [revenue equivalence](#revenue-equivalence) need not equate their expected revenues.

#### English auction

↑ **Parent:** [Auction](#auction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/English_auction)

In an ideal continuous-price auction with independent private values, bidders remain active up to their valuations. Without a reserve, the last remaining bidder wins at the second-highest valuation. With a [reserve price](#reserve-price) $r$, there is no sale if every valuation is below $r$; otherwise the winner pays the larger of $r$ and the second-highest valuation. Strict versus weak inequalities at the reserve have no revenue effect for continuous valuation distributions. This payment rule is distinct from a [first-price sealed-bid auction](#first-price-sealed-bid-auction).

#### Least unique bid auction

↑ **Parent:** [Auction](#auction)

Each bidder chooses a permitted amount. The bidder with the smallest amount submitted by exactly one bidder wins and pays that amount; if no amount is unique, nobody wins. With object value $V$, the winner's payoff is $V$ minus their bid, and losers pay nothing. Unlike a [first-price sealed-bid auction](#first-price-sealed-bid-auction), repeated lowest bids can be disqualified.

##### Two-bid three-player least unique bid auction

↑ **Parent:** [Least unique bid auction](#least-unique-bid-auction)

For bids $1,2$ and $V>2$, write $p_i$ for player $i$'s [probability](probability-theory.md#probability) of bidding $1$. The two expected payoffs are $(V-1)(1-p_j)(1-p_k)$ and $(V-2)p_jp_k$. Their unique [symmetric equilibrium](#symmetric-equilibrium) uses the displayed probability. Every permutation of $(1,0,t)$, $0\leq t\leq1$, is also a [Nash equilibrium](#nash-equilibrium): the mixed bidder is indifferent, while the two pure bidders weakly prefer their prescribed bids. There are no further equilibria. Three interior probabilities must all coincide, since subtracting two indifference equations gives a nonzero positive factor times their difference. Two interior probabilities with a pure opponent are impossible, and a single interior probability requires the other two bids to differ. Thus the nonsymmetric equilibria form six line segments with six pure endpoints, and their number is uncountable.

#### All-pay auction

↑ **Parent:** [Auction](#auction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/All-pay_auction)

In a standard all-pay auction, every player pays its bid or effort cost, and the highest bid receives the prize. With a value $v_i$, unit effort cost, and [winning probability](#winning-probability) $x_i(b)$, player $i$ has [quasilinear utility](utility-function.md#quasilinear-utility) $v_i x_i(b)-b_i$. Equal highest bids require an explicit tie rule.

##### Two-player complete-information all-pay equilibrium

↑ **Parent:** [All-pay auction](#all-pay-auction)

For effective prizes $A_1\geq A_2>0$ and unit effort costs, equilibrium effort CDFs on $[0,A_2]$ are $G_1(b)=b/A_2$ and $G_2(b)=1-A_2/A_1+b/A_1$. The weaker player has an atom at zero. Incremental utilities are $A_1-A_2$ and zero, and winning probabilities are $1-A_2/(2A_1)$ and $A_2/(2A_1)$. Direct payoff indifference and exclusion of larger bids verify the [Nash equilibrium](#nash-equilibrium). A further player with effective prize at most $A_2$ cannot profit by entering against these distributions.

#### First-price sealed-bid auction

↑ **Parent:** [Auction](#auction)

Each bidder submits one private bid; the highest bidder wins and pays its own bid, while losers pay nothing. A multi-unit version can award one item to each of the highest bidders, each paying its own bid. In a monotone symmetric equilibrium, a bidder can imitate another type's bid when checking incentive constraints.

##### No dominant positive-value bid in a first-price auction

↑ **Parent:** [First-price sealed-bid auction](#first-price-sealed-bid-auction)

In a [first-price sealed-bid auction](#first-price-sealed-bid-auction) with at least two bidders, continuous nonnegative bids, [quasilinear utility](utility-function.md#quasilinear-utility) and positive private value $v$, no bid is a [dominant strategy](#dominant-strategy). Against opponents all bidding zero, any positive bid can be lowered while still winning, increasing the payoff. Bid zero fails against an opposing bid $v/2$, since bidding $3v/4$ earns $v/4>0$. Nor does randomizing create a [dominant strategy](#dominant-strategy). Against all-zero opponents, a random bid has expected payoff strictly below $v$ unless it is identically zero and receives the item with certainty under the tie rule. In the strict case, a sufficiently small positive fixed bid earns more. In the exceptional case, the deviation against $v/2$ again improves the payoff. Finite expected utility is implicit; an expected payoff of negative infinity cannot dominate finite-payoff bids. The positive-value condition matters: a zero-value bidder weakly prefers bid zero.

##### Uniform private-value first-price bidding equilibrium

↑ **Parent:** [First-price sealed-bid auction](#first-price-sealed-bid-auction)

For $n\geq2$ [risk-neutral](utility-function.md#risk-neutrality) bidders with independent uniform valuations on $[0,1]$, this rule is a symmetric [Bayesian Nash equilibrium](#bayesian-nash-equilibrium). If opponents use $\beta(v)=av$, a bid $b\in[0,a]$ has expected utility $(v-b)(b/a)^{n-1}$. Its derivative has the sign of $(n-1)v-nb$, so with $a=(n-1)/n$ the best bid is $av$. Bids above $a$ guarantee winning but only increase payment. The type-$v$ equilibrium utility is $v^n/n$.

#### Interim payment identity

↑ **Parent:** [Auction](#auction)

For a risk-neutral single-parameter bidder with incentive-compatible type reports, interim utility satisfies $u'(\theta)=G(\theta)$ wherever the winning probability is continuous. Consequently expected payment is determined by allocation probabilities and the utility of the lowest type. The common normalization $u(0)=0$ must be justified, not obtained from allocation alone.

##### Revenue equivalence

↑ **Parent:** [Interim payment identity](#interim-payment-identity)

Two auctions with the same interim allocation probabilities and the same lowest-type utilities have the same interim expected payments under the usual risk-neutral single-parameter incentive conditions. Equal realized payments are not required. This conclusion follows directly from the [interim payment identity](#interim-payment-identity).

#### Private-value auction

↑ **Parent:** [Auction](#auction)

A private-value auction gives each bidder its own value for receiving an item; the value is determined by its own type rather than by another bidder's information. An [independent private values model](#independent-private-values-model) also assumes independence between types.

##### Unit-demand valuation

↑ **Parent:** [Private-value auction](#private-value-auction)

A bidder with unit demand values receiving one item but obtains no additional value from extra identical units. Selecting two winners means awarding one item to each of two bidders, not two units to one bidder.

##### Independent private values model

↑ **Parent:** [Private-value auction](#private-value-auction)

This model assigns independent private valuation types to the bidders. Symmetry adds identical type distributions and bidder roles. These assumptions determine interim winning probabilities from the valuation distribution in a monotone symmetric equilibrium.

###### Symmetric independent private values model

↑ **Parent:** [Independent private values model](#independent-private-values-model)

The [independent private values model](#independent-private-values-model) is symmetric when bidders have identical roles and draw their valuations independently from the same distribution. For [revenue equivalence](#revenue-equivalence) in the usual single-object setting, bidders additionally have [risk neutrality](utility-function.md#risk-neutrality) and [quasilinear utility](utility-function.md#quasilinear-utility). Under a strictly increasing symmetric equilibrium bidding rule, a type $v$ wins with probability $F(v)^{n-1}$.

// Target: mathematical-optimization.bigb

###### Revenue comparison for two uniform private values

↑ **Parent:** [Independent private values model](#independent-private-values-model)

For two independent uniform valuations on $[0,1]$, optimal [posted price](#posted-price) revenue is $2/(3\sqrt3)$, attained at $p=1/\sqrt3$. An [English auction](#english-auction) without reserve earns the expected minimum, $1/3$. With reserve $r\in[0,1]$, revenue is $r\Pr(\text{exactly one valuation exceeds }r)$ plus the expected smaller valuation when both exceed $r$, namely $1/3+r^2-4r^3/3$. It is maximized at $r=1/2$, giving $5/12$. Different reserve-dependent allocation probabilities explain why this differs from the no-reserve revenue without violating [revenue equivalence](#revenue-equivalence).

### Strategyproofness

↑ **Parent:** [Mechanism design](#mechanism-design)

A mechanism or [social choice function](#social-choice-function) is strategyproof if truthful reporting is a weakly dominant strategy: for every true type and every collection of other reports, no misreport yields strictly higher utility or a strictly preferred outcome. This is stronger than merely requiring truthful reports to form a [Nash equilibrium](#nash-equilibrium).

#### Rank-raising monotonicity lemma

↑ **Parent:** [Strategyproofness](#strategyproofness)

If a [strategyproof](#strategyproofness) [social choice function](#social-choice-function) selects $a$, raising $a$ in one agent's order without moving any formerly lower alternative above it preserves the outcome. A different outcome would make one of the changes between the old and new reports a profitable deviation. Arbitrary changes among alternatives wholly above or wholly below $a$ are allowed.

#### Gibbard-Satterthwaite theorem

↑ **Parent:** [Strategyproofness](#strategyproofness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbard–Satterthwaite_theorem)

With a finite set of at least three alternatives and unrestricted strict preference orders, every onto deterministic [strategyproof](#strategyproofness) [social choice function](#social-choice-function) is a [dictatorship in social choice](#dictatorship-in-social-choice). Restricting to two alternatives or to a restricted preference domain removes essential hypotheses.

##### Binary social ordering from strategyproof choice

↑ **Parent:** [Gibbard-Satterthwaite theorem](#gibbard-satterthwaite-theorem)

For an onto [strategyproof](#strategyproofness) rule on unrestricted strict preference orders, rank-raising monotonicity implies unanimity and respect for unanimous pairwise preference. Promote each alternative pair to the top two positions in all reports. The selected member depends only on each voter's comparison of that pair. These binary choices form a strict transitive social order: a directed three-cycle would contradict the rule's choice when that triple is placed above all other alternatives, because the chosen member must win both of its binary comparisons. The original outcome is the top of this order. This creates a social ordering with pairwise independence without presuming it as an axiom of the original choice rule.

###### Two-voter dictatorship from binary choice

↑ **Parent:** [Binary social ordering from strategyproof choice](#binary-social-ordering-from-strategyproof-choice)

For two voters and at least three alternatives, pairwise unanimity, pairwise independence and transitivity force the [binary social ordering from strategyproof choice](#binary-social-ordering-from-strategyproof-choice) to follow one fixed voter. If voter one wins a conflict $a$ against $b$, use profiles $(a>b>c,b>c>a)$ and $(c>a>b,b>c>a)$ to show it also wins $a$ against $c$ and $c$ against $b$. Repeating this implication yields both directions of every pair. If the initial conflict instead follows voter two, exchange the roles. The social choice, being the top of that ordering, is a [dictatorship in social choice](#dictatorship-in-social-choice). This proves the two-voter case of the [Gibbard-Satterthwaite theorem](#gibbard-satterthwaite-theorem).

##### Top-bottom decisiveness lemma

↑ **Parent:** [Gibbard-Satterthwaite theorem](#gibbard-satterthwaite-theorem)

For two agents and a [strategyproof](#strategyproofness) [social choice function](#social-choice-function), if an alternative is selected when one agent ranks it first and the other ranks it last, it is selected whenever the first agent ranks it first, whatever the other agent reports. Changing the first agent's order preserves its attainable top choice; changing the second agent's order cannot offer it an improvement over a selected bottom alternative.

### Social choice theory

↑ **Parent:** [Mechanism design](#mechanism-design)

Social choice theory studies how individual preferences determine a collective decision. A [social choice function](#social-choice-function) selects one alternative from a preference profile; [strategyproofness](#strategyproofness) asks whether agents can benefit by misrepresenting their preferences.

#### Condorcet winner

↑ **Parent:** [Social choice theory](#social-choice-theory)

A [Condorcet winner](#condorcet-winner) defeats every other alternative by a strict majority in pairwise voting. It is unique when it exists. For an odd electorate with [single-peaked preferences](#single-peaked-preferences), the median peak is a [Condorcet winner](#condorcet-winner): alternatives on either side lose to the majority whose peaks lie at or beyond the median in the other direction. With an even electorate ties may prevent a strict winner.

##### Weak Condorcet winner

↑ **Parent:** [Condorcet winner](#condorcet-winner)

A [weak Condorcet winner](#weak-condorcet-winner) is never defeated by a strict pairwise majority, allowing ties. For even electorates with [single-peaked preferences](#single-peaked-preferences), all alternatives between the two middle peaks have this property. A single-valued selection requires a tie convention; arbitrary tie selection is not automatically [strategyproof](#strategyproofness).

#### Single-peaked preferences

↑ **Parent:** [Social choice theory](#social-choice-theory)

A strict preference order is single-peaked on an axis when moving away from its most preferred alternative along either one side of the axis makes alternatives less preferred. Comparisons between opposite sides need not follow symmetric physical distance. A profile is single-peaked when all voters' orders share such an axis. This restricted domain admits the [median voter rule](#median-voter-rule), unlike the unrestricted-domain conclusion of the [Gibbard-Satterthwaite theorem](#gibbard-satterthwaite-theorem).

##### Median voter rule

↑ **Parent:** [Single-peaked preferences](#single-peaked-preferences)

On a fixed common axis, select the median of reported peaks. For odd $n$ this is the unique [Condorcet winner](#condorcet-winner). For even $n$, a fixed lower-median or upper-median convention selects a [weak Condorcet winner](#weak-condorcet-winner). Holding other peaks fixed, the attainable outcomes form an interval between two order statistics. Truthful reporting obtains the true peak if it is inside that interval, or its nearest interval endpoint otherwise, so no allowed report improves the outcome under [single-peaked preferences](#single-peaked-preferences).

#### Social choice function

↑ **Parent:** [Social choice theory](#social-choice-theory)

A deterministic social choice function maps profiles of preference orders to single alternatives. Unrestricted domain permits every profile in $\mathcal R^n$; onto means every alternative lies in the range. A unanimous rule selects an alternative whenever every agent ranks it first.

##### Two-alternative majority rule

↑ **Parent:** [Social choice function](#social-choice-function)

With an odd number of agents and two alternatives, select the alternative ranked first by a strict majority. The rule is onto, [strategyproof](#strategyproofness), and for at least three agents has no [dictator in social choice](#dictator-in-social-choice). A pivotal agent already gets its preferred alternative by reporting truthfully; a nonpivotal agent cannot change the outcome alone.

##### Dictatorship in social choice

↑ **Parent:** [Social choice function](#social-choice-function)

A dictatorship always selects the top alternative of one fixed agent $d$. Other agents cannot alter the selection against that agent's preference. This is the social-choice meaning of dictatorship, rather than a political classification.

###### Dictator in social choice

↑ **Parent:** [Dictatorship in social choice](#dictatorship-in-social-choice)

A dictator is the fixed agent whose top-ranked alternative is always selected by a [dictatorship in social choice](#dictatorship-in-social-choice).

## Pure strategy

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pure_strategy)

A pure strategy chooses one available action with certainty.

### Strict dominance

↑ **Parent:** [Pure strategy](#pure-strategy)

A strategy is strictly dominated when another strategy gives a strictly larger payoff against every opposing strategy. A strictly dominated strategy cannot receive positive probability in a [Nash equilibrium](#nash-equilibrium), because moving that probability to its dominator increases expected payoff.

## Finite game

↑ **Parent:** [Game theory](game-theory.md)

A finite game has finitely many players, each with finitely many [pure strategies](#pure-strategy).

### Symmetric finite game

↑ **Parent:** [Finite game](#finite-game)

A [finite game](#finite-game) is symmetric when all players have the same [pure strategies](#pure-strategy) and permuting the players permutes their payoffs. In the anonymous special case, a player's payoff depends on their own action and the multiset of opposing actions. A [symmetric equilibrium](#symmetric-equilibrium) exists even when there are more than two players, by the [gain-map proof of symmetric equilibrium](#gain-map-proof-of-symmetric-equilibrium).

## Mixed strategy

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mixed_strategy)

A mixed strategy is a probability distribution over a player's pure strategies.

### Support of a mixed strategy

↑ **Parent:** [Mixed strategy](#mixed-strategy)

The [support of a mixed strategy](#support-of-a-mixed-strategy) consists of the pure strategies used with positive probability. At a [Nash equilibrium](#nash-equilibrium), every supported pure strategy is a [best response](#best-response), while unused strategies may give no higher payoff.

// Target: computer-science.bigb

### Strategy support

↑ **Parent:** [Mixed strategy](#mixed-strategy)

The support of a finite [mixed strategy](#mixed-strategy) consists of the [pure strategies](#pure-strategy) assigned positive probability. At a [Nash equilibrium](#nash-equilibrium), every action in the support is a [best response](#best-response). In a game satisfying [nondegeneracy of a bimatrix game](#nondegeneracy-of-a-bimatrix-game), the two equilibrium supports have equal size.

## Bimatrix game

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bimatrix_game)

A bimatrix game is a finite two-player game specified by one payoff matrix for each player.

### Matching pennies

↑ **Parent:** [Bimatrix game](#bimatrix-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matching_pennies)

Each player chooses heads or tails. One receives $1$ if the choices agree and $-1$ otherwise; the other receives the negative payoff. At every pure profile, the losing player can improve by switching, so there is no pure [Nash equilibrium](#nash-equilibrium). Independent uniform randomization makes both pure choices equally valuable for each player and gives a mixed [Nash equilibrium](#nash-equilibrium).

### Lottery over joint action profiles

↑ **Parent:** [Bimatrix game](#bimatrix-game)

A probability distribution over joint action profiles implements a [convex combination](mathematical-optimization.md#convex-combination) of their two-player payoff vectors. The attainable expected payoffs form the [convex hull](mathematical-optimization.md#convex-hull) of the pure joint payoffs. The distribution need not factor into independent [mixed strategies](#mixed-strategy), and a freely enforceable lottery need not satisfy the incentive constraints of a [Nash equilibrium](#nash-equilibrium).

### Support enumeration for a bimatrix game

↑ **Parent:** [Bimatrix game](#bimatrix-game)

Enumerate pairs of [strategy supports](#strategy-support), solve the equations making each supported action indifferent, then check strict positivity of supported probabilities and all omitted-action payoff inequalities. These conditions suffice for a [Nash equilibrium](#nash-equilibrium). Under [nondegeneracy of a bimatrix game](#nondegeneracy-of-a-bimatrix-game), only pairs of equal support size need be tested.

### Symmetric bimatrix game

↑ **Parent:** [Bimatrix game](#bimatrix-game)

A square [bimatrix game](#bimatrix-game) is symmetric when exchanging players exchanges their payoffs: its [payoff matrices](#payoff-matrix) are $P,Q$ with $Q=P^T$. If $(x,y)$ is a [Nash equilibrium](#nash-equilibrium), then $(y,x)$ is also a [Nash equilibrium](#nash-equilibrium). A [symmetric bimatrix game](#symmetric-bimatrix-game) can still have asymmetric equilibria, so the two strategy vectors must be kept separate in the [Lemke-Howson algorithm](#lemke-howson-algorithm).

### Nondegeneracy of a bimatrix game

↑ **Parent:** [Bimatrix game](#bimatrix-game)

A [bimatrix game](#bimatrix-game) is nondegenerate if every [mixed strategy](#mixed-strategy) with $k$ positive coordinates has at most $k$ pure [best responses](#best-response) for the other player. This condition prevents ties in the leaving-variable choice along the usual [Lemke-Howson algorithm](#lemke-howson-algorithm) path and allows unique continuation once the dropped label has been selected.

### Nash equilibrium

↑ **Parent:** [Bimatrix game](#bimatrix-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nash_equilibrium)

A Nash equilibrium is a strategy profile in which no player can increase their expected payoff by changing only their own strategy.

#### Ranked university application game

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)

There are $mq$ distinctly ranked students and $m$ labelled universities with $q$ seats each. Each student applies to one university; each university selects the greatest ranks, and admitted students receive their admitted cohort's average rank. At a pure [Nash equilibrium](#nash-equilibrium), every student is admitted: any rejected student could move to a university with a vacancy. The university with the largest average must contain the top $q$ ranks, since any omitted higher rank could displace its lowest rank and improve. Repeat on the remaining students to obtain consecutive rank blocks. Assigning these blocks to the labelled universities gives exactly $m!$ pure equilibria.

#### Symmetric Nash equilibrium

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)

In a game invariant under permuting players, a symmetric [Nash equilibrium](#nash-equilibrium) gives every player the same strategy, which may be a [mixed strategy](#mixed-strategy). Independent randomization does not require realized resource loads to be equal. When resource delays are affine, a player's expected delay depends on their own certain resource use plus the expected use by the other players; replacing all loads by unconditional total expected loads loses that own-player correction.

#### Equilibrium oddness theorem

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)

A finite nondegenerate [bimatrix game](#bimatrix-game) has a finite odd number of [Nash equilibria](#nash-equilibrium). After shifting to positive payoffs, fully labelled vertex pairs in the bounded best-response polytopes correspond to equilibria plus one artificial zero pair. Dropping a fixed label gives a finite path graph whose endpoints are exactly these pairs. The number of endpoints is even, leaving an odd number of genuine equilibria. This is the endpoint-parity argument underlying the [Lemke-Howson algorithm](#lemke-howson-algorithm).

#### Symmetric equilibrium

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_equilibrium)

A symmetric equilibrium of a symmetric game has every player use the same strategy or the same distribution of strategies. Symmetry between players does not require identical behavior across contests with different prizes.

##### Symmetric equilibrium parity

↑ **Parent:** [Symmetric equilibrium](#symmetric-equilibrium)

In a nondegenerate [symmetric bimatrix game](#symmetric-bimatrix-game), player interchange pairs every nonsymmetric [Nash equilibrium](#nash-equilibrium) with a distinct swapped equilibrium. The [equilibrium oddness theorem](#equilibrium-oddness-theorem) gives an odd total; the remaining fixed points, which are the [symmetric equilibria](#symmetric-equilibrium), therefore also number an odd amount.

##### Symmetric Nash gain map

↑ **Parent:** [Symmetric equilibrium](#symmetric-equilibrium)

The continuous gain map takes a [probability simplex](algebraic-topology.md#probability-simplex) to itself. The [Brouwer fixed-point theorem](topological-analysis.md#brouwer-fixed-point-theorem) supplies a fixed point, whose positive gains would contradict the zero strategy-weighted average payoff excess. Thus all gains vanish, giving a strategy that is a [best response](#best-response) to itself. In a [symmetric bimatrix game](#symmetric-bimatrix-game), this produces a [symmetric equilibrium](#symmetric-equilibrium).

###### Gain-map proof of symmetric equilibrium

↑ **Parent:** [Symmetric Nash gain map](#symmetric-nash-gain-map)

For a [symmetric finite game](#symmetric-finite-game), pure-action expected payoffs $e(i,p)$ against independent identical opposing [mixed strategies](#mixed-strategy) are continuous. The displayed map takes the [probability simplex](algebraic-topology.md#probability-simplex) continuously into itself. At a [Brouwer fixed-point theorem](topological-analysis.md#brouwer-fixed-point-theorem) fixed point, put $r_i=[e(i,p)-e(p)]_+$ and $S=\sum_i r_i$. The fixed-point equations give $r_i=p_iS$. If $S>0$, every supported action has strictly positive excess payoff, contradicting $\sum_i p_i(e(i,p)-e(p))=0$. Hence $S=0$ and every supported action is a [best response](#best-response), proving a [symmetric Nash equilibrium](#symmetric-nash-equilibrium).

#### Complementarity construction of a symmetric Nash equilibrium

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)

For a symmetric [bimatrix game](#bimatrix-game) with payoff matrices $P,P^{\mathsf T}$, any nonzero $x$ satisfying these equations gives the symmetric [Nash equilibrium](#nash-equilibrium) $(x/\sum_i x_i,x/\sum_i x_i)$. Every positive coordinate attains the same maximal payoff. This one-vector construction differs from a two-vector [Lemke-Howson algorithm](#lemke-howson-algorithm) path, which can return asymmetric equilibria.

#### Lemke-Howson algorithm

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lemke–Howson_algorithm)

The Lemke-Howson algorithm follows an almost completely labeled path in the product of two best-response polytopes of a [bimatrix game](#bimatrix-game). Drop one label at the artificial zero pair, then alternately pivot away the duplicated label until the dropped label returns. A nonzero completely labeled endpoint, after normalization, gives a [Nash equilibrium](#nash-equilibrium). The two players' vectors must be kept separate even in a symmetric game.

##### Complementary pivoting

↑ **Parent:** [Lemke-Howson algorithm](#lemke-howson-algorithm)

Complementary pivoting follows adjacent bases while maintaining all but one label of a complementarity system. The [Lemke-Howson algorithm](#lemke-howson-algorithm) for a [bimatrix game](#bimatrix-game) follows the duplicated label between two tableaux until it restores the dropped label at a nonzero completely labelled pair. Normalization then gives a [Nash equilibrium](#nash-equilibrium).

<h4 id="nash-s-theorem">Nash's theorem</h4>

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)

Nash's theorem states that every [finite game](#finite-game) has at least one [Nash equilibrium](#nash-equilibrium) in [mixed strategies](#mixed-strategy).

##### Brouwer gain-map proof of bimatrix equilibrium

↑ **Parent:** [Nash's theorem](#nash-s-theorem)

For each player in a finite [bimatrix game](#bimatrix-game), add the positive pure-strategy gains to its current [mixed strategy](#mixed-strategy) and normalize. This gives a continuous self-map of the product of [probability simplices](algebraic-topology.md#probability-simplex). At a [Brouwer fixed-point theorem](topological-analysis.md#brouwer-fixed-point-theorem) fixed point, the gain coordinates equal the current strategy times their total gain. If that total were positive, every supported action would beat the current average payoff, contradicting that average. Thus every pure deviation has nonpositive gain for both players, proving a [Nash equilibrium](#nash-equilibrium).

#### Brouwer proof of Nash equilibrium for a two-by-two game

↑ **Parent:** [Nash equilibrium](#nash-equilibrium)

Normalize each player's positive pure-strategy payoff improvements to define a continuous self-map of the product of their mixed-strategy simplices. At a Brouwer fixed point every positive improvement must vanish, giving a Nash equilibrium.

## Best response

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Best_response)

A best response is a strategy that maximizes a player's [expected payoff](probability-theory.md#expected-value) when the other players' strategies are held fixed.

### Dominant strategy

↑ **Parent:** [Best response](#best-response)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dominant_strategy)

A dominant strategy is a [best response](#best-response) for every strategy profile of the other players.

#### Strictly dominant strategy

↑ **Parent:** [Dominant strategy](#dominant-strategy)

A strictly dominant strategy gives a strictly greater payoff than every alternative strategy for every strategy profile of the other players.

## Zero-sum game

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zero-sum_game)

In a two-player zero-sum game, one player’s payoff is the other player’s loss.

### Rock paper scissors

↑ **Parent:** [Zero-sum game](#zero-sum-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rock_paper_scissors)

With choices ordered rock, scissors, paper and winner payoff $1$, the row-player payoff matrix is $\left(\begin{smallmatrix}0&1&-1\\-1&0&1\\1&-1&0\end{smallmatrix}\right)$. Both the row and column sums vanish. Thus the uniform [mixed strategy](#mixed-strategy) guarantees expected payoff zero against every opposing strategy; the [value of a zero-sum game](#value-of-a-zero-sum-game) is zero. A player responding to a known nonuniform mixture can instead optimize its linear expected payoff over pure responses and their ties.

### Value of a zero-sum game

↑ **Parent:** [Zero-sum game](#zero-sum-game)

For a finite matrix [zero-sum game](#zero-sum-game), the value is the payoff that the maximizing player can guarantee and the minimizing player can prevent the payoff from exceeding, using [mixed strategies](#mixed-strategy). The common value of the two displayed optimizations exists by the [minimax theorem](#minimax-theorem). A pair of strategies can be verified directly by checking that every pure column pays the row mixture at least $v$ and every pure row earns at most $v$ against the column mixture.

### Cost-weighted finite search game

↑ **Parent:** [Zero-sum game](#zero-sum-game)

In a hide-and-search [zero-sum game](#zero-sum-game) with positive inspection costs $c_i$ and $c=\sum_i c_i$, hiding with probabilities $c_i/c$ gives the same expected search cost for every complete search order. For three locations, beginning at $i$ with probability $c_i/c$ and randomizing the remaining two orders also equalizes every hiding location. The common value is the displayed quantity.

### Matrix game

↑ **Parent:** [Zero-sum game](#zero-sum-game)

A matrix game is a finite two-player zero-sum game whose entry $A_{ij}$ is the row player's payoff when the players choose row $i$ and column $j$.

#### Positive-payoff linear programming for a matrix game

↑ **Parent:** [Matrix game](#matrix-game)

When every entry of a [payoff matrix](#payoff-matrix) $B$ is positive, its game value $v$ is positive. Setting $x=p/v$ converts the row player's [probability](probability-theory.md#probability) vector and guaranteed value into the displayed [linear program](mathematical-optimization.md#linear-programming), whose optimum is $1/v$. Conversely normalizing a feasible $x$ gives a [mixed strategy](#mixed-strategy) guaranteeing $1/(\mathbf1^Tx)$. The dual maximizes $\mathbf1^Ty$ under $By\le\mathbf1$, $y\ge0$ and recovers the column strategy by normalization. Adding a constant to every payoff preserves [Nash equilibria](#nash-equilibrium) and lets this positive-payoff formulation handle general finite [zero-sum games](#zero-sum-game).

#### Payoff matrix

↑ **Parent:** [Matrix game](#matrix-game)

A payoff matrix records the row player's gains when row $i$ meets column $j$. In a [zero-sum game](#zero-sum-game) the other player's payoff is the negative. For [mixed strategies](#mixed-strategy) $p,q$, the expected row payoff is $p^TAq$.

#### Matrix-game optimization problem

↑ **Parent:** [Matrix game](#matrix-game)

The row player solves

$$
\max_{p,v}v
\quad\text{subject to}\quad
A^Tp\geq ve,quad e^Tp=1,quad p\geq0.
$$

#### Mixed-strategy optimality certificate for a matrix game

↑ **Parent:** [Matrix game](#matrix-game)

If the column player has an optimal strategy at value $v$ and a row probability vector $p$ satisfies $p^TA\geq ve^T$, then $p$ is optimal: it guarantees $v$, while the optimal column strategy prevents every row strategy from exceeding $v$.

#### Symmetric inverse formula for a matrix-game equilibrium

↑ **Parent:** [Matrix game](#matrix-game)

If a symmetric invertible payoff matrix satisfies $A^{-1}e\geq0$, both players may use

$$
p=q=\frac{A^{-1}e}{e^TA^{-1}e},
$$

and the game value is $(e^TA^{-1}e)^{-1}$.

##### Three-card threshold-sum zero-sum game

↑ **Parent:** [Symmetric inverse formula for a matrix-game equilibrium](#symmetric-inverse-formula-for-a-matrix-game-equilibrium)

For

$$
A=\begin{pmatrix}2&3&4\\3&4&-5\\4&-5&-6\end{pmatrix},
$$

both players optimally choose cards $1,2,3$ with probabilities $41/50,2/25,1/10$, and the row player's expected payoff is $57/25$.

### Minimax theorem

↑ **Parent:** [Zero-sum game](#zero-sum-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimax_theorem)

The finite minimax theorem equates the maximizing player’s security level with the minimizing player’s security level.

### Optimal mixed strategy

↑ **Parent:** [Zero-sum game](#zero-sum-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Optimal_mixed_strategy)

An optimal mixed strategy guarantees the value of the game against every opposing pure strategy.

### Antisymmetric zero-sum game

↑ **Parent:** [Zero-sum game](#zero-sum-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antisymmetric_zero-sum_game)

A square game with antisymmetric payoff matrix has value zero.

#### Support certificate for an antisymmetric matrix game

↑ **Parent:** [Antisymmetric zero-sum game](#antisymmetric-zero-sum-game)

For an antisymmetric [payoff matrix](#payoff-matrix), such a vector guarantees that an opponent playing rows cannot win positively against it. Antisymmetry also gives $p^TA\ge0$, so the same [mixed strategy](#mixed-strategy) guarantees nonnegative payoff as a row strategy and proves game value zero. Furthermore $p^TAp=0$ forces $(Ap)_i=0$ whenever $p_i>0$. To prove uniqueness, use one certified strategy $q$: any other optimal $p$ satisfies $q^TAp=-(Aq)^Tp$, so a strict negative component of $Aq$ forces the corresponding probability in $p$ to vanish.

#### Consecutive-number antisymmetric game

↑ **Parent:** [Antisymmetric zero-sum game](#antisymmetric-zero-sum-game)

In this game the higher of two chosen integers wins one unit if they are consecutive, but pays two units if their difference is at least two. Ties pay zero. For any choices $1,\ldots,n$ with $n\ge3$, both players can optimally choose $1,2,3$ with probabilities $1/4,1/2,1/4$ and assign zero probability to larger numbers. If $p$ is this vector, $Ap$ is zero in its first three entries, $-5/4$ in its fourth when present, and $-2$ in all later entries. Thus $Ap\le0$ and $p^TA\ge0$, proving the zero value and both security guarantees.

## Dominated strategy

↑ **Parent:** [Game theory](game-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dominated_strategy)

A dominated strategy can be replaced by another strategy that performs at least as well against every opponent action.

### Dominated strategy elimination

↑ **Parent:** [Dominated strategy](#dominated-strategy)

In a finite [zero-sum game](#zero-sum-game), removing a [strictly dominated strategy](#strict-dominance) preserves the [value of a zero-sum game](#value-of-a-zero-sum-game): replace any probability on it by the dominating [pure strategy](#pure-strategy). This increases every payoff for the maximizing player, or decreases every payoff for the minimizing player. Repeat on the reduced game; new domination relations may appear after a deletion.

### Weakly dominated strategy

↑ **Parent:** [Dominated strategy](#dominated-strategy)

A strategy is weakly dominated if another gives at least as much payoff against every opponent strategy and strictly more against at least one. Unlike a [strictly dominated strategy](#strict-dominance), it may remain a [best response](#best-response) to opponents who never choose a strategy where the comparison is strict. Thus [weak domination does not exclude equilibrium strategies](#weak-domination-does-not-exclude-equilibrium-strategies).

#### Equilibrium preservation under iterated weak dominance

↑ **Parent:** [Weakly dominated strategy](#weakly-dominated-strategy)

Starting from the full finite [bimatrix game](#bimatrix-game), sequentially remove actions weakly dominated by current [mixed strategies](#mixed-strategy), with a strict improvement somewhere. At least one [Nash equilibrium](#nash-equilibrium) survives on the final action sets. Take an [Nash equilibrium](#nash-equilibrium) of the reduced game and restore actions in reverse. A restored action is no better against the fixed surviving opponent strategy than its dominating mixture of already available actions, so it introduces no profitable deviation. Any self-weight in a dominating mixture can be removed and renormalized because strict improvement forces that weight below one. Using dominance tested only against an arbitrary initially restricted opponent set does not guarantee an [Nash equilibrium](#nash-equilibrium) of the original full game.

#### Weak domination does not exclude equilibrium strategies

↑ **Parent:** [Weakly dominated strategy](#weakly-dominated-strategy)

In the [zero-sum game](#zero-sum-game) with row payoff matrix $\left(\begin{smallmatrix}0&1\\0&0\end{smallmatrix}\right)$, the second row is weakly dominated by the first. Nevertheless second row and first column form a [Nash equilibrium](#nash-equilibrium): both rows tie against that column, and both columns tie against that row. Weak dominance therefore cannot be used to discard all possible equilibrium strategies without further qualifications.

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Mathematical economics](mathematics.md#mathematical-economics)
- [Stackelberg competition](#stackelberg-competition)
