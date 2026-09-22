<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Nash equilibrium](../../../../../nash-equilibrium.md) is a profile in which each player's strategy is a [best response](../../../../../best-response.md) to all the others: no unilateral change increases that player's payoff. In this routing game the payoff can be taken as minus delay. A [pure strategy](../../../../../pure-strategy.md) is a single route; a [mixed strategy](../../../../../mixed-strategy.md) is a [probability distribution](../../../../../probability-distribution.md) over routes, with different players randomizing independently. A non-zero-sum game does not require the players' payoffs to add to a fixed total. [Nash's theorem](../../../../../nash-s-theorem.md) guarantees a mixed [Nash equilibrium](../../../../../nash-equilibrium.md) for every [finite game](../../../../../finite-game.md) with finitely many [pure strategies](../../../../../pure-strategy.md). Pure equilibria need not exist in general; the [congestion game](../../../../../congestion-game.md) here does have them, since a unilateral delay change equals the change in its finite congestion potential.

Put $x=n_1+n_3$ and $y=n_2+n_3$. The three current delays, in the order $ABD,ACD,ABCD$, are

$$
C_1=3+\frac{x}{100},\qquad
C_2=3+\frac{y}{100},\qquad
C_3=\frac94+\frac{x+y}{100}.
$$

For a player using the first route, switching to the second makes the new second-route load $y+1$, while switching to the third retains that player's use of $AB$ and adds one user to $CD$. The two comparisons are therefore

$$
3+\frac{x}{100}\leq3+\frac{y+1}{100},\qquad
3+\frac{x}{100}\leq\frac94+\frac{x+y+1}{100}.
$$

They reduce to $x\leq y+1$ and $y\geq74$. Reversing the two outer routes gives $y\leq x+1$ and $x\geq74$ for each second-route user. A third-route user who switches to the first retains their own use of $AB$, and one who switches to the second retains their own use of $CD$. The corresponding comparisons give $y\leq75$ and $x\leq75$. Thus the necessary and sufficient conditions, together with nonnegative integer counts summing to $n$, are

$$
\boxed{\begin{aligned}
n_1>0&\Longrightarrow x\leq y+1\text{ and }y\geq74,\\
n_2>0&\Longrightarrow y\leq x+1\text{ and }x\geq74,\\
n_3>0&\Longrightarrow x\leq75\text{ and }y\leq75.
\end{aligned}}
$$

They are sufficient because each used route has been compared with both alternatives, and necessary because each comparison is an available unilateral deviation. The unit changes in loads matter in a finite-player [congestion game](../../../../../congestion-game.md).

For $n=100$, the counts $(25,25,50)$ give $x=y=75$ and every player's delay is $15/4$. They satisfy all the conditions. To find every pure [Nash equilibrium](../../../../../nash-equilibrium.md), first note that $n_3=0$ is impossible: if either outer route is empty, its other route users fail the lower-load condition; if both are used, $x,y\geq74$ contradict $x+y=100$. Thus $n_3>0$, so $x,y\leq75$. Since $x=100-n_2$ and $y=100-n_1$, this forces $n_1,n_2\geq25$. Both are positive, so the remaining conditions force $x,y\geq74$ and hence $n_1,n_2\leq26$. Their differences are at most one, so every such pair works. The complete equilibrium count vectors are

$$
\boxed{(25,25,50),\quad(25,26,49),\quad(26,25,49),\quad(26,26,48).}
$$

Each vector also represents many pure profiles obtained by choosing which labeled players use each route. Therefore the displayed equilibrium is not unique, even as an aggregate count vector.

A coordinated allocation with fifty players on each outer route and nobody on $ABCD$ gives every player delay $7/2$, strictly better than $15/4$. It is not a [Nash equilibrium](../../../../../nash-equilibrium.md): a first-route user can switch to $ABCD$ and obtain delay

$$
\frac94+\frac{50+51}{100}=\frac{163}{50}<\frac72.
$$

This exhibits the conflict between coordinated welfare and unilateral incentives. In fact $7/2$ is below every user's delay in all four pure equilibrium count vectors above.

For a [symmetric Nash equilibrium](../../../../../symmetric-nash-equilibrium.md) when $n=100$, let each player independently choose the two outer routes with [probability](../../../../../probability.md) $q$ each and the middle route with [probability](../../../../../probability.md) $1-2q$. Conditional on choosing the first route, that player certainly uses $AB$, while each of the other $99$ players uses it with [probability](../../../../../probability.md) $1-q$. The expected delays of the first and third routes are consequently

$$
\mathbb E C_1=3+\frac{1+99(1-q)}{100}=4-\frac{99q}{100},\qquad
\mathbb E C_3=\frac94+\frac{2+198(1-q)}{100}=\frac{17}{4}-\frac{198q}{100}.
$$

The second has the same expected delay as the first by symmetry. Equalizing these gives

$$
\boxed{\Pr(ABD)=\Pr(ACD)=\frac{25}{99},\qquad\Pr(ABCD)=\frac{49}{99}.}
$$

All three [probabilities](../../../../../probability.md) are positive and all three pure routes have expected delay $15/4$, so every route is a [best response](../../../../../best-response.md) to the other players' common mixture. This proves a symmetric mixed [Nash equilibrium](../../../../../nash-equilibrium.md). Using [probabilities](../../../../../probability.md) $1/4,1/4,1/2$ would omit the player's own-load correction and would not make all three expected delays equal.

For completeness, the same calculation works for every positive number of players. If $n\leq75$, every player choosing $ABCD$ is a symmetric pure [Nash equilibrium](../../../../../nash-equilibrium.md). For $75<n<149$, a symmetric mixed equilibrium has

$$
\Pr(ABD)=\Pr(ACD)=\frac{n-75}{n-1},\qquad
\Pr(ABCD)=\frac{149-n}{n-1}.
$$

For $n\geq149$, each player choosing either outer route with [probability](../../../../../probability.md) one half is a symmetric mixed equilibrium. In that last regime the unused middle route has expected cost at least that of the outer routes, since their difference is $-3/4+(n+1)/200\geq0$. These formulas agree at the regime boundaries.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
