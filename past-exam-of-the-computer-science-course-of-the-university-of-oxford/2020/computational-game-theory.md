# Computational game theory

↑ **Parent:** [2020](../2020.md)

Source paper: [released examination archive](https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1), member `2019/T/a15684w1.pdf`. The dated cover identifies the undergraduate Second Public Examination, Trinity Term 2020, Friday 5 June, opening at 09:30 BST. The archive directory is misleading. The cover allows four hours for completion and upload; all printed parts are solved below.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)

## 1

↑ **Parent:** [Computational game theory](computational-game-theory.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use a simultaneous two-player [normal-form game](../../game-theory.md#normal-form-game), with X choosing the row and Y the column. Each player's [pure strategies](../../game-theory.md#pure-strategy) are $b$ and $nb$; a [payoff](../../game-theory.md#payoff) pair lists X first. Measure every dataset size in millions and use the stated normalization $M=1$. The source's reference to a shared half as “points” is interpreted in the same million-point units as the corpus, so the shared addition is $n/2$ to each initial dataset.

The [bimatrix game](../../game-theory.md#bimatrix-game) has [payoffs](../../game-theory.md#payoff)

$$
\begin{array}{c|cc}
 &Y:b&Y:nb\\ \hline
X:b&
\left(\dfrac{n+2}{2(n+3)}-\dfrac P2,\ 
\dfrac{n+4}{2(n+3)}-\dfrac P2\right)&
\left(\dfrac{n+1}{n+3}-P,\ \dfrac2{n+3}\right)\\[6pt]
X:nb&
\left(\dfrac1{n+3},\ \dfrac{n+2}{n+3}-P\right)&
\left(\dfrac13,\ \dfrac23\right).
\end{array}
$$

For example, joint purchase gives dataset sizes $1+n/2$ and $2+n/2$, total $3+n$, and each buyer pays $P/2$. A sole buyer gets the full corpus and pays $P$. The total [payoff](../../game-theory.md#payoff) is $1-P$ whenever a purchase occurs and $1$ when neither buys: the [game](../../game-theory.md#game) is not a [zero-sum game](../../game-theory.md#zero-sum-game), even though gross market shares always sum to one.

For the following calculations, set

$$
t=\frac n{n+3},\qquad 0<t<1.
$$

The [payoff](../../game-theory.md#payoff) differences “buy minus do not buy,” with the other player's action held fixed, are

$$
\begin{array}{c|cc}
 &\text{opponent does not buy}&\text{opponent buys}\\ \hline
\Delta_X&\dfrac{2t}{3}-P&\dfrac{t-P}{2}\\[4pt]
\Delta_Y&\dfrac t3-P&\dfrac{t-P}{2}.
\end{array}
$$

These four differences give all the [best response](../../game-theory.md#best-response) comparisons without mixing up row and column [payoffs](../../game-theory.md#payoff).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [weakly dominant strategy](../../game-theory.md#weakly-dominant-strategy) must be a [best response](../../game-theory.md#best-response) to either opponent action. For X this requires

$$
\frac{2t}{3}-P\ge0,\qquad\frac{t-P}{2}\ge0.
$$

The first is stronger because $t>0$. Thus

$$
\boxed{\text{X: }b\text{ is weakly dominant iff }0<P\le\frac{2n}{3(n+3)}.}
$$

For Y the comparisons are $t/3-P\ge0$ and $(t-P)/2\ge0$, giving

$$
\boxed{\text{Y: }b\text{ is weakly dominant iff }0<P\le\frac{n}{3(n+3)}.}
$$

Below each upper endpoint the corresponding [strategy](../../descriptive-set-theory.md#strategy-in-an-infinite-game) is strictly better against both opponent actions; at the endpoint one comparison ties and the other is strict. Thus the answers also satisfy the convention that weak dominance requires a strict advantage somewhere. Since [expected payoffs](../../game-theory.md#expected-payoff) are linear in the opponent's mixing [probability](../../probability-theory.md#probability), checking both opponent [pure strategies](../../game-theory.md#pure-strategy) suffices for every opponent [mixed strategy](../../game-theory.md#mixed-strategy).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At joint purchase, each player's gain from continuing to buy rather than deviating to $nb$ is $(t-P)/2$. Both actions are [best responses](../../game-theory.md#best-response) exactly when this is nonnegative. Therefore

$$
\boxed{(b,b)\text{ is a Nash equilibrium iff }0<P\le\frac n{n+3}.}
$$

At equality both players are indifferent to their individual [unilateral deviations](../../game-theory.md#unilateral-deviation), which is permitted in a [Nash equilibrium](../../game-theory.md#nash-equilibrium). The condition is less restrictive than requiring either player's action to be a [weakly dominant strategy](../../game-theory.md#weakly-dominant-strategy): only the opponent's actual action needs to be considered.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

When neither buys, X's [unilateral deviation](../../game-theory.md#unilateral-deviation) gains $2t/3-P$, while Y's gains $t/3-P$. For both to be nonpositive, $P$ must exceed the larger threshold. Hence

$$
\boxed{(nb,nb)\text{ is a Nash equilibrium iff }P\ge\frac{2n}{3(n+3)}.}
$$

Equality is included because a zero-gain deviation does not violate a [Nash equilibrium](../../game-theory.md#nash-equilibrium). Consequently both joint-purchase and joint-nonpurchase [Nash equilibria](../../game-theory.md#nash-equilibrium) exist throughout $2t/3\le P\le t$, a coordination region.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

**Neither asymmetric purchase outcome is a [Nash equilibrium](../../game-theory.md#nash-equilibrium) for any permitted $P>0,n>0$.** At $(b,nb)$, X's chosen purchase requires $P\le2t/3$, but Y's chosen nonpurchase, against X buying, requires $P\ge t$. These requirements are incompatible because $2t/3<t$.

At $(nb,b)$, Y's chosen purchase requires $P\le t/3$, whereas X's nonpurchase against a buying Y requires $P\ge t$. Again the inequalities are incompatible. Thus every [Nash equilibrium](../../game-theory.md#nash-equilibrium) in [pure strategies](../../game-theory.md#pure-strategy) has both players taking the same action; the conclusion is stronger than merely observing symmetry in their available actions, since their original market shares differ.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Write $P=999/1000$. If

$$
t>P\quad\Longleftrightarrow\quad
\frac n{n+3}>\frac{999}{1000}
\quad\Longleftrightarrow\quad
\boxed{n>2997},
$$

then both players prefer buying against a buyer, since $(t-P)/2>0$. Both prefer not buying against a nonbuyer: $2t/3<2/3<P$ and $t/3<1/3<P$. These strict opposite [best responses](../../game-theory.md#best-response) give the interior crossing of a [coordination game](../../game-theory.md#coordination-game).

An explicit [fully mixed Nash equilibrium](../../game-theory.md#fully-mixed-nash-equilibrium) follows from indifference. Let $p$ be X's [probability](../../probability-theory.md#probability) of buying and $q$ Y's. X is indifferent when

$$
(1-q)\left(\frac{2t}{3}-P\right)+q\frac{t-P}{2}=0,
$$

and Y is indifferent when

$$
(1-p)\left(\frac t3-P\right)+p\frac{t-P}{2}=0.
$$

Solving gives

$$
\boxed{
p=\frac{2(P-t/3)}{P+t/3},\qquad
q=\frac{2(P-2t/3)}{P-t/3},\qquad t=\frac n{n+3},\ n>2997.
}
$$

Both numerators and denominators are positive. For $p<1$ the required inequality is $2P-2t/3<P+t/3$, equivalent to $P<t$; the same comparison for $q<1$ again reduces to $P<t$. Thus $p,q\in(0,1)$, and the equations make both actions [best responses](../../game-theory.md#best-response) for each player. By linearity of [expected payoff](../../game-theory.md#expected-payoff), neither player can profit by any other [mixed strategy](../../game-theory.md#mixed-strategy). At $n=2997$ these formulas reach $p=q=1$ and are not fully mixed; the strict threshold matters.

## 2

↑ **Parent:** [Computational game theory](computational-game-theory.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**The assignment is [Pareto optimal](../../mathematical-optimization.md#pareto-efficiency).** Write $a_i$ for the room selected by the $i$th student. Suppose another assignment $a'$ makes every student at least as well off. The first student already selected their uniquely most valuable room, so $a'_1=a_1$. Once the rooms of students $1,\ldots,i-1$ are fixed, the rooms available to student $i$ in the original [serial dictatorship](../../game-theory.md#serial-dictatorship) are exactly the rooms that remain after those fixed assignments. Student $i$ chose the unique maximum among them, so weak improvement requires $a'_i=a_i$.

[Mathematical induction](../../foundations-of-mathematics.md#mathematical-induction) fixes every student's room. Thus $a'=a$ and nobody can be strictly better off, contradicting the definition of a [Pareto improvement](../../mathematical-optimization.md#pareto-improvement). Strict room rankings and the absence of [allocation externalities](../../game-theory.md#allocation-externality) are the essential assumptions: a student's [utility](../../mathematics.md#utility) is determined solely by their own room.[§13.2, Definition 13.1 and Theorem 13.2: Pareto efficiency for strict preferences](../../computer-science-bibliography.md#one-sided-matchings-house-allocation-problems-in-the-cornell-networks-and-markets-text)

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**No: arbitrary ties can produce an assignment that is not [Pareto optimal](../../mathematical-optimization.md#pareto-efficiency).** A two-student [counterexample](../../foundations-of-mathematics.md#counterexample) suffices. Give the first student value $1$ for both rooms; give the second student value $1$ for $r_1$ and $0$ for $r_2$. If the first student breaks the tie by taking $r_1$, the second must take $r_2$, and the [utility](../../mathematics.md#utility) [vector](../../vector-space.md#vector) is $(1,0)$.

Swapping the rooms gives [utility](../../mathematics.md#utility) [vector](../../vector-space.md#vector) $(1,1)$, so it is a [Pareto improvement](../../mathematical-optimization.md#pareto-improvement). Both choices in the original run maximized the corresponding student's available room value. The strict-ranking argument from (a) fails because the first student's [utility](../../mathematics.md#utility) need not decrease when that student's room changes.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**The equilibrium assignment is $(S_1,S_2,S_3,S_4)\mapsto(r_2,r_3,r_4,r_1)$, with [utility](../../mathematics.md#utility) [vector](../../vector-space.md#vector) $(0.7,0.7,0.9,0.4)$.** Apply [backward induction](../../foundations-of-mathematics.md#backward-induction) to the finite [perfect-information game](../../game-theory.md#perfect-information-game), accounting for the two friendship pairs in every terminal assignment. Student $S_4$ receives the last room and has no remaining choice. Given the first two rooms, $S_3$ chooses the remaining room maximizing their own room value plus $0.4$ if adjacent to $S_2$.

The following complete third-stage comparisons summarize the continuations. The [utility](../../mathematics.md#utility) in the last column is $S_2$'s resulting [utility](../../mathematics.md#utility), after $S_3$ makes the indicated [best response](../../game-theory.md#best-response).

| $S_1$ room | $S_2$ room | Optimal $S_3$ room | Resulting $U_2$ |
| --- | --- | --- | --- |
| $r_1$ | $r_2$ | $r_4$ | $0.5$ |
| $r_1$ | $r_3$ | $r_2$ | $0.7$ |
| $r_1$ | $r_4$ | $r_2$ | $0$ |
| $r_2$ | $r_1$ | $r_4$ | $0$ |
| $r_2$ | $r_3$ | $r_4$ | $0.7$ |
| $r_2$ | $r_4$ | $r_3$ | $0.4$ |
| $r_3$ | $r_1$ | $r_2$ | $0.4$ |
| $r_3$ | $r_2$ | $r_4$ | $0.5$ |
| $r_3$ | $r_4$ | $r_2$ | $0$ |
| $r_4$ | $r_1$ | $r_2$ | $0.4$ |
| $r_4$ | $r_2$ | $r_1$ or $r_3$ | $0.9$ |
| $r_4$ | $r_3$ | $r_2$ | $0.7$ |

For example, after $S_1$ takes $r_2$ and $S_2$ takes $r_3$, student $S_3$ compares $r_1$, giving $0$, with $r_4$, giving $0.5+0.4=0.9$. Choosing $r_4$ also gives $S_2$ the adjacency bonus, making $U_2=0.3+0.4=0.7$. The last room $r_1$ is adjacent to $S_1$'s $r_2$.

The table makes $S_2$ choose $r_3,r_3,r_2,r_2$ after first-stage choices $r_1,r_2,r_3,r_4$, respectively. Their resulting consequences for $S_1$ are $0.5,0.7,0$, and either $0$ or $0.4$. Thus $S_1$ strictly prefers $r_2$, proving the displayed outcome.

There is an off-path tie for $S_3$ after $(r_4,r_2)$, so the entire [subgame perfect equilibrium](../../game-theory.md#subgame-perfect-equilibrium) [strategy profile](../../game-theory.md#strategy-profile) need not be unique. Either choice, or any mixture of them, gives $S_1$ at most $0.4$ after choosing $r_4$, below $0.7$. The equilibrium assignment on the played path is therefore unaffected by this tie. Specifying these optimal continuations at every history, including the unplayed ones, supplies a [subgame perfect equilibrium](../../game-theory.md#subgame-perfect-equilibrium) rather than merely a proposed path.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**No. Strict room values do not remove the [allocation externalities](../../game-theory.md#allocation-externality) generated by friends.** Consider the following new instance, with the same friendship pairs $\{S_1,S_4\}$ and $\{S_2,S_3\}$ and friendship bonus $0.4$ for each student:

$$
\begin{array}{c|rrrr}
 &r_1&r_2&r_3&r_4\\ \hline
S_1&0.50&0.30&0.02&0.01\\
S_2&0.01&0.50&0.30&0.02\\
S_3&0.01&0.70&0.02&0.50\\
S_4&0.01&0.50&0.02&0.03
\end{array}
$$

Each row is strictly ranked and every room value is positive. In picking order $S_1,S_2,S_3,S_4$, [backward induction](../../foundations-of-mathematics.md#backward-induction) gives the following continuations. Room numbers in a tuple are listed in student order.

$$
\begin{array}{c|c|c}
S_1\text{ choice}&\text{resulting assignment}&U_1\\ \hline
r_1&(r_1,r_3,r_2,r_4)&0.50\\
r_2&(r_2,r_3,r_4,r_1)&0.70\\
r_3&(r_3,r_2,r_4,r_1)&0.02\\
r_4&(r_4,r_2,r_3,r_1)&0.01
\end{array}
$$

To check $S_2$'s incentives behind these continuations, the resulting [utilities](../../mathematics.md#utility) for their available choices, in ascending room order, are respectively $(0.50,0.70,0.02)$, $(0.01,0.70,0.42)$, $(0.41,0.50,0.02)$ and $(0.41,0.90,0.70)$. Student $S_3$'s own [best responses](../../game-theory.md#best-response) determine those figures, and $S_4$ again takes the remaining room. All comparisons selecting these continuations are strict.

Hence $S_1$ chooses $r_2$ and the [subgame perfect equilibrium](../../game-theory.md#subgame-perfect-equilibrium) outcome is

$$
a=(r_2,r_3,r_4,r_1),\qquad U(a)=(0.70,0.70,0.90,0.41).
$$

But the feasible assignment

$$
a'=(r_1,r_3,r_4,r_2),\qquad U(a')=(0.90,0.70,0.90,0.90)
$$

strictly improves $S_1$ and $S_4$ and leaves $S_2,S_3$ unchanged. Thus $a$ is not [Pareto optimal](../../mathematical-optimization.md#pareto-efficiency). This is compatible with equilibrium: a [Pareto improvement](../../mathematical-optimization.md#pareto-improvement) can require several players' actions to change. If $S_1$ alone takes $r_1$, the later [best responses](../../game-theory.md#best-response) lead to $(r_1,r_3,r_2,r_4)$, not to $a'$; anticipating that reaction gives $S_1$ only $0.50$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**Every [subgame perfect equilibrium](../../game-theory.md#subgame-perfect-equilibrium) outcome is [Pareto optimal](../../mathematical-optimization.md#pareto-efficiency) under the stated consecutive-friend and bonus conditions.** Partition the choosing order into blocks: a single student without a friend, or two friends who choose consecutively. Their slots in the choosing order are adjacent; the proof must separately establish when their allocated rooms will be adjacent.

Let $R$ be the rooms remaining before a friend block, with leader $i$ and follower $j$. Because $0\le v_{i,r},v_{j,r}\le1$ and $f_i,f_j>1$, each friend strictly prefers every adjacent-to-friend allocation to every nonadjacent one. After leader $i$ takes room $r$ with an available adjacent room, follower $j$ therefore takes their uniquely highest-valued room among the available neighbors of $r$. The leader consequently knows they will receive the adjacency bonus.

If $R$ contains at least one pair of adjacent rooms, let $E(R)$ be its nonisolated rooms: the rooms having an available neighbor. Leader $i$ must choose from $E(R)$, because choosing there guarantees [utility](../../mathematics.md#utility) greater than $1$, whereas an isolated choice gives at most $1$. Since the bonus is then fixed and room values are distinct, the leader chooses their unique maximum-value room in $E(R)$. The follower chooses their unique best neighbor. Later students cannot change either allocated room, so later play cannot alter these two students' [utilities](../../mathematics.md#utility).

If $R$ contains no adjacent pair, neither friend can obtain the bonus under any allocation of rooms from $R$. Both simply choose their uniquely most valuable remaining room in turn. Removing rooms cannot create a new physical adjacency, so no hidden later move can change that conclusion. A one-student block likewise chooses their unique best available room.

Now compare the equilibrium assignment $a$ with any proposed [Pareto improvement](../../mathematical-optimization.md#pareto-improvement) $a'$. Induct over these blocks, assuming earlier blocks' rooms are already fixed. Thus $a$ and $a'$ have the same remaining [set](../../set.md) $R$ at the present block. A lone student's room must stay fixed by strict preferences.

For a friend block obtaining adjacency in $a$, both students must retain adjacency in $a'$: losing a bonus larger than $1$ cannot be compensated by any room-value increase. The leader's room in $a'$ must therefore belong to $E(R)$. It cannot differ from the unique highest-valued room the leader selected there without reducing that leader's [utility](../../mathematics.md#utility). Once the leader's room is fixed, the follower likewise must retain the uniquely best available neighbor. If $R$ has no adjacent pair, both rooms stay fixed by the ordinary strict-ranking argument.

Thus every block's rooms are unchanged. The only assignment weakly improving all students is $a$ itself, so no strict improvement is possible. This proves [Pareto efficiency of serial dictatorship with consecutive friends](../../game-theory.md#pareto-efficiency-of-serial-dictatorship-with-consecutive-friends). The proof applies to every [subgame perfect equilibrium](../../game-theory.md#subgame-perfect-equilibrium), since the required choices at each block are strict [best responses](../../game-theory.md#best-response) determined by the available rooms.

## 3

↑ **Parent:** [Computational game theory](computational-game-theory.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [simple cooperative game](../../game-theory.md#simple-cooperative-game) is a [transferable utility game](../../game-theory.md#transferable-utility-game) $(N,v)$ with

$$
\boxed{v:2^N\to\{0,1\},\quad v(\varnothing)=0,\quad v(N)=1,\quad
S\subseteq T\Longrightarrow v(S)\le v(T).}
$$

A [coalition](../../game-theory.md#coalition-game-theory) of value $1$ is a [winning coalition](../../game-theory.md#winning-coalition); a value-$0$ [coalition](../../game-theory.md#coalition-game-theory) loses. The displayed definition uses the usual monotone, nontrivial convention: the empty [coalition](../../game-theory.md#coalition-game-theory) loses and the grand [coalition](../../game-theory.md#coalition-game-theory) wins.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

An [induced subgraph game](../../game-theory.md#induced-subgraph-game) is a [transferable utility game](../../game-theory.md#transferable-utility-game) represented by a weighted [undirected graph](../../graph-theory.md#undirected-graph) with one [vertex](../../graph.md#vertex-graph-theory) per player; a [coalition](../../game-theory.md#coalition-game-theory)'s value is the sum of the [edge weights](../../graph.md#edge-weight) in its [induced subgraph](../../graph-theory.md#induced-subgraph). With no [self-loops](../../graph.md#loop-graph-theory),

$$
\boxed{v(S)=\sum_{\{i,j\}\subseteq S,\ i\ne j}w_{ij},}
$$

where each unordered pair is counted once and an absent [edge](../../graph-theory.md#edge-of-a-graph) has weight zero. Weights may have either sign. In an [induced subgraph game with self-loops](../../game-theory.md#induced-subgraph-game-with-self-loops), write the loop weight at $i$ as $\ell_i$ and add $\sum_{i\in S}\ell_i$, counting each loop once. In particular, $v(\{i\})=\ell_i$ when loops are allowed and is zero otherwise.[§1, printed p. 258: weighted induced-subgraph representation; the self-loop extension is stated explicitly here](../../mathematics-bibliography.md#on-the-complexity-of-cooperative-solution-concepts-by-xiaotie-deng-and-christos-papadimitriou)

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**No representation exists, even allowing arbitrary signed weights and [self-loops](../../graph.md#loop-graph-theory).** Every singleton [coalition](../../game-theory.md#coalition-game-theory) loses, so each loop weight must be $\ell_i=v(\{i\})=0$. Every two-player [coalition](../../game-theory.md#coalition-game-theory) wins, which then forces

$$
w_{12}=w_{13}=w_{23}=1.
$$

The represented grand-[coalition](../../game-theory.md#coalition-game-theory) value would consequently be

$$
v(\{1,2,3\})=\ell_1+\ell_2+\ell_3+w_{12}+w_{13}+w_{23}=3,
$$

contradicting its required value $1$. The obstruction is the additive [edge](../../graph-theory.md#edge-of-a-graph) representation, not a restriction that weights be nonnegative: the singleton and pair values already determine every relevant weight.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

**Yes; without [self-loops](../../graph.md#loop-graph-theory), such a nontrivial [simple cooperative game](../../game-theory.md#simple-cooperative-game) has exactly one positive [edge](../../graph-theory.md#edge-of-a-graph), of weight $1$.** For each pair,

$$
w_{ij}=v(\{i,j\})\in\{0,1\},
$$

because singleton and loop contributions are zero. Summing all [edge weights](../../graph.md#edge-weight) gives $v(N)=1$, so precisely one unordered pair $\{a,b\}$ has weight $1$, and all other pairs have weight zero.

Thus the [winning coalitions](../../game-theory.md#winning-coalition) are exactly those containing both $a$ and $b$. For any $0\le\lambda\le1$, set

$$
\boxed{x_a=\lambda,\quad x_b=1-\lambda,\quad x_i=0\quad(i\notin\{a,b\}).}
$$

This [payoff](../../game-theory.md#payoff) [vector](../../vector-space.md#vector) is efficient, since $\sum_i x_i=v(N)=1$. Every [winning coalition](../../game-theory.md#winning-coalition) receives $1$ and every losing [coalition](../../game-theory.md#coalition-game-theory) receives a nonnegative total, so all inequalities $x(S)\ge v(S)$ hold. Hence it belongs to the [core of a cooperative game](../../game-theory.md#core-game-theory).

In fact these are all [core](../../game-theory.md#core-game-theory) allocations. Singleton conditions require $x_i\ge0$, and the winning pair requires $x_a+x_b\ge1$; efficiency then forces equality and zero [payoffs](../../game-theory.md#payoff) outside the pair. The endpoints are both [veto players](../../game-theory.md#veto-player), consistent with the general characterization of the [core of a simple cooperative game](../../game-theory.md#core-of-a-simple-cooperative-game).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

**No. Two positive [self-loops](../../graph.md#loop-graph-theory) and one negative [edge](../../graph-theory.md#edge-of-a-graph) give a [simple cooperative game](../../game-theory.md#simple-cooperative-game) with an empty [core of a cooperative game](../../game-theory.md#core-game-theory).** Give players $1,2$ loop weights $\ell_1=\ell_2=1$, put $w_{12}=-1$, and give every other loop and [edge](../../graph-theory.md#edge-of-a-graph) weight zero. For a [coalition](../../game-theory.md#coalition-game-theory) $S$,

$$
v(S)=\mathbf1_{\{1\in S\}}+\mathbf1_{\{2\in S\}}
-\mathbf1_{\{\{1,2\}\subseteq S\}}
=\mathbf1_{\{S\cap\{1,2\}\ne\varnothing\}}.
$$

Thus a [coalition](../../game-theory.md#coalition-game-theory) wins exactly when it contains player $1$ or player $2$. This is monotone, has values in $\{0,1\}$, and satisfies $v(\varnothing)=0,v(N)=1$. Extra players for any $n\ge3$ do not alter any [coalition](../../game-theory.md#coalition-game-theory) value.

The [core](../../game-theory.md#core-game-theory) singleton inequalities would require $x_1\ge1$, $x_2\ge1$ and $x_i\ge0$ for every other player, while efficiency requires $\sum_i x_i=1$. These requirements are inconsistent. Equivalently, the two disjoint winning singleton [coalitions](../../game-theory.md#coalition-game-theory) leave no [veto player](../../game-theory.md#veto-player). Signed weights are essential to this particular representation and are permitted in the [induced subgraph game](../../game-theory.md#induced-subgraph-game) model.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

**A loop-free [induced subgraph game](../../game-theory.md#induced-subgraph-game) is a [convex cooperative game](../../game-theory.md#convex-cooperative-game) if and only if every [edge weight](../../graph.md#edge-weight) is nonnegative.** Necessity follows by applying the [supermodular](../../function.md#supermodular-set-function) inequality to $S=\{i\}$ and $T=\{j\}$. Since both singleton values and the empty value are zero,

$$
v(\{i,j\})+v(\varnothing)\ge v(\{i\})+v(\{j\})
\quad\Longrightarrow\quad w_{ij}\ge0.
$$

Conversely, direct cancellation of common [edge](../../graph-theory.md#edge-of-a-graph) contributions gives, for any [coalitions](../../game-theory.md#coalition-game-theory) $S,T$,

$$
v(S\cup T)+v(S\cap T)-v(S)-v(T)
=\sum_{\substack{i\in S\setminus T\\j\in T\setminus S}}w_{ij}.
$$

Every summand is nonnegative, proving that $v$ is a [supermodular set function](../../function.md#supermodular-set-function) and hence convexity. Equivalently, a player's [marginal contribution](../../game-theory.md#marginal-contribution) to $S$ is $\Delta_i(S)=\sum_{j\in S}w_{ij}$, which cannot decrease as $S$ grows. This establishes the [convexity criterion for an induced subgraph game](../../game-theory.md#convexity-criterion-for-an-induced-subgraph-game) directly.[§1, printed p. 258, nonnegative-weight convexity; §2.2, printed p. 260, discussion preceding Lemma 4](../../mathematics-bibliography.md#on-the-complexity-of-cooperative-solution-concepts-by-xiaotie-deng-and-christos-papadimitriou)

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

**There is exactly one such nontrivial game for every $n\ge1$: the [unanimity game](../../game-theory.md#unanimity-game) requiring every player.** Put

$$
\boxed{u_N(S)=
\begin{cases}
1,&S=N,\\
0,&S\ne N.
\end{cases}
\qquad\text{Number of games}=1.}
$$

It is a [simple cooperative game](../../game-theory.md#simple-cooperative-game), and permuting players preserves every [coalition](../../game-theory.md#coalition-game-theory) value. Thus it has the required [symmetry of players in a cooperative game](../../game-theory.md#symmetry-of-players-in-a-cooperative-game). It is also a [convex cooperative game](../../game-theory.md#convex-cooperative-game): if both $S,T$ are winning, all four terms in the [supermodular](../../function.md#supermodular-set-function) inequality have value $1$; if exactly one is winning, their union is $N$ and their intersection loses, giving equality $1=1$; if neither wins, the right-hand side is zero and the inequality follows from nonnegativity. For $n=1$ the same definition gives the sole player value $1$.

To prove uniqueness, first establish that [convex simple games are unanimity games](../../game-theory.md#convex-simple-games-are-unanimity-games). If $S,T$ are [winning coalitions](../../game-theory.md#winning-coalition), the [supermodular](../../function.md#supermodular-set-function) inequality gives

$$
2=v(S)+v(T)\le v(S\cup T)+v(S\cap T)\le2,
$$

so their intersection is also winning. The family of [winning coalitions](../../game-theory.md#winning-coalition) is finite and nonempty. Its intersection $K$ is therefore winning and nonempty, since the empty [coalition](../../game-theory.md#coalition-game-theory) loses. Every winning [coalition](../../game-theory.md#coalition-game-theory) contains $K$, and monotonicity makes every superset of $K$ winning. Hence $v=u_K$.

If $K$ were a proper nonempty [subset](../../set.md#subset) of $N$, take $i\in K$ and $j\notin K$, and let $T=N\setminus\{i,j\}$. Then $T\cup\{i\}=N\setminus\{j\}$ contains $K$ and wins, whereas $T\cup\{j\}=N\setminus\{i\}$ loses. This violates [symmetry of players in a cooperative game](../../game-theory.md#symmetry-of-players-in-a-cooperative-game), which requires those two [coalition](../../game-theory.md#coalition-game-theory) values to agree. Thus $K=N$, proving the claimed count. The “nontrivial” convention excludes the identically zero game; if that degenerate game were also called simple, it would supply one additional symmetric convex example.

## ↑ Ancestors (8)

1. [2020](../2020.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
