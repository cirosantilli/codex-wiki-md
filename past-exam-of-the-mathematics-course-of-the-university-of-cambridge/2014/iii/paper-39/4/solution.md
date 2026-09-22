<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We derive the probabilities for a [sequential elimination all-pay contest](../../../../../sequential-elimination-all-pay-contest.md) from a discounted [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md), using [backward induction](../../../../../backward-induction.md), and only then take $\delta\uparrow1$. This preserves the selection supplied by discounting.

First consider a two-player [all-pay auction](../../../../../all-pay-auction.md) with effective prizes $A_1\geq A_2>0$, so the incremental payoff is $A_i$ times [winning probability](../../../../../winning-probability.md) minus effort. For $0\leq b\leq A_2$, the independent [mixed strategies](../../../../../mixed-strategy.md) have effort [cumulative distribution functions](../../../../../cumulative-distribution-function.md)

$$
G_1(b)=\frac b{A_2},\qquad
G_2(b)=1-\frac{A_2}{A_1}+\frac b{A_1}.
$$

The second player has an atom $1-A_2/A_1$ at zero. For positive bids on this support, the first player's payoff is $A_1G_2(b)-b=A_1-A_2$ and the second's is $A_2G_1(b)-b=0$. Bids above $A_2$ cannot improve either payoff. The first has no zero atom, so the second's zero bid also earns zero. If the first deviates to zero, it can win only when the second bids zero; even with every such tie resolved in its favor, its payoff is at most $A_1(1-A_2/A_1)=A_1-A_2$. The [two-player complete-information all-pay equilibrium](../../../../../two-player-complete-information-all-pay-equilibrium.md) therefore has [winning probabilities](../../../../../winning-probability.md)

$$
\boxed{p_1=1-\frac{A_2}{2A_1},\qquad p_2=\frac{A_2}{2A_1}.}
$$

These follow by integrating $G_2$ against the uniform $G_1$. A third player with effective prize at most $A_2$ cannot profit by entering: for $0<b\leq A_2$, its [winning probability](../../../../../winning-probability.md) is $G_1(b)G_2(b)\leq b/A_2$, giving payoff at most zero; above $A_2$ its effort exceeds its prize.

For the dynamic induction, relabel any remaining subgame's valuations as $v_1>\cdots>v_k$, with $r<k$ prizes left. Define the [backward-induction threshold in an elimination all-pay contest](../../../../../backward-induction-threshold-in-an-elimination-all-pay-contest.md)

$$
C_r=(1-\delta)\sum_{j=2}^{r}\delta^{j-2}v_j+\delta^{r-1}v_{r+1}.
$$

For $r=1$ the sum is empty and $C_1=v_2$. The [discounted continuation value in an elimination contest](../../../../../discounted-continuation-value-in-an-elimination-contest.md) is obtained from the following net utilities:

$$
\begin{aligned}
J_1&=v_1-C_r,\\
J_i&=\delta^{i-1}\left[v_i-(1-\delta)\sum_{j=i+1}^{r}\delta^{j-i-1}v_j-\delta^{r-i}v_{r+1}\right],&&2\leq i\leq r,\\
J_i&=0,&&i\geq r+1.
\end{aligned}
$$

The base case is the one-prize [all-pay auction](../../../../../all-pay-auction.md): only the two highest valuations need positive effort, with prizes $v_1,v_2$ and payoffs $v_1-v_2,0$. Every lower player has a nonprofitable deviation by the preceding calculation.

For $r\geq2$, if either of the top two wins, the other becomes the highest player in a subgame with $r-1$ prizes. The continuation threshold in either such subgame is the same number

$$
D=(1-\delta)\sum_{j=3}^{r}\delta^{j-3}v_j+\delta^{r-2}v_{r+1}.
$$

The remaining top player's continuation payoff is $v_i-D$. Its [effective prize in a sequential contest](../../../../../effective-prize-in-a-sequential-contest.md), net of the discounted payoff from losing, is therefore

$$
A_1=(1-\delta)v_1+\delta D,\qquad
A_2=(1-\delta)v_2+\delta D=C_r.
$$

Thus $A_1>A_2$ for $\delta<1$, and the two-player distributions above apply. Adding the losing-state baselines gives

$$
J_1=\delta(v_1-D)+(A_1-A_2)=v_1-C_r,\qquad
J_2=\delta(v_2-D)=v_2-C_r,
$$

which agree with the proposed formulas.

For a player of rank $i\geq3$, the inductive continuation utility after either top player wins is identical: its new rank is $i-1$, and the utility expression depends only on its own value and the lower-valued tail. Thus its current zero-effort payoff is that common continuation value multiplied by $\delta$, exactly the stated $J_i$. Its effective prize for deviating to win now is $A_i=v_i-J_i$. For $3\leq i\leq r$, direct subtraction gives

$$
C_r-A_i=(1-\delta)\sum_{j=2}^{i-1}\delta^{j-2}(v_j-v_i)>0.
$$

For $i\geq r+1$, $A_i=v_i\leq v_{r+1}\leq C_r$, since the coefficients in $C_r$ are nonnegative and sum to one. Such a player cannot gain by entering against the two active players. There is one additional zero-bid deviation to check for the highest player. If both active bids become zero, the tie could award a prize to any remaining player. Losing to any player below rank $2$ gives no greater continuation utility than losing to rank $2$: deleting rank $2$ makes the ordered remaining rival list componentwise smallest, and its continuation threshold is a nonnegative weighted sum of that list. Thus even resolving every all-zero tie in the highest player's favor gives payoff at most its usual losing baseline plus $A_1(1-A_2/A_1)=A_1-A_2$. No tie rule can improve this deviation. This verifies all [best responses](../../../../../best-response.md) and the continuation-utility formulas. Applying the construction to every remaining-player set proves a [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md) of the discounted contest, not merely an on-path prescription.

Now take the [vanishing-discount limit of an elimination all-pay contest](../../../../../vanishing-discount-limit-of-an-elimination-all-pay-contest.md). At every nonfinal subgame,

$$
A_1,A_2\longrightarrow v_{r+1},\qquad p_1,p_2\longrightarrow\frac12.
$$

Thus the two highest remaining players win with equal probabilities in a nonfinal stage. In the final stage the effective prizes are their actual valuations, so its lower-valued participant beats the higher one with probability equal to half their valuation ratio.

Return to the original ranks. Only the original top $m+1$ can ever win; at most $m-1$ higher players can have left before the final stage, so players of rank $m+2$ or worse never enter its top pair. Player $1$ must lose $m-1$ fair nonfinal contests to remain unawarded until the final stage, where its opponent has value $v_{m+1}$. Hence

$$
1-x_1=2^{-(m-1)}\frac{v_{m+1}}{2v_1}.
$$

A player $2\leq i\leq m$ first enters the top pair at stage $i-1$, after $i-2$ higher-ranked winners have left. To remain unawarded, it must lose the $m-i+1$ nonfinal contests from then on, followed by the final contest against rank $m+1$. Therefore

$$
1-x_i=2^{-(m-i+1)}\frac{v_{m+1}}{2v_i}.
$$

There are exactly $m$ distinct winners, so the [expected value](../../../../../expected-value.md) of their indicator sum is $m$. Combining these calculations gives

$$
\boxed{x_1=1-2^{-m}\frac{v_{m+1}}{v_1},\qquad
x_i=1-2^{-(m-i+2)}\frac{v_{m+1}}{v_i}\ (2\leq i\leq m),}
$$



$$
\boxed{x_{m+1}=m-\sum_{j=1}^m x_j,\qquad x_i=0\ (i\geq m+2).}
$$

This proves the [ranked winning probabilities in an undiscounted elimination contest](../../../../../ranked-winning-probabilities-in-an-undiscounted-elimination-contest.md). When $m=1$, it reduces to the ordinary two-player all-pay [winning probabilities](../../../../../winning-probability.md); when $m>1$, the repeated fair stages explain each power of $1/2$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
