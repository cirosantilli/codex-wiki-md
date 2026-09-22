<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

A [control policy](../../../../../control-policy.md) specifies each control as a nonanticipating measurable function of the observed history, possibly with additional randomization. It may depend on time and the entire past; a stationary [Markov policy](../../../../../markov-policy.md) uses only the current state. We use the standard admissibility assumptions allowing measurable choices and concatenation of continuation policies.

The [dynamic programming operator](../../../../../dynamic-programming-operator.md) is monotone: $f\le g$ implies $\mathcal Lf\le\mathcal Lg$. Nonnegative costs give $F_1\ge F_0=0$, so induction gives $F_{t+1}\ge F_t$. Thus **$F_t$ increases pointwise to an extended nonnegative limit $F_\infty$**. Backward induction identifies $F_t$ with the infimum of expected costs for the first $t$ periods: condition on the first control and next state, then optimize the continuation. Every infinite-horizon policy has at least that finite-horizon cost, so

$$
\boxed{F_\infty\le F.}
$$

For the [Bellman equation](../../../../../bellman-equation.md), any infinite-horizon policy, conditional on its first action and next state, has continuation cost at least $F(X_1)$. Its total cost is therefore at least $\mathcal LF(x)$; infimizing gives $F\ge\mathcal LF$. For the reverse inequality at a state with finite $\mathcal LF(x)$, choose a first action within $\varepsilon/2$ of its infimum and concatenate continuation policies whose costs are within $\varepsilon/(2\beta)$ of $F(y)$ at each next state $y$. This produces a policy of cost at most $\mathcal LF(x)+\varepsilon$. Such continuations are needed only at states of finite value, which have probability one under an action with finite continuation [expectation](../../../../../expected-value.md). Let $\varepsilon\downarrow0$. If $\mathcal LF(x)=\infty$, the first inequality already gives $F(x)=\infty$. Therefore

$$
\boxed{F=\mathcal LF.}
$$

Let $\Phi=\mathcal L\Phi\ge0$, and use the permitted selector $u_*$. Under the stationary policy $u_*(X_t)$, repeated [conditional expectation](../../../../../conditional-expectation.md) gives

$$
\Phi(x)=\mathbb E\left[\sum_{t=0}^{T-1}\beta^tc(X_t,u_*(X_t))+\beta^T\Phi(X_T)\right].
$$

If $\Phi(x)$ is infinite the desired comparison is immediate; otherwise these nonnegative quantities have finite [expectations](../../../../../expected-value.md) and the displayed recursion is legitimate. Drop the terminal term and apply [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) as $T\to\infty$. The policy's infinite-horizon cost is at most $\Phi(x)$, so

$$
\boxed{F(x)\le J^{u_*}(x)\le\Phi(x).}
$$

Thus the value is the least nonnegative Bellman [fixed point](../../../../../fixed-point.md). The argument works also for $\beta=1$ because costs and the dropped terminal term are nonnegative; it makes no unwarranted contraction or finite-value assumption.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
