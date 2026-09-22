# Bellman equation

↑ **Parent:** [Dynamic programming](dynamic-programming.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bellman_equation)

A [Bellman equation](bellman-equation.md) expresses the [dynamic programming principle](dynamic-programming-principle.md) as a [recurrence relation](recurrence-relation.md) for a [value function](value-function.md): optimize the current reward plus the best attainable continuation. Let $s$ be a [dynamic programming state](dynamic-programming-state.md), $A_t(s)$ the allowed actions at time $t$, $r_t(s,a)$ the immediate reward, and $F_t(s,a)$ the next [dynamic programming state](dynamic-programming-state.md). With terminal time $T$ and terminal reward $g$, the deterministic finite-horizon [Bellman equation](bellman-equation.md) is

$$
V_T(s)=g(s),\qquad
V_t(s)=\max_{a\in A_t(s)}\{r_t(s,a)+V_{t+1}(F_t(s,a))\},
\quad t=T-1,\ldots,0.
$$

Here $V_t(s)$ measures total reward from time $t$ through the terminal reward. Start with $g$ and evaluate backwards; the terminal condition anchors the [recurrence relation](recurrence-relation.md). For finite nonempty action sets, finite rewards, and finite terminal rewards, a [maximum](maximum-of-a-subset-of-a-total-order.md) exists at each step. If an optimum need not be attained, use a [supremum](supremum.md). A [minimization problem](minimization-problem.md) instead uses a [minimum](minimum-of-a-subset-of-a-total-order.md) or [infimum](infimum.md). The [0-1 knapsack problem](0-1-knapsack-problem.md) above is the same comparison between an immediate item value plus a continuation and the continuation after skipping. See [Bertsekas, MIT lecture 2: the backwards recursion](https://ocw.mit.edu/courses/6-231-dynamic-programming-and-stochastic-control-fall-2015/2beec55b0de261096962e514febe3b5c_MIT6_231F15_Lec2.pdf).

In a [Markov decision process](markov-decision-process.md), the next [dynamic programming state](dynamic-programming-state.md) $S_{t+1}$ is random. If $r_t(s,a)$ denotes the expected immediate reward and $\beta$ is a [discount factor](discount-factor.md), the finite-horizon [Bellman equation](bellman-equation.md) becomes

$$
V_T(s)=g(s),\qquad
V_t(s)=\max_{a\in A_t(s)}\left\{r_t(s,a)+\beta\mathbb E[V_{t+1}(S_{t+1})\mid S_t=s,\ a_t=a]\right\}.
$$

The [conditional expectation](conditional-expectation.md) averages over the next [dynamic programming state](dynamic-programming-state.md) before choosing the current action; that action cannot use a future outcome that has not yet been observed. For a finite [state space](state-space.md) with [transition probabilities](transition-probability.md) $p_t(s'\mid s,a)$, the continuation term is $\beta\sum_{s'}p_t(s'\mid s,a)V_{t+1}(s')$. Taking $\beta=1$ gives the undiscounted finite-horizon problem. With a [discount factor](discount-factor.md) $0\leq\beta<1$, rewards $k$ steps ahead carry a factor $\beta^k$, including the terminal reward. A maximizing action for each $(t,s)$ specifies a [Markov policy](markov-policy.md), which contains decisions rather than just optimal scores.

For an infinite horizon with a finite [state space](state-space.md), finite nonempty action sets, time-independent [transition probabilities](transition-probability.md), bounded rewards $|r(s,a)|\leq M$, and a [discount factor](discount-factor.md) $0\leq\beta<1$, the optimal [value function](value-function.md) satisfies

$$
V(s)=\max_{a\in A(s)}\left\{r(s,a)+\beta\sum_{s'}p(s'\mid s,a)V(s')\right\},
\qquad |V(s)|\leq\frac{M}{1-\beta}.
$$

In this setting the maximizing [dynamic programming operator](dynamic-programming-operator.md) is a [contraction mapping](contraction-mapping.md) in the [supremum norm](supremum-norm.md), so the [Banach fixed-point theorem](contraction-mapping-theorem.md) gives a unique bounded [fixed point](fixed-point.md) and convergence of repeated application to it. See [Bertsekas, MIT lecture 15: bounded discounted problems](https://ocw.mit.edu/courses/6-231-dynamic-programming-and-stochastic-control-fall-2015/ec7b70a77571e2f2c48a5a0fa5fa23d5_MIT6_231F15_Lec15.pdf). These hypotheses matter: with one state, one action, zero reward, and $\beta=1$, the [Bellman equation](bellman-equation.md) is merely $V(s)=V(s)$, so every finite constant is a [fixed point](fixed-point.md), although the actual total-reward [value function](value-function.md) is zero. The [average-reward Bellman equation](average-reward-bellman-equation.md) and [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md) address other settings with their own conditions.

**Table of contents**

- [Dynamic programming operator](dynamic-programming-operator.md)
- [Bellman comparison with nonnegative rewards and superunit discount](bellman-comparison-with-nonnegative-rewards-and-superunit-discount.md)
- [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md)
  - [Verification by a nonnegative control supermartingale](verification-by-a-nonnegative-control-supermartingale.md)
  - [Linear-quadratic optimal control](linear-quadratic-optimal-control.md)
    - [Discrete Riccati recurrence](discrete-riccati-recurrence.md)

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Bellman comparison with nonnegative rewards and superunit discount](bellman-comparison-with-nonnegative-rewards-and-superunit-discount.md)
- [Bellman equation](bellman-equation.md)
- [Discrete Riccati recurrence](discrete-riccati-recurrence.md)
- [Dynamic programming](dynamic-programming.md)
- [Dynamic programming operator](dynamic-programming-operator.md)
- [Dynamic programming state](dynamic-programming-state.md)
- [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md)
- [Markov decision process](markov-decision-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/28j/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/28i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/29i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/28i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/28j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/28i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/28j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/28k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/26k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/25k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/28k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/28k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/28k/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/28k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/30k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/30k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/30k/c/solution.md)
- [Policy iteration](policy-iteration.md)
- [Rewarded Bayesian box search Bellman equation](rewarded-bayesian-box-search-bellman-equation.md)
- [Value function](value-function.md)
