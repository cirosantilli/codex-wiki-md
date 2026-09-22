<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [payoff](../../../../../../payoff.md) table is blank in the original PDF, so denote its four row-player [payoffs](../../../../../../payoff.md) by $R,S,T,P$ for $CC,CD,DC,DD$, with the [prisoner's dilemma](../../../../../../prisoner-s-dilemma.md) ordering $T>R>P>S$. No numerical entries are inferred. Let the two [reactive strategies](../../../../../../reactive-strategy-game-theory.md) be $(p_1,q_1)$ and $(p_2,q_2)$, where $p_i$ is cooperation after the opponent's cooperation and $q_i$ cooperation after defection.

The joint action states form a four-state [Markov chain](../../../../../../markov-chain.md). In state order $CC,CD,DC,DD$, its transition [matrix](../../../../../../matrix.md) is

$$
\begin{pmatrix}
p_1p_2&p_1(1-p_2)&(1-p_1)p_2&(1-p_1)(1-p_2)\\
q_1p_2&q_1(1-p_2)&(1-q_1)p_2&(1-q_1)(1-p_2)\\
p_1q_2&p_1(1-q_2)&(1-p_1)q_2&(1-p_1)(1-q_2)\\
q_1q_2&q_1(1-q_2)&(1-q_1)q_2&(1-q_1)(1-q_2)
\end{pmatrix}.
$$

The prescribed initial memories give [independent](../../../../../../independent-random-variables.md) first actions with cooperation [probabilities](../../../../../../probability.md) $p_1,p_2$. Same-round actions remain [independent](../../../../../../independent-random-variables.md): each player's next action uses the other player's previous action and its own [independent](../../../../../../independent-random-variables.md) random draw. Thus their marginal cooperation [probabilities](../../../../../../probability.md) obey

$$
x_{t+1}=q_1+(p_1-q_1)y_t,
\qquad y_{t+1}=q_2+(p_2-q_2)x_t.
$$

Put $a_i=p_i-q_i$. If $|a_1a_2|<1$, the two-step recurrences contract and the [long-run payoff of reactive strategies](../../../../../../long-run-payoff-of-reactive-strategies.md) follows from

$$
\boxed{x_*=\frac{q_1+a_1q_2}{1-a_1a_2},\qquad
y_*=\frac{q_2+a_2q_1}{1-a_1a_2}.}
$$

The joint [stationary distribution](../../../../../../stationary-distribution.md) is $(x_*y_*,x_*(1-y_*),(1-x_*)y_*,(1-x_*)(1-y_*))$. Player 1's [mean](../../../../../../expected-value.md) [payoff](../../../../../../payoff.md) is $Rx_*y_*+Sx_*(1-y_*)+T(1-x_*)y_*+P(1-x_*)(1-y_*)$; exchange $S,T$ for player 2.

The deterministic boundaries must retain the initial memories rather than divide by zero. Two [Tit for tat](../../../../../../tit-for-tat.md) players cooperate forever and earn $R$. Two players who always do the opposite of the opponent's previous action alternate $DD,CC$ and average $(P+R)/2$. One of each cycles through all four states and each averages $(R+S+T+P)/4$. These are the only cases with $|a_1a_2|=1$. A periodic [Markov chain](../../../../../../markov-chain.md) need not have convergent state [probabilities](../../../../../../probability.md), but its long-time average [payoff](../../../../../../payoff.md) is defined by its cycle frequencies.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
