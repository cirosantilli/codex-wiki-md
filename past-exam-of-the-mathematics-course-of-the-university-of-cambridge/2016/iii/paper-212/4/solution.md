<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $u,v$ be the row and column [mixed strategies](../../../../../mixed-strategy.md), so their entries are nonnegative and sum to one. The payoffs are $u^{\mathsf T}Pv$ and $u^{\mathsf T}P^{\mathsf T}v$. A **[Nash equilibrium](../../../../../nash-equilibrium.md)** is a pair in which each strategy is a [best response](../../../../../best-response.md) to the other: neither player can improve its expected payoff by a unilateral change of [mixed strategy](../../../../../mixed-strategy.md). Equivalently, every positive-probability [pure strategy](../../../../../pure-strategy.md) attains that player's maximum pure-strategy payoff against the opposing mixture.

For the [complementarity construction of a symmetric Nash equilibrium](../../../../../complementarity-construction-of-a-symmetric-nash-equilibrium.md) put $s=\sum_i x_i>0$ and $u=x/s$. The equation $Px+z=\mathbf1$ gives $Px\leq\mathbf1$. Nonnegativity and $x^{\mathsf T}z=0$ imply $x_i>0\Rightarrow z_i=0\Rightarrow(Px)_i=1$. Therefore every used [pure strategy](../../../../../pure-strategy.md) has payoff $1/s$ against $u$, while all other [pure strategies](../../../../../pure-strategy.md) have payoff at most $1/s$. The same vector of pure-strategy payoffs applies to the column player in this symmetric [bimatrix game](../../../../../bimatrix-game.md). Thus **a symmetric [Nash equilibrium](../../../../../nash-equilibrium.md) is**

$$
\boxed{(u,u),\qquad u=\frac{x}{\sum_i x_i}.}
$$

For a genuine [Lemke-Howson algorithm](../../../../../lemke-howson-algorithm.md) path, use two separate vectors, $\xi$ for the row player and $\eta$ for the column player, with slacks

$$
P\eta+r=\mathbf1,\qquad P\xi+s=\mathbf1,\qquad \xi,\eta,r,s\geq0.
$$

Give labels $i=1,2,3$ to $\xi_i=0$ or $r_i=0$, and labels $3+j$ to $\eta_j=0$ or $s_j=0$. A nonzero completely labeled pair has $\xi_i r_i=0$ and $\eta_j s_j=0$, and normalization yields mutual [best responses](../../../../../best-response.md). At the artificial pair $(\xi,\eta)=(0,0)$ all six labels are present.

Drop label $3$ by increasing $\xi_3$. The two limiting rows of $P\xi\leq\mathbf1$ are $3\xi_3\leq1$ and $2\xi_3\leq1$, so the minimum-ratio pivot stops at $\xi_3=1/3$, where $s_2=0$. Label $5$ is now duplicated, since $\eta_2=0$ also carries it. Increase $\eta_2$ to remove that duplicate. The limiting inequalities are $3\eta_2\leq1$ and $4\eta_2\leq1$, so the next pivot stops at $\eta_2=1/4$, where $r_3=0$ restores the dropped label $3$. The endpoint is

$$
\xi=(0,0,1/3),\quad s=(1,0,1/3),\qquad \eta=(0,1/4,0),\quad r=(1/4,1,0).
$$

It has all six labels and satisfies both complementarity conditions. After normalization, **the [Lemke-Howson algorithm](../../../../../lemke-howson-algorithm.md) returns**

$$
\boxed{u=e_3,\qquad v=e_2.}
$$

Against column strategy $2$, row strategy $3$ pays $4$, exceeding $3$ and $0$. Against row strategy $3$, column strategy $2$ pays $3$, exceeding $0$ and $2$. This verifies the endpoint directly.

To find every other [Nash equilibrium](../../../../../nash-equilibrium.md), observe that row strategy $3$ strictly dominates row strategy $1$: the payoff differences against the three columns are $(2,1,2)$, all positive. By symmetry, column strategy $1$ is also [strictly dominated](../../../../../strict-dominance.md). Neither can appear in an equilibrium. The reduced strategies $2,3$ have row payoff matrix

$$
\begin{pmatrix}0&3\\4&2\end{pmatrix}.
$$

The two pure [Nash equilibria](../../../../../nash-equilibrium.md) are $(e_2,e_3)$ and $(e_3,e_2)$. If the opponent uses strategy $2$ with probability $q$, the payoffs of strategies $2,3$ are $3(1-q)$ and $2+2q$. Indifference requires $q=1/5$. The same computation applies to the other player. A player mixing both strategies forces this exact opposing mixture; a player playing a pure strategy has a unique opposing [best response](../../../../../best-response.md), producing one of the two pure equilibria. Hence **there are exactly three [Nash equilibria](../../../../../nash-equilibrium.md)**:

$$
\boxed{(e_2,e_3),\quad(e_3,e_2),\quad\bigl((0,1/5,4/5),(0,1/5,4/5)\bigr).}
$$

For the symmetric mixed equilibrium, the original complementarity construction can use $x=(0,1/12,1/3)$ and $z=(3/4,0,0)$; it gives payoff $12/5$ to each player after normalization.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 212](../../paper-212-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
