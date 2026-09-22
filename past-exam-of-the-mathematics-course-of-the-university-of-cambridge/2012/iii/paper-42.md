# Paper 42

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_42.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_42.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a minimization problem on a domain $D$, write the equality constraints as $h(x)=0$ and the inequality constraints as $g(x)\leq0$. Define the [optimization Lagrangian](../../../mathematical-optimization.md#optimization-lagrangian)

$$
L(x,\lambda,\mu)=f(x)+\lambda^T h(x)+\mu^Tg(x),\qquad \mu\geq0.
$$

The [Lagrangian sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem) states that a feasible $x^*$ is globally optimal if it globally minimizes $L(\cdot,\lambda^*,\mu^*)$ on $D$ for some multipliers with $\mu^*\geq0$ and satisfies [complementary slackness](../../../mathematical-optimization.md#complementary-slackness), $\mu_j^*g_j(x^*)=0$ for every $j$. Equality multipliers have unrestricted signs.

For any feasible $x$, the multiplier sign gives $L(x,\lambda^*,\mu^*)\leq f(x)$. Feasibility and [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) at $x^*$ give $L(x^*,\lambda^*,\mu^*)=f(x^*)$. Hence

$$
\boxed{f(x)\geq L(x,\lambda^*,\mu^*)\geq L(x^*,\lambda^*,\mu^*)=f(x^*).}
$$

This proves sufficiency. **Global Lagrangian minimization, rather than stationarity alone, is the certificate.** No [convexity](../../../real-analysis.md#convex-function) or constraint qualification is needed for this implication; [convexity](../../../real-analysis.md#convex-function) is one way to verify the required global minimum.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) with the sign convention

$$
L(x,\lambda)=3x_1-x_2+2x_3^2+\lambda(x_1^2+x_2^2+x_3-2).
$$

For every $\lambda>0$, this is a [strictly convex](../../../real-analysis.md#strictly-convex-function) quadratic in $x$, with unique global minimizer

$$
x_1(\lambda)=-\frac3{2\lambda},\qquad x_2(\lambda)=\frac1{2\lambda},\qquad x_3(\lambda)=-\frac\lambda4.
$$

These formulas follow by setting the three partial derivatives of the [optimization Lagrangian](../../../mathematical-optimization.md#optimization-lagrangian) to zero; its [Hessian](../../../calculus.md#hessian-matrix) is $\operatorname{diag}(2\lambda,2\lambda,4)$, which is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form).

Choose $\lambda>0$ to make this minimizer feasible. Its constraint value is $5/(2\lambda^2)-\lambda/4$, so the scalar equation is

$$
\frac5{2\lambda^2}-\frac\lambda4=2,\qquad\text{equivalently}\qquad\lambda^3+8\lambda^2-10=0.
$$

The left side of the first equation is strictly decreasing on $(0,\infty)$, with limits $+\infty$ and $-\infty$. Thus exactly one positive multiplier exists and can be obtained by a bracketed scalar root search. The [Lagrangian sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem) proves that its associated feasible point is the global optimum; strict Lagrangian [convexity](../../../real-analysis.md#convex-function) makes that optimum unique.

Consequently **the unique solution is**

$$
\boxed{x^*=\left(-\frac3{2\lambda},\frac1{2\lambda},-\frac\lambda4\right),\quad\lambda>0,\quad\lambda^3+8\lambda^2-10=0.}
$$

Its objective value is $-5/\lambda+\lambda^2/8$. This [scalar multiplier certificate for a quadratic equality constraint](../../../mathematical-optimization.md#scalar-multiplier-certificate-for-a-quadratic-equality-constraint) does not require finding the multiplier in radicals, and does not mistake the nonconvex equality surface for a [convex set](../../../mathematical-optimization.md#convex-set).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Introduce a free scalar $t$. The [epigraph](../../../calculus-of-variations.md#epigraph) reformulation is the [linear program](../../../mathematical-optimization.md#linear-programming)

$$
\min_{x\in\mathbb R^n,\,t\in\mathbb R}t\qquad\text{subject to}\qquad a_i^Tx+b_i\leq t\quad(1\leq i\leq n).
$$

For each fixed $x$, the smallest feasible $t$ equals the maximum of the affine expressions, so the reformulation preserves the optimum.

Associate nonnegative multipliers $y_i$ with these inequalities. Its [optimization Lagrangian](../../../mathematical-optimization.md#optimization-lagrangian) is

$$
L(x,t,y)=\left(1-\sum_i y_i\right)t+\left(\sum_i y_i a_i\right)^Tx+\sum_i y_i b_i.
$$

Because $x$ and $t$ are unrestricted, the infimum is finite precisely when the coefficients of both vanish. Therefore the [Lagrangian dual problem](../../../mathematical-optimization.md#lagrangian-dual-problem) is

$$
\boxed{\max_y\sum_i b_i y_i\qquad\text{subject to}\qquad\sum_i y_i a_i=0,\quad\sum_i y_i=1,\quad y_i\geq0.}
$$

A feasible dual vector is a [convex combination](../../../mathematical-optimization.md#convex-combination) of the slopes whose mean slope is zero. It gives a constant lower bound on the maximum of the affine functions. The primal is always feasible, by taking $x=0$ and sufficiently large $t$. If it has a finite optimum, [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) gives attainment and equality with this dual; otherwise the dual is infeasible and the primal is unbounded below.

## 2

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the PDF's first constraint, $2x_1+x_2\geq6$; the TeX aid substitutes a different inequality. Introduce a surplus $x_3$, slacks $x_4,x_5$, and one artificial variable $x_6$, all nonnegative. The initial [simplex dictionary](../../../numerical-analysis.md#simplex-dictionary) is

$$
x_6=6-2x_1-x_2+x_3,\qquad x_4=-2x_1+x_2,\qquad x_5=8-x_1-2x_2.
$$

The initial basis is $(x_6,x_4,x_5)$, with values $(6,0,8)$. In [two-phase simplex](../../../mathematical-optimization.md#two-phase-simplex), Phase I maximizes $w=-x_6=-6+2x_1+x_2-x_3$. We use the [Bland pivoting rule](../../../mathematical-optimization.md#bland-pivoting-rule): the smallest-index nonbasic variable with positive reduced cost enters, and among minimum-ratio ties the smallest-index basic variable leaves.

First $x_1$ enters. The ratios for $x_6,x_4,x_5$ are $3,0,8$, so $x_4$ leaves in a degenerate pivot. The resulting dictionary is

$$
x_1=\tfrac12x_2-\tfrac12x_4,\qquad x_6=6-2x_2+x_3+x_4,\qquad x_5=8-\tfrac52x_2+\tfrac12x_4,\qquad w=-6+2x_2-x_3-x_4.
$$

Next $x_2$ enters. It reduces $x_6$ and $x_5$ with ratios $3$ and $16/5$, while $x_1$ increases. Thus $x_6$ leaves. The Phase I maximum is $0$, with a feasible original basis; remove $x_6$ and obtain

$$
x_1=\tfrac32+\tfrac14x_3-\tfrac14x_4,\qquad x_2=3+\tfrac12x_3+\tfrac12x_4,\qquad x_5=\tfrac12-\tfrac54x_3-\tfrac34x_4.
$$

In Phase II the original objective is $z=21/2+(7/4)x_3+(5/4)x_4$. Bland's rule makes $x_3$ enter, and $x_5$ leaves at ratio $2/5$. This gives

$$
x_1=\tfrac85-\tfrac25x_4-\tfrac15x_5,\qquad x_2=\tfrac{16}5+\tfrac15x_4-\tfrac25x_5,\qquad x_3=\tfrac25-\tfrac35x_4-\tfrac45x_5,\qquad z=\tfrac{56}5+\tfrac15x_4-\tfrac75x_5.
$$

Finally $x_4$ enters. The decreasing basic variables $x_1,x_3$ have ratios $4$ and $2/3$, so $x_3$ leaves. The final tableau, with the basic columns suppressed, is

$$
\begin{array}{c|rr|r}
\text{row}&x_3&x_5&\text{right side}\\\hline
x_1&-2/3&-1/3&4/3\\
x_2&1/3&2/3&10/3\\
x_4&5/3&4/3&2/3\\\hline
z&1/3&5/3&34/3
\end{array}
$$

Each row means its row variable plus the displayed nonbasic terms equals the right side. Since $z=34/3-x_3/3-5x_5/3$, no nonnegative choice of nonbasic variables improves the objective. Thus

$$
\boxed{(x_1,x_2)=\left(\frac43,\frac{10}3\right),\qquad z^*=\frac{34}3.}
$$

The slacks are $x_3=x_5=0$, $x_4=2/3$.

A different entering rule is faster here. Selecting the largest eligible index in the initial Phase I objective makes $x_2$ enter and $x_5$ leave. The dictionary then has $x_6=2-(3/2)x_1+x_3+x_5/2$ and $x_4=4-(5/2)x_1-x_5/2$. Entering $x_1$ makes $x_6$ leave at $x_1=4/3$, directly reaching the final original basis $(x_1,x_2,x_4)$. Hence **two pivots suffice instead of Bland's four**, and Phase II needs no further pivot. This comparison concerns this instance, not a general superiority of that entering rule.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

If $x_1,x_2$ are integral, the derived surplus and slacks

$$
x_3=2x_1+x_2-6,\qquad x_4=x_2-2x_1,\qquad x_5=8-x_1-2x_2
$$

are also nonnegative integers. Therefore an all-integer [Gomory fractional cut](../../../mathematical-optimization.md#gomory-fractional-cut) can be taken from the final tableau's slack row

$$
x_4+\frac53x_3+\frac43x_5=\frac23.
$$

For a nonnegative integer dictionary row $x_B+\sum_j a_jx_j=b$, the quantity $x_B+\sum_j\lfloor a_j\rfloor x_j$ is an integer at most $b$, so it is at most $\lfloor b\rfloor$. Subtracting from the row proves the cut $\sum_j\{a_j\}x_j\geq\{b\}$. Applying it here gives

$$
\boxed{2x_3+x_5\geq2.}
$$

But the original row and $x_4\geq0$ give $5x_3+4x_5\leq2$. Nonnegativity then gives

$$
2x_3+x_5\leq\frac25(5x_3+4x_5)\leq\frac45<2.
$$

This contradicts the valid cut. Therefore **the integer program is infeasible**, certified by one [Gomory fractional cut](../../../mathematical-optimization.md#gomory-fractional-cut). It is essential to use the PDF's constraint: the altered TeX problem would have feasible integer points.

## 3

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [decision problem](../../../computer-science.md#decision-problem) belongs to [NP](../../../computer-science.md#np-complexity) if every yes-instance has a polynomial-length certificate verifiable by a deterministic [polynomial-time algorithm](../../../computer-science.md#polynomial-time-algorithm). It is [NP-hard](../../../computer-science.md#np-hardness) if every problem in [NP](../../../computer-science.md#np-complexity) has a [polynomial-time many-one reduction](../../../computer-science.md#polynomial-time-many-one-reduction) to it. It is [NP-complete](../../../computer-science.md#np-completeness) if it is both [NP-hard](../../../computer-science.md#np-hardness) and in [NP](../../../computer-science.md#np-complexity).

A [polynomial-time algorithm](../../../computer-science.md#polynomial-time-algorithm) for any [NP-complete](../../../computer-science.md#np-completeness) problem would therefore give one for every problem in [NP](../../../computer-science.md#np-complexity), implying $\mathrm P=\mathrm{NP}$. Conversely, if $\mathrm P=\mathrm{NP}$, all [NP-complete](../../../computer-science.md#np-completeness) decision problems have polynomial-time algorithms. **[NP-completeness](../../../computer-science.md#np-completeness) does not unconditionally prove that polynomial-time solution is impossible.** Optimization problems such as minimum tour cost are described as [NP-hard](../../../computer-science.md#np-hardness), while their threshold decision versions can be [NP-complete](../../../computer-science.md#np-completeness).

For a minimization problem with nonnegative costs, an [approximation algorithm](../../../mathematical-optimization.md#approximation-algorithm) of ratio $\alpha\geq1$ is a [polynomial-time algorithm](../../../computer-science.md#polynomial-time-algorithm) returning a feasible solution of cost at most $\alpha$ times the optimum on every instance. For maximization, one often uses $\alpha\geq1$ with value at least $\mathrm{OPT}/\alpha$; an equivalent convention uses ratios at most one. The metric-tour question uses the minimization convention.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Reduce the [Hamiltonian cycle](../../../graph-theory.md#hamilton-cycle) decision problem to the [metric travelling salesman problem](../../../mathematical-optimization.md#metric-travelling-salesman-problem). Given a simple graph on $n\geq3$ vertices, form the complete graph with distance $1$ on original edges and distance $2$ on nonedges. These symmetric distances satisfy the [triangle inequality](../../../topological-analysis.md#triangle-inequality), since a direct distance is at most $2$ and any two positive edge distances sum to at least $2$.

A tour has $n$ edges, each of cost at least $1$. It has cost at most $n$ exactly when every edge is an original graph edge, that is, exactly when the original graph has a [Hamiltonian cycle](../../../graph-theory.md#hamilton-cycle). The construction and threshold are polynomial in the input size. Thus **the [metric travelling salesman problem](../../../mathematical-optimization.md#metric-travelling-salesman-problem) is [NP-hard](../../../computer-science.md#np-hardness)**; its rational-cost threshold version is also in [NP](../../../computer-science.md#np-complexity) because a tour is a polynomial-size certificate.

Allowing repeated vertex visits does not reduce the optimum for a complete metric instance. Given a closed walk visiting every vertex, keep the vertices in order of first appearance and shortcut the portions between them, including the final return. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) makes the resulting Hamiltonian tour no more expensive. Conversely a Hamiltonian tour is an allowed closed walk. Hence the two optimal costs are equal, and **the repeated-visit metric version remains [NP-hard](../../../computer-science.md#np-hardness)**. If travel is described on a sparse graph, taking its shortest-path metric gives the corresponding closed-walk formulation rather than an easier exact problem.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $C^*$ be an optimal metric tour. Removing any one of its edges gives a [spanning tree](../../../combinatorics.md#spanning-tree), so the [minimum spanning tree](../../../combinatorics.md#minimum-spanning-tree) $T$ satisfies $c(T)\leq c(C^*)$. The [handshaking lemma](../../../combinatorics.md#degree-sum-formula) shows that its odd-degree set $U$ has even size.

Follow $C^*$ and retain only vertices of $U$, shortcutting between consecutive retained vertices. This produces a cyclic order on $U$ of total cost at most $c(C^*)$. If $U$ is nonempty, the alternating edges of that cyclic order form two [perfect matchings](../../../graph-theory.md#perfect-matching); their costs sum to the cycle cost. One has cost at most $c(C^*)/2$, so a [minimum-weight perfect matching](../../../graph-theory.md#minimum-weight-perfect-matching) $M$ has

$$
\boxed{c(M)\leq\tfrac12c(C^*).}
$$

For $|U|=2$, count the same undirected edge twice in the cyclic order; each alternating matching consists of one copy. For $U=\varnothing$, use the empty matching.

The multigraph with edges $T\uplus M$ is connected because it contains $T$. Each odd-degree vertex receives exactly one matching edge, and the other degrees are unchanged, so every degree is even. It therefore has an [Euler circuit](../../../graph-theory.md#euler-circuit). Constructively, follow unused edges until returning to the starting vertex; parity prevents getting stuck elsewhere. If unused edges remain, connectivity supplies a vertex of the current circuit incident with one, and its additional closed trail can be spliced into the circuit. Repetition gives a circuit using every edge exactly once, including parallel copies.

Shortcut repeated vertices of this [Euler circuit](../../../graph-theory.md#euler-circuit) to obtain a metric tour. Its cost is at most

$$
\boxed{c(T)+c(M)\leq\tfrac32c(C^*).}
$$

Computing a [minimum spanning tree](../../../combinatorics.md#minimum-spanning-tree), a [minimum-weight perfect matching](../../../graph-theory.md#minimum-weight-perfect-matching), an [Euler circuit](../../../graph-theory.md#euler-circuit) and the shortcut tour is polynomial-time; weighted [perfect matching](../../../graph-theory.md#perfect-matching) is a standard polynomial-time graph optimization problem. Thus **the [Christofides algorithm](../../../mathematical-optimization.md#christofides-algorithm) is a $3/2$-[approximation algorithm](../../../mathematical-optimization.md#approximation-algorithm) for symmetric metric tours**.

## 4

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The intended deletion theorem starts from the full action set $A=M\cup N$. Under that interpretation, each player's surviving action set remains nonempty: with only one action, no [mixed strategy](../../../game-theory.md#mixed-strategy) can weakly improve it and improve it strictly somewhere. Let the final reduced [bimatrix game](../../../game-theory.md#bimatrix-game) have a [Nash equilibrium](../../../game-theory.md#nash-equilibrium), which exists by [Nash's theorem](../../../game-theory.md#nash-s-theorem).

Restore the deleted actions in reverse order. Consider a row action $i$ when it is restored. At its deletion it had a weakly dominating [mixed strategy](../../../game-theory.md#mixed-strategy) $z$ in the then-current game. If $z_i>0$, remove that self-weight and renormalize: the strict-improvement clause guarantees $z_i<1$, and dividing the payoff comparison by $1-z_i$ gives a weakly dominating strategy supported on the other then-current row actions. Those other actions have already been restored in the reverse process. The chosen [Nash equilibrium](../../../game-theory.md#nash-equilibrium)'s column support lies in the final surviving set, so the dominance comparison applies to its column strategy $y$.

If the row player's [Nash equilibrium](../../../game-theory.md#nash-equilibrium) payoff in the restored game so far is $u$, every currently available pure row payoff against $y$ is at most $u$. The dominating mixture therefore has payoff at most $u$, and the restored action has payoff no greater than that mixture. It cannot improve the payoff. Column deviations are unchanged by adding a row action, since the actual [Nash equilibrium](../../../game-theory.md#nash-equilibrium) strategy remains fixed. The analogous argument works when restoring a column action. Induction restores the full game while preserving the final reduced [Nash equilibrium](../../../game-theory.md#nash-equilibrium) and its support.

Thus **iterated deletion of weakly dominated actions preserves at least one [Nash equilibrium](../../../game-theory.md#nash-equilibrium) supported entirely on surviving actions**. It need not preserve every [Nash equilibrium](../../../game-theory.md#nash-equilibrium) or give an order-independent reduced game.

The literal printed use of an arbitrary initial $A$ needs qualification. For example, take row payoffs $\left(\begin{smallmatrix}0&3\\1&0\end{smallmatrix}\right)$ and column payoffs $\left(\begin{smallmatrix}0&1\\0&1\end{smallmatrix}\right)$. On the restricted set containing both rows but only column $1$, row $1$ is strictly dominated by row $2$. Yet in the full game column $2$ is strictly dominant and its unique [Nash equilibrium](../../../game-theory.md#nash-equilibrium) uses row $1$. Deleting row $1$ based only on that restricted $A$ leaves no full-game [Nash equilibrium](../../../game-theory.md#nash-equilibrium) with the requested support. The proven [equilibrium preservation under iterated weak dominance](../../../game-theory.md#equilibrium-preservation-under-iterated-weak-dominance) therefore requires **initial $A=M\cup N$**, or concludes only about the initially restricted game.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the PDF's entry $P_{12}=4$, rather than the TeX aid's $2$. To check [nondegeneracy of a bimatrix game](../../../game-theory.md#nondegeneracy-of-a-bimatrix-game), every opponent strategy of support size $k$ must have at most $k$ pure [best responses](../../../game-theory.md#best-response). Against each pure column, the unique best rows are respectively $3,1,2$. Against each pure row, the unique best columns are respectively $1,2,2$.

The only mixture making all three rows indifferent solves $-y_1+2y_3=0$ and $-2y_1+2y_2-3y_3=0$, giving $y=(4,7,2)/13$, which has support size three. Thus no two-column-support mixture has three best rows. For the other player, column $1$ strictly dominates column $3$, because their payoff difference is $(1,1,2)$, so three best columns are impossible. These observations cover all support sizes, proving **the game is nondegenerate**.

For the [Lemke-Howson algorithm](../../../game-theory.md#lemke-howson-algorithm), use unnormalized strategy vectors $u,v$ in the polytopes

$$
\mathcal X=\{u\geq0:Q^Tu\leq\mathbf1\},\qquad\mathcal Y=\{v\geq0:Pv\leq\mathbf1\}.
$$

A row label $i\in\{1,2,3\}$ occurs at $u_i=0$ in $\mathcal X$ or at $(Pv)_i=1$ in $\mathcal Y$. A column label $3+j$ occurs at $(Q^Tu)_j=1$ in $\mathcal X$ or at $v_j=0$ in $\mathcal Y$. The origin pair has all six labels.

Drop row label $3$ by increasing $u_3$. Column $2$ is the first binding payoff constraint, at $u_3=1/4$, so label $5$ becomes duplicated. Drop $5$ in $\mathcal Y$ by increasing $v_2$; row $1$ binds first, at $v_2=1/4$, duplicating label $1$. Drop $1$ in $\mathcal X$ by increasing $u_1$ while keeping $u_2=0$ and the column-$2$ constraint binding. Since that constraint does not involve $u_1$, $u_3$ stays $1/4$. Column $1$ binds at $u_1=1/4$, duplicating label $4$.

Now drop $4$ in $\mathcal Y$ by increasing $v_1$. Keep $v_3=0$ and row $1$ binding, so $v_2=1/4$. Row $3$ reaches payoff $1$ at $v_1=1/6$, earlier than row $2$, which would bind at $v_1=1/4$. The missing label $3$ returns, terminating the path. The successive vertex-label pairs are

$$
\begin{array}{c|c|c|c|c}
\text{step}&u&\text{labels in }\mathcal X&v&\text{labels in }\mathcal Y\\\hline
0&(0,0,0)&1,2,3&(0,0,0)&4,5,6\\
1&(0,0,1/4)&1,2,5&(0,0,0)&4,5,6\\
2&(0,0,1/4)&1,2,5&(0,1/4,0)&1,4,6\\
3&(1/4,0,1/4)&2,4,5&(0,1/4,0)&1,4,6\\
4&(1/4,0,1/4)&2,4,5&(1/6,1/4,0)&1,3,6
\end{array}
$$

The final pair is completely labelled and nonzero. Normalize each vector by its own sum to obtain

$$
\boxed{x=(\tfrac12,0,\tfrac12),\qquad y=(\tfrac25,\tfrac35,0).}
$$

The row payoffs against $y$ are $(12/5,2,12/5)$ and the column payoffs against $x$ are $(2,2,1/2)$. Both supported actions are best responses, so this is a [Nash equilibrium](../../../game-theory.md#nash-equilibrium), with **payoffs $\boxed{(12/5,\,2)}$**.

## 5

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a [transferable utility game](../../../game-theory.md#transferable-utility-game) with $v(\varnothing)=0$, an efficient allocation satisfies $\sum_{i\in N}x_i=v(N)$. An [imputation](../../../game-theory.md#imputation-in-a-coalitional-game) is efficient and individually rational, $x_i\geq v(\{i\})$. Write $x(S)=\sum_{i\in S}x_i$ and define the [excess of a coalition](../../../game-theory.md#excess-of-a-coalition) as $e(S,x)=v(S)-x(S)$.

The [core of a cooperative game](../../../game-theory.md#core-game-theory) is

$$
\boxed{\{x:x(N)=v(N),\quad x(S)\geq v(S)\text{ for every }S\subseteq N\}.}
$$

It consists of allocations immune to a [coalition](../../../game-theory.md#coalition-game-theory)'s blocking: no [coalition](../../../game-theory.md#coalition-game-theory) can obtain more for its members by leaving. The singleton inequalities imply individual rationality. The core may be empty.

The [nucleolus](../../../game-theory.md#nucleolus), when the [imputation](../../../game-theory.md#imputation-in-a-coalitional-game) set is nonempty, is the unique [imputation](../../../game-theory.md#imputation-in-a-coalitional-game) that lexicographically minimizes the list of [coalition](../../../game-theory.md#coalition-game-theory) excesses arranged from largest to smallest. It first minimizes the largest complaint, then the second largest among ties, and so on. Including the empty and grand [coalitions](../../../game-theory.md#coalition-game-theory) adds constant zeros and does not change the solution. Minimization on efficient allocations without individual rationality instead defines the [prenucleolus](../../../game-theory.md#prenucleolus), a different convention that matters for this paper's game.

The [Shapley value](../../../game-theory.md#shapley-value) is the average [marginal contribution](../../../game-theory.md#marginal-contribution) of each player over all uniformly ordered player arrivals:

$$
\boxed{\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}\frac{|S|!(n-|S|-1)!}{n!}\bigl(v(S\cup\{i\})-v(S)\bigr).}
$$

Exactly $|S|!(n-|S|-1)!$ orderings have $S$ as the predecessor set of $i$. This is an average-contribution fairness rule, rather than a blocking-stability condition; it need not be individually rational for an arbitrary game.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Put $w(S)=|S|!(n-|S|-1)!/n!$ for $S\subseteq N\setminus\{i\}$. Under the bijection $S\mapsto R=(N\setminus\{i\})\setminus S$, the weights satisfy $w(S)=w(R)$ and $N\setminus S=R\cup\{i\}$. Consequently

$$
\sum_Sw(S)v(N\setminus S)=\sum_Rw(R)v(R\cup\{i\}).
$$

Subtracting $\sum_Sw(S)v(S)$ proves the alternative [Shapley value](../../../game-theory.md#shapley-value) expression

$$
\boxed{\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}w(S)\bigl(v(N\setminus S)-v(S)\bigr).}
$$

For the [dual coalitional game](../../../game-theory.md#dual-coalitional-game) $v'(S)=v(N)-v(N\setminus S)$, its [marginal contribution](../../../game-theory.md#marginal-contribution) at predecessor set $S$ is

$$
v'(S\cup\{i\})-v'(S)=v(N\setminus S)-v(N\setminus(S\cup\{i\}))=v(R\cup\{i\})-v(R).
$$

The same weight-preserving complement bijection therefore gives $\phi_i(v')=\phi_i(v)$, and both equal the displayed expression. **The [Shapley value](../../../game-theory.md#shapley-value) is invariant under coalitional duality.** This [Shapley self-duality](../../../game-theory.md#shapley-self-duality) calculation complements within $N\setminus\{i\}$, not within $N$ without accounting for the distinguished player.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For three players, the predecessor-set weights are $1/3$ for sizes zero and two, and $1/6$ for size one. Thus

$$
\begin{aligned}
\phi_1&=\tfrac13(4)+\tfrac16(10-3)+\tfrac16(11-2)+\tfrac13(12-5)=\tfrac{19}3,\\
\phi_2&=\tfrac13(3)+\tfrac16(10-4)+\tfrac16(5-2)+\tfrac13(12-11)=\tfrac{17}6,\\
\phi_3&=\tfrac13(2)+\tfrac16(11-4)+\tfrac16(5-3)+\tfrac13(12-10)=\tfrac{17}6.
\end{aligned}
$$

Therefore **the [Shapley value](../../../game-theory.md#shapley-value) is $\boxed{(19/3,17/6,17/6)}$**, whose coordinates sum to $12$.

For the [nucleolus](../../../game-theory.md#nucleolus), use [imputations](../../../game-theory.md#imputation-in-a-coalitional-game) $x_1+x_2+x_3=12$, $x_1\geq4$, $x_2\geq3$, $x_3\geq2$. The excess of $\{1,3\}$ is $11-(12-x_2)=x_2-1\geq2$. Thus the smallest possible largest excess is at least $2$. It is attained when $x_2=3$, $x_3=9-x_1$, and $5\leq x_1\leq7$: the remaining proper-coalition excesses then are

$$
e_1=4-x_1,\quad e_2=0,\quad e_3=x_1-7,\quad e_{12}=7-x_1,\quad e_{23}=x_1-7,
$$

all at most $2$, while $e_{13}=2$. Conversely, a largest excess of $2$ forces $x_2=3$ and precisely this interval for $x_1$.

On this first-stage face the top excess $2$ is fixed. The next largest excess is $7-x_1\geq0$, because the other varying excesses are nonpositive and $e_2=0$ is fixed. Its unique minimum is zero at $x_1=7$. No further lexicographic tie remains. Hence **the [nucleolus](../../../game-theory.md#nucleolus) is $\boxed{(7,3,2)}$**. Its proper-coalition excesses, sorted decreasingly, are $(2,0,0,0,0,-3)$.

Finally, a core allocation would require $x_2\geq3$ and $x_1+x_3\geq11$, whose sum contradicts the efficient total $12$. Thus **the [core of a cooperative game](../../../game-theory.md#core-game-theory) is empty**. The game is not superadditive, so neither core nonemptiness nor individual rationality of the [Shapley value](../../../game-theory.md#shapley-value) should be presumed. Under the distinct [prenucleolus](../../../game-theory.md#prenucleolus) convention the answer would be $(15/2,2,5/2)$. Balancing $e_2=3-x_2$ and $e_{13}=x_2-1$ gives a first-stage maximum of $1$ and forces $x_2=2$. The remaining first-stage constraints restrict $x_1$ to $[7,8]$. The next largest complaints are $e_{12}=8-x_1$ and $e_{23}=x_1-7$, balanced at $x_1=15/2$, with $x_3=5/2$. This is not an [imputation](../../../game-theory.md#imputation-in-a-coalitional-game) and is not the [nucleolus](../../../game-theory.md#nucleolus) under the definition in (a).

## 6

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [Gibbard-Satterthwaite theorem](../../../game-theory.md#gibbard-satterthwaite-theorem) concerns a deterministic [social choice function](../../../game-theory.md#social-choice-function) on all profiles of strict preferences over a finite set of at least three alternatives. If it is onto and [strategyproof](../../../game-theory.md#strategyproofness), it is a [dictatorship in social choice](../../../game-theory.md#dictatorship-in-social-choice): one fixed voter always obtains its top alternative. Equivalently, every onto nondictatorial rule on this unrestricted domain is manipulable. Dictatorships themselves are [strategyproof](../../../game-theory.md#strategyproofness). We prove the implication for two voters.

First derive the [rank-raising monotonicity lemma](../../../game-theory.md#rank-raising-monotonicity-lemma). If changing one report changes the selected alternative from $a$ to $b$, [strategyproofness](../../../game-theory.md#strategyproofness) in the old profile requires $a\succ b$ in the old order, while [strategyproofness](../../../game-theory.md#strategyproofness) in the new profile requires $b\succ a$ in the new order. Therefore a change that never lowers the selected $a$ relative to any formerly lower alternative cannot change the outcome.

Onto-ness now implies unanimity. For every $a$, some profile selects it. Raise $a$ to first place in each voter's order; the preceding lemma keeps the outcome at $a$. Moreover the outcome cannot be $b$ when both voters rank some $a$ above $b$: starting from such an outcome, raise $b$ to second place directly below $a$ in each order. These changes never lower $b$ relative to anything, so would preserve $b$ at a profile unanimously topping $a$, a contradiction. Thus the rule respects unanimous pairwise preference.

For each pair $a,b$, promote that pair to the first two places in each report, preserving the voter's order between them. Both dominate every outsider unanimously, so the outcome is $a$ or $b$. The result depends only on the two voters' comparisons of $a,b$, not on the lower alternatives: changing a tail cannot reverse the choice between two alternatives whose relative order did not change, since one direction of that change would be a profitable report. These binary choices define a complete strict social relation satisfying pairwise unanimity and independence from other comparisons.

This relation is transitive. To see why, suppose its choices on some triple form a directed cycle. Put those three alternatives first in both reports, preserving their individual relative orders. Unanimity excludes all outsiders, so the rule chooses one of the three, say $a$. Promoting $a$ with either other member to the first two positions does not lower $a$ and therefore preserves its selection. Thus $a$ must win both its binary comparisons, contradicting the cycle. A complete strict relation with no directed three-cycle is transitive. Also the original social choice is its top: for any original selected $a$, promoting $a$ and any $b$ preserves $a$, so it wins every binary comparison.

It remains to prove two-voter dictatorship for this binary relation. Choose any conflict between $a,b$. Suppose voter 1 prefers $a$ to $b$, voter 2 prefers $b$ to $a$, and the social relation follows voter 1. Say voter 1 wins this ordered comparison. For any third alternative $c$, consider the two profile patterns

$$
\begin{array}{c|cc}
&\text{voter 1}&\text{voter 2}\\\hline
\text{pattern I}&a\succ b\succ c&b\succ c\succ a\\
\text{pattern II}&c\succ a\succ b&b\succ c\succ a
\end{array}
$$

with other alternatives below the triple. In pattern I, the social relation has $a\succ b$ by independence and $b\succ c$ by unanimity, hence $a\succ c$. This proves that voter 1 wins the conflict $a$ against $c$. In pattern II, it has $c\succ a$ by unanimity and $a\succ b$ by independence, hence $c\succ b$, proving that voter 1 also wins $c$ against $b$.

Thus winning $a$ against $b$ implies winning $a$ against every third $c$ and every such $c$ against $b$. Applying the implication to $a$ against $c$ gives $b$ against $c$, and then to $b$ against $c$ gives $b$ against $a$. The implication therefore supplies both directions of all pairs involving the original alternatives and any new one. For an arbitrary ordered pair $x,y$ distinct from a fixed base alternative $a$, use the already obtained win of $x$ against $a$ and the third alternative $y$ to get the win of $x$ against $y$. Hence voter 1 wins every conflict. Unanimous comparisons also follow its preference, so the social relation is always voter 1's full order, and the social choice is its top.

If the initially chosen conflict follows voter 2, swap the voter roles in the same argument. We have therefore proved **every onto two-voter [strategyproof](../../../game-theory.md#strategyproofness) rule with at least three alternatives is dictatorial**. This [two-voter dictatorship from binary choice](../../../game-theory.md#two-voter-dictatorship-from-binary-choice) proof establishes the required special case without assuming the general theorem's conclusion.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

There is a parity qualification in the printed claim. With the usual strict-majority definition, an even electorate need not have a [Condorcet winner](../../../game-theory.md#condorcet-winner). On the axis $a<b<c$, the two orders $a\succ b\succ c$ and $c\succ b\succ a$ are both [single-peaked preferences](../../../game-theory.md#single-peaked-preferences), but every pairwise contest is tied. Thus no alternative strictly defeats every other one. We first prove the intended strict-winner result for odd $n$.

Let $n=2k+1$ and order the peaks along the common axis. Their median $w$ has at least $k+1$ peaks at or to each side. For any $y<w$, the $k+1$ voters whose peaks are at or to the right of $w$ prefer $w$ to $y$ by single-peakedness. For any $y>w$, the corresponding $k+1$ voters on the left prefer $w$. Thus **the median peak is the unique [Condorcet winner](../../../game-theory.md#condorcet-winner)**.

The corresponding [median voter rule](../../../game-theory.md#median-voter-rule) is [strategyproof](../../../game-theory.md#strategyproofness). Fix the other $2k$ peaks $q_1\leq\cdots\leq q_{2k}$. As one voter reports a peak $p$, the selected median is

$$
\operatorname{median}(q_1,\ldots,q_{2k},p)=\min\{q_{k+1},\max\{q_k,p\}\},
$$

where minimum and maximum refer to the common axis. All attainable outcomes lie between $q_k$ and $q_{k+1}$. If the true peak lies inside this interval, truthful reporting obtains the voter's top. If it lies left of the interval, truthful reporting obtains its left endpoint, which the voter's single-peaked order prefers to every larger attainable outcome. The case right of the interval is symmetric. No report improves the outcome. For one voter the rule simply selects its peak.

There is also a proof that does not depend on knowing the axis. If a voter truly prefers a proposed new winner $z$ to the current strict [Condorcet winner](../../../game-theory.md#condorcet-winner) $w$, that voter already opposes $w$ in the contest $w$ versus $z$. The strict majority supporting $w$ in that contest therefore consists of other voters and is unaffected by its report. Thus $z$ cannot become a strict [Condorcet winner](../../../game-theory.md#condorcet-winner) after a profitable misreport. This proves [strategyproofness](../../../game-theory.md#strategyproofness) on the domain of profiles for which the selected strict winner exists, including all admissible odd-electorate single-peaked profiles.

For even $n$, a [weak Condorcet winner](../../../game-theory.md#weak-condorcet-winner) is guaranteed: every alternative between the two middle peaks weakly defeats each other alternative, allowing ties. With a fixed common axis, consistently choosing the lower median or consistently choosing the upper median gives a single-valued [strategyproof](../../../game-theory.md#strategyproofness) rule, by the same interval-clamping argument for an [order statistic](../../../probability-theory.md#order-statistic). Arbitrary tie selection is not asserted to have this property. The corrected conclusion is therefore **a unique strict winner and its [strategyproof](../../../game-theory.md#strategyproofness) selection for odd electorates; a weak winner with a specified median rule for even electorates**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
