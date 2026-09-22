<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For decision problems, the usual meaning of “no harder” is a [polynomial-time reduction](../../../../../polynomial-time-reduction.md): $\Pi\leq_p\Pi'$ if there is a polynomial-time computable map $f$ taking each instance $x$ of $\Pi$ to an instance of $\Pi'$ such that $x$ is a yes-instance exactly when $f(x)$ is. A [polynomial-time algorithm](../../../../../polynomial-time-algorithm.md) for $\Pi'$ would then solve $\Pi$ in polynomial time. A problem is [NP-hard](../../../../../np-hardness.md) if every problem in [NP](../../../../../np-complexity.md) admits such a reduction to it.

For a [zero-sum game](../../../../../zero-sum-game.md) with rational [payoff matrix](../../../../../payoff-matrix.md) $A$, the row player can calculate its value by [linear programming](../../../../../linear-programming.md):

$$
\max v\quad\text{subject to}\quad
p\geq0,\quad \mathbf1^\top p=1,\quad A^\top p\geq v\mathbf1.
$$

The [minimax theorem](../../../../../minimax-theorem.md) identifies this optimum with the game value. Rational [linear programming](../../../../../linear-programming.md) has [polynomial-time algorithms](../../../../../polynomial-time-algorithm.md), and an optimal rational value can be compared exactly with rational $V$ in polynomial time in the binary input length. Thus the decision problem belongs to [P](../../../../../p-complexity.md). If it were [NP-hard](../../../../../np-hardness.md), composing the reductions with this algorithm would put every problem in [NP](../../../../../np-complexity.md) in [P](../../../../../p-complexity.md), contradicting the assumed separation. Therefore

$$
\boxed{\mathbf P\neq\mathbf{NP}\ \Longrightarrow\
\text{deciding whether a rational zero-sum game has value }V
\text{ is not NP-hard}.}
$$

The finite rational encoding is part of the computational model; arbitrary real inputs without an encoding would not define the same complexity question.

For the [set cover reduction to equilibrium support](../../../../../set-cover-reduction-to-equilibrium-support.md), first take $2\leq k<m$ and assume every element belongs to some subset. Suppose rows $i_1,\ldots,i_k$ cover $S$. Let player 1 use the uniform [mixed strategy](../../../../../mixed-strategy.md) on these rows and let player 2 play column $0$. The row player's payoff is one for every row, so any row mixture is a [best response](../../../../../best-response.md) to column $0$. If $q_j$ denotes the probability that a random supported row covers element $j$, then $q_j\geq1/k$, and player 2's payoff from column $j>0$ is

$$
\frac{k}{k-1}(1-q_j)\leq
\frac{k}{k-1}\left(1-\frac1k\right)=1.
$$

Column $0$ also pays one. It is therefore a [best response](../../../../../best-response.md), giving a [Nash equilibrium](../../../../../nash-equilibrium.md) whose row-player [support of a mixed strategy](../../../../../support-of-a-mixed-strategy.md) contains exactly $k$ rows.

Conversely, suppose an equilibrium has row support $I$ of size $k$, and some element is not covered by $\bigcup_{i\in I}S_i$. For that column $q_j=0$, so player 2 can earn $k/(k-1)>1$. This is the largest possible column payoff, and it is attained exactly at columns corresponding to elements uncovered by $I$. The column player's [mixed strategy](../../../../../mixed-strategy.md) must consequently put all its probability on these columns, with none on column $0$. Every currently supported row gives player 1 payoff zero. Choose any positive-probability column $j$; because $\bigcup_iS_i=S$, there is some row $i'$ containing $j$. Deviating to $i'$ gives strictly positive expected payoff, contradicting the [best response](../../../../../best-response.md) condition. Thus $I$ must be a cover, proving

$$
\boxed{\text{a cover by }k\text{ subsets exists}
\iff\text{an equilibrium with row support exactly }k\text{ exists}}
$$

under the stated union and $k\geq2$ conditions.

The printed formulation omits both conditions. For $k=1$, its payoffs contain division by zero. Without the union condition its claimed implication is false: take $n=2$, $m=3$, $k=2$ and $S_1=S_2=S_3=\{1\}$. No selection covers $S=\{1,2\}$, but any row mixture supported on two rows, paired with pure column $2$, is a [Nash equilibrium](../../../../../nash-equilibrium.md). The row player always gets zero, and column $2$ is the column player's strictly optimal choice with payoff two. This gives an explicit counterexample to the unrestricted wording.

These restrictions do not weaken the complexity conclusion. The [set cover problem](../../../../../set-cover-problem.md) remains [NP-complete](../../../../../np-completeness.md) when every element occurs in some subset and $k\geq2$: globally uncovered elements and the easy cases $k=0,1$ can be recognized and replaced by fixed promised yes- or no-instances. A cover by at most $k<m$ subsets can be padded to exactly $k$. The constructed game has polynomial size, so deciding whether a [Nash equilibrium](../../../../../nash-equilibrium.md) of the specified support size exists is [NP-hard](../../../../../np-hardness.md). Computing a complete description of all equilibria would resolve this question and hence is at least this difficult. In addition, the equilibrium set may be infinite; a complete output must then describe families rather than list individual points. There is a finite representation by feasible pairs of supports and their associated strategy polytopes, but there are exponentially many support pairs to consider. This reduction concerns locating specified supports or describing all equilibria, rather than finding one unrestricted equilibrium.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
