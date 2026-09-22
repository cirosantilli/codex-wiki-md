<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite [bimatrix game](../../../../../bimatrix-game.md), let $A,B\in\mathbb R^{r\times s}$ be the two players' [payoff matrices](../../../../../payoff-matrix.md). A pair of [mixed strategies](../../../../../mixed-strategy.md) $(p,q)\in\Delta_r\times\Delta_s$ is a [Nash equilibrium](../../../../../nash-equilibrium.md) if

$$
p^TAq\geq (p')^TAq\quad\text{for all }p'\in\Delta_r,
\qquad p^TBq\geq p^TBq'\quad\text{for all }q'\in\Delta_s.
$$

Here $\Delta_r$ is the [probability simplex](../../../../../probability-simplex.md) on the first player's pure actions, and similarly for $\Delta_s$. The two [payoff matrices](../../../../../payoff-matrix.md) need not be negatives of each other. [Nash's theorem](../../../../../nash-s-theorem.md) asserts that **every finite two-person game has an equilibrium in mixed strategies**.

We prove it using the [Brouwer gain-map proof of bimatrix equilibrium](../../../../../brouwer-gain-map-proof-of-bimatrix-equilibrium.md). Put $u=p^TAq$, $v=p^TBq$ and define the positive pure-deviation gains

$$
g_i(p,q)=\max\{0,(Aq)_i-u\},\qquad
h_j(p,q)=\max\{0,(p^TB)_j-v\}.
$$

Write $G=\sum_i g_i$, $H=\sum_jh_j$ and define

$$
T(p,q)=\left(\left(\frac{p_i+g_i}{1+G}\right)_{i=1}^r,
\left(\frac{q_j+h_j}{1+H}\right)_{j=1}^s\right).
$$

Every coordinate is nonnegative and each player's coordinates sum to one. The map is continuous, since the payoffs and positive-part function are continuous and both denominators are at least one. Thus $T$ is a continuous self-map of the nonempty compact [convex set](../../../../../convex-set.md) $\Delta_r\times\Delta_s$. The [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) supplies a fixed point $(p,q)$.

At that fixed point the first coordinate equations give $g_i=Gp_i$. Suppose $G>0$. For every $i$ with $p_i>0$, this makes $g_i>0$, so $(Aq)_i-u=g_i=Gp_i$. But averaging the payoff excess over the support gives

$$
0=\sum_i p_i\bigl((Aq)_i-u\bigr)=G\sum_i p_i^2>0,
$$

a contradiction. Therefore $G=0$, and every $g_i$ is zero. Each pure action has payoff at most $u$, so every mixed deviation, being a [convex combination](../../../../../convex-combination.md) of pure actions, has payoff at most $u$ too. The same argument for $h_j=Hq_j$ gives $H=0$ and excludes every unilateral deviation by the second player. The fixed point is therefore a [Nash equilibrium](../../../../../nash-equilibrium.md), proving the stated theorem without a zero-sum assumption.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
