# Actuarial statistics

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)

Actuarial statistics uses [probability theory](probability-theory.md) and [statistical inference](statistical-inference.md) to quantify insurance claims, premiums, and the uncertainty of future losses. [Aggregate claims model](#aggregate-claims-model) describes portfolios, [reinsurance](#reinsurance) redistributes losses, and the [Bühlmann model](#buhlmann-model) combines experience with population information.

**Table of contents**

- [No claims discount system](#no-claims-discount-system)
  - [Two-year no-claims threshold with reset to zero](#two-year-no-claims-threshold-with-reset-to-zero)
  - [Persistent claim intensity can destroy the discount Markov property](#persistent-claim-intensity-can-destroy-the-discount-markov-property)
  - [Three-level discount equilibrium with geometric annual counts](#three-level-discount-equilibrium-with-geometric-annual-counts)
  - [Three-level no claims discount equilibrium](#three-level-no-claims-discount-equilibrium)
  - [Two-year premium-loss claim threshold](#two-year-premium-loss-claim-threshold)
    - [Incremental second-claim threshold at the highest discount level](#incremental-second-claim-threshold-at-the-highest-discount-level)
- [Expected value premium principle](#expected-value-premium-principle)
- [Credibility estimate](#credibility-estimate)
  - [Bayesian credibility](#bayesian-credibility)
    - [Normal-normal credibility](#normal-normal-credibility)
      - [Normal-normal credibility with unequal exposures](#normal-normal-credibility-with-unequal-exposures)
    - [Inflation-adjusted Poisson-gamma credibility](#inflation-adjusted-poisson-gamma-credibility)
    - [Exact beta-binomial credibility with unequal exposures](#exact-beta-binomial-credibility-with-unequal-exposures)
- [Bühlmann model](#buhlmann-model)
  - [Bühlmann–Straub model](#buhlmann-straub-model)
    - [Bühlmann–Straub credibility estimate](#buhlmann-straub-credibility-estimate)
      - [Exact Bühlmann–Straub credibility for Poisson-gamma counts](#exact-buhlmann-straub-credibility-for-poisson-gamma-counts)
      - [Bühlmann–Straub credibility factor](#buhlmann-straub-credibility-factor)
  - [Bühlmann credibility premium](#buhlmann-credibility-premium)
    - [Balanced-panel method-of-moments credibility](#balanced-panel-method-of-moments-credibility)
    - [Poisson credibility with a shape-three Pareto intensity](#poisson-credibility-with-a-shape-three-pareto-intensity)
    - [Bühlmann credibility for inverse-gamma observations](#buhlmann-credibility-for-inverse-gamma-observations)
    - [Sequential Bühlmann credibility update](#sequential-buhlmann-credibility-update)
  - [Credibility factor](#credibility-factor)
  - [Variance of hypothetical means](#variance-of-hypothetical-means)
  - [Expected process variance](#expected-process-variance)
- [Classical risk model](#classical-risk-model)
  - [Finite-claim ruin probability](#finite-claim-ruin-probability)
  - [Maximum aggregate loss in a classical risk model](#maximum-aggregate-loss-in-a-classical-risk-model)
  - [Equilibrium claim-size distribution](#equilibrium-claim-size-distribution)
    - [New better than used in expectation](#new-better-than-used-in-expectation)
      - [Adjustment-coefficient lower bound for NBUE claims](#adjustment-coefficient-lower-bound-for-nbue-claims)
  - [Ultimate ruin probability](#ultimate-ruin-probability)
    - [Ultimate ruin with exponential claims](#ultimate-ruin-with-exponential-claims)
    - [Ruin integro-differential equation](#ruin-integro-differential-equation)
      - [Two-exponential-mixture survival probability](#two-exponential-mixture-survival-probability)
  - [Certain ruin with nonpositive loading and finite claim variance](#certain-ruin-with-nonpositive-loading-and-finite-claim-variance)
  - [Survival probability under risk pooling](#survival-probability-under-risk-pooling)
  - [Survival renewal equation for a classical risk model](#survival-renewal-equation-for-a-classical-risk-model)
    - [Survival integro-differential equation for a classical risk model](#survival-integro-differential-equation-for-a-classical-risk-model)
      - [Erlang claim-size differential equation for survival probability](#erlang-claim-size-differential-equation-for-survival-probability)
      - [Exponential-mixture differential equation for survival probability](#exponential-mixture-differential-equation-for-survival-probability)
    - [First-claim decomposition for survival probability](#first-claim-decomposition-for-survival-probability)
  - [Zero-capital survival probability](#zero-capital-survival-probability)
  - [Adjustment coefficient](#adjustment-coefficient)
    - [Adjustment coefficient for shape-one-half gamma claims](#adjustment-coefficient-for-shape-one-half-gamma-claims)
      - [Exponential misspecification of shape-one-half gamma claims](#exponential-misspecification-of-shape-one-half-gamma-claims)
    - [Polynomial moment bounds for the adjustment coefficient](#polynomial-moment-bounds-for-the-adjustment-coefficient)
    - [Deterministic claims maximize the adjustment coefficient at fixed mean and loading](#deterministic-claims-maximize-the-adjustment-coefficient-at-fixed-mean-and-loading)
    - [Adjustment coefficient for shape-two Erlang claims](#adjustment-coefficient-for-shape-two-erlang-claims)
    - [Adjustment coefficient with independent claim expenses](#adjustment-coefficient-with-independent-claim-expenses)
    - [Secant-slope existence criterion for an adjustment coefficient](#secant-slope-existence-criterion-for-an-adjustment-coefficient)
    - [Lundberg inequality](#lundberg-inequality)
      - [Exponential surplus martingale](#exponential-surplus-martingale)
      - [Cramér–Lundberg ruin asymptotic](#cramer-lundberg-ruin-asymptotic)
        - [Leading exponential term determines a ruin adjustment coefficient](#leading-exponential-term-determines-a-ruin-adjustment-coefficient)
        - [Interior adjustment coefficient ruin prefactor](#interior-adjustment-coefficient-ruin-prefactor)
          - [Erlang shape-two ruin prefactor](#erlang-shape-two-ruin-prefactor)
  - [Relative safety loading](#relative-safety-loading)
- [Reinsurance](#reinsurance)
  - [Reinsurance retention](#reinsurance-retention)
  - [Equal expected recoveries from excess of loss and stop loss](#equal-expected-recoveries-from-excess-of-loss-and-stop-loss)
  - [Excess of loss reinsurance](#excess-of-loss-reinsurance)
    - [Limited excess of loss reinsurance](#limited-excess-of-loss-reinsurance)
      - [Conditional lognormal layer recovery](#conditional-lognormal-layer-recovery)
        - [Claims inflation of a fixed reinsurance layer](#claims-inflation-of-a-fixed-reinsurance-layer)
    - [Total variance stationary condition for excess of loss](#total-variance-stationary-condition-for-excess-of-loss)
      - [Variance-minimizing retention for shape-three Pareto claims](#variance-minimizing-retention-for-shape-three-pareto-claims)
      - [Variance-minimizing exponential retention](#variance-minimizing-exponential-retention)
    - [Capped claim moments](#capped-claim-moments)
  - [Aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance)
    - [Retained stop loss moments for an exponential aggregate](#retained-stop-loss-moments-for-an-exponential-aggregate)
    - [Stop loss variance minimization principle](#stop-loss-variance-minimization-principle)
  - [Quota share reinsurance](#quota-share-reinsurance)
    - [Equal-loading quota share and vanishing retention](#equal-loading-quota-share-and-vanishing-retention)
    - [Quota-share retention under exponential utility](#quota-share-retention-under-exponential-utility)
    - [Quota share comparison at matched retained variance](#quota-share-comparison-at-matched-retained-variance)
    - [Variance-minimizing quota share split](#variance-minimizing-quota-share-split)
- [Aggregate claims model](#aggregate-claims-model)
  - [Insurance exposure](#insurance-exposure)
  - [Claim count](#claim-count)
  - [Claim size](#claim-size)
    - [Claims inflation](#claims-inflation)
  - [Heterogeneous individual claims model](#heterogeneous-individual-claims-model)
    - [Variance comparison for compound portfolio approximations](#variance-comparison-for-compound-portfolio-approximations)
  - [Claim count distribution](#claim-count-distribution)
    - [Panjer claim-count class](#panjer-claim-count-class)
      - [Panjer recursion](#panjer-recursion)
        - [Panjer recursion with zero severities](#panjer-recursion-with-zero-severities)
  - [Poisson superposition of insurance portfolios](#poisson-superposition-of-insurance-portfolios)
  - [Random sum of independent claims](#random-sum-of-independent-claims)
    - [Compound mixed Poisson distribution](#compound-mixed-poisson-distribution)
    - [Compound binomial distribution](#compound-binomial-distribution)
      - [Binomial accident portfolio with Poisson clusters](#binomial-accident-portfolio-with-poisson-clusters)
    - [Compound geometric distribution](#compound-geometric-distribution)
      - [Zero-based geometric sum of exponential variables](#zero-based-geometric-sum-of-exponential-variables)
    - [Negative-binomial sum of exponential claims](#negative-binomial-sum-of-exponential-claims)
      - [Finite Erlang-mixture tail for a negative-binomial exponential aggregate](#finite-erlang-mixture-tail-for-a-negative-binomial-exponential-aggregate)
    - [Random-sum transform identity](#random-sum-transform-identity)
      - [Cumulant composition for a random sum](#cumulant-composition-for-a-random-sum)
    - [Geometric-sum moment-generating function](#geometric-sum-moment-generating-function)
      - [Geometric sum of shape-two gamma variables](#geometric-sum-of-shape-two-gamma-variables)
    - [Compound Poisson distribution](#compound-poisson-distribution)
      - [Nested Poisson flood count](#nested-poisson-flood-count)
      - [Covariance of two components of a compound Poisson sum](#covariance-of-two-components-of-a-compound-poisson-sum)
      - [Zero claim sizes in a compound Poisson representation](#zero-claim-sizes-in-a-compound-poisson-representation)
      - [Compound Poisson cumulants](#compound-poisson-cumulants)
      - [Normal approximation to a compound Poisson aggregate](#normal-approximation-to-a-compound-poisson-aggregate)
      - [Three-cumulant shifted gamma approximation](#three-cumulant-shifted-gamma-approximation)
      - [Raw moment recursion for a compound Poisson distribution](#raw-moment-recursion-for-a-compound-poisson-distribution)
      - [Retained compound Poisson aggregate](#retained-compound-poisson-aggregate)
    - [Hurdle decomposition of a positive random sum](#hurdle-decomposition-of-a-positive-random-sum)
    - [Gamma-mixed Poisson aggregate with exponential claims](#gamma-mixed-poisson-aggregate-with-exponential-claims)

## No claims discount system

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

A policyholder's future insurance premiums depend on a finite discount level, updated according to whether a claim is submitted in each year. With independent yearly accidents and repair costs, and a claim decision depending only on the current level and cost, the level is a [discrete-time Markov chain](markov-process.md#discrete-time-markov-chain). Accident probability and submitted-claim probability differ when the policyholder pays small repair costs without claiming.

### Two-year no-claims threshold with reset to zero

↑ **Parent:** [No claims discount system](#no-claims-discount-system)

In a [no claims discount system](#no-claims-discount-system) with discounts $0,\alpha,\beta$, a reported claim resets next year's discount to zero. With no later accidents, the next two premiums after reporting are $C+(1-\alpha)C$. At the zero level, not reporting instead gives $(1-\alpha)C+(1-\beta)C$; at either other level it gives $2(1-\beta)C$. Their differences give the displayed repair-cost thresholds. A fully reimbursed loss above its threshold should be reported under this undiscounted two-year rule. Current premiums cancel. Different thresholds generally produce state-dependent submitted-claim probabilities, even with a common accident mechanism.

### Persistent claim intensity can destroy the discount Markov property

↑ **Parent:** [No claims discount system](#no-claims-discount-system)

Let a policyholder have one fixed [exponential distribution](continuous-probability-distribution.md#exponential-distribution) intensity $\Lambda$ of rate $\nu$, with conditionally independent annual [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) counts. Its one-year marginal count is geometric, but averaging that count does not make the discount process a [Markov chain](markov-process.md#markov-chain). In the three-level rule, start at zero discount. At time three, the histories $0,\alpha,\beta,\beta$ and $0,0,\alpha,\beta$ both end at the same top level. The first means three no-claim years, giving next no-claim probability $(\nu+3)/(\nu+4)$. The second means a positive count followed by two zero counts, giving $(\nu+2)/(\nu+4)$: divide the integrals of $(1-e^{-\lambda})e^{-(\nu+3)\lambda}$ and $(1-e^{-\lambda})e^{-(\nu+2)\lambda}$. These are distinct, so the [Markov property](markov-process.md#markov-property) fails when only the current discount is recorded. Conditioning on the intensity, or recording its [Bayesian posterior](statistical-inference.md#bayesian-posterior), restores the required predictive information.

### Three-level discount equilibrium with geometric annual counts

↑ **Parent:** [No claims discount system](#no-claims-discount-system)

Suppose annual [claim counts](#claim-count) are independent with [geometric distribution](discrete-probability-distribution.md#geometric-distribution) mass $pq^j$, $j\ge0$. In a [no claims discount system](#no-claims-discount-system) with discounts $0,\alpha,\beta$, a claim returns either of the first two levels to zero; at the top, one claim sends the level to $\alpha$ and two or more send it to zero. The [transition matrix](markov-process.md#stochastic-matrix) is $\bigl(\begin{smallmatrix}q&p&0\\q&0&p\\q^2&pq&p\end{smallmatrix}\bigr)$. Solving $\pi P=\pi$ gives the displayed [stationary distribution](markov-process.md#stationary-distribution). With full premium $c$, the stationary [expected value](probability-theory.md#expected-value) of the premium is $c[1-(\alpha pq+\beta p^2)/(1-p^2q)]$. Independent annual sampling is essential; a persistent random intensity does not justify this marginal transition matrix.

### Three-level no claims discount equilibrium

↑ **Parent:** [No claims discount system](#no-claims-discount-system)

For a three-level [birth-death chain](markov-process.md#birth-death-chain) whose down-or-stay claim probabilities are $p_1,p_2,p_3$, with each in $(0,1)$, [detailed balance](markov-process.md#detailed-balance) is $\pi_1(1-p_1)=\pi_2p_2$ and $\pi_2(1-p_2)=\pi_3p_3$. Normalizing gives the displayed [stationary distribution](markov-process.md#stationary-distribution). The finite chain is irreducible and has endpoint holding probabilities, so it is aperiodic and its level proportions converge to this distribution from any initial level.

### Two-year premium-loss claim threshold

↑ **Parent:** [No claims discount system](#no-claims-discount-system)

Let $b$ be the undiscounted annual premium and $d_i$ the discount fraction at level $i$. Compare the next two levels $i_r^0$ after no current claim with $i_r^1$ after a current claim, assuming no later accidents. Their total additional premium is the displayed threshold. A repair cost above it makes a claim advantageous under this two-year rule. For discounts $0,\alpha,\beta$ and one-level moves with reflecting endpoints, the thresholds at levels one, two, and three are respectively $b\beta$, $b(2\beta-\alpha)$, and $b(\beta-\alpha)$. The premium scale must be specified or fixed as the monetary unit.

#### Incremental second-claim threshold at the highest discount level

↑ **Parent:** [Two-year premium-loss claim threshold](#two-year-premium-loss-claim-threshold)

For a [no claims discount system](#no-claims-discount-system) with discounts $0,\alpha,\beta$, assume a policyholder starts at $\beta$, the first claim lowers next year's discount to $\alpha$, and a second claim in the same year lowers it to zero. With no further losses and undiscounted future premiums, claiming for the first loss costs $c(\beta-\alpha)$ in extra premium. Once that claim is submitted, the second claim adds $c\alpha$ next year and $c(\beta-\alpha)$ the year after, a total $c\beta$. Thus the second decision uses the incremental threshold, not the cost of both claims relative to no claim. For independent unit-rate [exponential distribution](continuous-probability-distribution.md#exponential-distribution) losses the probabilities are $e^{-c(\beta-\alpha)}$ and $e^{-c\beta}$, respectively; the latter remains the conditional probability given submission of the first claim.

## Expected value premium principle

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

The expected value principle prices a nonnegative insurance loss $L$ by its [expected value](probability-theory.md#expected-value) times one plus a positive loading. In the [classical risk model](#classical-risk-model), annual expected claim cost $\lambda\mu$ gives premium rate $(1+\theta)\lambda\mu$. Under [quota share reinsurance](#quota-share-reinsurance), the reinsurer prices its ceded fraction $(1-\alpha)S$ using its own loading, which need not equal the direct insurer's loading.

## Credibility estimate

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

A [credibility estimate](#credibility-estimate) combines a risk's individual experience with population information. In the basic equal-exposure form, the [credibility factor](#credibility-factor) $Z$ weights the observed [sample mean](variance.md#sample-mean), while $1-Z$ weights a prior or collective [expected value](probability-theory.md#expected-value). The [Bühlmann credibility premium](#buhlmann-credibility-premium) is the best affine estimate under [mean squared error](statistical-modelling.md#mean-squared-error); an exact [Bayesian posterior](statistical-inference.md#bayesian-posterior) mean can also have this form, as in the [natural conjugate credibility identity](exponential-family.md#natural-conjugate-credibility-identity).

### Bayesian credibility

↑ **Parent:** [Credibility estimate](#credibility-estimate)

Bayesian credibility estimates a risk's conditional mean by its [Bayesian posterior](statistical-inference.md#bayesian-posterior) expected value under [squared-error loss](statistical-inference.md#squared-error-loss). When that posterior mean is an affine combination of exposure-weighted individual experience and a prior mean, the coefficient of the experience is its [credibility factor](#credibility-factor). Exact Bayesian credibility is distinct from merely selecting the best affine estimator when the true posterior mean is nonlinear.

#### Normal-normal credibility

↑ **Parent:** [Bayesian credibility](#bayesian-credibility)

Conditionally independent [normal distribution](probability-theory.md#normal-distribution) observations of mean $\theta$ and known variance $\sigma_1^2$, with normal prior mean $\mu$ and variance $\sigma_2^2$, give [normal-normal conjugacy with known observation variance](probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance). Their [posterior mean](statistical-inference.md#posterior-mean) has the displayed exact [credibility estimate](#credibility-estimate) form. It minimizes posterior [squared-error loss](statistical-inference.md#squared-error-loss) and predicts the conditional mean of the next observation.

##### Normal-normal credibility with unequal exposures

↑ **Parent:** [Normal-normal credibility](#normal-normal-credibility)

For conditionally independent annual averages $X_j\mid\theta\sim N(\theta,v/m_j)$ and prior $\theta\sim N(\mu,\sigma^2)$, the [posterior mean](statistical-inference.md#posterior-mean) is $Z\overline X_w+(1-Z)\mu$, with $\overline X_w=\sum_jm_jX_j/W$. Completing the quadratic [likelihood](statistical-modelling.md#likelihood-function) gives posterior precision $\sigma^{-2}+W/v$. This is an exact [Bayesian credibility](#bayesian-credibility) version of the [Bühlmann–Straub credibility estimate](#buhlmann-straub-credibility-estimate). Increasing the between-risk prior variance increases the experience weight; increasing process variance decreases it. The next total pure premium is $m_{n+1}$ times the estimated per-life mean.

#### Inflation-adjusted Poisson-gamma credibility

↑ **Parent:** [Bayesian credibility](#bayesian-credibility)

For a common [gamma distribution](continuous-probability-distribution.md#gamma-distribution) (shape $\alpha$, rate $\beta$) frequency [prior distribution](statistical-inference.md#prior-probability) and conditionally [independent](random-variable.md#independent-random-variables) [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) yearly counts of means $w_j\Theta$, observed average amounts $y_j$ determine counts $k_j=w_jy_j/c_j$. The [posterior distribution](statistical-inference.md#bayesian-posterior) shape is $\alpha+\sum_jk_j$ and rate is $\beta+\sum_jw_j$. The future per-policy [mean](probability-theory.md#expected-value) is the display, equal to [credibility factor](#credibility-factor) $W/(W+\beta)$ times $\sum_j(w_j/W)(c_{n+1}/c_j)y_j$ plus the complementary weight times $c_{n+1}\alpha/\beta$. The data must lie on their count lattice; impossible noninteger recovered counts have zero [likelihood](statistical-modelling.md#likelihood-function).

// Destination: probability-theory.bigb

#### Exact beta-binomial credibility with unequal exposures

↑ **Parent:** [Bayesian credibility](#bayesian-credibility)

For a common success chance with beta prior and conditionally independent binomial observations of sizes $m_i$, put $M=\sum_i m_i$ and $s=\sum_i x_i$. [Beta-binomial conjugacy](statistical-inference.md#beta-binomial-conjugacy) gives posterior mean $(\alpha+s)/(\alpha+\beta+M)$, equal to $Z(s/M)+(1-Z)\alpha/(\alpha+\beta)$. Multiplying by the next exposure predicts its expected count. The factor tends to one as exposure increases and to zero as prior concentration increases at fixed prior mean.

<h2 id="buhlmann-model">Bühlmann model</h2>

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

Given a latent risk parameter $\Theta$, observations are [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with [conditional expectation](measure-theory.md#conditional-expectation) $m(\Theta)$ and [conditional variance](variance.md#conditional-variance) $v(\Theta)$. The [Bühlmann credibility premium](#buhlmann-credibility-premium) estimates $m(\Theta)$ by an affine function of past observations under [mean squared error](statistical-modelling.md#mean-squared-error). Its population parameters are $m=\mathbb Em(\Theta)$, [expected process variance](#expected-process-variance) $v=\mathbb Ev(\Theta)$, and [variance of hypothetical means](#variance-of-hypothetical-means) $a=\operatorname{Var}(m(\Theta))$.

<h3 id="buhlmann-straub-model">Bühlmann–Straub model</h3>

↑ **Parent:** [Bühlmann model](#buhlmann-model)

Conditional on a common [latent variable](statistical-modelling.md#latent-variable) $\Theta$, annual averages $X_j$ are independent, have common [conditional expectation](measure-theory.md#conditional-expectation) $\mu(\Theta)$, and have [conditional variance](variance.md#conditional-variance) $\sigma^2(\Theta)/m_j$ for known positive exposures $m_j$. Its structural parameters are $m_0=\mathbb E\mu(\Theta)$, [expected process variance](#expected-process-variance) $v=\mathbb E\sigma^2(\Theta)$ and [variance of hypothetical means](#variance-of-hypothetical-means) $a=\operatorname{Var}(\mu(\Theta))$. It generalizes the equal-exposure [Bühlmann model](#buhlmann-model).

<h4 id="buhlmann-straub-credibility-estimate">Bühlmann–Straub credibility estimate</h4>

↑ **Parent:** [Bühlmann–Straub model](#buhlmann-straub-model)

For total exposure $W=\sum_jm_j$ and weighted average $\overline X_w=\sum_jm_jX_j/W$, the best affine [mean squared error](statistical-modelling.md#mean-squared-error) estimate of the conditional mean is $Z\overline X_w+(1-Z)m_0$, where $Z=Wa/(Wa+v)$. If the coefficients sum to $B$, their error is $a(1-B)^2+v\sum_jb_j^2/m_j$. [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) minimizes the latter term at $b_j=B m_j/W$, and a one-dimensional quadratic minimization then gives $B=Z$.

<h5 id="exact-buhlmann-straub-credibility-for-poisson-gamma-counts">Exact Bühlmann–Straub credibility for Poisson-gamma counts</h5>

↑ **Parent:** [Bühlmann–Straub credibility estimate](#buhlmann-straub-credibility-estimate)

With a [Poisson-gamma conjugacy with unequal exposures](statistical-inference.md#poisson-gamma-conjugacy-with-unequal-exposures) model, $m_0=v=\alpha/\beta$ and $a=\alpha/\beta^2$, so the [Bühlmann–Straub credibility factor](#buhlmann-straub-credibility-factor) is $W/(W+\beta)$. The credibility estimate simplifies to $(\alpha+\sum_jY_j)/(\beta+W)$, exactly the [posterior mean](statistical-inference.md#posterior-mean) and hence the [Bayes estimator under squared error loss](statistical-inference.md#bayes-estimator-under-squared-error-loss). The agreement is exact because that posterior mean is already affine in the exposure-weighted data.

<h5 id="buhlmann-straub-credibility-factor">Bühlmann–Straub credibility factor</h5>

↑ **Parent:** [Bühlmann–Straub credibility estimate](#buhlmann-straub-credibility-estimate)

The experience weight is $Z=Wa/(Wa+v)$, where $W$ is total observed exposure, $a$ the [variance of hypothetical means](#variance-of-hypothetical-means), and $v$ the [expected process variance](#expected-process-variance). With positive $a$, it is $W/(W+v/a)$. More exposure raises the weight; larger process noise lowers it. If $a=0$, the unknown conditional mean is constant and one can set $Z=0$.

<h3 id="buhlmann-credibility-premium">Bühlmann credibility premium</h3>

↑ **Parent:** [Bühlmann model](#buhlmann-model)

The Bühlmann credibility premium is the best affine [mean squared error](statistical-modelling.md#mean-squared-error) estimate of a risk’s conditional claim [expected value](probability-theory.md#expected-value). In the [Bühlmann model](#buhlmann-model) it is $Z\overline X+(1-Z)m$, where $Z=na/(na+v)$. The [linear least-squares projection](probability-and-statistics.md#linear-least-squares-projection) equations use $\operatorname{Var}(X_j)=a+v$ and $\operatorname{Cov}(X_i,X_j)=a$ for distinct years.

#### Balanced-panel method-of-moments credibility

↑ **Parent:** [Bühlmann credibility premium](#buhlmann-credibility-premium)

For independent comparable risks observed over $n\ge2$ years, estimate the [expected process variance](#expected-process-variance) $v$ by the average within-risk sample variance. The sample variance $B$ of the risk means estimates $a+v/n$, where $a$ is the [variance of hypothetical means](#variance-of-hypothetical-means). Thus $B-\widehat v/n$ is unbiased for $a$; truncating at zero produces a practical nonnegative estimate but introduces bias. Use the grand mean for $m$ and plug these estimates into the [Bühlmann credibility premium](#buhlmann-credibility-premium) $\widehat Z\overline X_s+(1-\widehat Z)\widehat m$. At least two risks are needed for $B$; a single year cannot estimate within-risk variance this way.

#### Poisson credibility with a shape-three Pareto intensity

↑ **Parent:** [Bühlmann credibility premium](#buhlmann-credibility-premium)

Let a fixed policy intensity have [prior density](statistical-inference.md#prior-density) $3\theta^{-4}$ on $\theta>1$, and let $n$ annual [claim counts](#claim-count) be conditionally independent with [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) mean $\theta$. The [expected process variance](#expected-process-variance) is $3/2$ and the [variance of hypothetical means](#variance-of-hypothetical-means) is $3/4$, so the [Bühlmann credibility factor](#credibility-factor) is $n/(n+2)$. A total count $k$ gives the displayed [credibility premium](#credibility-estimate). By contrast, the [Bayesian posterior](statistical-inference.md#bayesian-posterior) density is proportional to $\theta^{k-4}e^{-n\theta}$ on $\theta>1$. Its mean is the ratio $\int_1^\infty\theta^{k-3}e^{-n\theta}\,d\theta/\int_1^\infty\theta^{k-4}e^{-n\theta}\,d\theta$. For $n=2,k=5$, that [Bayesian credibility](#bayesian-credibility) estimate is $5/3$, whereas the affine estimate is $2$.

<h4 id="buhlmann-credibility-for-inverse-gamma-observations">Bühlmann credibility for inverse-gamma observations</h4>

↑ **Parent:** [Bühlmann credibility premium](#buhlmann-credibility-premium)

In the [Gamma prior for an inverse-gamma scale](continuous-probability-distribution.md#gamma-prior-for-an-inverse-gamma-scale) model, assume $k>2$. The [variance of hypothetical means](#variance-of-hypothetical-means) is $a=\alpha/[\lambda^2(k-1)^2]$, and the [expected process variance](#expected-process-variance) is $v=\alpha(\alpha+1)/[\lambda^2(k-1)^2(k-2)]$. The [Bühlmann credibility factor](#credibility-factor) is $Z=n/(n+v/a)$, giving the displayed expression. The optimal affine [credibility estimate](#credibility-estimate) is $(1-Z)\alpha/[\lambda(k-1)]+Z\overline X$. Its fixed-weight arithmetic-mean form differs from the reciprocal-based [posterior mean](statistical-inference.md#posterior-mean).

<h4 id="sequential-buhlmann-credibility-update">Sequential Bühlmann credibility update</h4>

↑ **Parent:** [Bühlmann credibility premium](#buhlmann-credibility-premium)

With fixed structural parameters and $K=v/a$, the [Bühlmann credibility estimate](#buhlmann-credibility-premium) has form $(\sum_{i=1}^nx_i+Km_0)/(n+K)$. The next observation updates it by the displayed rule. Consequently the estimate decreases exactly when the new observation is less than the previous credibility estimate, with strict equality handled separately.

### Credibility factor

↑ **Parent:** [Bühlmann model](#buhlmann-model)

The credibility factor in the [Bühlmann model](#buhlmann-model) is the weight $Z=na/(na+v)$ placed on the [sample mean](variance.md#sample-mean) after $n$ observations. The remaining weight is placed on the population [expected value](probability-theory.md#expected-value). More experience or larger [variance of hypothetical means](#variance-of-hypothetical-means) increases $Z$; larger [expected process variance](#expected-process-variance) decreases it.

### Variance of hypothetical means

↑ **Parent:** [Bühlmann model](#buhlmann-model)

The variance of hypothetical means in the [Bühlmann model](#buhlmann-model) is the between-risk [variance](variance.md) of the conditional claim [expected value](probability-theory.md#expected-value). It creates the shared [covariance](variance.md#covariance) $a$ between different years of the same risk and determines how much individual experience should influence the premium.

### Expected process variance

↑ **Parent:** [Bühlmann model](#buhlmann-model)

The expected process variance in the [Bühlmann model](#buhlmann-model) averages within-risk [conditional variance](variance.md#conditional-variance) over the population of risks. It measures variation that repeated observations can average out and contributes $v/n$ to the [variance](variance.md) of the [sample mean](variance.md#sample-mean).

## Classical risk model

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

The classical risk model has surplus $U_t=u+ct-\sum_{j=1}^{N_t}X_j$, where $N_t$ is a [Poisson process](probability-theory.md#poisson-process) of rate $\lambda$, independent claim sizes are positive, and premiums flow in at constant rate $c$. The [relative safety loading](#relative-safety-loading) is $\rho=c/(\lambda\mathbb EX_1)-1$. Ruin is the first time surplus becomes negative.

### Finite-claim ruin probability

↑ **Parent:** [Classical risk model](#classical-risk-model)

In a [classical risk model](#classical-risk-model), $T_j$ is the time of the $j$th claim. The displayed probability restricts ruin to the first $n$ claims and increases to the [ultimate ruin probability](#ultimate-ruin-probability). Conditioning on the first arrival and severity gives $\psi_{n+1}(u)=\mathbb E[\overline F_X(u+cT_1)+\int_0^{u+cT_1}\psi_n(u+cT_1-x)f_X(x)\,dx]$, with $\psi_0=0$. For [exponential distribution](continuous-probability-distribution.md#exponential-distribution) claims of mean $\mu$ and [relative safety loading](#relative-safety-loading) $\rho$, put $d=1+\rho$ and $h=d+1$. Then $\psi_1(u)=e^{-u/\mu}/h$ and $\psi_2(u)=e^{-u/\mu}(h^{-1}+(u/\mu)h^{-2}+dh^{-3})$. The recursion follows because a surviving first claim leaves fresh independent future arrivals and claims. The formulas follow by integrating the rate-$\lambda$ first-arrival density; the claim-arrival rate cancels with $c=d\lambda\mu$.

### Maximum aggregate loss in a classical risk model

↑ **Parent:** [Classical risk model](#classical-risk-model)

Starting from capital $u$, ruin occurs exactly when the aggregate loss exceeds $u$. Positive [relative safety loading](#relative-safety-loading) and the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) make $S(t)-ct$ tend to minus infinity, so its supremum is finite almost surely. For [exponential distribution](continuous-probability-distribution.md#exponential-distribution) claims of rate $\alpha$, $L$ has an atom $1-\lambda/(\alpha c)$ at zero, and, conditional on $L>0$, has [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate $\alpha-\lambda/c$. The [ultimate ruin probability](#ultimate-ruin-probability) determines this mixture directly.

### Equilibrium claim-size distribution

↑ **Parent:** [Classical risk model](#classical-risk-model)

For a nonnegative claim size $X$ of finite positive mean $\mu$, its equilibrium claim-size distribution has this density and survival function $\overline F_I(x)=\mu^{-1}\int_x^\infty\overline F_X(t)\,dt$. The [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments) normalizes the density. Its [moment-generating function](probability-theory.md#moment-generating-function) is $(M_X(r)-1)/(\mu r)$ wherever finite, so at an [adjustment coefficient](#adjustment-coefficient) it equals one plus the safety loading.

#### New better than used in expectation

↑ **Parent:** [Equilibrium claim-size distribution](#equilibrium-claim-size-distribution)

A nonnegative lifetime or claim law is new better than used in expectation if its [mean residual life](survival-analysis.md#mean-residual-life) at every age with positive survival is at most its original mean. The displayed equivalent inequality says that its [equilibrium claim-size distribution](#equilibrium-claim-size-distribution) is no larger in [stochastic order](convergence-of-random-variables.md#stochastic-order) than the original law. For an [Erlang distribution](continuous-probability-distribution.md#erlang-distribution) of shape two and rate one, the two survival functions are $(1+x/2)e^{-x}$ and $(1+x)e^{-x}$, so the condition holds.

##### Adjustment-coefficient lower bound for NBUE claims

↑ **Parent:** [New better than used in expectation](#new-better-than-used-in-expectation)

For [NBUE](#new-better-than-used-in-expectation) claims in the [classical risk model](#classical-risk-model), the equilibrium claim size $Y$ is stochastically bounded by $X$. The positive exponential [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments) gives $M_Y(R)\le M_X(R)$. Since $M_Y(R)=1+\theta$ and $M_X(R)=1+(1+\theta)\mu R$, rearrangement proves the displayed bound.

### Ultimate ruin probability

↑ **Parent:** [Classical risk model](#classical-risk-model)

The probability that the insurance surplus in a [classical risk model](#classical-risk-model) becomes negative at some finite time, starting from capital $u\ge0$. Ultimate survival has probability $1-\psi(u)$. A finite-horizon ruin probability instead restricts the crossing time to a specified time interval.

#### Ultimate ruin with exponential claims

↑ **Parent:** [Ultimate ruin probability](#ultimate-ruin-probability)

For rate-$\alpha$ [exponential distribution](continuous-probability-distribution.md#exponential-distribution) claims and $c>\lambda/\alpha$, the [ruin integro-differential equation](#ruin-integro-differential-equation) reduces to $\psi''+(\alpha-\lambda/c)\psi'=0$. Differentiate the convolution and use its equation $A'=\alpha\psi-\alpha A$ to eliminate it. Positive [relative safety loading](#relative-safety-loading) implies $\psi(u)\to0$ as $u\to\infty$, and the [zero-capital survival probability](#zero-capital-survival-probability) gives $\psi(0)=\lambda/(\alpha c)$. These two conditions determine the displayed solution. The [adjustment coefficient](#adjustment-coefficient) is $\alpha-\lambda/c$.

#### Ruin integro-differential equation

↑ **Parent:** [Ultimate ruin probability](#ultimate-ruin-probability)

In the [classical risk model](#classical-risk-model), condition on the first arrival of the [Poisson process](probability-theory.md#poisson-process). If available capital just before it is $v$, ruin has probability $\overline F_X(v)+\int_0^v f_X(x)\psi(v-x)\,dx$. Integrate this expression at $v=u+ct$ against $\lambda e^{-\lambda t}$ and change variables from $t$ to $v$. Differentiating the lower limit gives the displayed equation. The claim-density [convolution](fourier-analysis.md#convolution) is continuous for bounded $\psi$, so the first-arrival representation also supplies the differentiability required by the equation.

##### Two-exponential-mixture survival probability

↑ **Parent:** [Ruin integro-differential equation](#ruin-integro-differential-equation)

In the [classical risk model](#classical-risk-model) with density $3e^{-4x}+e^{-2x}/2$ and [relative safety loading](#relative-safety-loading) $3/5$, the claim mean is $5/16$ and $\lambda/c=2$. The convolution terms $A_a(u)=\int_0^u\phi(u-x)e^{-ax}\,dx$ satisfy $A_a'=\phi-aA_a$. Applying $(D+4)(D+2)$ to $\phi'=2\phi-6A_4-A_2$ yields $\phi^{(3)}+4\phi''+3\phi'=0$. Its solution is fixed by $\phi(\infty)=1$, $\phi(0)=3/8$ and $\phi'(0)=3/4$, giving the displayed probability. The derivative condition comes from the original integral equation and excludes spurious solutions of the higher-order equation.

### Certain ruin with nonpositive loading and finite claim variance

↑ **Parent:** [Classical risk model](#classical-risk-model)

For positive claims with finite variance and $c\le\lambda\mu$, the [classical risk model](#classical-risk-model) has ruin probability one from any finite capital. At claim times, surplus increments are independent copies of $cT-X$ with mean $c/\lambda-\mu$. Negative mean sends their partial sums to minus infinity by the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers). At zero mean, the increments have finite nonzero variance. For every fixed $K$, the [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) gives limiting probability $1/2$ of a partial sum below $-K$. The probability of unboundedness below is therefore at least $1/2$; as a tail event it has probability zero or one by the [Kolmogorov zero-one law](probability-theory.md#kolmogorov-s-zero-one-law), and hence one.

### Survival probability under risk pooling

↑ **Parent:** [Classical risk model](#classical-risk-model)

Independent positively loaded portfolios with zero initial capitals have separate joint survival probability $\prod_i(1-\lambda_i\mu_i/c_i)$. Pool their claims and premium incomes to obtain zero-capital merged survival $1-(\sum_i\lambda_i\mu_i)/(\sum_i c_i)$. This is the premium-weighted average of the individual survival probabilities and is at least their product. The event of aggregate solvency permits transfers of surplus between the original portfolios.

### Survival renewal equation for a classical risk model

↑ **Parent:** [Classical risk model](#classical-risk-model)

The ultimate [survival probability](markov-process.md#survival-probability) satisfies $\varphi(u)=\varphi(0)+(\lambda/c)\int_0^u\varphi(u-x)(1-F(x))\,dx$. Condition on the first arrival of the [Poisson process](probability-theory.md#poisson-process), differentiate the resulting exponentially weighted integral, and integrate the convolution derivative equation from zero. [Tonelli theorem](measure-theory.md#tonelli-theorem) converts the claim-density convolution to the tail convolution. The kernel mass is $\lambda\mu/c<1$, so this is a [defective renewal equation](probability-theory.md#defective-renewal-equation).

#### Survival integro-differential equation for a classical risk model

↑ **Parent:** [Survival renewal equation for a classical risk model](#survival-renewal-equation-for-a-classical-risk-model)

In the [classical risk model](#classical-risk-model) with premium rate $c>0$ and claim [Poisson process](probability-theory.md#poisson-process) rate $\lambda$, the [first-claim decomposition for survival probability](#first-claim-decomposition-for-survival-probability) implies the displayed equation for ultimate [survival probability](markov-process.md#survival-probability). Change the first-claim integral to an integral over available capital and differentiate its lower limit. The bounded [survival probability](markov-process.md#survival-probability) function convolved with the integrable claim [probability density function](continuous-probability-distribution.md#probability-density-function) is continuous, so this also establishes the needed differentiability. In particular $\varphi'(0)=(\lambda/c)\varphi(0)$.

##### Erlang claim-size differential equation for survival probability

↑ **Parent:** [Survival integro-differential equation for a classical risk model](#survival-integro-differential-equation-for-a-classical-risk-model)

For an [Erlang distribution](continuous-probability-distribution.md#erlang-distribution) claim density $f(x)=\beta^2xe^{-\beta x}$ and $r=\lambda/c$, write $H=\phi*f$. The [survival integro-differential equation](#survival-integro-differential-equation-for-a-classical-risk-model) gives $\phi'=r(\phi-H)$. The convolution satisfies $(D+\beta)^2H=\beta^2\phi$, because $H=\beta^2e^{-\beta u}\int_0^u(u-t)\phi(t)e^{\beta t}dt$. Applying $(D+\beta)^2$ to the first equation eliminates $H$ and gives the displayed third-order equation. The original integral equation also supplies $\phi'(0)=r\phi(0)$ and $\phi''(0)=r^2\phi(0)$; these conditions must not be lost when solving the higher-order equation.

##### Exponential-mixture differential equation for survival probability

↑ **Parent:** [Survival integro-differential equation for a classical risk model](#survival-integro-differential-equation-for-a-classical-risk-model)

For a [mixture distribution](probability-theory.md#mixture-distribution) of [exponential distributions](continuous-probability-distribution.md#exponential-distribution), introduce one [convolution](fourier-analysis.md#convolution) state $A_j(u)=\int_0^u\varphi(z)e^{-\beta_j(u-z)}\,dz$ for each rate $\beta_j$. It satisfies $A_j'=\varphi-\beta_jA_j$. Together with the [survival integro-differential equation](#survival-integro-differential-equation-for-a-classical-risk-model) these form a constant-coefficient first-order system; applying the differential operators $D+\beta_j$ eliminates the [convolution](fourier-analysis.md#convolution) states. For equal mixing weights at rates one and one half, with $r=\lambda/c$, the result is $\varphi'''+(3/2-r)\varphi''+(1/2-3r/4)\varphi'=0$. The original integral equation supplies initial conditions lost in elimination.

#### First-claim decomposition for survival probability

↑ **Parent:** [Survival renewal equation for a classical risk model](#survival-renewal-equation-for-a-classical-risk-model)

In a [classical risk model](#classical-risk-model), before the first claim at time $t$, available capital is $u+ct$. A claim of size $x\le u+ct$ leaves future survival probability $\varphi(u+ct-x)$ by the [Markov property](markov-process.md#markov-property). Integrating over the independent first-arrival [exponential distribution](continuous-probability-distribution.md#exponential-distribution) and claim density gives $\varphi(u)=\int_0^\infty\lambda e^{-\lambda t}\int_0^{u+ct}\varphi(u+ct-x)f(x)\,dx\,dt$.

### Zero-capital survival probability

↑ **Parent:** [Classical risk model](#classical-risk-model)

In a [classical risk model](#classical-risk-model) with positive [relative safety loading](#relative-safety-loading), zero initial capital has ultimate [survival probability](markov-process.md#survival-probability) $1-\lambda\mu/c$, where $\lambda$ is the claim-arrival rate, $\mu$ the claim [expected value](probability-theory.md#expected-value) and $c$ the premium rate. It depends on the claim law through its mean alone. It is not the event of never receiving a claim: premium accumulates between arrivals.

### Adjustment coefficient

↑ **Parent:** [Classical risk model](#classical-risk-model)

The adjustment coefficient is a positive root of $\lambda(M_X(r)-1)=cr$ in the [classical risk model](#classical-risk-model). When the [moment-generating function](probability-theory.md#moment-generating-function) is finite at $R$, the process $\exp(R[\sum_{j=1}^{N_t}X_j-ct])$ is a [continuous-time martingale](martingale.md#continuous-time-martingale). It yields the [Lundberg inequality](#lundberg-inequality) and, under the relevant tilted integrability, the [Cramér–Lundberg ruin asymptotic](#cramer-lundberg-ruin-asymptotic).

#### Adjustment coefficient for shape-one-half gamma claims

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

The [gamma distribution](continuous-probability-distribution.md#gamma-distribution) of shape one half and rate $\beta$ has [moment-generating function](probability-theory.md#moment-generating-function) $(1-r/\beta)^{-1/2}$. With mean $\mu=1/(2\beta)$ and positive [relative safety loading](#relative-safety-loading) $\rho$, write $x=R/\beta$. Dividing out the zero root after squaring the adjustment equation gives $(1+\rho)^2x^2-(1+\rho)(\rho-3)x-4\rho=0$. Its unique positive root lies between zero and one, so it belongs to the transform domain and gives the display.

##### Exponential misspecification of shape-one-half gamma claims

↑ **Parent:** [Adjustment coefficient for shape-one-half gamma claims](#adjustment-coefficient-for-shape-one-half-gamma-claims)

Replacing a shape-one-half gamma claim law by an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) with the same mean overestimates the [adjustment coefficient](#adjustment-coefficient). Indeed $R_I-R=\beta[3(1+\rho)-\sqrt{(\rho+9)(\rho+1)}]/[2(1+\rho)]>0$ because the difference of the squared terms is $8\rho(1+\rho)$. The resulting putative [Lundberg inequality](#lundberg-inequality) bound $e^{-R_Iu}$ is smaller than the valid true-model bound $e^{-Ru}$ for $u>0$; the former is not justified for the true claim law. The true variance is twice the assumed variance, and its exponential tail decays more slowly.

#### Polynomial moment bounds for the adjustment coefficient

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

For positive claims with a finite positive [moment-generating function](probability-theory.md#moment-generating-function) neighbourhood, use $e^u>1+u+u^2/2$ and $e^u>1+u+u^2/2+u^3/6$ for $u>0$ in the defining [adjustment coefficient](#adjustment-coefficient) equation. They imply the displayed strict [upper bounds](set.md#upper-bound-in-a-partially-ordered-set), where $r_2$ is the positive quadratic root. Its defining [polynomial](polynomial.md) is negative at zero and positive at $r_1$, proving $r_2<r_1$. Higher exponential-series truncations similarly yield [upper bounds](set.md#upper-bound-in-a-partially-ordered-set) from more raw [moments](probability-theory.md#moment).

#### Deterministic claims maximize the adjustment coefficient at fixed mean and loading

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

Fix positive claim [expected value](probability-theory.md#expected-value) $\mu$ and [relative safety loading](#relative-safety-loading) $\theta>0$ in a [classical risk model](#classical-risk-model). Assume the random claim law has an [adjustment coefficient](#adjustment-coefficient) $R_X>0$. By [Jensen inequality](real-analysis.md#jensen-s-inequality), $M_X(r)\ge e^{\mu r}$. Thus $e^{\mu R_X}-1-(1+\theta)\mu R_X\le0$. The expression on the left is strictly [convex](real-analysis.md#convex-function), has negative derivative at zero and tends to infinity, so its unique positive zero $R_\mu$ satisfies $R_X\le R_\mu$. If the claim size is not almost surely constant, strict [Jensen inequality](real-analysis.md#jensen-s-inequality) gives $R_X<R_\mu$. Consequently the [Lundberg inequality](#lundberg-inequality) upper bound $e^{-R_\mu u}$ for deterministic claims is smaller for $u>0$. Comparing these upper bounds alone does not establish an ordering of actual [ultimate ruin probabilities](#ultimate-ruin-probability).

#### Adjustment coefficient for shape-two Erlang claims

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

For an [Erlang distribution](continuous-probability-distribution.md#erlang-distribution) of shape two and rate $2/\beta$, the claim [expected value](probability-theory.md#expected-value) is $\beta$ and its [moment-generating function](probability-theory.md#moment-generating-function) is $(1-\beta r/2)^{-2}$ for $r<2/\beta$. The [adjustment coefficient](#adjustment-coefficient) equation is $\lambda[(1-\beta R/2)^{-2}-1]=cR$. With $z=\beta R/2$, divide out the zero root to get $k(1-z)^2=2-z$. The smaller quadratic root lies in $(0,1)$ when $c>\lambda\beta$; the larger root lies beyond the finite-transform domain and must be rejected. This proves the displayed coefficient.

#### Adjustment coefficient with independent claim expenses

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

If each claim includes an independent expense $A$, replace its payment law by the [convolution of independent random variables](probability-theory.md#convolution-of-independent-random-variables) $X+A$. Its [moment-generating function](probability-theory.md#moment-generating-function) is $M_X(r)M_A(r)$ and its [expected value](probability-theory.md#expected-value) is $\mathbb EX+\mathbb EA$. Keeping the [relative safety loading](#relative-safety-loading) $\theta$ fixed therefore changes the premium rate as well. The new coefficient solves $M_X(R)M_A(R)-1=(1+\theta)(\mathbb EX+\mathbb EA)R$, within the common finite-transform domain.

#### Secant-slope existence criterion for an adjustment coefficient

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

For positive claims with finite nonzero [expected value](probability-theory.md#expected-value) $\mu$, the function $(M_X(r)-1)/r$ is continuous and strictly increasing on the positive finite-transform domain, starting at $\mu$. If $M_X$ diverges at a finite upper endpoint, or is finite for all positive arguments, the secant slope tends to infinity. In the latter case use $M_X(r)\ge\mathbb P(X\ge a)e^{ar}$ for some $a>0$ of positive tail probability. Every target $(1+\theta)\mu$ with positive [relative safety loading](#relative-safety-loading) therefore has exactly one positive root.

#### Lundberg inequality

↑ **Parent:** [Adjustment coefficient](#adjustment-coefficient)

For a [classical risk model](#classical-risk-model) with [adjustment coefficient](#adjustment-coefficient) $R>0$, the ultimate ruin probability from capital $u\geq0$ satisfies $\psi(u)\leq e^{-Ru}$. Stop the exponential [continuous-time martingale](martingale.md#continuous-time-martingale) at ruin or a finite horizon, bound its value on the ruin event, and then increase the horizon.

##### Exponential surplus martingale

↑ **Parent:** [Lundberg inequality](#lundberg-inequality)

In a [classical risk model](#classical-risk-model), an [adjustment coefficient](#adjustment-coefficient) $R$ makes $\lambda(M_X(R)-1)-cR=0$. The [random-sum transform identity](#random-sum-transform-identity) and [independent increments](stochastic-process.md#independent-increments) show that $\mathbb E[Z_t\mid\mathcal F_s]=Z_s$. This nonnegative [martingale](martingale.md) starts at one. At the ruin [stopping time](martingale.md#stopping-time) $\tau$, $Z_\tau>e^{Ru}$. Applying the [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) only to $\tau\wedge t$ yields $\mathbb P(\tau\le t)\le e^{-Ru}$; passage to increasing horizons proves the [Lundberg inequality](#lundberg-inequality) without an unjustified expectation identity at an unbounded stopping time.

<h5 id="cramer-lundberg-ruin-asymptotic">Cramér–Lundberg ruin asymptotic</h5>

↑ **Parent:** [Lundberg inequality](#lundberg-inequality)

In the [classical risk model](#classical-risk-model) with positive [relative safety loading](#relative-safety-loading) $\rho$ and [adjustment coefficient](#adjustment-coefficient) $R$, tilting the ruin [defective renewal equation](probability-theory.md#defective-renewal-equation) gives a proper [renewal equation](probability-theory.md#renewal-equation). The [key renewal theorem](probability-theory.md#key-renewal-theorem) yields $e^{Ru}\psi(u)\to \rho/[R\int_0^\infty xe^{Rx}f_I(x)\,dx]$. The constant is positive if the denominator is finite and zero if it is infinite; the claim-size density provides the nonarithmetic hypothesis.

###### Leading exponential term determines a ruin adjustment coefficient

↑ **Parent:** [Cramér–Lundberg ruin asymptotic](#cramer-lundberg-ruin-asymptotic)

If the [Cramér–Lundberg ruin asymptotic](#cramer-lundberg-ruin-asymptotic) has a finite positive constant, compare it with the leading nonzero term of a finite exponential representation. An [adjustment coefficient](#adjustment-coefficient) smaller than that term's decay rate would give limit zero; a larger coefficient would give infinity. Thus the two rates agree and the prefactor is the leading coefficient. Terms with zero coefficient are absent and do not determine a decay rate.

###### Interior adjustment coefficient ruin prefactor

↑ **Parent:** [Cramér–Lundberg ruin asymptotic](#cramer-lundberg-ruin-asymptotic)

When the [adjustment coefficient](#adjustment-coefficient) lies inside the finite domain of the claim [moment-generating function](probability-theory.md#moment-generating-function), the tilted kernel has finite mean $(\lambda M'(R)-c)/(cR)$. The forcing integral is $(c-\lambda\mu)/(cR)$. Their ratio is the constant $C$ in $\psi(u)\sim Ce^{-Ru}$, by the [key renewal theorem](probability-theory.md#key-renewal-theorem). An extra exponential moment controls the forcing tails and proves [direct Riemann integrability](real-analysis.md#direct-riemann-integrability).

###### Erlang shape-two ruin prefactor

↑ **Parent:** [Interior adjustment coefficient ruin prefactor](#interior-adjustment-coefficient-ruin-prefactor)

For unit-rate [Erlang distribution](continuous-probability-distribution.md#erlang-distribution) of shape two claims put $q=\lambda/c<1/2$. The [adjustment coefficient](#adjustment-coefficient) satisfies $q(2-R)=(1-R)^2$, so $1-R=(q+\sqrt{q^2+4q})/2$. In the interior-adjustment prefactor $(1-2q)/(2q(1-R)^{-3}-1)$, substituting $q=(1-R)^2/(2-R)$ gives the displayed expression. It is positive for $0<R<1$ and tends to one as the loading tends to zero.

### Relative safety loading

↑ **Parent:** [Classical risk model](#classical-risk-model)

If the expected claim outflow per unit time is $\lambda\mu$, the relative safety loading is $\rho=c/(\lambda\mu)-1$. Positive loading means expected premium income exceeds expected claim outflow. This is the net profit condition in the [classical risk model](#classical-risk-model).

## Reinsurance

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

Reinsurance transfers part of an insurer’s claim liability to another insurer. If aggregate claims are $S$, a retained payout $g(S)$ with $0\leq g(S)\leq S$ leaves the reinsurer with $S-g(S)$. [Quota share reinsurance](#quota-share-reinsurance) retains a fixed fraction, whereas [aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance) retains losses only up to a fixed aggregate threshold.

### Reinsurance retention

↑ **Parent:** [Reinsurance](#reinsurance)

A threshold limiting the insurer's retained payment under a [reinsurance](#reinsurance) contract. Under [excess of loss reinsurance](#excess-of-loss-reinsurance) it applies to each [claim size](#claim-size); under [aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance) it applies to the total loss over the stated period. These contracts therefore cap different quantities even when their thresholds have the same numerical value.

### Equal expected recoveries from excess of loss and stop loss

↑ **Parent:** [Reinsurance](#reinsurance)

For independent exponential claims of mean $\mu$ and a zero-based geometric count of parameter $p$, [excess of loss reinsurance](#excess-of-loss-reinsurance) at per-claim [reinsurance retention](#reinsurance-retention) $M$ has expected recovery $(1-p)\mu e^{-M/\mu}/p$. The [zero-based geometric sum of exponential variables](#zero-based-geometric-sum-of-exponential-variables) has tail $(1-p)e^{-px/\mu}$, so [aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance) at [reinsurance retention](#reinsurance-retention) $\widetilde M$ has expected recovery $(1-p)\mu e^{-p\widetilde M/\mu}/p$. Equating them gives the displayed [reinsurance retention](#reinsurance-retention) relation. This comparison concerns claim payouts, before any reinsurance premium is charged.

### Excess of loss reinsurance

↑ **Parent:** [Reinsurance](#reinsurance)

Per-claim [reinsurance](#reinsurance) under which the insurer retains each claim up to a level $M$ and the reinsurer pays its [positive part](function.md#positive-part-of-a-real-valued-function) $(x-M)_+$. The annual retained amount is a sum of capped claims, so it is generally different from the cap of the annual sum in [aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance).

#### Limited excess of loss reinsurance

↑ **Parent:** [Excess of loss reinsurance](#excess-of-loss-reinsurance)

A [reinsurance](#reinsurance) layer with attachment $M$ and payment limit $A$ pays nothing below $M$, the excess between $M$ and $M+A$, and $A$ above that. Its expected recovery is $\int_M^{M+A}\mathbb P(X>x)\,dx$, by the [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments). For continuous claims, conditioning on penetration of the layer divides this expectation by $\mathbb P(X>M)$.

##### Conditional lognormal layer recovery

↑ **Parent:** [Limited excess of loss reinsurance](#limited-excess-of-loss-reinsurance)

For a [lognormal distribution](probability-theory.md#log-normal-distribution), let $d_j(t)=(\log t-\mu-j\sigma^2)/\sigma$ for $j=0,1$. The [truncated lognormal moment](probability-theory.md#truncated-lognormal-moment) formula gives the recovery numerator

$$
e^{\mu+\sigma^2/2}[\Phi(d_1(M+A))-\Phi(d_1(M))]-M[\Phi(d_0(M+A))-\Phi(d_0(M))]+A[1-\Phi(d_0(M+A))].
$$

Divide by $1-\Phi(d_0(M))$ to condition on $X>M$. This handles both the partially penetrating claims and the capped payments beyond the upper attachment.

###### Claims inflation of a fixed reinsurance layer

↑ **Parent:** [Conditional lognormal layer recovery](#conditional-lognormal-layer-recovery)

For positive inflation factor $h$, $L_{M,A}(hX)=hL_{M/h,A/h}(X)$. The conditioning event also changes to $X>M/h$. If claims have a [lognormal distribution](probability-theory.md#log-normal-distribution), the same result follows by replacing their log-mean $\mu$ by $\mu+\log h$ and keeping the contractual attachment and limit fixed. Merely multiplying the original conditional mean by $h$ would hold those effective thresholds incorrectly fixed.

#### Total variance stationary condition for excess of loss

↑ **Parent:** [Excess of loss reinsurance](#excess-of-loss-reinsurance)

For positive claim sizes with finite [second moment](probability-theory.md#second-moment) in a [compound Poisson distribution](#compound-poisson-distribution) aggregate of parameter $\lambda$, the two [excess of loss reinsurance](#excess-of-loss-reinsurance) payouts are $\min(X,M)$ and $(X-M)_+$. The derivative of their total aggregate [variance](variance.md) is $2\lambda(M\overline F(M)-\mathbb E[(X-M)_+])$. Thus the displayed condition characterizes stationarity. When the tail probability is positive it says that the retention equals the [mean residual life](survival-analysis.md#mean-residual-life). Global minimality requires an additional sign or comparison argument.

##### Variance-minimizing retention for shape-three Pareto claims

↑ **Parent:** [Total variance stationary condition for excess of loss](#total-variance-stationary-condition-for-excess-of-loss)

For a [Pareto distribution](continuous-probability-distribution.md#pareto-distribution) of shape three and minimum $d>0$ with count rate $\lambda>0$, the sum of insurer and reinsurer aggregate [variances](variance.md) is $V(M)=\lambda(3d^2-3dM+2M^2)$ for $0\le M\le d$, and $\lambda(3d^2-d^3/M)$ for $M\ge d$. The first branch has its unique minimum at $3d/4$; the second is increasing. The branches agree in value and slope at $d$, giving the displayed global minimum. This criterion minimizes the sum of party [variances](variance.md); the total portfolio [variance](variance.md) includes their [covariance](variance.md#covariance) and remains $3\lambda d^2$.

##### Variance-minimizing exponential retention

↑ **Parent:** [Total variance stationary condition for excess of loss](#total-variance-stationary-condition-for-excess-of-loss)

For [exponential distribution](continuous-probability-distribution.md#exponential-distribution) claims of mean $\mu$ and [compound Poisson distribution](#compound-poisson-distribution) count parameter $\lambda$, the total party [variance](variance.md) under [excess of loss reinsurance](#excess-of-loss-reinsurance) is $g(M)=2\lambda\mu^2(1-(M/\mu)e^{-M/\mu})$. Its derivative is $2\lambda e^{-M/\mu}(M-\mu)$, so $M=\mu$ is the unique global minimum, with value $2\lambda\mu^2(1-e^{-1})$.

#### Capped claim moments

↑ **Parent:** [Excess of loss reinsurance](#excess-of-loss-reinsurance)

For a positive claim and $r>0$, the [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments) gives the displayed expression. In particular the first moment is $\int_0^M\overline F(x)\,dx$ and the raw second moment is $2\int_0^M x\overline F(x)\,dx$. If the claim law has a density, capping adds an [atom of a measure](measure-theory.md#atom-measure-theory) at $M$ with mass $\mathbb P(X\ge M)$.

### Aggregate stop loss reinsurance

↑ **Parent:** [Reinsurance](#reinsurance)

With aggregate retention $M\geq0$, the direct insurer pays $\min(S,M)$ and the reinsurer pays $(S-M)_+$, where $+$ denotes the [positive part](function.md#positive-part-of-a-real-valued-function). The threshold applies to the whole annual loss; applying a threshold to individual claims is a different contract.

#### Retained stop loss moments for an exponential aggregate

↑ **Parent:** [Aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance)

If $S$ has [exponential distribution](continuous-probability-distribution.md#exponential-distribution) with [expected value](probability-theory.md#expected-value) $\mu$, the [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments) gives $\mathbb E\min(S,M)=\mu(1-e^{-m})$ and $\operatorname{Var}(\min(S,M))=\mu^2(1-2me^{-m}-e^{-2m})$, where $m=M/\mu$. At matching retained [expected value](probability-theory.md#expected-value), the excess [variance](variance.md) under [quota share reinsurance](#quota-share-reinsurance) is $2\mu^2e^{-m}(m-1+e^{-m})\geq0$.

#### Stop loss variance minimization principle

↑ **Parent:** [Aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance)

Among retained payouts $g(S)$ with $0\leq g(x)\leq x$ and the same [expected value](probability-theory.md#expected-value) as $\min(S,M)$, [aggregate stop loss reinsurance](#aggregate-stop-loss-reinsurance) minimizes the [variance](variance.md). Pointwise $(g(x)-M)^2\geq(\min(x,M)-M)^2$, and subtracting the identical squared distance of their common [expected value](probability-theory.md#expected-value) from $M$ proves the claim. Equality requires equal payouts almost surely.

### Quota share reinsurance

↑ **Parent:** [Reinsurance](#reinsurance)

Quota share reinsurance retains a fixed proportion $\alpha\in[0,1]$ of each claim. The annual retained aggregate is $\alpha S$, whose [expected value](probability-theory.md#expected-value) and [variance](variance.md) are $\alpha\mathbb ES$ and $\alpha^2\operatorname{Var}(S)$.

#### Equal-loading quota share and vanishing retention

↑ **Parent:** [Quota share reinsurance](#quota-share-reinsurance)

If insurer and reinsurer use the same positive [relative safety loading](#relative-safety-loading) $\theta$, retained claim sizes and net premiums both scale by the retention $\alpha$: $X_\alpha=\alpha X$ and $c_\alpha=\alpha c$. Substitution into the [adjustment coefficient](#adjustment-coefficient) equation gives $R_\alpha=R_1/\alpha$. Thus there is no maximizing positive retention on $(0,1]$; the supremum is approached as $\alpha\downarrow0$. At full cession, if allowed, both retained claims and net premiums vanish, and the insurer's nonnegative capital remains constant. The coefficient is then not uniquely defined by the degenerate equation, although [ultimate ruin probability](#ultimate-ruin-probability) is zero in this idealized model.

#### Quota-share retention under exponential utility

↑ **Parent:** [Quota share reinsurance](#quota-share-reinsurance)

For independent [Poisson process](probability-theory.md#poisson-process) arrivals and [exponential distribution](continuous-probability-distribution.md#exponential-distribution) claim sizes of mean $\mu$, minimizing the logarithm of the negative expected [exponential utility](utility-function.md#constant-absolute-risk-aversion-utility) gives $H'(\alpha)=\lambda\beta\mu[(1-\beta\mu\alpha)^{-2}-(1+\theta_R)]$. Its strictly positive second derivative makes the displayed stationary point unique. On $0\le\alpha\le1$, the optimum is $\min(1,\alpha_*)$. On the strictly open interval $0<\alpha<1$, there is no maximizer when $\alpha_*\ge1$, only a supremum at full retention. The stationary retention increases with reinsurer loading and is independent of the direct insurer's loading.

#### Quota share comparison at matched retained variance

↑ **Parent:** [Quota share reinsurance](#quota-share-reinsurance)

Suppose $S=S_I+S_R$ has finite positive [variance](variance.md) $v$, and a matching [quota share reinsurance](#quota-share-reinsurance) contract exists with fraction $\alpha^*=\sqrt{\operatorname{Var}(S_I)/v}\in[0,1]$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds $\operatorname{Cov}(S,S_I)\leq\alpha^*v$. Expanding $\operatorname{Var}(S-S_I)$ then proves that the matching quota share minimizes the other party's [variance](variance.md), and hence the sum of party [variances](variance.md). Claimwise retentions $0\leq h(x)\leq x$ in a [compound Poisson distribution](#compound-poisson-distribution) automatically satisfy the required [variance](variance.md) range, because $\operatorname{Var}(S_I)=\lambda\mathbb E[h(X)^2]\leq\lambda\mathbb E[X^2]$.

#### Variance-minimizing quota share split

↑ **Parent:** [Quota share reinsurance](#quota-share-reinsurance)

For any aggregate with positive finite [variance](variance.md) $v$, [quota share reinsurance](#quota-share-reinsurance) with retained fraction $\alpha$ has total party [variance](variance.md) $v(\alpha^2+(1-\alpha)^2)=v/2+2v(\alpha-1/2)^2$. Equal sharing uniquely minimizes this objective. The two party totals remain dependent; adding their individual [variances](variance.md) is a different objective from the fixed [variance](variance.md) of their sum.

## Aggregate claims model

↑ **Parent:** [Actuarial statistics](actuarial-statistics.md)

An aggregate claims model separates the number $N$ of claims from their sizes $X_j$, with total $S=\sum_{j=1}^N X_j$ and the empty sum equal to zero. Under [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) for claim sizes, independent of $N$, [conditional expectation](measure-theory.md#conditional-expectation) gives tractable moments and transforms.

### Insurance exposure

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

[Insurance exposure](#insurance-exposure) scales the opportunity for claims: $w_j$ policy-years produce expected count $w_j\Theta$ at common annual frequency $\Theta$. Conditionally [independent](random-variable.md#independent-random-variables) [insurance exposures](#insurance-exposure) add, so the total count and total [insurance exposure](#insurance-exposure) are [sufficient statistics](probability-and-statistics.md#sufficient-statistic) in a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) frequency model. A yearly claim average has [conditional expectation](measure-theory.md#conditional-expectation) [independent](random-variable.md#independent-random-variables) of the number of policies, but its [conditional variance](variance.md#conditional-variance) falls with that number.

### Claim count

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

The number of insurance claims in a specified exposure period. Its [probability generating function](probability-theory.md#probability-generating-function) combines with the [moment-generating function](probability-theory.md#moment-generating-function) of an independent [claim size](#claim-size) through the [random-sum transform identity](#random-sum-transform-identity). A [Poisson distribution](discrete-probability-distribution.md#poisson-distribution), [geometric distribution](discrete-probability-distribution.md#geometric-distribution), or [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) provides a possible count model, with different dispersion and zero-claim [probabilities](probability-theory.md#probability).

### Claim size

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

The monetary amount of an individual insurance claim. Its [probability distribution](probability-theory.md#probability-distribution) describes loss severity, separately from the [claim count](#claim-count). In an independent [random sum of independent claims](#random-sum-of-independent-claims), severity mean $\mu$ and expected count combine to give aggregate mean $\mathbb EN\,\mu$.

#### Claims inflation

↑ **Parent:** [Claim size](#claim-size)

Claims [claims inflation](#claims-inflation) changes the monetary size of a claim over calendar time. With a fixed annual rate $r$, a time-zero size $c_0$ becomes the displayed end-of-year amount. Historical claim amounts must be converted to a common price year before their empirical monetary averages are combined. When the per-claim amounts are known, dividing total amount by the year's per-claim amount recovers the claim count.

### Heterogeneous individual claims model

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

Each policy has an independent [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) $B_i$ of probability $q_i$, and its independent severity $Y_i$ has [expected value](probability-theory.md#expected-value) $\mu_i$ and [variance](variance.md) $\sigma_i^2$. Independent policies give $\mathbb ET=\sum_iq_i\mu_i$ and $\operatorname{Var}(T)=\sum_i[q_i\sigma_i^2+q_i(1-q_i)\mu_i^2]$. Conditioning on the claim indicator proves the formulas. Keeping the policy label preserves the dependence between the occurrence probability and the severity law; replacing all labels by a single mixture is an approximation unless the relevant laws agree.

#### Variance comparison for compound portfolio approximations

↑ **Parent:** [Heterogeneous individual claims model](#heterogeneous-individual-claims-model)

Put $Q=\sum_iq_i$, $M=\sum_iq_i\mu_i$, and $A=\sum_iq_i\mathbb EY_i^2$. A [compound Poisson distribution](#compound-poisson-distribution) with count mean $Q$ and severity law $\sum_i(q_i/Q)F_i$ has [variance](variance.md) $V_{\mathrm P}=A$. A [compound binomial distribution](#compound-binomial-distribution) with $n$ trials, probability $Q/n$, and that same severity law has [variance](variance.md) $V_{\mathrm B}=A-M^2/n$. The individual-policy variance is $V=A-\sum_i(q_i\mu_i)^2$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\sum_i(q_i\mu_i)^2\geq M^2/n$, proving the ordering. Equality of the first two variances requires constant $q_i\mu_i$; it need not imply equality of the distributions. If all probabilities and severity laws are identical, the binomial compound approximation is exactly the individual model.

### Claim count distribution

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

The [probability distribution](probability-theory.md#probability-distribution) of the nonnegative integer number of claims over a specified accounting period. Its [probability generating function](probability-theory.md#probability-generating-function) determines the count probabilities. A [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) gives equal count [expected value](probability-theory.md#expected-value) and [variance](variance.md); a [Poisson mixture](discrete-probability-distribution.md#poisson-mixture) allows heterogeneity in the underlying risk intensity.

#### Panjer claim-count class

↑ **Parent:** [Claim count distribution](#claim-count-distribution)

The nonnegative integer laws whose probabilities satisfy this recurrence for all $n\ge1$. Their [probability generating function](probability-theory.md#probability-generating-function) solves $(1-az)G'(z)=(a+b)G(z)$. This is the $(a,b,0)$ count class used in the Panjer aggregate algorithm; the count recurrence itself should be distinguished from that aggregate recursion. It includes the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution), [binomial distribution](discrete-probability-distribution.md#binomial-distribution), and [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) with suitable parameters.

##### Panjer recursion

↑ **Parent:** [Panjer claim-count class](#panjer-claim-count-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Panjer_recursion)

For positive integer severities with [probability mass function](probability-theory.md#probability-mass-function) $f_j$ and independent count in the [Panjer claim-count class](#panjer-claim-count-class), the aggregate [probability mass function](probability-theory.md#probability-mass-function) starts at $g_0=p_0$ and satisfies the displayed recurrence. If $P,F,G$ are the count, severity and aggregate [probability generating functions](probability-theory.md#probability-generating-function), respectively, then $G=P\circ F$ and $(1-aF)G'=(a+b)F'G$. Equating the coefficient of $z^{r-1}$ gives $r g_r=\sum_{j=1}^r[ a(r-j)+(a+b)j]f_jg_{r-j}$. The positivity assumption excludes zero severities; otherwise the initial value and recursion denominator change.

###### Panjer recursion with zero severities

↑ **Parent:** [Panjer recursion](#panjer-recursion)

For a [claim count distribution](#claim-count-distribution) in the [Panjer claim-count class](#panjer-claim-count-class) and independent nonnegative integer severities with mass $f_j$, the [probability generating function](probability-theory.md#probability-generating-function) composition is $G_S=G_N\circ G_X$. Combining it with $(1-az)G_N'=(a+b)G_N$ gives $(1-aG_X)G_S'=(a+b)G_SG_X'$. Equating coefficients yields the displayed recursion. Zero severities change both the initial mass and the denominator. For nondegenerate proper Panjer count laws $a<1$, so the denominator is positive. An identically zero count is handled directly if its redundant parameter choice makes the denominator vanish.

### Poisson superposition of insurance portfolios

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

Independent claim [Poisson processes](probability-theory.md#poisson-process) of rates $\lambda_i$ merge into a [Poisson process](probability-theory.md#poisson-process) of rate $\lambda=\sum_i\lambda_i$, by the [Superposition theorem for Poisson point processes](probability-theory.md#superposition-theorem-for-poisson-point-processes). The merged claim law is a [mixture distribution](probability-theory.md#mixture-distribution) of the individual claim laws with weights $\lambda_i/\lambda$. Equivalently, multiplication of the individual compound-Poisson transforms produces $\exp(\lambda[\sum_i(\lambda_i/\lambda)M_i(r)-1])$.

### Random sum of independent claims

↑ **Parent:** [Aggregate claims model](#aggregate-claims-model)

For independent claim sizes with common [expected value](probability-theory.md#expected-value) $m$ and [variance](variance.md) $v$, independent of the nonnegative integer count $N$, the aggregate satisfies $\mathbb ES=m\mathbb EN$ and $\operatorname{Var}(S)=v\mathbb EN+m^2\operatorname{Var}(N)$. Its [moment-generating function](probability-theory.md#moment-generating-function) is $G_N(M_X(t))$ wherever finite. These identities follow from the [law of total expectation](measure-theory.md#law-of-total-expectation) and [law of total variance](probability-theory.md#law-of-total-variance).

#### Compound mixed Poisson distribution

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

A compound mixed Poisson distribution is a [random sum of independent claims](#random-sum-of-independent-claims) whose count has a [Poisson mixture](discrete-probability-distribution.md#poisson-mixture) law: conditional on a nonnegative random intensity $\Lambda$, $N$ has [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with parameter $\Lambda$. The claim sizes are [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), independent of the intensity and count mechanism. If $M_X$ is their [moment-generating function](probability-theory.md#moment-generating-function), then $M_S(t)=\mathbb E\exp(\Lambda(M_X(t)-1))$ wherever finite. A [gamma distribution](continuous-probability-distribution.md#gamma-distribution) intensity of shape $r$ and rate $\alpha$ gives a [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) count with shape $r$ and success probability $\alpha/(\alpha+1)$. Independent intensities with common gamma rate add their shapes by [additivity of independent gamma distributions with a common rate](continuous-probability-distribution.md#additivity-of-independent-gamma-distributions-with-a-common-rate).

#### Compound binomial distribution

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

For an independent [binomial distribution](discrete-probability-distribution.md#binomial-distribution) count $N\sim\operatorname{Binomial}(n,p)$, the aggregate can also be represented as $\sum_{j=1}^n B_jX_j$, with independent parameter-$p$ [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) $B_j$ and independent claim sizes. Its [cumulant-generating function](probability-theory.md#cumulant-generating-function) is $n\log(1-p+pM_X(t))$. Its third [cumulant](probability-theory.md#cumulant) is $n(pm_3-3p^2m_1m_2+2p^3m_1^3)$ in severity [moments](probability-theory.md#moment). Constant positive claims $d$ give $np(1-p)(1-2p)d^3$, which is negative when $p>1/2$. Thus positive claim sizes do not by themselves force a positive third [central moment](probability-theory.md#central-moment).

##### Binomial accident portfolio with Poisson clusters

↑ **Parent:** [Compound binomial distribution](#compound-binomial-distribution)

For independent factories with accident probability $p$, and independent [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) claim counts of mean $\lambda$ per accident, the accident count is binomial and each accident supplies a cluster. The [random-sum transform identity](#random-sum-transform-identity) gives the displayed [probability generating function](probability-theory.md#probability-generating-function). In particular the no-claim chance is $(1-p+pe^{-\lambda})^m$; a factory with an accident can still have zero claims. The binomial accident law has Panjer parameters $a=-p/(1-p)$ and $b=(m+1)p/(1-p)$.

#### Compound geometric distribution

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

Take an independent [geometric distribution](discrete-probability-distribution.md#geometric-distribution) count with $\mathbb P(N=k)=p(1-p)^k$, $k\ge0$, and sum its independent positive claims. Its [moment-generating function](probability-theory.md#moment-generating-function) is the displayed composition wherever finite. With $q=1-p$ and severity [moments](probability-theory.md#moment) $m_j$, the third [cumulant](probability-theory.md#cumulant) is $(q/p)m_3+3(q/p)^2m_1m_2+2(q/p)^3m_1^3$, which is strictly positive for nonzero positive claims and $0<p<1$. The law has an atom of mass $p$ at zero. Its positive-count convention would instead add a factor $M_X(t)$ to the numerator, as in the [geometric-sum moment-generating function](#geometric-sum-moment-generating-function).

##### Zero-based geometric sum of exponential variables

↑ **Parent:** [Compound geometric distribution](#compound-geometric-distribution)

If independent summands have [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of mean $\mu$ and the independent count has a zero-based [geometric distribution](discrete-probability-distribution.md#geometric-distribution) of parameter $p$, their [random sum of independent claims](#random-sum-of-independent-claims) has an atom $p$ at zero and an exponential positive component of rate $p/\mu$. Its [Laplace transform of a nonnegative random variable](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) is $p/[1-(1-p)/(1+\mu s)]=p+(1-p)p/(p+\mu s)$. Thus $\mathbb P(S>x)=(1-p)e^{-px/\mu}$ for $x>0$. Unlike the [geometric sum of exponential variables](continuous-probability-distribution.md#geometric-sum-of-exponential-variables) with a positive count, this law is not purely exponential.

#### Negative-binomial sum of exponential claims

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

Let $p+q=1$ and let the original independent count have [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) with [probability mass function](probability-theory.md#probability-mass-function) $\binom{n+k-1}{k}p^nq^k$ on $k\ge0$. With unit-rate [exponential distribution](continuous-probability-distribution.md#exponential-distribution) severities, its [moment-generating function](probability-theory.md#moment-generating-function) is $[p+qp/(p-t)]^n$ for $t<p$. Thus it also has a [random sum of independent claims](#random-sum-of-independent-claims) representation with independent [binomial distribution](discrete-probability-distribution.md#binomial-distribution) count $B$ and rate-$p$ [exponential distribution](continuous-probability-distribution.md#exponential-distribution) steps. For $n=2$ the law is $p^2\delta_0+2pq\operatorname{Exp}(p)+q^2\operatorname{Erlang}(2,p)$. The [hurdle decomposition of a positive random sum](#hurdle-decomposition-of-a-positive-random-sum) therefore has zero mass $p^2$ and positive density $p^2e^{-px}(2q+q^2x)/(1-p^2)$.

##### Finite Erlang-mixture tail for a negative-binomial exponential aggregate

↑ **Parent:** [Negative-binomial sum of exponential claims](#negative-binomial-sum-of-exponential-claims)

For independent rate-$\lambda$ [exponential distribution](continuous-probability-distribution.md#exponential-distribution) claims and a zero-based [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) count of shape $k$ and parameter $p$, the [random-sum transform identity](#random-sum-transform-identity) gives $M_S(t)=[p(\lambda-t)/(p\lambda-t)]^k$. This equals the transform of a [compound binomial distribution](#compound-binomial-distribution) with count $\operatorname{Bin}(k,1-p)$ and rate-$p\lambda$ [claim sizes](#claim-size). Conditional on its positive count $n$, the total has [Erlang distribution](continuous-probability-distribution.md#erlang-distribution), whose [survival function](survival-analysis.md#survival-function) is the inner exponential-polynomial sum. Conditioning yields the displayed finite [mixture distribution](probability-theory.md#mixture-distribution) formula for $x>0$. It replaces an infinite mixture and includes the zero-total atom $p^k$ through the omitted $n=0$ term.

#### Random-sum transform identity

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X_j$ independent of a nonnegative integer count $N$, set $S=\sum_{j=1}^N X_j$, including $S=0$ when $N=0$. Conditioning on the count gives $\mathbb E[e^{tS}\mid N=k]=M_X(t)^k$, hence the displayed composition of the [moment-generating function](probability-theory.md#moment-generating-function) with the [probability generating function](probability-theory.md#probability-generating-function). For positive summands the identity holds for all $t\le0$; positive $t$ requires convergence of the composed series. This permits [Laplace transforms of nonnegative random variables](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) to identify the law even when positive [exponential moments](probability-theory.md#exponential-moment) do not exist.

##### Cumulant composition for a random sum

↑ **Parent:** [Random-sum transform identity](#random-sum-transform-identity)

For a [random sum of independent claims](#random-sum-of-independent-claims), conditioning on the count gives $M_S(t)=\mathbb E[M_X(t)^N]$ and therefore the displayed [cumulant-generating function](probability-theory.md#cumulant-generating-function). Write $a_j=\kappa_{N,j}$ and $b_j=\kappa_{X,j}$. The chain rule gives $\kappa_{S,1}=a_1b_1$, $\kappa_{S,2}=a_1b_2+a_2b_1^2$, and $\kappa_{S,3}=a_1b_3+3a_2b_1b_2+a_3b_1^3$. In raw severity [moments](probability-theory.md#moment) $m_j=\mathbb EX^j$, the third [cumulant](probability-theory.md#cumulant) is $a_1m_3+3(a_2-a_1)m_1m_2+(a_3-3a_2+2a_1)m_1^3$. Positive exponential moments justify two-sided differentiation near zero; finite ordinary moments alone suffice for the corresponding left derivatives when claims are positive.

#### Geometric-sum moment-generating function

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

For a [geometric distribution](discrete-probability-distribution.md#geometric-distribution) count on the positive integers, independent of [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X_i$, the [moment-generating function](probability-theory.md#moment-generating-function) of $S=\sum_{i=1}^NX_i$ is the displayed expression. Condition on the count and sum a [geometric series](real-analysis.md#geometric-series). For real $t$, the finite domain requires $M_X(t)<\infty$ and $(1-p)M_X(t)<1$. Positive summands always permit $t\leq0$, even when no positive exponential moment exists; this gives a [Laplace transform of a nonnegative random variable](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable). The aggregate has no mass at zero when all summands are strictly positive.

##### Geometric sum of shape-two gamma variables

↑ **Parent:** [Geometric-sum moment-generating function](#geometric-sum-moment-generating-function)

Let the summands have [gamma distribution](continuous-probability-distribution.md#gamma-distribution) with shape two and rate $\beta$, and let the independent positive-support [geometric distribution](discrete-probability-distribution.md#geometric-distribution) count have parameter $p$. Put $a=\beta(1-\sqrt{1-p})$ and $b=\beta(1+\sqrt{1-p})$. The aggregate [moment-generating function](probability-theory.md#moment-generating-function) factors as $ab/((a-t)(b-t))$, so it is the sum of two independent [exponential distributions](continuous-probability-distribution.md#exponential-distribution) of rates $a,b$. Its [probability density function](continuous-probability-distribution.md#probability-density-function) is $ab(e^{-as}-e^{-bs})/(b-a)$ for $s>0$, nonnegative and integrating to one. This contrasts with the [geometric sum of exponential variables](continuous-probability-distribution.md#geometric-sum-of-exponential-variables), which is itself exponential.

#### Compound Poisson distribution

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compound_Poisson_distribution)

The law of a sum of independent identically distributed claims with an independent [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) count of parameter $\lambda$. If the claim [moment-generating function](probability-theory.md#moment-generating-function) is $M_X$, the aggregate transform is $\exp(\lambda(M_X(r)-1))$ wherever finite. It has an atom at zero when the claims are positive. This is the fixed-time law of a [Compound Poisson process](stochastic-process.md#compound-poisson-process).

##### Nested Poisson flood count

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

If a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) count $M$ of clusters has mean $\nu$, and each cluster independently contains a Poisson number of claims of mean $\lambda$, then the total count is a [compound Poisson distribution](#compound-poisson-distribution) with the displayed [probability generating function](probability-theory.md#probability-generating-function). Conditioning gives $\mathbb EN=\nu\lambda$ and $\operatorname{Var}N=\nu\lambda(1+\lambda)$, so it is not Poisson for positive parameters. With independent severities of mean $\mu$ and variance $\sigma^2$, the aggregate payment has mean $\nu\lambda\mu$ and variance $\nu[\lambda(\sigma^2+\mu^2)+\lambda^2\mu^2]$. Independent validity thinning replaces the per-cluster count mean by $\lambda(1-p)$ and multiplies expected payment by $1-p$.

##### Covariance of two components of a compound Poisson sum

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

Let $N\sim\operatorname{Pois}(\lambda)$ be [independent](random-variable.md#independent-random-variables) of [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $(Y_i,Z_i)$ with finite second [moments](probability-theory.md#moment). Conditioning on $N$ gives [covariance](variance.md#covariance) $N\operatorname{Cov}(Y_1,Z_1)$ and [conditional expectations](measure-theory.md#conditional-expectation) $N\mathbb EY_1,N\mathbb EZ_1$. [Law of total covariance](variance.md#law-of-total-covariance) and $\operatorname{Var}N=\lambda$ yield the formula. For per-claim [excess of loss reinsurance](#excess-of-loss-reinsurance) payouts $Y=\min(X,M)$ and $Z=(X-M)_+$, it becomes $\lambda M\mathbb E[(X-M)_+]$. The insurer and reinsurer aggregates share their claim count and are generally dependent.

##### Zero claim sizes in a compound Poisson representation

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

If zero-sized claims are allowed, a [compound Poisson distribution](#compound-poisson-distribution) count parameter need not be unique. [Poisson thinning](probability-theory.md#poisson-thinning) of zero claims gives the displayed positive-claim count parameter and the conditional [claim size](#claim-size) [probability distribution](probability-theory.md#probability-distribution) given $X>0$, without changing the aggregate. If no positive claims occur, the aggregate is identically zero. This matters when representing a finite weighted sum of [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) counts whose coefficients include zero.

##### Compound Poisson cumulants

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

Conditioning on the [independent](random-variable.md#independent-random-variables) [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) count in a random sum gives $\mathbb Ee^{tS}=\exp(\lambda(M_X(t)-1))$ wherever finite. Differentiation at zero gives the displayed [cumulants](probability-theory.md#cumulant) when the relevant derivatives exist. The aggregate [variance](variance.md) is the count rate times the raw second claim [moment](probability-theory.md#moment), not just the claim [variance](variance.md). Positive [moment-generating function](probability-theory.md#moment-generating-function) arguments need an exponential [moment](probability-theory.md#moment); finite first and second claim [moments](probability-theory.md#moment) suffice for the aggregate [mean](probability-theory.md#expected-value) and [variance](variance.md) by conditioning or right derivatives at zero of the [Laplace transform of a nonnegative random variable](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable).

##### Normal approximation to a compound Poisson aggregate

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

For a [compound Poisson distribution](#compound-poisson-distribution) of count parameter $\lambda$ and severity [moments](probability-theory.md#moment) $m_1,m_2$, the [expected value](probability-theory.md#expected-value) is $\lambda m_1$ and the [variance](variance.md) is $\lambda m_2$. As $\lambda\to\infty$ with the severity law fixed and $m_2<\infty$, the standardized aggregate converges in distribution to the standard [normal distribution](probability-theory.md#normal-distribution). Indeed, the logarithm of its [characteristic function](probability-theory.md#characteristic-function) is $\lambda[\varphi_X(t/\sqrt{\lambda m_2})-1]-it\lambda m_1/\sqrt{\lambda m_2}$; the second-order expansion of $\varphi_X$ makes this tend to $-t^2/2$. The approximation loses the zero atom and assigns positive [probability](probability-theory.md#probability) to negative losses.

##### Three-cumulant shifted gamma approximation

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

Approximate a [compound Poisson distribution](#compound-poisson-distribution) of positive claims by a [shifted gamma distribution](continuous-probability-distribution.md#shifted-gamma-distribution) whose first three [cumulants](probability-theory.md#cumulant) agree. Here $m_j=\mathbb E X^j$ are raw severity [moments](probability-theory.md#moment), while the compound [cumulants](probability-theory.md#cumulant) are $\lambda m_j$. Solve $k+\alpha/\nu=\lambda m_1$, $\alpha/\nu^2=\lambda m_2$, and $2\alpha/\nu^3=\lambda m_3$ to obtain the displayed parameters. The approximation captures positive [skewness](probability-theory.md#skewness), but not the atom $e^{-\lambda}$ at zero. Its shift can be negative; with exponential claims of mean $\mu$ it is $-\lambda\mu/3$. Matching three [cumulants](probability-theory.md#cumulant) alone supplies no general tail-error bound.

##### Raw moment recursion for a compound Poisson distribution

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

Write $m_k=\mathbb E S^k$, $m_0=1$, and $\mu_j=\mathbb E X^j$. Apply the [Poisson size-bias identity](discrete-probability-distribution.md#poisson-size-bias-identity) with $h(s)=s^{k-1}$, and expand $(S+X)^{k-1}$ using the [binomial theorem](combinatorics.md#binomial-theorem) and [independence](random-variable.md#independent-random-variables). A finite $k$th severity [moment](probability-theory.md#moment) suffices. In particular, the aggregate [expected value](probability-theory.md#expected-value), [variance](variance.md), and third [central moment](probability-theory.md#central-moment) are $\lambda\mu_1$, $\lambda\mu_2$, and $\lambda\mu_3$, respectively; the latter two use raw severity [moments](probability-theory.md#moment).

##### Retained compound Poisson aggregate

↑ **Parent:** [Compound Poisson distribution](#compound-poisson-distribution)

Applying a measurable per-claim retention $g$ to independent claim sizes preserves the [compound Poisson distribution](#compound-poisson-distribution) form. The transformed severity is the [pushforward measure](measure-theory.md#pushforward-measure) of the original severity law. With count parameter $\lambda$, the retained aggregate has [expected value](probability-theory.md#expected-value) $\lambda\mathbb E g(X)$ and [variance](variance.md) $\lambda\mathbb E[g(X)^2]$. Zero retained marks may be removed by [Poisson thinning](probability-theory.md#poisson-thinning).

#### Hurdle decomposition of a positive random sum

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

For positive claim sizes, a [random sum of independent claims](#random-sum-of-independent-claims) is zero exactly when its count is zero. Its law is a [mixture distribution](probability-theory.md#mixture-distribution) of a zero atom of mass $p=\mathbb P(N=0)$ and, with weight $1-p$, a random sum whose count has the [zero-truncated claim-count distribution](probability-theory.md#zero-truncated-claim-count-distribution). An independent [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) multiplying that positive component gives the same law. This is distinct from arbitrarily inserting additional zeros into an otherwise unchanged count law.

#### Gamma-mixed Poisson aggregate with exponential claims

↑ **Parent:** [Random sum of independent claims](#random-sum-of-independent-claims)

If $\Lambda$ has [gamma distribution](continuous-probability-distribution.md#gamma-distribution) with shape $2$ and rate $p/q$, $N\mid\Lambda$ has [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with intensity $\Lambda$, and the independent claim sizes have [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of mean $\mu$, where $p+q=1$, the aggregate law is $p^2\delta_0+2pq\,\operatorname{Exp}(p/\mu)+q^2\operatorname{Gamma}(2,\text{rate }p/\mu)$. This follows by expanding its [moment-generating function](probability-theory.md#moment-generating-function) as $[p+q\,p/(p-\mu t)]^2$.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
