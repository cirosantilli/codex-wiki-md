<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a [bimatrix game](../../../../../bimatrix-game.md) with row and column payoff [matrices](../../../../../matrix.md) $A,B$, an equilibrium pair is a pair of [mixed strategies](../../../../../mixed-strategy.md) $(p,q)$ for which neither player gains by a unilateral change:

$$
p^TAq\ge {p'}^TAq\quad\text{for every }p',\qquad
p^TBq\ge p^TBq'\quad\text{for every }q'.
$$

This is a [Nash equilibrium](../../../../../nash-equilibrium.md), or mutual [best response](../../../../../best-response.md) pair. Every finite game with nonempty finite pure-strategy sets has at least one mixed-strategy equilibrium by [Nash's theorem](../../../../../nash-s-theorem.md). Equivalently, the strategy domains are compact convex probability simplexes and the expected payoffs are continuous and linear in each player's own strategy. The existence assertion need not hold if only [pure strategies](../../../../../pure-strategy.md) are allowed.

Write the probability vectors in the order Bach, Mozart, Schubert. Against $q=(q_B,q_M,q_S)$ the row player's three pure-action payoffs are

$$
4q_B+q_M,\qquad 2q_M,\qquad3q_S.
$$

Against $p=(p_B,p_M,p_S)$ the column player's payoffs are

$$
2p_B,\qquad p_B+4p_M,\qquad3p_S.
$$

A supported action must attain the corresponding maximum, and an omitted action must give no larger payoff.

We first justify that both players have the same [support of a mixed strategy](../../../../../support-of-a-mixed-strategy.md), rather than assume it. Each player's maximum payoff is strictly positive for every opponent probability vector. Thus $p_M>0$ implies $q_M>0$, $q_B>0$ implies $p_B>0$, and $p_S>0$ is equivalent to $q_S>0$. If $p_B>0$ but $q_B=0$, then either $q_M>0$, making Mozart's payoff $2q_M$ strictly exceed Bach's $q_M$, or $q_S=1$, making Bach's payoff zero and Schubert's positive. Both contradict [best response](../../../../../best-response.md). Therefore $p_B>0$ also implies $q_B>0$. Similarly, if $q_M>0$ but $p_M=0$, then $p_B>0$ makes the column payoff for Bach $2p_B$ exceed Mozart's $p_B$, or $p_S=1$ makes Mozart's payoff zero and Schubert's positive. Thus $q_M>0$ implies $p_M>0$. The supports coincide, and there are only seven nonempty possibilities.

For singleton supports the three matching pure pairs are equilibria. For each two-element support, solve the two players' indifference equations and normalize their probabilities. For example, on Bach–Mozart, the equations are $4q_B=q_M$ and $p_B=4p_M$, giving $q=(1/5,4/5,0)$ and $p=(4/5,1/5,0)$. On Bach–Schubert they are $4q_B=3q_S$ and $2p_B=3p_S$. On Mozart–Schubert they are $2q_M=3q_S$ and $4p_M=3p_S$. In each case the omitted action gives strictly less than the common supported payoff.

For full support, the row indifference equations give $q_M=4q_B$ and $3q_S=2q_M$; the column equations give $p_B=4p_M$ and $3p_S=2p_B$. Normalization determines the remaining pair. The full list, with row strategy first, is

$$
\boxed{
\begin{array}{c|c|c}
\text{support}&p&q\\\hline
B&(1,0,0)&(1,0,0)\\
M&(0,1,0)&(0,1,0)\\
S&(0,0,1)&(0,0,1)\\
B,M&(4/5,1/5,0)&(1/5,4/5,0)\\
B,S&(3/5,0,2/5)&(3/7,0,4/7)\\
M,S&(0,3/7,4/7)&(0,3/5,2/5)\\
B,M,S&(12/23,3/23,8/23)&(3/23,12/23,8/23).
\end{array}}
$$

All displayed supported probabilities are positive. The supported payoff pairs in the four nonpure cases are respectively $(8/5,8/5)$, $(12/7,6/5)$, $(6/5,12/7)$ and $(24/23,24/23)$; these values also verify the omitted-action inequalities directly. The common-support argument excludes every other support pair, and each indifference system has a unique solution. Hence **there are exactly seven equilibrium pairs**, three pure and four genuinely mixed. This is a complete [support enumeration for a bimatrix game](../../../../../support-enumeration-for-a-bimatrix-game.md), not just a list of selected equilibria.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
