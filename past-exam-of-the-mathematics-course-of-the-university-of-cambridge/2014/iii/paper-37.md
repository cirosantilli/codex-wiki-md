# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_37.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [Charnes-Cooper transformation](../../../mathematical-optimization.md#charnes-cooper-transformation) on the positive-denominator region:

$$
t=\frac1{d^Tx+\beta},\qquad y=tx.
$$

It gives $Ay\le bt$, $d^Ty+\beta t=1$ and $c^Ty+\alpha t=(c^Tx+\alpha)/(d^Tx+\beta)$.

We must check that allowing $t=0$ introduces no false feasible solution. If $t=0$, then $Ay\le0$. The [recession cone](../../../mathematical-optimization.md#recession-cone) of the nonempty [linear polyhedron](../../../mathematical-optimization.md#linear-polyhedron) $P=\{x:Ax\le b\}$ is $\{y:Ay\le0\}$. Indeed for $x_0\in P$, $x_0+uy\in P$ for every $u\ge0$. Boundedness of $P$ therefore forces $y=0$, contradicting $d^Ty=1$. Thus every transformed feasible point has $t>0$.

Conversely set $x=y/t$. The constraints give $x\in P$ and $d^Tx+\beta=1/t>0$, with the same objective value. The assumed original optimizer with positive denominator supplies a transformed feasible point. Every transformed point corresponds to an original point and has objective at most that optimizer's value. Hence **the transformed [linear program](../../../mathematical-optimization.md#linear-programming) attains the original optimum, and its optimizer recovers $x=y/t$.** Positivity on every point of $P$ is not needed here; the given positive-denominator optimum suffices.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The feasible triangle has vertices

$$
v_1=(18/7,2/7),\qquad v_2=(12/11,14/11),\qquad v_3=(2/5,-4/5).
$$

These come from the three pairs of active boundary lines and satisfy the remaining inequalities. Its denominator $3x_1+x_2+2$ is positive at each vertex, with minimum $12/5$, so is positive throughout the triangle because it is an [affine function](../../../vector-space.md#affine-function).

For a direct [linear programming optimality certificate](../../../mathematical-optimization.md#linear-programming-optimality-certificate), add twice the second inequality to the third to get $-x_1-3x_2\le2$. Thus $x_1+3x_2+2\ge0$, equivalently $2(x_1-x_2)\le3x_1+x_2+2$. Division by the positive denominator gives an objective at most $1/2$. Both inequalities used in the bound are equalities at $v_3$, where the first inequality is also satisfied. Therefore

$$
\boxed{x^*=(2/5,-4/5),\qquad\max\frac{x_1-x_2}{3x_1+x_2+2}=\frac12.}
$$

Equality requires the two bounding inequalities to be tight, so this optimizer is unique.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The feasible point $x=(8/5,0,1/5)$ makes the second and third constraints tight; the first has left side two. Its objective is $27/5$.

To prove optimality from first principles, multiply each of the second and third inequalities by $3/5$ and add. For every nonnegative feasible $x$,

$$
3x_1+x_2+3x_3\le3x_1+\frac{12}5x_2+3x_3\le\frac35(5+4)=\frac{27}5.
$$

This is an explicit [weak duality](../../../mathematical-optimization.md#weak-duality) bound, proved here simply by adding inequalities. The displayed point attains it, so

$$
\boxed{\phi(0)=27/5,\qquad x^*=(8/5,0,1/5).}
$$

Equality forces $x_2=0$ and both contributing constraints tight, proving uniqueness as well.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The same [weak duality](../../../mathematical-optimization.md#weak-duality) certificate gives the upper bound $(27+3\epsilon_2+3\epsilon_3)/5$ for every feasible point. Keep $x_2=0$ and solve the tight second and third constraints:

$$
x_1=\frac{16+4\epsilon_2-\epsilon_3}{10},\qquad x_3=\frac{2-2\epsilon_2+3\epsilon_3}{10}.
$$

These are nonnegative precisely when their numerators are nonnegative. The remaining first-constraint slack is $4+\epsilon_1-\epsilon_3/2$. All three are positive for sufficiently small perturbations, so the point is feasible and attains the bound. This illustrates [linear programming sensitivity within a fixed optimal basis](../../../mathematical-optimization.md#linear-programming-sensitivity-within-a-fixed-optimal-basis):

$$
\boxed{\phi(\epsilon)=\frac{27+3\epsilon_2+3\epsilon_3}5\quad\text{near }0.}
$$

More generally this expression is valid throughout the region specified by those three feasibility inequalities.

With $\epsilon_1=\epsilon_2=0$, the conditions reduce to

$$
\boxed{-\frac23\le\epsilon_3\le8.}
$$

The endpoints are included. Outside this interval the bound cannot be attained: its equality conditions require exactly the point above, which then has a negative $x_3$ or violates the first constraint. Whenever feasible, the problem attains a maximum because the first constraint and nonnegativity bound all coordinates, so its value is strictly smaller outside the interval. For $\epsilon_3<-4$ it is infeasible. Thus the range is exact, not just a sufficient neighborhood.

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use safety for failure counts within the available components, equivalently tolerance of up to that many failures. An exact-count condition with more failures than components would otherwise be vacuous. Assume the client is not itself a server; that exceptional case needs no network connection.

Create a [flow network](../../../graph-theory.md#flow-network) by replacing each undirected link by two oppositely directed arcs of capacity one. Add a new sink $z$ and arcs from every server to $z$, each of capacity $B=|E|+1$. Find a [maximum flow](../../../graph-theory.md#maximum-flow-problem) from $c$ to $z$ with the [Edmonds–Karp algorithm](../../../graph-theory.md#edmonds-karp-algorithm). By the [max-flow min-cut theorem](../../../graph-theory.md#max-flow-min-cut-theorem), its value $\lambda$ is the minimum cut capacity. A cut using a server-to-sink arc costs at least $B$, whereas cutting all original links costs at most $|E|$, so a minimum cut uses none of the added arcs.

A source-side cut therefore contains no server. Each original undirected edge crossing it contributes exactly one of its two arcs, so its capacity is the number of original links separating the client from every server. Conversely, if a set of failed links disconnects all servers, the vertices still reachable from $c$ define a cut contained in that failed set. Thus $\lambda$ is exactly the minimum number of links whose failure can disconnect the client from all servers. This is [server connectivity under component failures](../../../graph-theory.md#server-connectivity-under-component-failures).

Deleting fewer than $\lambda$ links leaves some connection, while deleting a minimum cut destroys every connection. Therefore

$$
\boxed{k_{\max}=\lambda-1.}
$$

If $\lambda=0$, the network is already disconnected and has no nonnegative safe failure count. The transformed graph has $|V|+1$ vertices and $2|E|+|S|$ arcs. The [Edmonds–Karp algorithm](../../../graph-theory.md#edmonds-karp-algorithm) runs in $O(|V'||E'|^2)$ steps, so both the construction and computation are polynomial in the original graph size.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use [vertex splitting](../../../graph-theory.md#vertex-splitting) to encode node failures as well as link failures. Replace each vertex $v$ by $v_{\rm in},v_{\rm out}$ and an internal arc $v_{\rm in}\to v_{\rm out}$. Give that arc capacity one for an intermediary node, and capacity $B=|E|+|V|+1$ for the client and servers. Replace an undirected link $uv$ by arcs $u_{\rm out}\to v_{\rm in}$ and $v_{\rm out}\to u_{\rm in}$, each of capacity one. Connect server outputs to a common sink with capacity $B$ and take $c_{\rm out}$ as source.

A minimum cut avoids capacity-$B$ arcs because failure of all original links provides a cheaper separating set. We can normalize its source side so that $v_{\rm out}$ being on that side implies $v_{\rm in}$ is also there: moving $v_{\rm in}$ to that side cannot increase the cut capacity, since its sole outgoing arc leads to $v_{\rm out}$. In such a cut, at most one direction of any original link crosses. Every unit internal arc crossing corresponds to failing its intermediary node; every unit link arc corresponds to failing that link. Their failures disconnect all servers, so the cut capacity is the cost of a real failure set.

Conversely remove the internal arcs of failed nodes and both arcs of failed links. The reachable-side cut contains only arcs corresponding to those failures, with at most one crossing orientation per failed link; its capacity is at most their number. The [max-flow min-cut theorem](../../../graph-theory.md#max-flow-min-cut-theorem) thus identifies the minimum mixed failure count $\lambda_{\rm mix}$ exactly. Hence

$$
\boxed{\text{the network is }m\text{-safe if and only if }\lambda_{\rm mix}>m.}
$$

The split graph has $O(|V|)$ vertices and $O(|E|+|V|+|S|)$ arcs, so the same [Edmonds–Karp algorithm](../../../graph-theory.md#edmonds-karp-algorithm) gives a polynomial-time decision procedure.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Name the outer pentagon vertices, in order from the client clockwise, $c,T,R,B,L$. Name the upper inner vertex $U$, the left inner vertex $A$, and the lower-right inner vertex $D$. The two remaining inner vertices are the labelled servers $s_1,s_2$.

Four edge-disjoint server paths are

$$
c-A-s_1,\qquad c-U-s_2,\qquad c-T-R-B-D-s_2,\qquad c-L-A-U-D-s_1.
$$

Each uses different links, although some intermediary vertices are shared. Any three failed links therefore leave at least one path intact. The client has exactly four incident links; failing those four disconnects it. Thus the minimum link cut has size four, giving

$$
\boxed{k_{\max}=3.}
$$

For mixed failures use the three paths $c-A-s_1$, $c-U-s_2$ and $c-T-R-B-D-s_1$. Their internal vertices are disjoint, as are their links. One failed link or intermediary node can destroy at most one of these paths, so any two failures leave a path intact. Failing the three intermediary nodes $A,U,D$ disconnects both servers: $s_1$ has neighbors $A,D$, and $s_2$ has neighbors $U,D$. Therefore

$$
\boxed{m_{\max}=2.}
$$

The two certificates distinguish [edge-disjoint paths](../../../graph-theory.md#edge-disjoint-paths) from [internally vertex-disjoint paths](../../../graph-theory.md#internally-vertex-disjoint-paths), exactly the distinction needed between the two failure models.

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use net monetary gain as payoff and order each player's [pure strategies](../../../game-theory.md#pure-strategy) as $1,2,4$. The [payoff matrix](../../../game-theory.md#payoff-matrix) for the first player is

$$
\boxed{A=\begin{pmatrix}0&2&-1\\1&0&-2\\-4&-4&0\end{pmatrix}.}
$$

The second player's matrix is $-A$. Equal choices return both stakes, so the diagonal is zero; when the first player wins, their net gain is the other's stake, and when they lose it is minus their own stake. This is a [matrix game](../../../game-theory.md#matrix-game), hence a [zero-sum game](../../../game-theory.md#zero-sum-game) and a [normal-form game](../../../game-theory.md#normal-form-game).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The game is degenerate in the [nondegeneracy of a bimatrix game](../../../game-theory.md#nondegeneracy-of-a-bimatrix-game) sense. Against the first player's [pure strategy](../../../game-theory.md#pure-strategy) $4$, the second player's choices $1$ and $2$ are both [best responses](../../../game-theory.md#best-response), with payoff four. A [mixed strategy](../../../game-theory.md#mixed-strategy) of support size one therefore has two pure [best responses](../../../game-theory.md#best-response). The usual [Lemke-Howson algorithm](../../../game-theory.md#lemke-howson-algorithm) path needs additional tie handling or perturbation in such a game; the [zero-sum game](../../../game-theory.md#zero-sum-game) structure gives a simpler direct [linear program](../../../mathematical-optimization.md#linear-programming).

Add five to every entry of the first player's matrix, obtaining

$$
B=\begin{pmatrix}5&7&4\\6&5&3\\1&1&5\end{pmatrix}.
$$

This does not change either player's [best responses](../../../game-theory.md#best-response) or [Nash equilibria](../../../game-theory.md#nash-equilibrium); it raises the game value by five. Since all entries are positive, its value $v_B$ is positive. If $p$ is a row [mixed strategy](../../../game-theory.md#mixed-strategy) guaranteeing $v_B$, put $x=p/v_B$. Then $B^Tx\ge\mathbf1$ and $\mathbf1^Tx=1/v_B$.

Conversely any feasible $x$ has $s=\mathbf1^Tx>0$, and $p=x/s$ guarantees payoff $1/s$ in the shifted game. Maximizing that guaranteed payoff is therefore equivalent to minimizing $s$ under $B^Tx\ge\mathbf1$, $x\ge0$. These are precisely the displayed constraints. The dual program maximizes $\mathbf1^Ty$ subject to $By\le\mathbf1$, $y\ge0$; normalizing an optimal $y$ gives the column strategy. This is [positive-payoff linear programming for a matrix game](../../../game-theory.md#positive-payoff-linear-programming-for-a-matrix-game).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Introduce nonnegative surplus variables

$$
r_1=5x_1+6x_2+x_3-1,\quad r_2=7x_1+5x_2+x_3-1,\quad r_3=4x_1+3x_2+5x_3-1.
$$

At the proposed starting [basic feasible solution](../../../mathematical-optimization.md#basic-feasible-solution), the basic variables are $x_1,r_1,r_2$ and the nonbasic variables are $x_2,x_3,r_3$. Its [simplex dictionary](../../../numerical-analysis.md#simplex-dictionary), with objective $z=x_1+x_2+x_3$, is

$$
\begin{aligned}
x_1&=(1-3x_2-5x_3+r_3)/4,\\
r_1&=(1+9x_2-21x_3+5r_3)/4,\\
r_2&=(3-x_2-31x_3+7r_3)/4,\\
z&=(1+x_2-x_3+r_3)/4.
\end{aligned}
$$

Increase $x_3$ to decrease $z$. The [simplex ratio test](../../../mathematical-optimization.md#simplex-ratio-test) gives limits $1/5$ from $x_1$, $1/21$ from $r_1$, and $3/31$ from $r_2$. The smallest is $1/21$, so $x_3$ enters and $r_1$ leaves. After this single pivot the dictionary is

$$
\begin{aligned}
x_1&=(4+5r_1-r_3-27x_2)/21,\\
x_3&=(1-4r_1+5r_3+9x_2)/21,\\
r_2&=(8+31r_1-2r_3-75x_2)/21,\\
z&=(5+r_1+4r_3+3x_2)/21.
\end{aligned}
$$

All objective coefficients of nonbasic variables are strictly positive. Thus the [simplex method](../../../mathematical-optimization.md#simplex-method) has reached its unique optimum:

$$
\boxed{x=(4/21,0,1/21),\qquad z=5/21.}
$$

The feasible dual vector $y=(1/21,0,4/21)$ has the same objective, providing an independent [weak duality](../../../mathematical-optimization.md#weak-duality) certificate. Normalization gives

$$
\boxed{p=(4/5,0,1/5),\qquad q=(1/5,0,4/5),\qquad v=21/5-5=-4/5.}
$$

These are all the equilibria: the dual's strict slack in row two forces $p_2=0$, and the primal's strict slack in column two forces $q_2=0$. Equality of the two active row and column payoffs then fixes the displayed [probabilities](../../../probability-theory.md#probability). The value is the first player's expected net loss; the second gains $4/5$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For a fixed number choice, increasing one's own stake changes only the amount lost when one loses. It does not change the amount won, which is the opponent's stake, or the zero payoff of a tie. Thus doubling is either [weakly dominated](../../../game-theory.md#weakly-dominated-strategy) by retaining the original stake or [payoff-equivalent](../../../game-theory.md#payoff-equivalent-strategies) to it. This establishes that there is no strategic advantage in doubling, but does not imply strict harm in every equilibrium.

For the first player, each of the two equilibrium choices loses with positive [probability](../../../probability-theory.md#probability): choice one loses against the second player's four, and choice four loses against their one. Doubling either therefore gives a strictly smaller expected payoff than $-4/5$. By contrast, against the first player's support $\{1,4\}$, the second player's choices one and four either win or tie. Their own stake is never lost, so doubling it does not change their payoff.

More precisely, retain the first player's original-stake [probabilities](../../../probability-theory.md#probability) $(4/5,0,1/5)$. The second player may split their total [probability](../../../probability-theory.md#probability) $1/5$ on choice one, and $4/5$ on choice four, arbitrarily between original and double stakes. The first player's unused choice two has payoff at most $(1/5)2-(4/5)2=-6/5<-4/5$, even when the second player doubles their one stake. The doubled first-player choices are also worse. The second player's choice two, with either stake, is worse against the displayed first-player strategy. Hence these splits remain [Nash equilibria](../../../game-theory.md#nash-equilibrium) of the enlarged [zero-sum game](../../../game-theory.md#zero-sum-game).

**The first player should not double; the second player is indifferent between doubling and retaining the original stakes on their equilibrium choices.** This distinction is an example of [weak domination does not exclude equilibrium strategies](../../../game-theory.md#weak-domination-does-not-exclude-equilibrium-strategies).

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Give each permanent member weight seven, each nonpermanent member weight one, and use the strict threshold $t=38$. If a [coalition](../../../game-theory.md#coalition-game-theory) omits a permanent member, its weight is at most $4\cdot7+10=38$, so it loses. If it includes all five permanent members and $r$ others, its weight is $35+r$, which exceeds 38 exactly when $r\ge4$. These are precisely the required winning [coalitions](../../../game-theory.md#coalition-game-theory). Thus a [weighted voting game](../../../game-theory.md#weighted-voting-game) representation is

$$
\boxed{w_i=7\text{ for permanent members},\quad w_i=1\text{ otherwise},\quad t=38.}
$$

The strict-threshold convention is important: in the alternative convention requiring weight at least the quota, the quota is 39.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For a [simple cooperative game](../../../game-theory.md#simple-cooperative-game), the [Shapley value](../../../game-theory.md#shapley-value) is the [probability](../../../probability-theory.md#probability) that a player is pivotal in a uniformly random ordering. Symmetry gives one value for permanent members and another for nonpermanent members.

A particular nonpermanent member is pivotal exactly when all five permanent members and exactly three of the other nine nonpermanent members precede them. The predecessor set then has size eight. There are $\binom93$ such sets, each giving $8!6!$ orderings. Their [Shapley value](../../../game-theory.md#shapley-value) is therefore

$$
\beta=\binom93\frac{8!6!}{15!}=\frac4{2145}.
$$

Every ordering has exactly one pivotal member, since the empty [coalition](../../../game-theory.md#coalition-game-theory) loses and the full [coalition](../../../game-theory.md#coalition-game-theory) wins. This proves efficiency directly: $5\alpha+10\beta=1$, where $\alpha$ is the value of each permanent member. Hence

$$
\boxed{\alpha=\frac{421}{2145},\qquad\beta=\frac4{2145}.}
$$

The vector has five entries $421/2145$ and ten entries $4/2145$. As a check, a permanent member is pivotal when they are last among the permanent members and occupy a position from nine to fifteen; counting those orderings gives the same $\alpha$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

**False.** Take three players of weight one and strict threshold one, so a [coalition](../../../game-theory.md#coalition-game-theory) wins exactly when it contains at least two players. Set $S=\{1,2\}$ and $T=\{2,3\}$. Then

$$
v(S)=v(T)=v(S\cup T)=1,\qquad v(S\cap T)=v(\{2\})=0.
$$

The [convex cooperative game](../../../game-theory.md#convex-cooperative-game) inequality would require $1\ge1+1-0=2$. Thus even this elementary majority [weighted voting game](../../../game-theory.md#weighted-voting-game) is not convex.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

**True, with the usual normalization $v(\varnothing)=0$.** For a [convex cooperative game](../../../game-theory.md#convex-cooperative-game), the [supermodular](../../../function.md#supermodular-set-function) inequality implies increasing [marginal contributions](../../../game-theory.md#marginal-contribution): if $A\subseteq B$ and $i\notin B$, apply it to $A\cup\{i\}$ and $B$ to obtain

$$
v(A\cup\{i\})-v(A)\le v(B\cup\{i\})-v(B).
$$

Fix an ordering $\pi$ and let $P_i$ be the set of players before $i$. Its [marginal contribution vector](../../../game-theory.md#marginal-contribution-vector) is $m_i^\pi=v(P_i\cup\{i\})-v(P_i)$. Summing in order telescopes to $\sum_i m_i^\pi=v(N)$. For any [coalition](../../../game-theory.md#coalition-game-theory) $S$, $S\cap P_i\subseteq P_i$, so increasing marginals give

$$
\sum_{i\in S}m_i^\pi\ge\sum_{i\in S}\bigl(v((S\cap P_i)\cup\{i\})-v(S\cap P_i)\bigr)=v(S).
$$

These are exactly the efficiency and [coalition](../../../game-theory.md#coalition-game-theory) constraints of the [core of a cooperative game](../../../game-theory.md#core-game-theory). Thus every [marginal contribution](../../../game-theory.md#marginal-contribution) vector is in the [core](../../../game-theory.md#core-game-theory). The [core](../../../game-theory.md#core-game-theory) is a [convex set](../../../mathematical-optimization.md#convex-set), being an intersection of linear [half-spaces](../../../geometry-and-topology.md#half-space) and an efficiency [hyperplane](../../../vector-space.md#hyperplane). The [Shapley value](../../../game-theory.md#shapley-value) is the average of the [marginal contribution](../../../game-theory.md#marginal-contribution) vectors over all orderings, so it too lies in the [core](../../../game-theory.md#core-game-theory). This proves [Shapley value belongs to the core of a convex game](../../../game-theory.md#shapley-value-belongs-to-the-core-of-a-convex-game), without needing a separate existence theorem for the [core](../../../game-theory.md#core-game-theory).

## 6

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let $r$ be the number of true values among $a,b,c$. Count the ten [clause](../../../computer-science.md#clause-of-a-boolean-formula) occurrences for the two choices of $d$. With $d=0$, the three positive singletons contribute $r$, the three negated-pair [clauses](../../../computer-science.md#clause-of-a-boolean-formula) contribute $3-\binom r2$, and the last three [clauses](../../../computer-science.md#clause-of-a-boolean-formula) all hold. With $d=1$, the four singleton [clauses](../../../computer-science.md#clause-of-a-boolean-formula) contribute $r+1$, the negated pairs again contribute $3-\binom r2$, and the last three contribute $r$. Therefore

$$
\begin{array}{c|cc|c}
r&d=0&d=1&\text{maximum}\\\hline
0&6&4&6\\
1&7&6&7\\
2&7&7&7\\
3&6&7&7
\end{array}
$$

The original three-[literal](../../../computer-science.md#boolean-literal) [clause](../../../computer-science.md#clause-of-a-boolean-formula) is satisfied exactly when $r\ge1$, and then a value of $d$ satisfies exactly seven gadget [clauses](../../../computer-science.md#clause-of-a-boolean-formula). If $r=0$, no choice reaches seven. Thus **the required equivalence holds, and seven is also an upper bound for every assignment to the gadget.** This is the [seven-clause gadget for MAX-2SAT](../../../computer-science.md#seven-clause-gadget-for-max-2sat).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The decision problem is in [NP](../../../computer-science.md#np-complexity): an assignment is a certificate, and counting its satisfied [clause](../../../computer-science.md#clause-of-a-boolean-formula) occurrences is polynomial in the input size.

Reduce [3-SAT](../../../computer-science.md#3-sat) to it. For each of the $m$ original [clauses](../../../computer-science.md#clause-of-a-boolean-formula), use the [seven-clause gadget for MAX-2SAT](../../../computer-science.md#seven-clause-gadget-for-max-2sat) with its three [literals](../../../computer-science.md#boolean-literal) in place of $a,b,c$ and with a fresh auxiliary variable. Keep all ten [clause](../../../computer-science.md#clause-of-a-boolean-formula) occurrences per gadget, including any repeated occurrences across gadgets. Set the target to $k=7m$.

If the original formula is satisfiable, choose each auxiliary value as in part (a), giving seven satisfied [clauses](../../../computer-science.md#clause-of-a-boolean-formula) per gadget. Conversely, no gadget can exceed seven. If an assignment satisfies at least $7m$ [clauses](../../../computer-science.md#clause-of-a-boolean-formula) in total, every gadget must reach seven, so every original [clause](../../../computer-science.md#clause-of-a-boolean-formula) is satisfied by the original-variable assignment. The construction has $10m$ [clauses](../../../computer-science.md#clause-of-a-boolean-formula) and $m$ auxiliary variables, so is polynomial. Consequently **the decision version of [MAX-2SAT](../../../computer-science.md#maximum-2-satisfiability) is [NP-complete](../../../computer-science.md#np-completeness).**

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Use the usual nonempty-[clause](../../../computer-science.md#clause-of-a-boolean-formula) convention and normalize repeated [literals](../../../computer-science.md#boolean-literal) within a [clause](../../../computer-science.md#clause-of-a-boolean-formula); tautologies are always satisfied. If empty [clauses](../../../computer-science.md#clause-of-a-boolean-formula) are admitted, discard them first: they contribute nothing to any assignment or to the optimum. Let $m$ be the resulting number of [clause](../../../computer-science.md#clause-of-a-boolean-formula) occurrences.

Assign independent fair truth values. A singleton [clause](../../../computer-science.md#clause-of-a-boolean-formula) is satisfied with [probability](../../../probability-theory.md#probability) $1/2$, a proper two-variable [clause](../../../computer-science.md#clause-of-a-boolean-formula) with [probability](../../../probability-theory.md#probability) $3/4$, and a tautology with [probability](../../../probability-theory.md#probability) one. By [linearity of expectation](../../../probability-theory.md#linearity-of-expectation), the expected number satisfied is at least $m/2$, hence at least $\mathrm{OPT}/2$.

To derandomize, use the [method of conditional probabilities](../../../computer-science.md#method-of-conditional-probabilities). After some variables have been fixed, let $F$ be the conditional expected number of satisfied [clauses](../../../computer-science.md#clause-of-a-boolean-formula). For the next variable the two [conditional expectations](../../../measure-theory.md#conditional-expectation) $F_0,F_1$ satisfy $F=(F_0+F_1)/2$. Fix the value with the larger expectation. This never decreases $F$. When all variables have been fixed, $F$ is the actual integer number of satisfied [clauses](../../../computer-science.md#clause-of-a-boolean-formula), so

$$
\boxed{\text{the algorithm satisfies at least }m/2\ge\mathrm{OPT}/2\text{ clauses}.}
$$

Compute each [conditional expectation](../../../measure-theory.md#conditional-expectation) by summing the [probabilities](../../../probability-theory.md#probability) of the [clauses](../../../computer-science.md#clause-of-a-boolean-formula). Each has at most two variables, so its contribution is computed in constant time; scanning all [clauses](../../../computer-science.md#clause-of-a-boolean-formula) for each variable gives $O(nm)$ arithmetic operations. This is a polynomial-time [approximation algorithm](../../../mathematical-optimization.md#approximation-algorithm) with [approximation ratio](../../../mathematical-optimization.md#approximation-ratio) $1/2$.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Apply the condition after the usual [clause](../../../computer-science.md#clause-of-a-boolean-formula) normalization, so each variable has at most one singleton [clause](../../../computer-science.md#clause-of-a-boolean-formula). For a variable with such a [clause](../../../computer-science.md#clause-of-a-boolean-formula), make its favored [literal](../../../computer-science.md#boolean-literal) true with [probability](../../../probability-theory.md#probability) $p>1/2$; for other variables use a fair value. Make these choices independently. Then every singleton is satisfied with [probability](../../../probability-theory.md#probability) $p$.

Each [literal](../../../computer-science.md#boolean-literal) of a proper two-variable [clause](../../../computer-science.md#clause-of-a-boolean-formula) is true with [probability](../../../probability-theory.md#probability) at least $1-p$. Independence bounds the [probability](../../../probability-theory.md#probability) that both are false by $p^2$, so the [clause](../../../computer-science.md#clause-of-a-boolean-formula) is satisfied with [probability](../../../probability-theory.md#probability) at least $1-p^2$. Tautologies have [probability](../../../probability-theory.md#probability) one. Thus the expected fraction satisfied is at least $\min(p,1-p^2)$. One term increases and the other decreases, so their intersection maximizes this bound:

$$
p=1-p^2\quad\Longrightarrow\quad\boxed{p=\frac{\sqrt5-1}{2}\approx0.618034.}
$$

The [method of conditional probabilities](../../../computer-science.md#method-of-conditional-probabilities) also works with these biased [probabilities](../../../probability-theory.md#probability): before fixing a variable, the current expectation is the weighted average of its two [conditional expectations](../../../measure-theory.md#conditional-expectation), so choosing the larger cannot decrease it. Each [clause](../../../computer-science.md#clause-of-a-boolean-formula) contributes a constant-degree expression in $p$; since $p^2=1-p$, these expectations can be compared exactly in the fixed quadratic field $\mathbb Q(\sqrt5)$ with polynomial bit complexity. The final deterministic assignment therefore has

$$
\boxed{\text{approximation ratio }\frac{\sqrt5-1}{2}.}
$$

This is the [golden ratio approximation for MAX-2SAT](../../../computer-science.md#golden-ratio-approximation-for-max-2sat), under the stated restriction on normalized singleton [clauses](../../../computer-science.md#clause-of-a-boolean-formula). Arbitrary conflicting singleton [clauses](../../../computer-science.md#clause-of-a-boolean-formula) do not admit the same independent-bias guarantee.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
