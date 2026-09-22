# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper37.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [decision problem](../../../computer-science.md#decision-problem) is in [NP](../../../computer-science.md#np-complexity) if every yes-instance has a [complexity certificate](../../../computer-science.md#certificate-complexity) of length bounded by a polynomial in the input length, and a deterministic verifier can check that certificate in [polynomial time](../../../computer-science.md#polynomial-time). More precisely, for some polynomial $p$ and verifier $V$,

$$
w\in L\quad\Longleftrightarrow\quad\exists z,\ |z|\leq p(|w|),\quad V(w,z)=1,
$$

where $V$ runs in [polynomial time](../../../computer-science.md#polynomial-time). Equivalently, a nondeterministic machine decides the problem in [polynomial time](../../../computer-science.md#polynomial-time). A problem is [NP-complete](../../../computer-science.md#np-completeness) if it belongs to [NP](../../../computer-science.md#np-complexity) and is [NP-hard](../../../computer-science.md#np-hardness): every problem in [NP](../../../computer-science.md#np-complexity) has a [polynomial-time many-one reduction](../../../computer-science.md#polynomial-time-many-one-reduction) to it. Such a reduction maps instances $w$ to instances $r(w)$ with $w\in L$ if and only if $r(w)$ is a yes-instance of the target problem.

For [3-SAT](../../../computer-science.md#3-sat), the [complexity certificate](../../../computer-science.md#certificate-complexity) is one truth value for each [Boolean variable](../../../computer-science.md#boolean-variable). Check every [Boolean literal](../../../computer-science.md#boolean-literal), negate its variable's truth value when appropriate, evaluate the disjunction in each [Boolean clause](../../../computer-science.md#clause-of-a-boolean-formula), and check their conjunction. This takes time linear in the encoded [Boolean formula](../../../computer-science.md#boolean-formula), apart from equally polynomial bookkeeping for variable names. A satisfying assignment passes; an unsatisfiable [Boolean formula](../../../computer-science.md#boolean-formula) has no passing assignment. Thus **[3-SAT](../../../computer-science.md#3-sat) belongs to [NP](../../../computer-science.md#np-complexity)**.

For the diagram's [three-colour clause gadget](../../../graph-theory.md#three-colour-clause-gadget), name the three colours by the [graph triangle](../../../graph.md#triangle-in-a-graph) $T,F,X$. Each input $a,b,\bar c$ is adjacent to $X$, so each has colour $T$ or $F$. Suppose that none has colour $T$. Then all three have colour $F$. Because $x_1$ is adjacent to $a$ and $x_2$ to $b$, neither has colour $F$. The [edge](../../../graph-theory.md#edge-of-a-graph) $x_1x_2$ forces these two colours to be $T$ and $X$ in some order. The [graph triangle](../../../graph.md#triangle-in-a-graph) $x_1,x_2,x_3$ now forces $x_3$ to have colour $F$. Since $x_4$ is adjacent to $x_3$ and $T$, it must have colour $X$. The [graph triangle](../../../graph.md#triangle-in-a-graph) $x_4,x_5,T$ forces $x_5$ to have colour $F$. But $x_5$ is adjacent to $\bar c$, which also has colour $F$, contradicting a proper [graph colouring](../../../graph-theory.md#graph-coloring). Therefore **at least one input has colour $T$**.

To give the [polynomial-time many-one reduction](../../../computer-science.md#polynomial-time-many-one-reduction), use one common palette [graph triangle](../../../graph.md#triangle-in-a-graph) $T,F,X$. For each [Boolean variable](../../../computer-science.md#boolean-variable) $v$, create two [graph vertices](../../../graph.md#vertex-graph-theory) $v,\bar v$ and join them to each other and to $X$. This [Boolean-pair colouring gadget](../../../graph-theory.md#boolean-pair-colouring-gadget) forces them to have opposite colours $T,F$. For each [Boolean clause](../../../computer-science.md#clause-of-a-boolean-formula), introduce five fresh auxiliary [graph vertices](../../../graph.md#vertex-graph-theory) and the [edges](../../../graph-theory.md#edge-of-a-graph) of the [three-colour clause gadget](../../../graph-theory.md#three-colour-clause-gadget), identifying its inputs with that clause's three [Boolean literal](../../../computer-science.md#boolean-literal) [vertices](../../../graph.md#vertex-graph-theory) and using the common $T$. In the notation of the diagram, its ten additional [edges](../../../graph-theory.md#edge-of-a-graph) are the two triangles $x_1x_2x_3$ and $x_4x_5T$, the bridge $x_3x_4$, and the three input [edges](../../../graph-theory.md#edge-of-a-graph). With $r$ variables and $m$ clauses the constructed [undirected graph](../../../graph-theory.md#undirected-graph) has $3+2r+5m$ [vertices](../../../graph.md#vertex-graph-theory) and at most $3+3r+10m$ [edges](../../../graph-theory.md#edge-of-a-graph). Repeated literals do not affect the argument. Its construction takes [polynomial time](../../../computer-science.md#polynomial-time).

A proper [graph colouring](../../../graph-theory.md#graph-coloring) defines a consistent truth assignment by declaring $v$ true precisely when its [vertex](../../../graph.md#vertex-graph-theory) has colour $T$. The only-if result just proved makes every clause true. Conversely, a satisfying assignment colours every literal [vertex](../../../graph.md#vertex-graph-theory) consistently, and the supplied if-direction extends each satisfied clause's colours to its fresh auxiliary [vertices](../../../graph.md#vertex-graph-theory). These extensions do not conflict, since different clauses share only already-coloured palette and literal [vertices](../../../graph.md#vertex-graph-theory). Thus the [Boolean formula](../../../computer-science.md#boolean-formula) is satisfiable exactly when the constructed [undirected graph](../../../graph-theory.md#undirected-graph) is three-colourable. Since [3-SAT](../../../computer-science.md#3-sat) is [NP-complete](../../../computer-science.md#np-completeness), composition of reductions proves [NP-hardness](../../../computer-science.md#np-hardness) of the [three-colourability problem](../../../graph-theory.md#three-colourability-problem).

Finally, a list of three colour labels, one for each [graph vertex](../../../graph.md#vertex-graph-theory), is a [complexity certificate](../../../computer-science.md#certificate-complexity) for the [three-colourability problem](../../../graph-theory.md#three-colourability-problem). Checking all [edges](../../../graph-theory.md#edge-of-a-graph) takes $O(|V|+|E|)$ time. Hence this problem is in [NP](../../../computer-science.md#np-complexity) as well, and **the [three-colourability problem](../../../graph-theory.md#three-colourability-problem) is [NP-complete](../../../computer-science.md#np-completeness)**.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [linear polyhedron](../../../mathematical-optimization.md#linear-polyhedron) $P\subseteq\mathbb R^n$ is full-dimensional if its [affine hull](../../../vector-space.md#affine-hull) is $\mathbb R^n$. For a [convex set](../../../mathematical-optimization.md#convex-set), this is equivalent to containing an open [Euclidean ball](../../../functional-analysis.md#euclidean-ball): an open ball has full affine span, while $n+1$ [affinely independent](../../../geometry-and-topology.md#affine-independence) points in the set span a [simplex](../../../algebraic-topology.md#simplex) with nonempty [interior](../../../topology.md#interior-topology). In particular, a nonempty [linear polyhedron](../../../mathematical-optimization.md#linear-polyhedron) need not be full-dimensional; a singleton or a [hyperplane](../../../vector-space.md#hyperplane) is an example.

Assume $U\geq1$, increasing the coefficient bound to one if necessary. If $x_0\in P$ and $A_i$ denotes the $i$th row, then $\|A_i\|_2\leq\sqrt n U$. For $r=\varepsilon/(nU)$ and $\|h\|_2\leq r$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
A_i(x_0+h)\geq b_i-\|A_i\|_2\|h\|_2\geq b_i-\varepsilon.
$$

Thus **$B(x_0,r)\subseteq P_\varepsilon$ with $r>0$**, proving that $P_\varepsilon$ is a [full-dimensional linear polyhedron](../../../mathematical-optimization.md#full-dimensional-linear-polyhedron). This part works for every positive $\varepsilon$; the particular small value also ensures that relaxation cannot create feasibility when $P$ is empty.

Here is that exact-feasibility point. Put $D=[(n+1)U]^{n+1}$. If $P$ is empty, a [Farkas certificate for linear inequalities](../../../convex-optimization.md#farkas-certificate-for-linear-inequalities) gives $\lambda\geq0$ with $A^T\lambda=0$ and $b^T\lambda>0$. Normalize $\mathbf1^T\lambda=1$, and maximize $b^T\lambda$ over the compact [linear polyhedron](../../../mathematical-optimization.md#linear-polyhedron)

$$
Q=\{\lambda\geq0:A^T\lambda=0,\ \mathbf1^T\lambda=1\}.
$$

Choose a maximizing [extreme point](../../../mathematical-optimization.md#extreme-point). Its positive support has size $k\leq n+1$: a dependence among its supported columns $(A_i^T,1)$ would permit small perturbations of both signs in $Q$, contradicting extremality. Select $k$ independent equations for those $k$ coordinates. [Cramer's rule](../../../linear-algebra.md#cramer-s-rule) expresses them over a common nonzero [integer](../../../number-theory.md#integer) [determinant](../../../linear-algebra.md#determinant) $\Delta$, with $|\Delta|\leq k!U^k\leq D$. Since $b$ is [integer](../../../number-theory.md#integer) and $b^T\lambda>0$, its numerator is a positive [integer](../../../number-theory.md#integer) after choosing a positive denominator. Hence $b^T\lambda\geq1/D$. This is the [normalized integer Farkas infeasibility gap](../../../convex-optimization.md#normalized-integer-farkas-infeasibility-gap). A point in $P_\varepsilon$ would imply

$$
0=\lambda^TAx\geq b^T\lambda-\varepsilon\geq\frac1D-\frac1{2(n+1)D}>0,
$$

a contradiction. Consequently **$P=\varnothing$ if and only if $P_\varepsilon=\varnothing$**.

The [ellipsoid method](../../../mathematical-optimization.md#ellipsoid-method) takes the [integer](../../../number-theory.md#integer) [matrix](../../../vector-space.md#matrix) $A$, [vector](../../../vector-space.md#vector) $b$, dimension $n$, and a bound $U$ (or their binary encodings). It computes the prescribed $\varepsilon$, an inner radius $r$, and an outer radius $R$ whose logarithms have polynomial size. For an explicit outer bound, let $M=(nU)^n$. A nonempty $P$ has a [rational feasibility certificate for integer inequalities](../../../mathematical-optimization.md#rational-feasibility-certificate-for-integer-inequalities) with $|x_j|\leq M$. To see this bound, intersect $P$ with an [orthant](../../../mathematical-optimization.md#orthant) containing a feasible point. This intersection is a nonempty [linear polyhedron](../../../mathematical-optimization.md#linear-polyhedron) containing no whole nontrivial affine line, and it has an [extreme point](../../../mathematical-optimization.md#extreme-point). Indeed, if its active rows do not yet span the ambient space, move along a nonzero direction annihilating them. The [orthant](../../../mathematical-optimization.md#orthant) prevents motion in both directions from being feasible forever, so in at least one direction a new independent row becomes active. Repeating at most $n$ times produces an [extreme point](../../../mathematical-optimization.md#extreme-point). At that point choose $n$ independent [active constraints](../../../mathematical-optimization.md#active-constraint), including coordinate constraints where needed. [Cramer's rule](../../../linear-algebra.md#cramer-s-rule) and the [Hadamard determinant inequality](../../../linear-algebra.md#hadamard-determinant-inequality) bound the numerators by $n^{n/2}U^n\leq M$, while a nonzero [integer](../../../number-theory.md#integer) denominator has absolute value at least one. Thus the point has norm at most $nM$. Choosing $R=2nM+2$ ensures that, whenever $P$ is nonempty, an entire radius-$r$ [Euclidean ball](../../../functional-analysis.md#euclidean-ball) in $P_\varepsilon$ lies inside $B(0,R)$.

Start with the [ellipsoid](../../../geometry-and-topology.md#ellipsoid) $E_0=B(0,R)$ and retain $K=P_\varepsilon\cap B(0,R)$. At each iteration test the centre $c$ against every relaxed inequality. If it passes all tests, $P_\varepsilon$ is nonempty and hence so is $P$. Otherwise a violated row gives the [separation oracle](../../../convex-optimization.md#separation-oracle): the feasible set lies in $\{x:A_i(x-c)\geq0\}$. Cut the current [ellipsoid](../../../geometry-and-topology.md#ellipsoid) by this [half-space](../../../geometry-and-topology.md#half-space) through its centre and replace it by the standard containing [ellipsoid](../../../geometry-and-topology.md#ellipsoid). Every step retains $K$ and, for $n\geq2$, reduces [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) by a factor at most $\exp[-1/(2(n+1))]$. In dimension one the corresponding step bisects an interval.

If more than $2n(n+1)\log(R/r)$ cuts occur without finding a feasible centre, the [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) is smaller than that of a radius-$r$ ball. This contradicts the retained ball whenever $P$ is nonempty, so the [algorithm](../../../computer-science.md#algorithm) can declare $P$ empty. Both $\log R$ and $\log(1/r)$ are polynomial in $n$ and $\log U$, and each inequality test uses $O(mn)$ arithmetic operations for $m$ rows. The bit implementation uses rational rounding with outward enlargement of the containing [ellipsoids](../../../geometry-and-topology.md#ellipsoid); the encoding bounds allow polynomial precision while keeping a constant fraction of the volume decrease. Detailed update and rounding formulae are not needed for this account. The essential role of the [full-dimensional relaxation of integer inequalities](../../../mathematical-optimization.md#full-dimensional-relaxation-of-integer-inequalities) is to supply a positive inner-volume bound without changing the emptiness decision; applying a [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) stopping test directly to a lower-dimensional $P$ would fail.

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $(j_1,\ldots,j_k)$ for the partial [assignment problem](../../../mathematical-optimization.md#assignment-problem) solution sending person $i$ to job $j_i$. The prescribed [assignment lower bound from independent task minima](../../../mathematical-optimization.md#assignment-lower-bound-from-independent-task-minima) is

$$
L(j_1,\ldots,j_k)=\sum_{i=1}^k a_{i,j_i}+\sum_{j\notin\{j_1,\ldots,j_k\}}\min_{i>k}a_{ij}.
$$

Every completion must pay at least the minimum in each remaining column, so this is a valid [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set), even if the minima use the same person several times. At $k=3$, the one remaining job must go to person 4, and the bound is the exact completed cost.

Use [branch and bound](../../../mathematical-optimization.md#branch-and-bound) with the smallest open bound expanded first. The initial bounds are

$$
\begin{array}{c|rrrr}
\text{prefix}&(1)&(2)&(3)&(4)\\
L&60&58&65&78
\end{array}
$$

For example, $L(2)=12+11+13+22=58$. Expand $(2)$, giving

$$
L(2,1)=68,\qquad L(2,3)=59,\qquad L(2,4)=64.
$$

Expand $(2,3)$. Its children are $(2,3,1)$ with bound 64 and $(2,3,4)$ with bound 65. Completing the first gives $(2,3,1,4)$ at cost 64, our first incumbent. The second cannot improve it. We may also discard $(2,1)$, $(2,4)$, $(3)$ and $(4)$, since their [lower bounds](../../../set.md#lower-bound-in-a-partially-ordered-set) are at least 64; equality may be pruned when seeking one optimum.

The remaining open prefix is $(1)$, whose children have bounds

$$
L(1,2)=68,\qquad L(1,3)=61,\qquad L(1,4)=66.
$$

Only $(1,3)$ can improve the incumbent. Its children $(1,3,2)$ and $(1,3,4)$ have exact completed costs 69 and 61, respectively. The latter completes to $(1,3,4,2)$ and replaces the incumbent. Every other branch has already been bounded above this value. Thus **the optimal assignment is**

$$
\boxed{1\mapsto1,\quad2\mapsto3,\quad3\mapsto4,\quad4\mapsto2,\qquad \text{cost}=11+13+23+14=61.}
$$

This [branch and bound](../../../mathematical-optimization.md#branch-and-bound) computation produces fourteen partial nodes: four initial nodes, three below $(2)$, two below $(2,3)$, three below $(1)$ and two below $(1,3)$. The last person is assigned automatically at a depth-three node.

For the [travelling salesman problem](../../../mathematical-optimization.md#travelling-salesman-problem), let $x_{ij}=1$ mean that the tour goes directly from city $i$ to city $j$. Retain only the constraints

$$
\sum_{j\ne i}x_{ij}=1,\qquad \sum_{i\ne j}x_{ij}=1,\qquad x_{ij}\in\{0,1\},\quad x_{ii}=0.
$$

This is an [assignment problem](../../../mathematical-optimization.md#assignment-problem) between cities as departure points and cities as arrival points, solvable by the [Hungarian algorithm](../../../mathematical-optimization.md#hungarian-algorithm). Its optimum is a [cycle cover of a directed graph](../../../graph-theory.md#cycle-cover-of-a-directed-graph), possibly with several disjoint cycles. Since every tour is such a cover, its cost is a [lower bound](../../../set.md#lower-bound-in-a-partially-ordered-set) on the best tour cost. This is the [assignment relaxation of the travelling salesman problem](../../../mathematical-optimization.md#assignment-relaxation-of-the-travelling-salesman-problem).

If the minimizing cover is a single [Hamiltonian cycle](../../../graph-theory.md#hamilton-cycle), it supplies a tour and can update the incumbent. Otherwise choose one proper subtour $C$. No tour can contain all [edges](../../../graph-theory.md#edge-of-a-graph) of $C$, since that would close a cycle before visiting the remaining cities. Make one child subproblem for each [edge](../../../graph-theory.md#edge-of-a-graph) of $C$, forbidding that [edge](../../../graph-theory.md#edge-of-a-graph), and solve its modified [assignment problem](../../../mathematical-optimization.md#assignment-problem). These branches may overlap but together retain every possible tour. Prune a child if it is infeasible or its assignment bound is at least the incumbent cost. Further subtours cause further branching. Each branch adds a new forbidden [edge](../../../graph-theory.md#edge-of-a-graph), so the search is finite, and the covering property plus the valid [lower bounds](../../../set.md#lower-bound-in-a-partially-ordered-set) proves optimality when no open branch remains. This enforces the effect of [subtour elimination constraints](../../../mathematical-optimization.md#subtour-elimination-constraints) through [branch and bound](../../../mathematical-optimization.md#branch-and-bound).

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Nash bargaining problem](../../../game-theory.md#nash-bargaining-problem) consists of a [compact convex set](../../../mathematical-optimization.md#compact-convex-set) $S$ of feasible two-player [payoff](../../../game-theory.md#payoff) [vectors](../../../vector-space.md#vector) and a [disagreement point](../../../game-theory.md#disagreement-point) $d\in S$. If bargaining fails, the players receive $d$; agreement selects a feasible [vector](../../../vector-space.md#vector). The [convex set](../../../mathematical-optimization.md#convex-set) allows jointly agreed [correlated payoff lotteries](../../../game-theory.md#lottery-over-joint-action-profiles) over outcomes. Assume essentiality: some feasible [vector](../../../vector-space.md#vector) strictly improves both coordinates of $d$. The admissible answers satisfy [bargaining individual rationality](../../../game-theory.md#bargaining-individual-rationality), $u_i\geq d_i$.

The four characterizing axioms are [Pareto efficiency](../../../mathematical-optimization.md#pareto-efficiency) (no feasible [vector](../../../vector-space.md#vector) weakly improves both chosen [payoffs](../../../game-theory.md#payoff) and strictly improves one), [bargaining symmetry](../../../game-theory.md#bargaining-symmetry) (interchanging identical player roles leaves the answer unchanged), [positive affine invariance in bargaining](../../../game-theory.md#positive-affine-invariance-in-bargaining) (independently replacing utilities by $a_i u_i+b_i$, $a_i>0$, transforms the answer by the same maps), and [bargaining independence of irrelevant alternatives](../../../game-theory.md#bargaining-independence-of-irrelevant-alternatives) (restricting to an admissible smaller feasible set that still contains the chosen [vector](../../../vector-space.md#vector) leaves the choice unchanged). The last axiom keeps the [disagreement point](../../../game-theory.md#disagreement-point) fixed.

The arbitration procedure maximizes the [Nash product](../../../game-theory.md#nash-product) over individually rational [vectors](../../../vector-space.md#vector):

$$
f(S,d)=\operatorname*{argmax}_{u\in S,\ u\geq d}(u_1-d_1)(u_2-d_2).
$$

A maximizer exists by [compactness](../../../topology.md#compact-space) and has positive gains by essentiality. It is unique, since the [logarithm](../../../calculus.md#logarithm) of the product is a [strictly concave function](../../../real-analysis.md#strictly-concave-function) of the two gains on their positive domain. The product is strictly increasing in either positive gain, giving [Pareto efficiency](../../../mathematical-optimization.md#pareto-efficiency). A positive affine utility change multiplies the product by $a_1a_2$, giving [positive affine invariance in bargaining](../../../game-theory.md#positive-affine-invariance-in-bargaining). Uniqueness gives [bargaining symmetry](../../../game-theory.md#bargaining-symmetry) and [bargaining independence of irrelevant alternatives](../../../game-theory.md#bargaining-independence-of-irrelevant-alternatives).

For completeness, these axioms also force the procedure. Normalize the product-maximizing [vector](../../../vector-space.md#vector) to $(1,1)$ and $d$ to zero using [positive affine invariance in bargaining](../../../game-theory.md#positive-affine-invariance-in-bargaining). For any normalized feasible [vector](../../../vector-space.md#vector) $z$, the [directional derivative](../../../calculus.md#directional-derivative) of the product along the feasible segment from $(1,1)$ to $z$ is $z_1+z_2-2$. The initial part of that segment has positive gains, so optimality implies $z_1+z_2\leq2$. Choose $M$ sufficiently large that the transformed feasible set is contained in the symmetric triangle

$$
T_M=\{z:z_1,z_2\geq-M,\ z_1+z_2\leq2\}.
$$

On this triangle, [bargaining symmetry](../../../game-theory.md#bargaining-symmetry) requires equal coordinates and [Pareto efficiency](../../../mathematical-optimization.md#pareto-efficiency) then forces $(1,1)$. By [bargaining independence of irrelevant alternatives](../../../game-theory.md#bargaining-independence-of-irrelevant-alternatives), restricting from $T_M$ to the original normalized set still selects $(1,1)$. Undoing the normalization proves the [Nash bargaining solution](../../../game-theory.md#nash-bargaining-solution) characterization. This is the [supporting triangle for Nash bargaining](../../../game-theory.md#supporting-triangle-for-nash-bargaining) argument.

For the numerical game, the maximin [disagreement point](../../../game-theory.md#disagreement-point) is the [vector](../../../vector-space.md#vector) of the players' separate [security level payoffs](../../../game-theory.md#security-level-payoff). If player I uses its first action with [probability](../../../probability-theory.md#probability) $p$, its worst expected [payoff](../../../game-theory.md#payoff) is

$$
\min\{4-2p,\ 2+6p\}.
$$

The two lines meet at $p=1/4$; before that point the increasing second line is smaller and afterwards the decreasing first line is smaller. Hence $d_1=7/2$. If player II uses its first action with [probability](../../../probability-theory.md#probability) $q$, its worst [payoff](../../../game-theory.md#payoff) is

$$
\min\{2+2q,\ 3+2q\}=2+2q,
$$

maximized at $q=1$, giving $d_2=4$. Thus **$d=(7/2,4)$**. These are separate worst-case guarantees; they need not equal the actual [payoffs](../../../game-theory.md#payoff) when both security strategies are used together.

The cooperative feasible set is the [convex hull](../../../mathematical-optimization.md#convex-hull) of the four outcome [vectors](../../../vector-space.md#vector). The outcomes $(2,4)$ and $(2,3)$ are dominated by $C=(4,5)$. Its [Pareto frontier](../../../mathematical-optimization.md#pareto-frontier) is the segment joining $C$ to $B=(8,2)$, with equation $y=8-3x/4$. Any maximizer of the positive [Nash product](../../../game-theory.md#nash-product) is on this frontier. [Bargaining individual rationality](../../../game-theory.md#bargaining-individual-rationality) restricts its relevant portion to $4\leq x\leq16/3$. There we maximize

$$
g(x)=(x-7/2)(4-3x/4),\qquad g'(x)=\frac{53}{8}-\frac32x,\qquad g''(x)=-\frac32.
$$

The stationary point lies strictly inside that interval and is the unique maximum. Therefore **the [Nash bargaining solution](../../../game-theory.md#nash-bargaining-solution) is**

$$
\boxed{(x,y)=\left(\frac{53}{12},\frac{75}{16}\right).}
$$

The gains are $11/12$ and $11/16$, with [Nash product](../../../game-theory.md#nash-product) $121/192$. The arbitration can implement the [vector](../../../vector-space.md#vector) by the agreed [correlated payoff lottery](../../../game-theory.md#lottery-over-joint-action-profiles) assigning [probability](../../../probability-theory.md#probability) $5/48$ to outcome $B$ and $43/48$ to outcome $C$. Indeed $4+4(5/48)=53/12$ and $5-3(5/48)=75/16$. This is a [correlated payoff lottery](../../../game-theory.md#lottery-over-joint-action-profiles); independent [mixed strategies](../../../game-theory.md#mixed-strategy) are not required to implement the cooperative agreement.

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $u_i$ denote player $i$'s expected [payoff](../../../game-theory.md#payoff), so the definition also covers [mixed strategies](../../../game-theory.md#mixed-strategy). If $p_i^*$ is a [dominant strategy](../../../game-theory.md#dominant-strategy), then

$$
u_i(p_i^*,p_{-i})\geq u_i(q_i,p_{-i})
$$

for every opponents' profile $p_{-i}$ and every alternative $q_i$. In particular this holds at $p_{-i}=p_{-i}^*$. Thus no player can improve its [payoff](../../../game-theory.md#payoff) by a unilateral deviation from $(p_1^*,\ldots,p_n^*)$, which is exactly the definition of a [Nash equilibrium](../../../game-theory.md#nash-equilibrium). **A profile of [dominant strategies](../../../game-theory.md#dominant-strategy) is a [Nash equilibrium](../../../game-theory.md#nash-equilibrium).**

For the [second-price sealed-bid auction](../../../game-theory.md#vickrey-auction), use the usual [private-value auction](../../../game-theory.md#private-value-auction) assumptions: a bidder with value $v$ has [quasilinear utility](../../../utility-function.md#quasilinear-utility) $v$ minus its payment if it wins, and zero if it loses. Fix the highest opposing bid $h$. If $h<v$, winning gives $v-h>0$, and bidding $v$ wins. If $h>v$, winning gives $v-h<0$, and bidding $v$ loses. If $h=v$, winning or losing gives zero, irrespective of the tie rule. Any other bid can only change whether the bidder wins, not the payment $h$ conditional on winning. It therefore cannot improve on the truthful bid in any of these cases. Hence **bidding the true value is a weakly [dominant strategy](../../../game-theory.md#dominant-strategy)**. Neither symmetry nor independence of the opposing values is needed for this argument.

For part (a), in a [first-price sealed-bid auction](../../../game-theory.md#first-price-sealed-bid-auction) with $n\geq2$, continuous nonnegative bids and $v>0$, no fixed bid is a [dominant strategy](../../../game-theory.md#dominant-strategy). A positive bid $b$ can be improved against opponents all bidding zero: replace it by $b/2>0$, still win, and increase the [payoff](../../../game-theory.md#payoff) by $b/2$. Bid zero can be improved against an opposing highest bid $h=v/2$: bidding $3v/4$ wins and earns $v/4>0$, whereas zero loses. This proves the [no dominant positive-value bid in a first-price auction](../../../game-theory.md#no-dominant-positive-value-bid-in-a-first-price-auction) result.

Allowing [mixed strategies](../../../game-theory.md#mixed-strategy) does not change that conclusion. Against all-zero opponents, a random bid has expected [payoff](../../../game-theory.md#payoff) strictly below $v$ unless it is always zero and the tie rule awards this bidder the item with certainty. Any positive bid incurs a strictly positive payment, and any [probability](../../../probability-theory.md#probability) of losing at zero also reduces the [payoff](../../../game-theory.md#payoff) below $v$. In the strict case choose a sufficiently small positive fixed bid $\delta$ so that $v-\delta$ exceeds the random bid's expected [payoff](../../../game-theory.md#payoff). In the exceptional case the preceding deviation against $h=v/2$ still improves it. The assumptions matter: for value zero, bid zero is weakly dominant; with only one bidder it is also optimal. Consequently **there is no [dominant strategy](../../../game-theory.md#dominant-strategy) for a positive-value bidder in the standard first-price setting**.

Part (b)'s printed nonexistence request is false under the stated [symmetric independent private values model](../../../game-theory.md#symmetric-independent-private-values-model). Lack of a [dominant strategy](../../../game-theory.md#dominant-strategy) does not imply lack of a [Nash equilibrium](../../../game-theory.md#nash-equilibrium). For incomplete private information the appropriate equilibrium is a [Bayesian Nash equilibrium](../../../game-theory.md#bayesian-nash-equilibrium), a [Nash equilibrium](../../../game-theory.md#nash-equilibrium) of the game whose strategies are bidding rules as functions of private values. Here is an explicit counterexample with a full deviation check.

Let the $n\geq2$ [risk-neutral](../../../utility-function.md#risk-neutrality) bidders have independent valuations with the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$, and put $a=(n-1)/n$. Suppose every opponent bids $\beta(w)=aw$. A bidder with value $v$ who bids $b\in[0,a]$ wins with [probability](../../../probability-theory.md#probability) $(b/a)^{n-1}$, since the opposing values must all be below $b/a$. Ties have [probability](../../../probability-theory.md#probability) zero, including at either endpoint. Its expected [quasilinear utility](../../../utility-function.md#quasilinear-utility) is

$$
U_v(b)=(v-b)(b/a)^{n-1}.
$$

For $b>0$,

$$
U_v'(b)=a^{-(n-1)}b^{n-2}\bigl((n-1)v-nb\bigr).
$$

Thus $U_v$ increases up to $b=av$ and decreases thereafter. For $v=0$, bid zero is optimal directly. A bid above $a$ wins with certainty and pays more than bidding $a$, so it cannot improve on the maximum already found in $[0,a]$. A randomized bid is a mixture of these [payoffs](../../../game-theory.md#payoff) and also cannot improve on their maximum. The [best response](../../../game-theory.md#best-response) for every value is therefore the proposed bidding rule itself. This proves the [uniform private-value first-price bidding equilibrium](../../../game-theory.md#uniform-private-value-first-price-bidding-equilibrium):

$$
\boxed{\beta(v)=\frac{n-1}{n}v\quad\text{is a symmetric Bayesian Nash equilibrium}.}
$$

The value-$v$ expected equilibrium [payoff](../../../game-theory.md#payoff) is $v^n/n$. The bidding rule is a [pure strategy](../../../game-theory.md#pure-strategy) in the Bayesian game, even though values are random. Therefore **the requested general nonexistence claim in (b) has a counterexample**, rather than a valid proof. The defect is present in the original PDF, not introduced by the converted text.

## 6

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

In a two-player [symmetric finite game](../../../game-theory.md#symmetric-finite-game), represent [mixed strategies](../../../game-theory.md#mixed-strategy) by [probability](../../../probability-theory.md#probability) [vectors](../../../vector-space.md#vector) and let $e(x,y)=x^TAy$ be the [payoff](../../../game-theory.md#payoff) to a player using $x$ against one using $y$. A resident strategy $x^*$ is an [evolutionarily stable strategy](../../../game-theory.md#evolutionarily-stable-strategy) if every distinct mutant strategy $y$ has an invasion barrier $\varepsilon_0(y)>0$ such that, for $0<\varepsilon<\varepsilon_0(y)$,

$$
e\bigl(x^*,(1-\varepsilon)x^*+\varepsilon y\bigr)>e\bigl(y,(1-\varepsilon)x^*+\varepsilon y\bigr).
$$

Thus when mutants are sufficiently rare, the resident has strictly larger fitness against the population mixture. The barrier may depend on the mutant; a common barrier is not part of this definition.

For fixed $y\ne x^*$ put

$$
a_y=e(x^*,x^*)-e(y,x^*),\qquad b_y=e(x^*,y)-e(y,y).
$$

By [bilinearity](../../../linear-algebra.md#bilinearity) the resident-minus-mutant fitness difference is

$$
(1-\varepsilon)a_y+\varepsilon b_y.
$$

If this is positive for all sufficiently small positive $\varepsilon$, taking $\varepsilon\downarrow0$ gives $a_y\geq0$. If $a_y=0$, strict positivity requires $b_y>0$. Conversely, if $a_y>0$, choose $0<\varepsilon_0\leq a_y/[2(a_y+|b_y|)]$; then the difference is at least $a_y-\varepsilon(a_y+|b_y|)>a_y/2>0$. If $a_y=0$ and $b_y>0$, it is $\varepsilon b_y>0$ for every $0<\varepsilon<1$. This proves the [two-condition criterion for evolutionary stability](../../../game-theory.md#two-condition-criterion-for-evolutionary-stability): **for every $y\ne x^*$, either**

$$
\boxed{e(x^*,x^*)>e(y,x^*)}
$$

**or**

$$
\boxed{e(x^*,x^*)=e(y,x^*)\quad\text{and}\quad e(x^*,y)>e(y,y).}
$$

The weak first comparison is the symmetric [Nash equilibrium](../../../game-theory.md#nash-equilibrium) condition; the second excludes neutrally competitive mutants when that comparison is an equality.

For the [Hawk-Dove game](../../../game-theory.md#hawk-dove-game), let $x^*=(1/2,1/2)$ and $y=(p,1-p)$, $0\leq p\leq1$. Against the resident, both [pure strategies](../../../game-theory.md#pure-strategy) give $1/2$, so

$$
e(x^*,x^*)=e(y,x^*)=\frac12.
$$

Direct multiplication of the [payoff matrix](../../../game-theory.md#payoff-matrix) gives

$$
e(x^*,y)=\frac32-2p,\qquad e(y,y)=1-2p^2.
$$

Consequently

$$
e(x^*,y)-e(y,y)=2\left(p-\frac12\right)^2>0\qquad(p\ne1/2).
$$

The equality case of the [two-condition criterion for evolutionary stability](../../../game-theory.md#two-condition-criterion-for-evolutionary-stability) therefore applies to every distinct mutant. More explicitly, the fitness difference in a mixed population is $2\varepsilon(p-1/2)^2$, positive for every $0<\varepsilon<1$. Hence **$\boxed{(1/2,1/2)\text{ is an evolutionarily stable strategy}}$**, with the common invasion barrier one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
