# Five-state harmonic absorption example

↑ **Parent:** [Harmonic function for a Markov chain](harmonic-function-for-a-markov-chain.md)

Take a [birth-death chain](birth-death-chain.md) on $\{0,1,2,3,4\}$. At each interior state, move up one state with [probability](probability.md) $p=1/2$ and down one state with [probability](probability.md) $q=1/2$. The endpoints are [absorbing states](absorbing-state.md): $P_{00}=P_{44}=1$. This is a small [gambler's ruin](gambler-s-ruin.md) model in which the state can represent capital, and reaching $4$ is success.

<a id="image-five-states-with-fair-interior-transitions-and-absorbing-endpoints-each-displayed-value-is-the-probability-of-reaching-4-before-0"></a>
![](harmonic-markov-absorption-network.png)

**[Figure 1](#image-five-states-with-fair-interior-transitions-and-absorbing-endpoints-each-displayed-value-is-the-probability-of-reaching-4-before-0). Five states with fair interior transitions and absorbing endpoints; each displayed value is the probability of reaching 4 before 0.**

Let $T_a=\inf\{n\geq0:X_n=a\}$ be the [hitting time](first-passage-time.md) of endpoint $a$, and let $T=\min(T_0,T_4)$ be the first endpoint [hitting time](first-passage-time.md). The desired [hitting probability](hitting-probability.md) is $h_i=\mathbb P_i(T_4<T_0)$. [First-step analysis](first-step-analysis.md) and the [Markov property](markov-property.md) give

$$
h_0=0,\qquad h_4=1,\qquad h_i=\tfrac12h_{i-1}+\tfrac12h_{i+1}\quad(i=1,2,3).
$$

The interior equation says adjacent differences are equal. Four equal increments must bridge the boundary values $0$ and $1$, so

$$
h_i=\frac i4,\qquad (h_0,h_1,h_2,h_3,h_4)=(0,\tfrac14,\tfrac12,\tfrac34,1).
$$

For example, from state $2$ the [hitting probability](hitting-probability.md) is $1/2$, and its one-step average is $\tfrac12(1/4)+\tfrac12(3/4)=1/2$. Individual [sample paths](sample-path.md) can wander back and forth, but the same averaging rule already accounts for all of them.

Now ask how long it takes to reach either endpoint. The [expected hitting time](expected-hitting-time.md) $t_i=\mathbb E_iT$ counts steps, including the transition that first reaches an endpoint. [First-step analysis](first-step-analysis.md) gives

$$
t_0=t_4=0,\qquad t_i=1+\tfrac12t_{i-1}+\tfrac12t_{i+1}\quad(i=1,2,3).
$$

This is a discrete [Poisson equation](poisson-s-equation.md), $(I-P)t=1$ in the interior. The extra $1$ counts the step just taken. The quadratic values

$$
t_i=i(4-i),\qquad (t_0,t_1,t_2,t_3,t_4)=(0,3,4,3,0)
$$

satisfy the equations; from state $2$, $t_2=1+\tfrac12(3)+\tfrac12(3)=4$ steps. The [hitting probability](hitting-probability.md) is harmonic, whereas the [expected hitting time](expected-hitting-time.md) has a nonzero source term. These are special cases of [expected duration of symmetric gambler's ruin](expected-duration-of-symmetric-gambler-s-ruin.md); see [Hao Wu's MIT lecture 16, gambler's ruin, slide 9](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/ddeda684b0dd6a1422418c7eca3ce843_MIT18_445S15_lecture16.pdf).

For a [biased random walk](biased-random-walk.md) with $p=0.6$ upward and $q=0.4$ downward, keep the same [absorbing states](absorbing-state.md). The interior harmonic equation becomes $h_i=ph_{i+1}+qh_{i-1}$. Using [biased gambler's ruin probability](biased-gambler-s-ruin-probability.md) with these boundary values gives

$$
r=\frac qp=\frac23,\qquad h_i=\frac{1-r^i}{1-r^4},\qquad (h_0,h_1,h_2,h_3,h_4)=\left(0,\frac{27}{65},\frac9{13},\frac{57}{65},1\right).
$$

The three interior [hitting probabilities](hitting-probability.md) are approximately $0.415385$, $0.692308$, and $0.876923$. Thus starting at $2$ now succeeds about $69.23\%$ of the time. A direct check is $0.6(57/65)+0.4(27/65)=9/13$. The curved profile reflects the unequal transition weights: its successive increments shrink by the factor $q/p=2/3$. The formula, with the endpoint denoted $T$ there, is verified in [Karger and Lynch's MIT lecture 26, sections 2.3-2.4](https://courses.csail.mit.edu/6.042/past-devel/archive/spring00/archive/lectures/L26.pdf); the five-state numbers here are direct substitutions.

<a id="image-hitting-4-before-0-for-fair-and-upward-biased-walks-compared-with-the-fair-walk-s-expected-number-of-steps-to-either-endpoint-lines-join-discrete-state-values"></a>
![](harmonic-hitting-probability-profiles.png)

**[Figure 2](#image-hitting-4-before-0-for-fair-and-upward-biased-walks-compared-with-the-fair-walk-s-expected-number-of-steps-to-either-endpoint-lines-join-discrete-state-values). Hitting 4 before 0 for fair and upward-biased walks, compared with the fair walk's expected number of steps to either endpoint; lines join discrete state values.**

Why does harmonic averaging produce the correct [hitting probability](hitting-probability.md)? With the [natural filtration](natural-filtration.md) $\mathcal F_n=\sigma(X_0,\ldots,X_n)$, the [Markov property](markov-property.md) gives the [conditional expectation](conditional-expectation.md) identity

$$
\mathbb E[h(X_{n+1})\mid\mathcal F_n]=(Ph)(X_n).
$$

For a function harmonic everywhere, this makes $h(X_n)$ a [martingale](martingale-split.md) whenever it is integrable. For a function harmonic only in the interior, $M_n=h(X_{n\wedge T})$ is a [stopped martingale](stopped-martingale.md). In either five-state example, $0\leq M_n\leq1$. Also, from any interior state at most three consecutive upward steps reach $4$, with [probability](probability.md) at least $p^3>0$. Repeated three-step blocks give $\mathbb P_i(T>3k)\leq(1-p^3)^k$, so $T$ is [almost surely](almost-sure-convergence.md) finite and has finite [expected value](expected-value-split.md); compare [finite-interval exit times have geometric tails](finite-interval-exit-times-have-geometric-tails.md). Applying [optional stopping](optional-sampling-theorem-for-a-supermartingale.md) at $n\wedge T$ and then the [bounded convergence theorem](bounded-convergence-theorem.md) gives

$$
h_i=\mathbb E_i[h(X_T)]=\mathbb P_i(X_T=4).
$$

The boundedness and finite [hitting time](first-passage-time.md) justify this passage to the limit. See [Steven Lalley's notes, harmonic functions and stopped expectations, theorem 1](https://galton.uchicago.edu/~lalley/Courses/312/HarmonicFunctions.pdf), and [stopped martingale in discrete time](stopped-martingale-in-discrete-time.md) for this bounded version of [optional stopping](optional-sampling-theorem-for-a-supermartingale.md).

Uniqueness has a short [maximum principle](maximum-principle.md) explanation. On a finite [state space](state-space.md), the difference of two harmonic extensions with the same [boundary conditions](boundary-condition.md) is zero on the boundary. If its positive maximum occurs inside, the weighted average forces every successor with positive [transition probability](transition-probability.md) to have the same maximum. A path to the boundary propagates that maximum to zero, a contradiction. Applying the argument to the negative of the difference proves uniqueness. Reachability of the boundary is essential: an interior [closed communicating class](closed-communicating-class.md) can retain an arbitrary constant.

// Target: markov-process.bigb

## ↑ Ancestors (8)

1. [Harmonic function for a Markov chain](harmonic-function-for-a-markov-chain.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
