<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Nash equilibrium](../../../../../nash-equilibrium.md) of a multi-person game is a collection of strategies such that each player's strategy is a [best response](../../../../../best-response.md) to the others: no unilateral change raises that player's expected payoff. For [mixed strategies](../../../../../mixed-strategy.md), every pure action used with positive probability must attain the same maximal payoff. Take $c>0$.

In this [costly turnout game](../../../../../costly-turnout-game.md), compute the payoff difference between voting and abstaining, holding the others' strategies fixed. The opponent $A$ is pivotal exactly when one of $B,C$ votes. Without $A$ the proposition then passes, while with $A$ the tied ballot fails. The [pivotal voting probability](../../../../../pivotal-voting-probability.md) is $2\beta(1-\beta)$, so

$$
\Delta_A=8c\cdot2\beta(1-\beta)-3c
=c\bigl(16\beta(1-\beta)-3\bigr).
$$

If $A$ mixes with $0<\alpha<1$, indifference is necessary. Therefore

$$
\boxed{0<\alpha<1\ \Longrightarrow\
\beta(1-\beta)=\frac3{16},
\quad\beta=\frac14\ \text{or}\ \frac34.}
$$

For supporter $B$, voting is pivotal when $A$ abstains and $C$ abstains, or when $A$ votes and $C$ votes. Thus its voting advantage, and likewise that of $C$, is

$$
\Delta_B=\Delta_C
=4c\bigl((1-\alpha)(1-\beta)+\alpha\beta\bigr)-3c.
$$

At $(\alpha,\beta)=(1,3/4)$, this equals zero, while $\Delta_A=c(16(3/4)(1/4)-3)=0$. Every player is indifferent between voting and abstaining at these opponent strategies; in particular, $A$'s pure vote and both supporters' mixtures are [best responses](../../../../../best-response.md). Hence

$$
\boxed{(\alpha,\beta)=(1,3/4)\text{ is an equilibrium}.}
$$

It is not unique. At $(\alpha,\beta)=(0,1/4)$, both supporter advantages are $4c(3/4)-3c=0$, and $\Delta_A=0$ again. This gives a second [symmetric Nash equilibrium](../../../../../symmetric-nash-equilibrium.md). To see these are the only equilibria with a common supporter probability, note that $\beta=0$ or $1$ makes $\Delta_A=-3c$, forcing $\alpha=0$; neither endpoint then satisfies the supporters' [best response](../../../../../best-response.md) condition. For $0<\beta<1$, supporter indifference requires

$$
(1-\alpha)(1-\beta)+\alpha\beta=\frac34.
$$

If $A$ also mixes, its two possible values $\beta=1/4,3/4$ force $\alpha=0,1$ respectively, contradicting strict mixing. Finally $\alpha=0$ gives $\beta=1/4$, and $\alpha=1$ gives $\beta=3/4$. Thus

$$
\boxed{\text{The equilibria in the specified symmetric family are }
(0,1/4)\text{ and }(1,3/4).}
$$

Allowing $B,C$ to have distinct probabilities $\beta,\gamma$ gives two additional [Nash equilibria](../../../../../nash-equilibrium.md). The three voting advantages are

$$
\begin{aligned}
\Delta_A/c&=8\bigl(\beta(1-\gamma)+(1-\beta)\gamma\bigr)-3,\\
\Delta_B/c&=4\bigl((1-\alpha)(1-\gamma)+\alpha\gamma\bigr)-3,\\
\Delta_C/c&=4\bigl((1-\alpha)(1-\beta)+\alpha\beta\bigr)-3.
\end{aligned}
$$

If both supporters mix, subtracting their indifference equations gives $(2\alpha-1)(\gamma-\beta)=0$. At $\alpha=1/2$ a supporter has advantage $-c$, so cannot mix; hence $\beta=\gamma$ and the two symmetric equilibria result. If $B$ always abstains and $C$ mixes, the latter's indifference gives $\alpha=1/4$, and $A$'s indifference gives $\gamma=3/8$. Then $\Delta_B=-3c/4<0$, so abstention really is optimal. Interchanging $B,C$ gives the other equilibrium. If $B$ always votes and $C$ mixes, the corresponding equations give $\alpha=3/4$, $\gamma=5/8$, but $\Delta_B=-3c/4$, contradicting voting. The four configurations with both supporters pure also fail a [best response](../../../../../best-response.md) condition. Consequently the full collection of [turnout equilibria with two supporters and one opponent](../../../../../turnout-equilibria-with-two-supporters-and-one-opponent.md) is

$$
\boxed{(\alpha,\beta,\gamma)\in
\left\{(0,\tfrac14,\tfrac14),\
(1,\tfrac34,\tfrac34),\
(\tfrac14,0,\tfrac38),\
(\tfrac14,\tfrac38,0)\right\}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
