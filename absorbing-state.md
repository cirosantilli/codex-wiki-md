# Absorbing state

↑ **Parent:** [Markov chain](markov-chain-split.md)

For a finite, time-homogeneous [Discrete-time Markov chain](discrete-time-markov-chain.md) with row-stochastic [transition matrix](stochastic-matrix.md) $P$, a state $a$ is absorbing exactly when $P_{aa}=1$. Nonnegativity and the row sum then force $P_{aj}=0$ for $j\ne a$: once entered, $a$ is never left. Equivalently, $\{a\}$ is a [closed communicating class](closed-communicating-class.md). A larger [closed communicating class](closed-communicating-class.md) may keep moving internally; closure means confinement to a set, whereas absorption at a state means remaining at one point.

An [absorbing state](absorbing-state.md) is useful for recording a terminal outcome: after a toy routine finishes, keep its outcome in the [state space](state-space.md) so that the same [transition matrix](stochastic-matrix.md) still describes subsequent steps. Calling a finite [Markov chain](markov-chain-split.md) absorbing usually also requires that some [absorbing state](absorbing-state.md) be accessible from every state. Merely containing an [absorbing state](absorbing-state.md) is insufficient: another [closed communicating class](closed-communicating-class.md) could prevent absorption. See [Grinstead and Snell, Introduction to Probability, section 11.2](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=423) for this convention.

Consider a constructed routine with unfinished modes $u,v$ and terminal outcomes $A,B$. All the following [transition probabilities](transition-probability.md) are chosen for illustration, not estimated from observations. In state order $(u,v,A,B)$, take

$$
P=\begin{pmatrix}
1/2&1/4&1/4&0\\
1/4&1/4&0&1/2\\
0&0&1&0\\
0&0&0&1
\end{pmatrix}.
$$

The [communicating class](communicating-class.md) $\{u,v\}$ is open, while $\{A\}$ and $\{B\}$ are [closed communicating classes](closed-communicating-class.md) consisting of [absorbing states](absorbing-state.md). Both terminal outcomes are accessible from both unfinished modes, sometimes by an indirect path.

<a id="image-a-constructed-four-state-routine-arrows-give-transition-probabilities-and-the-two-absorbing-outcomes-have-different-eventual-probabilities-and-waiting-times"></a>
![](markov-classes-absorption-terminal-routine.png)

**[Figure 4](#image-a-constructed-four-state-routine-arrows-give-transition-probabilities-and-the-two-absorbing-outcomes-have-different-eventual-probabilities-and-waiting-times). A constructed four-state routine: arrows give transition probabilities, and the two absorbing outcomes have different eventual probabilities and waiting times.**

Let $T=\inf\{n\geq0:X_n\in\{A,B\}\}$ be the terminal [hitting time](first-passage-time.md). Write $h_i=\mathbb P_i(X_T=A)$ for the [absorption probability](splitting-probability.md) and $t_i=\mathbb E_iT$ for the [expected hitting time](expected-hitting-time.md), with the subscript denoting the starting state. [First-step analysis](first-step-analysis.md) gives

$$
h_u=\tfrac12h_u+\tfrac14h_v+\tfrac14,\qquad
h_v=\tfrac14h_u+\tfrac14h_v,
$$



$$
t_u=1+\tfrac12t_u+\tfrac14t_v,\qquad
t_v=1+\tfrac14t_u+\tfrac14t_v.
$$

Here $h_A=1$, $h_B=0$, and $t_A=t_B=0$. Solving these two pairs of [linear equations](linear-equation.md) yields

$$
(h_u,h_v)=\left(\frac35,\frac15\right),\qquad
(t_u,t_v)=\left(\frac{16}5,\frac{12}5\right).
$$

Starting at $u$ therefore ends at $A$ with [probability](probability.md) $0.6$ and takes $3.2$ steps on average to reach either terminal state. The terminal [hitting time](first-passage-time.md) counts the transition into the outcome, but no later self-transitions. Outcome and duration answer different questions: from $v$, outcome $A$ is less likely, yet termination is faster on average.

The [matrix power](matrix-power.md) $P^2$ gives the [probability distribution](probability-distribution-split.md) after two steps from $u$ as

$$
(P^2)_{u,\cdot}=\left(\frac5{16},\frac3{16},\frac38,\frac18\right).
$$

Thus $\mathbb P_u(T>2)=1/2$, and the [probability](probability.md) of having already reached $A$ is $3/8$, still below its eventual [absorption probability](splitting-probability.md) $3/5$. From either unfinished mode, each next step has terminal [probability](probability.md) at least $1/4$. Consequently $\mathbb P_i(T>n)\leq(3/4)^n$, proving termination [almost surely](almost-sure-convergence.md) and finite [expected hitting time](expected-hitting-time.md) directly. The [Fundamental matrix of a finite absorbing Markov chain](fundamental-matrix-of-a-finite-absorbing-markov-chain.md) packages both calculations and counts visits to unfinished modes.

**Table of contents**

- [Fundamental matrix of a finite absorbing Markov chain](fundamental-matrix-of-a-finite-absorbing-markov-chain.md)

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Absorbing Markov chain](absorbing-markov-chain.md)
- [Absorbing state](absorbing-state.md)
- [Communicating class](communicating-class.md)
- [Extinction probability of a branching process](extinction-probability-of-a-branching-process.md)
- [Five-state harmonic absorption example](five-state-harmonic-absorption-example.md)
- [Fundamental matrix of a finite absorbing Markov chain](fundamental-matrix-of-a-finite-absorbing-markov-chain.md)
- [Galton-Watson extinction fixed point](galton-watson-extinction-fixed-point.md)
- [Galton-Watson process](galton-watson-process-split.md)
- [Harmonic function for a Markov chain](harmonic-function-for-a-markov-chain.md)
- [Invariant measures of the two-dimensional voter model](invariant-measures-of-the-two-dimensional-voter-model.md)
- [Irreducible Markov chain](irreducible-markov-chain.md)
- [Mixed panel and exact-death likelihood](mixed-panel-and-exact-death-likelihood.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/5/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/5/ii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/5/ii/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/9h/ii/solution.md)
- [Progressive illness-death model](progressive-illness-death-model.md)
- [Three-state irreversible disease model](three-state-irreversible-disease-model.md)
- [Transition intensity matrix](transition-intensity-matrix.md)
- [Uniform decreasing Markov chain](uniform-decreasing-markov-chain.md)
- [Voter model](voter-model.md)
