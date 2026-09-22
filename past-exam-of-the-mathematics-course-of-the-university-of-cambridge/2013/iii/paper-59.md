# Paper 59

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_59.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_59.pdf)

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
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Cook-Levin theorem](../../../computer-science.md#cook-levin-theorem) states that the [Boolean satisfiability problem](../../../computer-science.md#boolean-satisfiability-problem) is [NP-complete](../../../computer-science.md#np-completeness) under [polynomial-time many-one reductions](../../../computer-science.md#polynomial-time-many-one-reduction). Membership in [NP](../../../computer-science.md#np-complexity) follows by guessing an assignment and evaluating the formula in time polynomial in its description length.

For hardness, let $L\in\mathrm{NP}$ have a deterministic polynomial-time verifier $M(x,y)$, with a polynomial witness-length bound. Use a fixed polynomial [certificate](../../../computer-science.md#certificate-complexity) length: a short [certificate](../../../computer-science.md#certificate-complexity) is encoded by its length followed by padded data, and the verifier checks this encoding. Pad the computation to exactly $T=T(|x|)$ steps, with accepting and rejecting states absorbing. Enlarge $T$ polynomially if necessary to cover input/witness initialization. A standard polynomial slowdown permits a single-tape [Turing machine](../../../computer-science.md#turing-machine), so it suffices to handle that model.

Encode a tape cell by a fixed number of bits recording its alphabet symbol and either no head or the head's finite control state. Starting with one head, a cell's next label depends only on its own label and the two neighboring labels: a head can change the symbol where it sits and can enter only a neighbor. Each such finite local function has a constant-size [Boolean circuit](../../../computer-science.md#boolean-circuit). The initial row fixes $x$, blanks and the starting head, leaving only the witness bits as [Boolean circuit](../../../computer-science.md#boolean-circuit) inputs. There are $O(T)$ relevant cells with blank margins beyond every possible head position, and $T$ updates. Repeating these local [Boolean circuits](../../../computer-science.md#boolean-circuit) produces a [Boolean circuit](../../../computer-science.md#boolean-circuit) $C_x(y)$ of size $O(T^2)$, with an output detecting an accepting head in the final row. The construction is computable in [polynomial time](../../../computer-science.md#polynomial-time). Induction on rows shows that every assignment to $y$ produces exactly the verifier's valid computation; invalid local encodings can be assigned arbitrary [Boolean circuit](../../../computer-science.md#boolean-circuit) behavior because they never arise from the valid initial row.

Convert this [Boolean circuit](../../../computer-science.md#boolean-circuit) to [conjunctive normal form](../../../computer-science.md#conjunctive-normal-form) using a [Tseitin transformation](../../../computer-science.md#tseytin-transformation). Introduce one variable for each wire, and encode each gate output $z$ by:

| Gate relation | [Clauses](../../../computer-science.md#clause-of-a-boolean-formula) imposing equivalence |
| --- | --- |
| $z=x\wedge y$ | $(\neg z\vee x)\wedge(\neg z\vee y)\wedge(z\vee\neg x\vee\neg y)$ |
| $z=x\vee y$ | $(z\vee\neg x)\wedge(z\vee\neg y)\wedge(\neg z\vee x\vee y)$ |
| $z=\neg x$ | $(z\vee x)\wedge(\neg z\vee\neg x)$ |

Unit [clauses](../../../computer-science.md#clause-of-a-boolean-formula) fix constant sources and assert the final output. Each input assignment has exactly one extension to its gate values, so the resulting formula $F_x$ is satisfiable precisely when some witness makes $M(x,y)$ accept. It has $O(T^2)$ [clauses](../../../computer-science.md#clause-of-a-boolean-formula) of bounded length and is produced in [polynomial time](../../../computer-science.md#polynomial-time). Thus

$$
\boxed{x\in L\iff F_x\text{ is satisfiable},\qquad\mathrm{SAT}\text{ is NP-complete}}.
$$

This proof also gives hardness for [clauses](../../../computer-science.md#clause-of-a-boolean-formula) of at most three [literals](../../../computer-science.md#boolean-literal), without needing a separate satisfiability assumption.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A proposed assignment for [2UN-SAT](../../../computer-science.md#2un-sat) can be checked in [polynomial time](../../../computer-science.md#polynomial-time), including checking the syntactic restriction, so the language belongs to [NP](../../../computer-science.md#np-complexity).

For an explicit reduction, parse any [Boolean formula](../../../computer-science.md#boolean-formula) into a [Boolean circuit](../../../computer-science.md#boolean-circuit) over binary AND ([logical conjunction](../../../mathematical-logic.md#logical-conjunction)), binary OR ([logical disjunction](../../../mathematical-logic.md#logical-disjunction)) and unary NOT ([negation](../../../computer-science.md#negation)), and apply the gate equivalences in part (a), asserting its output. Every gate [clause](../../../computer-science.md#clause-of-a-boolean-formula) has at most two positive [literals](../../../computer-science.md#boolean-literal): the AND [clauses](../../../computer-science.md#clause-of-a-boolean-formula) have respectively one, one and one; the OR [clauses](../../../computer-science.md#clause-of-a-boolean-formula) have one, one and two; and the NOT [clauses](../../../computer-science.md#clause-of-a-boolean-formula) have two and zero. The unit output/constant [clauses](../../../computer-science.md#clause-of-a-boolean-formula) also obey the restriction. Hence the resulting formula is an instance of [2UN-SAT](../../../computer-science.md#2un-sat).

The [Tseitin transformation](../../../computer-science.md#tseytin-transformation) is linear in the gate description, and its auxiliary variables enforce the gate values rather than relaxing their relation to the inputs. Therefore the original formula is satisfiable if and only if the transformed restricted formula is satisfiable. This is a [polynomial-time many-one reduction](../../../computer-science.md#polynomial-time-many-one-reduction) from [SAT](../../../computer-science.md#boolean-satisfiability-problem), whose hardness follows from the [Cook-Levin theorem](../../../computer-science.md#cook-levin-theorem). Consequently

$$
\boxed{\mathrm{2UN\text{-}SAT}\text{ is NP-complete}}.
$$

The condition limits positive [literals](../../../computer-science.md#boolean-literal), without limiting total [clause](../../../computer-science.md#clause-of-a-boolean-formula) length.

## 2

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

With a read-only input tape, [deterministic space complexity class](../../../computer-science.md#deterministic-space-complexity-class) $\mathrm{SPACE}(s(n))$ consists of languages decidable by deterministic [Turing machines](../../../computer-science.md#turing-machine) using $O(s(n))$ work-tape cells. The [nondeterministic space complexity class](../../../computer-science.md#nondeterministic-space-complexity-class) $\mathrm{NSPACE}(s(n))$ uses [Nondeterministic Turing machines](../../../computer-science.md#nondeterministic-turing-machine), with the bound holding on every computation path and acceptance meaning that some path accepts. Input storage is not charged. We use the standard finite-state, fixed-alphabet model.

The [Savitch theorem](../../../computer-science.md#savitch-s-theorem) is

$$
\boxed{s(n)\geq\log_2 n\Longrightarrow\mathrm{NSPACE}(s(n))\subseteq\mathrm{SPACE}(s(n)^2)}.
$$

First suppose a work-space budget $m\geq\lceil\log_2(n+2)\rceil$ is available. A [configuration graph](../../../computer-science.md#configuration-graph) for computations restricted to $m$ cells has configurations encoded in $O(m)$ bits: work contents, control state and head positions, including $O(\log n)$ bits for the input head. Its size is at most $2^{cm}$ for a machine-dependent constant $c$. Add accept and exit sinks if needed; the size bound merely changes $c$. A reachable configuration has a simple path of length smaller than the number of configurations.

For encoded configurations $u,v$, define $R(u,v,k)$ to ask whether a path of length at most $2^k$ exists. At $k=0$, test equality or one transition. For $k>0$, enumerate every candidate middle configuration $w$ and test

$$
R(u,v,k)=\bigvee_w\bigl[R(u,w,k-1)\wedge R(w,v,k-1)\bigr].
$$

Any path of the given length can be split into two halves of length at most $2^{k-1}$; conversely concatenation gives a path of length at most $2^k$. This proves the recursion. Taking $k=\lceil cm\rceil$ suffices. Depth is $O(m)$, and each recursive frame stores only its endpoints, the current middle configuration and counters in $O(m)$ bits. The two recursive calls are made sequentially and reuse their space. The total is $O(m^2)$, even though the time can be very large.

The printed hypothesis does not say that $s$ is computable. The [space-bound discovery by exit reachability](../../../computer-science.md#space-bound-discovery-by-exit-reachability) removes that issue. Begin with $m=\lceil\log_2(n+2)\rceil$ and use the preceding recursion to test both whether an accepting state is reachable within the budget and whether a reachable state has a transition leaving the budget. Accept in the first case. If acceptance is absent and an exit is reachable, double $m$ and repeat. If neither is reachable, reject: all computations remain within this finite [configuration graph](../../../computer-science.md#configuration-graph), and none accepts.

Every path of the original machine uses at most $C s(n)$ cells. Once $m$ reaches that bound there can be no reachable exit, so this procedure terminates. The final budget is $O(s(n))$ by doubling, and all stages reuse the same storage. Hence its deterministic space is $O(s(n)^2)$ without requiring a machine that first computes $s(n)$. This proves the stated general form.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Here a directed cycle has at least one edge. If zero-length paths were treated as cycles, an edgeless one-vertex [graph](../../../graph.md) would already satisfy the predicate; that convention would give the trivial nonempty-graph predicate instead of the intended [directed cycle detection](../../../computer-science.md#directed-cycle-detection) problem.

For [NL](../../../computer-science.md#nl-complexity) membership, guess a starting vertex $v$, follow a guessed directed walk for between one and $N=|V|$ edges, and accept if it returns to $v$. Store only the start, current vertex and step counter. A [graph](../../../graph.md) with a nonempty closed walk contains a simple directed cycle of at most $N$ edges, including a self-loop if present. Thus the algorithm uses [logarithmic space](../../../computer-science.md#logarithmic-space) and is complete for the predicate.

For hardness, reduce the [directed graph reachability problem](../../../computer-science.md#st-connectivity) to cycle detection. Form $G^{(N+1)}$ and add the single backward arc

$$
(t,N+1)\longrightarrow(s,1).
$$

All layering arcs advance exactly one layer, including the waiting arcs $(v,i)\to(v,i+1)$, so the layered [graph](../../../graph.md) alone is a [Directed acyclic graph](../../../combinatorics.md#directed-acyclic-graph). Any cycle in the augmented [graph](../../../graph.md) must contain the backward arc and therefore contains a path from $(s,1)$ to $(t,N+1)$.

If $t$ is reachable from $s$ in $G$, use a simple path of length at most $N-1$ and pad it with waits to exactly $N$ steps. It becomes the required layered path and closes to a cycle. Conversely, projecting such a layered path and deleting waits gives a walk from $s$ to $t$ in $G$. This includes the case $s=t$, where reachability has a zero-length witness but the augmented [graph](../../../graph.md) has a genuinely positive-length cycle.

There are $N(N+1)$ vertices and polynomially many arcs. A transducer enumerates pairs/layers and checks old adjacency by scanning its input, using only $O(\log N)$ bits. Hence this is a [logspace many-one reduction](../../../computer-science.md#logspace-many-one-reduction), proving

$$
\boxed{\mathrm{CYCLE}\text{ is NL-complete}}.
$$

## 3

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [circuit size class](../../../computer-science.md#circuit-size-class) $\mathrm{SIZE}(T(n))$ consists of languages whose length-$n$ [indicator functions](../../../measure-theory.md#indicator-function) have [Boolean circuits](../../../computer-science.md#boolean-circuit) of size at most $T(n)$, for all sufficiently large $n$, over a fixed finite bounded-fan-in complete basis. The notation $\mathrm{SIZE}(O(T(n)))$ allows a constant factor. Input-node counting conventions do not affect the polynomial and exponential bounds here.

The nonuniform class [P/poly](../../../computer-science.md#p-poly) is

$$
\boxed{\mathrm{P/poly}=\bigcup_{d\geq0}\mathrm{SIZE}(O(n^d))}.
$$

There is no requirement that a uniform algorithm construct the [Boolean circuits](../../../computer-science.md#boolean-circuit). Equivalently, a polynomial-time machine can receive polynomial-length advice depending only on the input length, and the advice need not be computable.

Choose an [undecidable](../../../foundations-of-mathematics.md#undecidable-decision-problem) set $A\subseteq\mathbb N$, for example the set in the [halting problem](../../../foundations-of-mathematics.md#halting-problem) of indices of machines that halt on empty input, and define $U_A=\{1^n:n\in A\}$. For each length $n$, use a constant-zero [Boolean circuit](../../../computer-science.md#boolean-circuit) if $n\notin A$, and an AND of all $n$ input bits if $n\in A$. These [Boolean circuits](../../../computer-science.md#boolean-circuit) have size $O(n+1)$ and accept exactly $U_A$. Thus [undecidable unary languages with linear-size circuits](../../../computer-science.md#undecidable-unary-languages-with-linear-size-circuits) belong to [P/poly](../../../computer-science.md#p-poly).

Every [NP](../../../computer-science.md#np-complexity) language is decidable by enumerating its finitely many polynomial-length [certificate](../../../computer-science.md#certificate-complexity) encodings and running the polynomial-time verifier. If $U_A$ were decidable, testing $1^n$ would decide $A$, a contradiction. Therefore

$$
\boxed{U_A\in\mathrm{P/poly}\setminus\mathrm{NP},\qquad\mathrm{P/poly}\ne\mathrm{NP}}.
$$

This separates the classes in the stated direction; it does not claim that [NP](../../../computer-science.md#np-complexity) is not contained in [P/poly](../../../computer-science.md#p-poly).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For each fixed input length, take the complete truth table of the language. For every accepted string $z\in\{0,1\}^n$, form the minterm

$$
M_z(x)=\bigwedge_{i=1}^n\begin{cases}x_i,&z_i=1,\\\neg x_i,&z_i=0.\end{cases}
$$

An OR of these minterms equals the [indicator function](../../../measure-theory.md#indicator-function), since $M_z(x)=1$ precisely at $x=z$. This is the [truth-table upper bound for circuit size](../../../computer-science.md#truth-table-upper-bound-for-circuit-size).

Generate the $n$ negated input wires once and share them. With $m\leq2^n$ accepted strings, use at most $m(n-1)$ binary AND gates and $m-1$ binary OR gates, besides the [negations](../../../computer-science.md#negation). Empty truth tables use a constant-zero [Boolean circuit](../../../computer-science.md#boolean-circuit); length zero is handled by a constant [Boolean circuit](../../../computer-science.md#boolean-circuit). Thus

$$
\boxed{L\in\mathrm{SIZE}(O(n2^n))\quad\text{for every }L\subseteq\{0,1\}^*}.
$$

This is an existence bound for a nonuniform [circuit family](../../../computer-science.md#circuit-family), even when the language is [undecidable](../../../foundations-of-mathematics.md#undecidable-decision-problem). It supplies no algorithm for computing the truth tables of an arbitrary language.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [AND-NOT circuit value problem](../../../computer-science.md#and-not-circuit-value-problem) belongs to [P](../../../computer-science.md#p-complexity): validate the [Boolean circuit](../../../computer-science.md#boolean-circuit) and evaluate its gates in a [topological ordering](../../../combinatorics.md#topological-ordering). Evaluation takes [polynomial time](../../../computer-science.md#polynomial-time) even if its description is not already in a [topological ordering](../../../combinatorics.md#topological-ordering).

For [P-completeness](../../../computer-science.md#p-completeness) we use [logspace many-one reductions](../../../computer-science.md#logspace-many-one-reduction). Start from the supplied [circuit value problem](../../../computer-science.md#circuit-value-problem) over the usual AND ([logical conjunction](../../../mathematical-logic.md#logical-conjunction)), OR ([logical disjunction](../../../mathematical-logic.md#logical-disjunction)) and NOT ([negation](../../../computer-science.md#negation)) basis. Retain AND and NOT gates, and replace every OR gate by the [De Morgan's laws](../../../computer-science.md#de-morgan-s-laws) gadget

$$
\boxed{x\vee y=\neg(\neg x\wedge\neg y)}.
$$

This adds only a constant number of gates per old gate, preserves its truth value for all inputs and keeps the [Boolean circuit](../../../computer-science.md#boolean-circuit) acyclic. If the format includes constant source nodes, replace them by additional input nodes assigned fixed bits zero and one; these are inputs, not disallowed gates. Larger fan-in gates can first be replaced by binary trees of their inputs.

To output the new description, keep the old gate index and a constant-size gadget position, rescan old references when necessary, and assign consistent new indices to each gadget's terminal output. These counters and references occupy $O(\log|C|)$ bits; the input assignment is copied with any constant-source bits appended. Thus the construction is a [logspace many-one reduction](../../../computer-science.md#logspace-many-one-reduction) preserving acceptance. Since [Boolean circuit](../../../computer-science.md#boolean-circuit) Value is [P-complete](../../../computer-science.md#p-completeness) under such reductions,

$$
\boxed{\mathrm{AND\text{-}NOT\ CIRCUIT\ VALUE}\text{ is P-complete}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The class [NC1](../../../computer-science.md#nc1) consists of languages having polynomial-size, bounded-fan-in [Boolean circuit](../../../computer-science.md#boolean-circuit) families of depth $O(\log n)$. Under a uniform convention one requires the wiring to be constructible in [logarithmic space](../../../computer-science.md#logarithmic-space); the construction below meets that requirement as well as the nonuniform one.

Write a length-$n$ binary input with most significant bit first as $x_1\cdots x_n$. Since $2^m\equiv(-1)^m\pmod3$,

$$
x\equiv\sum_{i=1}^n(-1)^{n-i}x_i\pmod3.
$$

Represent residues zero, one and two by two bits, respectively $00,01,10$. Each input produces residue zero when it is zero; when it is one it produces residue one or two according to the parity of $n-i$. This uses only constants and wires.

A two-residue addition modulo three is a fixed function of four [Boolean variables](../../../computer-science.md#boolean-variable) and has a constant-size, constant-depth bounded-fan-in [Boolean circuit](../../../computer-science.md#boolean-circuit). Define its unused $11$ encodings arbitrarily; valid inputs always produce a valid residue encoding. Use a balanced binary tree of these adders, padding with zero residues to a power of two. There are $O(n)$ adders and $O(\log n)$ layers. A final constant-size gate checks that the residue is $00$.

This [balanced finite-monoid reduction circuit](../../../computer-science.md#balanced-finite-monoid-reduction-circuit) is uniform: leaf signs follow index parity and internal connections follow the indices in the balanced tree, all calculable in [logarithmic space](../../../computer-science.md#logarithmic-space). Leading zeros cause no difficulty; the empty input can be assigned the zero-integer constant convention. Consequently

$$
\boxed{\mathrm{MOD3}\in\mathrm{NC}^1}.
$$

## 4

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [decision tree](../../../computer-science.md#decision-tree) queries individual input bits, chooses subsequent queries from previous answers and labels each leaf with an output. Its [decision-tree depth](../../../computer-science.md#decision-tree-depth) is the largest number of queries on any root-to-leaf path; $D(f)$ is the least such depth over trees computing $f$. An [evasive Boolean function](../../../computer-science.md#evasive-boolean-function) on $n$ bits has $D(f)=n$.

Remove repeated queries along any path, since their answers are already known. A leaf at depth $r\leq d<n$ fixes $r$ bits and leaves at least one bit free. The inputs reaching it form a subcube on which $f$ is constant, say $b$. Its contribution to the alternating sum is

$$
b(-1)^{\sum\text{fixed bits}}\prod_{\text{free bits}}(1-1)=0.
$$

Here $\operatorname{wt}(x)$ is the [Hamming weight](../../../coding-theory.md#hamming-weight). The leaf subcubes partition the input cube, so adding their contributions proves

$$
\boxed{D(f)<n\Longrightarrow\sum_{x\in\{0,1\}^n}(-1)^{\operatorname{wt}(x)}f(x)=0}.
$$

The contrapositive is the [alternating-sum criterion for decision-tree evasiveness](../../../computer-science.md#alternating-sum-criterion-for-decision-tree-evasiveness): a nonzero alternating sum forces all $n$ bits to be necessary in the worst case.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $N=\binom n2$ be the number of independent undirected-edge bits; use unordered pairs $i<j$. The paper's [common-center graph property](../../../graph-theory.md#common-center-graph-property) means that all present edges share a vertex. Isolated vertices are allowed, and the empty [graph](../../../graph.md) satisfies the property. This convention matters in the count.

The empty [graph](../../../graph.md) contributes $+1$ to the alternating sum. The $N$ one-edge [graphs](../../../graph.md) contribute $-N$. A [graph](../../../graph.md) with at least two edges and a common center has a unique center, since two different edges have just that common endpoint. For a fixed center, its possible edge sets are subsets of the $n-1$ incident edges. Their contribution after removing sets of size zero and one is

$$
\sum_{k=2}^{n-1}(-1)^k\binom{n-1}{k}
=(1-1)^{n-1}-1+(n-1)=n-2.
$$

These [graphs](../../../graph.md) are counted once for each of their unique centers. Thus the [alternating count of common-center graphs](../../../graph-theory.md#alternating-count-of-common-center-graphs) is

$$
\boxed{\sum_G(-1)^{|E(G)|}\mathrm{STAR}_n(G)
=1-\binom n2+n(n-2)=\frac{(n-1)(n-2)}2\ne0\quad(n\geq3)}.
$$

Part (a) gives $D(\mathrm{STAR}_n)\geq N$, while querying all $N$ bits always suffices. Therefore

$$
\boxed{D(\mathrm{STAR}_n)=\binom n2;\quad\mathrm{STAR}_n\text{ is evasive}}.
$$

The relevant input length is $N$, not the number $n$ of [graph](../../../graph.md) vertices.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A [query certificate](../../../computer-science.md#query-certificate) for input $x$ is a subset $S$ of coordinates such that every $y$ agreeing with $x$ on $S$ has the same value of $f$. Define [certificate complexity of a Boolean function](../../../computer-science.md#certificate-complexity-of-a-boolean-function) by

$$
C(f,x)=\min\{|S|:S\text{ certifies }f(x)\},\quad C_b(f)=\max_{f(x)=b}C(f,x),\quad C(f)=\max(C_0,C_1).
$$

If no input has output $b$, take $C_b(f)=0$. Unlike a [decision tree](../../../computer-science.md#decision-tree), a [query certificate](../../../computer-science.md#query-certificate) may be selected with full knowledge of the input.

Take a full [star graph](../../../graph-theory.md#star-graph-theory) centered at $v$, containing all $n-1$ incident edges and no others. For any edge $e$ not incident to $v$, changing only its bit from zero to one destroys the [common-center graph property](../../../graph-theory.md#common-center-graph-property): two spokes already force $v$ as the only possible common endpoint. Therefore every positive [query certificate](../../../computer-science.md#query-certificate) for this input must include every nonincident edge bit, otherwise this one-bit change would preserve its answers but change the output. There are $\binom{n-1}{2}$ such bits. Conversely, fixing all those bits to zero suffices for a [query certificate](../../../computer-science.md#query-certificate), because all remaining edges are incident to $v$. Hence

$$
\boxed{C_1(\mathrm{STAR}_n)=\binom{n-1}{2},\qquad C(\mathrm{STAR}_n)=\Omega(n^2)}.
$$

The upper bound for $C_1$ holds for any accepted [graph](../../../graph.md) by choosing any valid center and certifying its nonincident edges absent.

For completeness, the negative side is much smaller. Given a [graph](../../../graph.md) with no common center, choose a present edge $\{a,b\}$, an edge not containing $a$, and an edge not containing $b$. These at most three present edges have empty common intersection and certify rejection. A triangle with isolated additional vertices needs all three of its present edges: with at most two queries, set every unqueried edge absent and the remaining present edges share a vertex. Thus the [certificates for the common-center graph property](../../../graph-theory.md#certificates-for-the-common-center-graph-property) satisfy

$$
\boxed{C_0(\mathrm{STAR}_n)=3,\qquad C(\mathrm{STAR}_n)=\max\left\{3,\binom{n-1}{2}\right\}\quad(n\geq3)}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
