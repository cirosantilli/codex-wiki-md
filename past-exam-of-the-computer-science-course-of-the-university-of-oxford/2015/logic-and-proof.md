# Logic and proof

↑ **Parent:** [2015](../2015.md)

Solutions to the three questions of the [University of Oxford](../../university-of-oxford.md) [computer science](../../computer-science.md) Finals examination held on 10 June 2015. Question 3(d) has a false assertion as printed; its solution gives a [countermodel](../../mathematical-logic.md#countermodel) and explains the additional hypotheses under which the usual [least Herbrand model](../../mathematical-logic.md#least-herbrand-model) argument works.[Cover and printed pp. 2–4, Questions 1–3; the unrestricted quantifier-free matrix in Question 3(d) is visible on printed p. 4](../../computer-science-bibliography.md#logic-and-proof-examination-paper-of-the-university-of-oxford-2015)

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
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [A](#3/a/a)
      - [Solution](#3/a/a/solution)
    - [B](#3/a/b)
      - [Solution](#3/a/b/solution)
    - [C](#3/a/c)
      - [Solution](#3/a/c/solution)
    - [D](#3/a/d)
      - [Solution](#3/a/d/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)

## 1

↑ **Parent:** [Logic and proof](logic-and-proof.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Apply the distributive law of [Boolean algebra](../../mathematical-logic.md#boolean-algebra) to the two [logical conjunctions](../../mathematical-logic.md#logical-conjunction). With $A=P$, $B=\neg Q$, $C=\neg P$, and $D=Q$, the identity $(A\land B)\lor(C\land D)\equiv(A\lor C)\land(A\lor D)\land(B\lor C)\land(B\lor D)$ gives

$$
\begin{aligned}
(P\land\neg Q)\lor(\neg P\land Q)
&\equiv(P\lor\neg P)\land(P\lor Q)\land(\neg Q\lor\neg P)\land(\neg Q\lor Q)\\
&\equiv\top\land(P\lor Q)\land(\neg P\lor\neg Q)\land\top\\
&\equiv\boxed{(P\lor Q)\land(\neg P\lor\neg Q).}
\end{aligned}
$$

The second step uses complementation and commutativity in [Boolean algebra](../../mathematical-logic.md#boolean-algebra); the last uses the identity law for [logical conjunction](../../mathematical-logic.md#logical-conjunction). The result is in [conjunctive normal form](../../theoretical-computer-science.md#conjunctive-normal-form): its first [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) requires at least one input to be true, and its second [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) prohibits both inputs being true. Together they express [exclusive or](../../theoretical-computer-science.md#exclusive-or).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Replace each implication by a [logical disjunction](../../mathematical-logic.md#logical-disjunction) and use the [conjunctive normal form](../../theoretical-computer-science.md#conjunctive-normal-form) for [exclusive or](../../theoretical-computer-science.md#exclusive-or) from part (a). The resulting [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula) are

$$
\begin{array}{c|l}
F_1&C_1=\neg H\lor Y\\
F_2&C_2=\neg T\lor\neg I\\
F_3&C_3=H\lor T,\quad C_4=\neg H\lor\neg T\\
F_4&C_5=Y\lor I,\quad C_6=\neg Y\lor\neg I.
\end{array}
$$

Here the displayed array is a list of the six [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula), whose [logical conjunction](../../mathematical-logic.md#logical-conjunction) is equivalent to all four constraints.

Use [resolution](../../mathematical-logic.md#resolution) first on $I$, then on $T$, and finally on $H$:

$$
\begin{aligned}
C_7&=\operatorname{Res}_{I}(C_2,C_5)=\neg T\lor Y,\\
C_8&=\operatorname{Res}_{T}(C_3,C_7)=H\lor Y,\\
C_9&=\operatorname{Res}_{H}(C_1,C_8)=Y\lor Y=\boxed{Y.}
\end{aligned}
$$

Removing the repeated [Boolean literal](../../theoretical-computer-science.md#boolean-literal) in the final [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) uses idempotence. Neither $C_4$ nor $C_6$ is needed: even the weaker assumptions that the coin has at least one outcome and that at least one person wins already force $Y$, once the two implications hold.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take the single [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula)

$$
\boxed{F=P\lor Q\lor R.}
$$

This is a [3-CNF formula](../../theoretical-computer-science.md#3-cnf-formula). Suppose a [2-CNF formula](../../theoretical-computer-science.md#2-cnf-formula) $K$ were [logically equivalent](../../mathematical-logic.md#logical-equivalence) to $F$. Every [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) $C$ of $K$ would then be a consequence of $F$.

Consider any nontautological [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) $C$ containing at most two [Boolean literals](../../theoretical-computer-science.md#boolean-literal). Choose a [Boolean valuation](../../mathematical-logic.md#boolean-valuation) falsifying its [Boolean literals](../../theoretical-computer-science.md#boolean-literal). At least one of $P,Q,R$ does not occur in $C$; assign that [Boolean variable](../../theoretical-computer-science.md#boolean-variable) true. The resulting [Boolean valuation](../../mathematical-logic.md#boolean-valuation) satisfies $F$ while falsifying $C$. This contradicts $F\models C$. An empty [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) also cannot be a consequence of the satisfiable $F$.

Consequently every [Boolean clause](../../theoretical-computer-science.md#clause-of-a-boolean-formula) of $K$ would have to be a tautology. Their [logical conjunction](../../mathematical-logic.md#logical-conjunction) would be true under every [Boolean valuation](../../mathematical-logic.md#boolean-valuation), whereas $F$ is false when $P=Q=R=0$. This proves that no such $K$ exists.

The argument even allows additional ordinary [Boolean variables](../../theoretical-computer-science.md#boolean-variable) in $K$: at most two [Boolean literals](../../theoretical-computer-science.md#boolean-literal) still leave one of $P,Q,R$ free to be made true. Introducing extra variables together with [existential quantification](../../mathematical-logic.md#existential-quantification) would change the requested notion of [logical equivalence](../../mathematical-logic.md#logical-equivalence), so it is not a way around the argument.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Enumerate the [vertices](../../graph.md#vertex-graph-theory) as $V=\{1,\ldots,n\}$ and introduce a [Boolean variable](../../theoretical-computer-science.md#boolean-variable) $X_{u,v}$ for each ordered pair of [vertices](../../graph.md#vertex-graph-theory). Its intended meaning is that a proposed [graph automorphism](../../graph.md#graph-automorphism) sends $u$ to $v$. Build four groups of [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula).

First require exactly one image for each [vertex](../../graph.md#vertex-graph-theory):

$$
A=\bigwedge_{u\in V}\left[
\left(\bigvee_{v\in V}X_{u,v}\right)
\land\bigwedge_{v<w}(\neg X_{u,v}\lor\neg X_{u,w})\right].
$$

Next require that distinct [vertices](../../graph.md#vertex-graph-theory) have distinct images:

$$
B=\bigwedge_{v\in V}\bigwedge_{u<w}(\neg X_{u,v}\lor\neg X_{w,v}).
$$

Together $A$ and $B$ specify an injective [function](../../function.md) $f:V\to V$. Since $V$ is finite, this [function](../../function.md) is a [bijection](../../function.md#bijection); a separate surjectivity condition is unnecessary.

Write $e(u,w)=1$ when $(u,w)\in E$ and $e(u,w)=0$ otherwise. Prohibit every pair of images that would change adjacency:

$$
C=\bigwedge_{\substack{u,w,v,z\in V\\ e(u,w)\ne e(v,z)}}
(\neg X_{u,v}\lor\neg X_{w,z}).
$$

Checking both possible mismatches preserves both edges and nonedges. Finally require a moved [vertex](../../graph.md#vertex-graph-theory):

$$
D=\bigvee_{u\in V}\neg X_{u,u}.
$$

The desired [propositional formula](../../mathematical-logic.md#propositional-formula) is

$$
\boxed{\varphi_G=A\land B\land C\land D.}
$$

If a [Boolean valuation](../../mathematical-logic.md#boolean-valuation) satisfies $\varphi_G$, $A$ selects a unique image for every [vertex](../../graph.md#vertex-graph-theory), $B$ makes the resulting [function](../../function.md) a [bijection](../../function.md#bijection), $C$ preserves adjacency in both directions, and $D$ makes this [graph automorphism](../../graph.md#graph-automorphism) different from the [identity function](../../function.md#identity-function). Conversely, given such a [graph automorphism](../../graph.md#graph-automorphism) $f$, set $X_{u,v}$ true exactly when $v=f(u)$. Each of $A,B,C,D$ is then satisfied.

There are $n^2$ [Boolean variables](../../theoretical-computer-science.md#boolean-variable), $O(n^3)$ image and injectivity [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula), and at most $n^4$ adjacency [Boolean clauses](../../theoretical-computer-science.md#clause-of-a-boolean-formula). With the [graph](../../graph.md) stored by its [adjacency matrix](../../graph-theory.md#adjacency-matrix), testing a mismatch takes constant time. Thus the construction has [polynomial time](../../theoretical-computer-science.md#polynomial-time) and output length $O(n^4\log(n+1))$ with binary-indexed variable names. For $n=0$, interpret the empty [logical disjunction](../../mathematical-logic.md#logical-disjunction) $D$ as false; for $n=1$, $A$ and $D$ conflict. These cases correctly have no nonidentity [graph automorphism](../../graph.md#graph-automorphism).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [propositional compactness theorem](../../mathematical-logic.md#propositional-compactness-theorem) states that an arbitrary set $S$ of [propositional formulas](../../mathematical-logic.md#propositional-formula) is satisfiable if and only if every finite [subset](../../set.md#subset) of $S$ is satisfiable:

$$
\boxed{S\text{ has a model}\quad\Longleftrightarrow\quad
\text{every finite }S_0\subseteq S\text{ has a model}.}
$$

The satisfying [Boolean valuation](../../mathematical-logic.md#boolean-valuation) may depend on $S_0$ on the right; the conclusion on the left provides one [Boolean valuation](../../mathematical-logic.md#boolean-valuation) satisfying all of $S$ simultaneously.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Let $S=\{F_i:i\ge1\}$. Every finite [subset](../../set.md#subset) of $S$ is satisfiable: if $F_N$ has the largest index occurring, the successive [semantic entailments](../../mathematical-logic.md#semantic-entailment) imply $F_N\models F_i$ for every earlier index, so any [Boolean valuation](../../mathematical-logic.md#boolean-valuation) satisfying $F_N$ satisfies that finite [subset](../../set.md#subset). The [propositional compactness theorem](../../mathematical-logic.md#propositional-compactness-theorem) therefore also shows that $S$ itself is satisfiable.

Suppose that $G$ had exactly the common models of $S$. Then $S\models G$, and hence $S\cup\{\neg G\}$ is unsatisfiable. By the [propositional compactness theorem](../../mathematical-logic.md#propositional-compactness-theorem), finitely many $F_i$ together with $\neg G$ are already unsatisfiable. Enlarge the finite list if necessary so it is nonempty, and let $N$ be its greatest index. We obtain

$$
F_N\models G.
$$

On the other hand, the asserted equality of model classes gives $G\models F_{N+1}$. Transitivity of [semantic entailment](../../mathematical-logic.md#semantic-entailment) would yield

$$
F_N\models F_{N+1},
$$

contradicting the strictness assumption at index $N$. Thus

$$
\boxed{\text{No single propositional formula defines the common models of all }F_i.}
$$

The obstruction is the finite character of [propositional formulas](../../mathematical-logic.md#propositional-formula): a single consequence of an infinite set already follows from finitely many premises, whereas this chain continues to impose strictly stronger requirements forever.

## 2

↑ **Parent:** [Logic and proof](logic-and-proof.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [first-order theory](../../mathematical-logic.md#first-order-theory) in a fixed [first-order signature](../../mathematical-logic.md#first-order-signature) is a set of [first-order sentences](../../mathematical-logic.md#first-order-sentence). Under the closed-theory convention used in the question, it contains all its [semantic entailments](../../mathematical-logic.md#semantic-entailment): $T\models\theta$ implies $\theta\in T$. One can equivalently begin with a set of axioms and take its closure under consequence.

A [complete theory](../../model-theory.md#complete-theory) is a consistent [first-order theory](../../mathematical-logic.md#first-order-theory) that decides every [first-order sentence](../../mathematical-logic.md#first-order-sentence) $\theta$ in its [first-order signature](../../mathematical-logic.md#first-order-signature):

$$
\boxed{T\models\theta\quad\text{or}\quad T\models\neg\theta.}
$$

Consistency ensures that exactly one of these alternatives holds.

A [decidable theory](../../mathematical-logic.md#decidable-theory) is one for which an [algorithm](../../algorithm.md) always terminates and determines whether a given [first-order sentence](../../mathematical-logic.md#first-order-sentence) is a consequence:

$$
\boxed{\{\theta:T\models\theta\}\text{ is decidable}.}
$$

If the [first-order theory](../../mathematical-logic.md#first-order-theory) is already closed under consequence, this is its membership problem. It is a condition on the consequences, not merely on whether the chosen set of axioms has a decidable membership test.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A [first-order theory](../../mathematical-logic.md#first-order-theory) $T$ admits [quantifier elimination](../../model-theory.md#quantifier-elimination) when every [first-order formula](../../mathematical-logic.md#first-order-formula) $\varphi(\bar x)$ has a [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) $\psi(\bar x)$, in the same [first-order signature](../../mathematical-logic.md#first-order-signature) and with no additional [free variables](../../mathematical-logic.md#free-variable), such that

$$
\boxed{T\models\forall\bar x\,[\varphi(\bar x)\leftrightarrow\psi(\bar x)].}
$$

Thus all [first-order models](../../mathematical-logic.md#model-of-a-first-order-theory) of $T$ agree that the two [first-order formulas](../../mathematical-logic.md#first-order-formula) define the same tuples. This definition concerns [first-order formulas](../../mathematical-logic.md#first-order-formula) with [free variables](../../mathematical-logic.md#free-variable), as well as [first-order sentences](../../mathematical-logic.md#first-order-sentence); merely deciding closed assertions would be weaker. The existence of an effective procedure is an additional issue, supplied by the explicit construction in part (d).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the [Rado graph](../../random-graph.md#rado-graph) on the [natural numbers](../../arithmetic.md#natural-number). Interpret the binary relation by

$$
\boxed{E(i,j)\quad\Longleftrightarrow\quad
[i<j\land\mathit{Bit}(i,j)]\lor[j<i\land\mathit{Bit}(j,i)].}
$$

The relation is symmetric by its definition, and $E(i,i)$ is always false. Thus this [first-order structure](../../mathematical-logic.md#first-order-structure) satisfies $F_1$ and $F_2$.

To verify an extension axiom, take distinct $x_1,\ldots,x_n$. Choose a [natural number](../../arithmetic.md#natural-number) $k$ larger than every $x_i$ and put

$$
y=2^k+\sum_{i=1}^{m-1}2^{x_i}.
$$

The powers are distinct, so there are no carries in this [binary representation](../../arithmetic.md#binary-number). In particular $y>x_i$ for every $i$, and the [bit](../../information-theory.md#bit) in position $x_i$ is one exactly when $i<m$. Therefore $y$ is different from all the given [vertices](../../graph.md#vertex-graph-theory), is adjacent to $x_1,\ldots,x_{m-1}$, and is not adjacent to the others. If the $x_i$ are not distinct, the antecedent of the extension axiom is false, so it places no restriction. The case $n=0$, if included in the convention for [natural numbers](../../arithmetic.md#natural-number), simply asks for a nonempty domain, which this [first-order structure](../../mathematical-logic.md#first-order-structure) has.

For example, prescribing adjacency to $1$ and $3$ and nonadjacency to $2$ permits $k=4$ and $y=16+2+8=26$, whose [binary representation](../../arithmetic.md#binary-number) is $11010$. This explicitly realizes the required pattern. Hence

$$
\boxed{(\mathbb N,E)\models T_0.}
$$

Reordering a tuple makes the extension axioms applicable to any two disjoint finite sets of [vertices](../../graph.md#vertex-graph-theory), with any desired adjacency and nonadjacency pattern. This is the extension property defining the [theory of the random graph](../../model-theory.md#theory-of-the-random-graph).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

It suffices to eliminate one [existential quantifier](../../mathematical-logic.md#existential-quantification) from a [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) $\theta(y,\bar x)$. Indeed, [logical connectives](../../mathematical-logic.md#logical-connective) preserve equivalence, and a [universal quantifier](../../mathematical-logic.md#universal-quantification) can be rewritten using $\forall y\,\alpha\equiv\neg\exists y\,\neg\alpha$. An induction on the construction of a [first-order formula](../../mathematical-logic.md#first-order-formula) then eliminates all its [quantifiers](../../mathematical-logic.md#quantifier) from the inside out.

Convert $\theta$ to [disjunctive normal form](../../theoretical-computer-science.md#disjunctive-normal-form). Since [existential quantification](../../mathematical-logic.md#existential-quantification) distributes over a finite [logical disjunction](../../mathematical-logic.md#logical-disjunction), consider a single [logical conjunction](../../mathematical-logic.md#logical-conjunction) of atomic [first-order formulas](../../mathematical-logic.md#first-order-formula) and their negations. There are no function or constant symbols in this [first-order signature](../../mathematical-logic.md#first-order-signature), so its atoms are equalities between variables and instances of $E$ between variables.

For a tuple $\bar x=(x_1,\ldots,x_r)$, enumerate its possible complete atomic diagrams $\delta(\bar x)$. Such a [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) specifies which variables are equal and, between distinct equality classes, exactly which pairs are adjacent. Keep only the diagrams in which [first-order equality](../../mathematical-logic.md#logical-equality) is an [equivalence relation](../../set-theory.md#equivalence-relation) and $E$ is symmetric and irreflexive. There are finitely many diagrams for each $r$, and every tuple in a [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory) of $T$ satisfies exactly one of them. Every retained diagram is realizable: insert one [vertex](../../graph.md#vertex-graph-theory) for each equality class successively, using the extension axioms to prescribe its adjacency to earlier [vertices](../../graph.md#vertex-graph-theory).

Fix one diagram $\delta$. A potential [existential witness](../../mathematical-logic.md#existential-witness) for $y$ has one of two forms.

- **An existing [vertex](../../graph.md#vertex-graph-theory).** If $y=x_i$, substitute $x_i$ for $y$ in the [logical conjunction](../../mathematical-logic.md#logical-conjunction). The diagram $\delta$ decides the [truth value](../../mathematical-logic.md#truth-value) of every resulting atom, and so decides whether this choice works.
- **A new [vertex](../../graph.md#vertex-graph-theory).** Require $y\ne x_i$ for every $i$. Simplify $y=y$ to true and $E(y,y)$ to false. Use symmetry to rewrite every remaining edge requirement involving $y$ in the form $E(x_i,y)$ or $\neg E(x_i,y)$. An equality $y=x_i$, a positive loop requirement, or opposite edge requirements on the same equality class makes this case impossible. Otherwise the requirements give a consistent adjacency pattern on finitely many distinct [vertices](../../graph.md#vertex-graph-theory). Any equality classes without a specified edge requirement can be assigned either pattern. Reorder representatives with the desired neighbours first; the appropriate extension axiom supplies a fresh [vertex](../../graph.md#vertex-graph-theory) with precisely this pattern.

All [first-order formulas](../../mathematical-logic.md#first-order-formula) involving only $\bar x$ are already decided by $\delta$. Therefore, for each diagram, the existence of a suitable $y$ has a definite answer, determined by a finite syntactic test. Let $\mathcal D$ be the set of diagrams for which at least one disjunct and at least one of the two witness cases succeeds. Then

$$
\boxed{T\models\forall\bar x\left[
\exists y\,\theta(y,\bar x)\leftrightarrow
\bigvee_{\delta\in\mathcal D}\delta(\bar x)\right].}
$$

The right side is a [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula). An empty [logical disjunction](../../mathematical-logic.md#logical-disjunction) means false, and for an empty tuple the empty atomic diagram means true. These logical truth constants also handle closed [first-order sentences](../../mathematical-logic.md#first-order-sentence) in this constant-free [first-order signature](../../mathematical-logic.md#first-order-signature).

For a concrete illustration of the fresh-witness case,

$$
T\models\forall x_1\forall x_2\forall x_3\left[
\exists y\,(E(y,x_1)\land\neg E(y,x_2)\land y\ne x_3)
\leftrightarrow x_1\ne x_2\right].
$$

If $x_1=x_2$, the edge requirements conflict. Otherwise the extension property supplies a [vertex](../../graph.md#vertex-graph-theory) outside the finite set of parameters with the desired pattern; the extra avoidance of $x_3$ causes no obstruction. The general diagram construction handles all such equality coincidences systematically and proves [quantifier elimination](../../model-theory.md#quantifier-elimination).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

By part (c), $T$ has a [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory), so it is consistent. By part (d), every [first-order sentence](../../mathematical-logic.md#first-order-sentence) is equivalent modulo $T$ to a [quantifier-free sentence](../../mathematical-logic.md#quantifier-free-sentence). In the [first-order signature](../../mathematical-logic.md#first-order-signature) consisting only of $E$ and [first-order equality](../../mathematical-logic.md#logical-equality), there are no constant symbols, no ground [first-order terms](../../mathematical-logic.md#first-order-term), and no nullary predicates. Thus a closed [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) reduces to true or false, using the logical truth constants. All [first-order models](../../mathematical-logic.md#model-of-a-first-order-theory) of $T$ therefore agree on every [first-order sentence](../../mathematical-logic.md#first-order-sentence):

$$
\boxed{T\text{ is complete}.}
$$

The construction in part (d) is effective. Conversion to [disjunctive normal form](../../theoretical-computer-science.md#disjunctive-normal-form), enumeration of finite equality partitions and adjacency patterns, and testing the finitely many witness cases are all terminating operations. Apply them recursively to a given [first-order sentence](../../mathematical-logic.md#first-order-sentence) and evaluate the final truth constant. This decides whether the [first-order sentence](../../mathematical-logic.md#first-order-sentence) belongs to $T$, giving

$$
\boxed{T\text{ is decidable}.}
$$

No useful bound on the running time is needed for decidability; the potentially large enumeration still always terminates.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Use the [back-and-forth method](../../model-theory.md#back-and-forth-method). Enumerate the two domains without repetitions as $a_0,a_1,\ldots$ and $b_0,b_1,\ldots$. We construct a sequence of finite maps, each a [partial isomorphism of structures](../../model-theory.md#partial-embedding),

$$
f_0\subseteq f_1\subseteq f_2\subseteq\cdots,
$$

starting with the empty [function](../../function.md). Each $f_s$ is a [bijection](../../function.md#bijection) between finite subsets of the domains and preserves both adjacency and nonadjacency on its domain.

At a **forth** step, choose the first $a_i$ outside the current domain. List the finitely many domain [vertices](../../graph.md#vertex-graph-theory) as $u_1,\ldots,u_r$. In $\mathcal B$, prescribe that the new image $b$ be adjacent to $f_s(u_j)$ exactly when $a_i$ is adjacent to $u_j$ in $\mathcal A$. Since the image [vertices](../../graph.md#vertex-graph-theory) are distinct, an extension axiom in $\mathcal B$ supplies such a $b$ outside the entire current range. Extend $f_s$ by $a_i\mapsto b$. This preserves injectivity, adjacency and nonadjacency, including the absence of loops.

At a **back** step, choose the first $b_i$ outside the current range. Apply the same argument to the inverse [partial isomorphism of structures](../../model-theory.md#partial-embedding) in $\mathcal A$, finding a fresh preimage with the required adjacency pattern to the current domain. Extend $f_s$ by this new pair. Alternate forth and back steps indefinitely.

Define

$$
\boxed{f=\bigcup_{s\ge0}f_s.}
$$

Because each finite [function](../../function.md) extends the preceding one, this is a well-defined injective [function](../../function.md). The forth steps eventually include every $a_i$ in its domain, and the back steps eventually include every $b_i$ in its range, so $f$ is a [bijection](../../function.md#bijection). Given any $u,v$, both lie in the domain of some finite $f_s$, where the edge equivalence already holds. It therefore also holds for $f$:

$$
\boxed{(u,v)\in E_{\mathcal A}\quad\Longleftrightarrow\quad
(f(u),f(v))\in E_{\mathcal B}.}
$$

Thus the two [first-order structures](../../mathematical-logic.md#first-order-structure) are isomorphic. Alternating the steps is essential for surjectivity: repeatedly extending only the domain would merely construct an embedding into $\mathcal B$.

## 3

↑ **Parent:** [Logic and proof](logic-and-proof.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

Use unary predicates $H$ and $M$ for happiness and merriness, a binary predicate $L$ with $L(x,y)$ meaning that $x$ loves $y$, and a constant symbol $\ell$ for Lucy. The domain consists of people. The following four [first-order sentences](../../mathematical-logic.md#first-order-sentence) use this same [first-order signature](../../mathematical-logic.md#first-order-signature).

<h4 id="3/a/a">A</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/a/solution">Solution</h5>

↑ **Parent:** [A](#3/a/a)

The [existential quantifier](../../mathematical-logic.md#existential-quantification) supplies the person loved, with a choice that may depend on $x$:

$$
\boxed{\forall x\,[H(x)\lor\exists y\,L(x,y)].}
$$

The outer [universal quantifier](../../mathematical-logic.md#universal-quantification) ranges over everyone. The [logical disjunction](../../mathematical-logic.md#logical-disjunction) is inclusive; it permits a person both to be happy and to love somebody.

<h4 id="3/a/b">B</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/b/solution">Solution</h5>

↑ **Parent:** [B](#3/a/b)

The property of loving at least one person is the antecedent:

$$
\boxed{\forall x\,[(\exists y\,L(x,y))\to L(x,\ell)].}
$$

An equivalent [first-order sentence](../../mathematical-logic.md#first-order-sentence), useful for [Skolemization](../../mathematical-logic.md#skolemization), is $\forall x\forall y\,[L(x,y)\to L(x,\ell)]$. The person loved in the antecedent need not be Lucy; the conclusion concerns Lucy specifically.

<h4 id="3/a/c">C</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/c/solution">Solution</h5>

↑ **Parent:** [C](#3/a/c)

The same person $y$ must both love $x$ and be loved by $x$:

$$
\boxed{\forall x\,[(\exists y\,(L(y,x)\land L(x,y)))\to H(x)].}
$$

Equivalently, use $\forall x\forall y\,[(L(y,x)\land L(x,y))\to H(x)]$. There is no restriction that $x$ and $y$ be distinct; this matters when the later [ground resolution](../../mathematical-logic.md#ground-resolution) proof considers Lucy loving herself.

<h4 id="3/a/d">D</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/d/solution">Solution</h5>

↑ **Parent:** [D](#3/a/d)

Lucy's happiness is a single antecedent, while the conclusion applies to everyone:

$$
\boxed{H(\ell)\to\forall x\,M(x).}
$$

Since $x$ does not occur in the antecedent, this is equivalent to $\forall x\,[H(\ell)\to M(x)]$. The [universal quantifier](../../mathematical-logic.md#universal-quantification) does not assert that everyone is happy; it is the merriness conclusion that is universal.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

First convert the four [first-order sentences](../../mathematical-logic.md#first-order-sentence) to [clausal form](../../mathematical-logic.md#clausal-form). In the first, pull the [existential quantifier](../../mathematical-logic.md#existential-quantification) across the [logical disjunction](../../mathematical-logic.md#logical-disjunction), then replace its witness by a fresh unary [Skolem function](../../mathematical-logic.md#skolem-function) $f(x)$. The usual nonempty-domain convention for [first-order logic](../../mathematical-logic.md#first-order-logic) makes this transformation valid even when $H(x)$ already holds. The four [Skolem normal forms](../../mathematical-logic.md#skolem-normal-form) are

$$
\begin{aligned}
A'&=\forall x\,[H(x)\lor L(x,f(x))],\\
B'&=\forall x\forall y\,[\neg L(x,y)\lor L(x,\ell)],\\
C'&=\forall x\forall y\,[\neg L(y,x)\lor\neg L(x,y)\lor H(x)],\\
D'&=\forall x\,[\neg H(\ell)\lor M(x)].
\end{aligned}
$$

The [Skolemization](../../mathematical-logic.md#skolemization) of $A$ preserves satisfiability in an expanded [first-order signature](../../mathematical-logic.md#first-order-signature); it does not assert [logical equivalence](../../mathematical-logic.md#logical-equivalence) for every arbitrary interpretation of the new [Skolem function](../../mathematical-logic.md#skolem-function). The other three [first-order sentences](../../mathematical-logic.md#first-order-sentence) only require elimination of implications and movement of [universal quantifiers](../../mathematical-logic.md#universal-quantification).

For a [ground resolution](../../mathematical-logic.md#ground-resolution) refutation, negate the desired conclusion and introduce a fresh constant $c$ for a person who is not merry. This adds the [ground clause](../../mathematical-logic.md#ground-clause) $\neg M(c)$. Use these ground instances of the four universal [first-order sentences](../../mathematical-logic.md#first-order-sentence):

$$
\begin{aligned}
K_1&=H(\ell)\lor L(\ell,f(\ell)),\\
K_2&=\neg L(\ell,f(\ell))\lor L(\ell,\ell),\\
K_3&=\neg L(\ell,\ell)\lor H(\ell),\\
K_4&=\neg H(\ell)\lor M(c),\\
K_5&=\neg M(c).
\end{aligned}
$$

Here $K_3$ comes from $C'$ with $x=y=\ell$, after removing a duplicate negative literal. All [first-order terms](../../mathematical-logic.md#first-order-term) in these [ground clauses](../../mathematical-logic.md#ground-clause) are ground. Resolving gives

$$
\begin{aligned}
K_6&=\operatorname{Res}_{L(\ell,f(\ell))}(K_1,K_2)
      =H(\ell)\lor L(\ell,\ell),\\
K_7&=\operatorname{Res}_{L(\ell,\ell)}(K_6,K_3)=H(\ell),\\
K_8&=\operatorname{Res}_{H(\ell)}(K_7,K_4)=M(c),\\
K_9&=\operatorname{Res}_{M(c)}(K_8,K_5)=\square.
\end{aligned}
$$

Repeated positive literals in $K_7$ have again been removed. The empty [ground clause](../../mathematical-logic.md#ground-clause) proves unsatisfiability of the premises together with the negated conclusion. Therefore

$$
\boxed{A,B,C,D\models\forall x\,M(x).}
$$

The key is to apply the first three premises to Lucy herself: either she is already happy, or she loves somebody, hence loves herself, which forces her happiness and activates the final premise.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For a [first-order signature](../../mathematical-logic.md#first-order-signature) with at least one constant symbol, its [Herbrand universe](../../mathematical-logic.md#herbrand-universe) is the set of all [ground terms](../../mathematical-logic.md#ground-term) built from its constant and function symbols. If necessary add a fresh constant to make this set nonempty. A [Herbrand structure](../../mathematical-logic.md#herbrand-structure) has exactly this domain; each constant denotes itself and each function symbol forms the corresponding syntactic [first-order term](../../mathematical-logic.md#first-order-term). Its remaining choices are the [truth values](../../mathematical-logic.md#truth-value) of the ground predicate atoms. For example, with constant $a$ and unary function $f$, the [Herbrand universe](../../mathematical-logic.md#herbrand-universe) is $\{a,f(a),f(f(a)),\ldots\}$.

One useful clausal form of [Herbrand's theorem](../../mathematical-logic.md#herbrand-s-theorem) is the following. For a set $S$ of universally quantified, equality-free [first-order clauses](../../mathematical-logic.md#first-order-clause),

$$
\boxed{S\text{ is unsatisfiable}\quad\Longleftrightarrow\quad
\text{some finite set of ground instances of }S\text{ is propositionally unsatisfiable}.}
$$

Ground instances substitute [ground terms](../../mathematical-logic.md#ground-term) for all variables. On the right, treat the ground predicate atoms as independent [Boolean variables](../../theoretical-computer-science.md#boolean-variable). Equivalently, $S$ is satisfiable if and only if it has a [Herbrand model](../../mathematical-logic.md#herbrand-model). A general [first-order sentence](../../mathematical-logic.md#first-order-sentence) can first be put into [Skolem normal form](../../mathematical-logic.md#skolem-normal-form) and [clausal form](../../mathematical-logic.md#clausal-form), with the new symbols included in the [Herbrand universe](../../mathematical-logic.md#herbrand-universe).

An equivalent existential version says that a valid equality-free [first-order sentence](../../mathematical-logic.md#first-order-sentence) $\exists\bar x\,\theta(\bar x)$ with [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) $\theta$ has finitely many ground tuples $\bar t_1,\ldots,\bar t_r$ such that $\bigvee_{i=1}^r\theta(\bar t_i)$ is propositionally valid, adding a constant if needed. This explains why a finite [ground resolution](../../mathematical-logic.md#ground-resolution) refutation can establish a consequence involving infinitely many possible [ground terms](../../mathematical-logic.md#ground-term).

The equality-free qualification matters. If [first-order equality](../../mathematical-logic.md#logical-equality) is present, one must handle its axioms and use a term model modulo a suitable congruence, or use the corresponding theorem with equality. Literal syntactic term interpretation alone cannot model a consistent requirement such as $a=b$ for distinct constant symbols.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

**The assertion is false as printed, even for a satisfiable equality-free [Horn clause](../../theoretical-computer-science.md#horn-clause).** The original paper allows an arbitrary [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) $G^*$, so in particular permits negative atoms.[Printed p. 4, Question 3(d), final sentence: the matrix is specified as quantifier-free, without a positivity restriction](../../computer-science-bibliography.md#logic-and-proof-examination-paper-of-the-university-of-oxford-2015)

Take a [first-order signature](../../mathematical-logic.md#first-order-signature) with a constant $a$ and unary predicates $P,Q$, and let

$$
F=\forall x\,[\neg P(x)\lor Q(x)],
\qquad G=\exists x\,\neg P(x).
$$

The matrix of $F$ is a [Horn clause](../../theoretical-computer-science.md#horn-clause), and the [Herbrand universe](../../mathematical-logic.md#herbrand-universe) is the singleton $\{a\}$. The possible [Herbrand models](../../mathematical-logic.md#herbrand-model) of $F$ assign $(P(a),Q(a))$ the values $(0,0)$, $(0,1)$, or $(1,1)$. Neither ground atom is true in every such [Herbrand model](../../mathematical-logic.md#herbrand-model), so the paper's intersection construction gives

$$
P^{\mathcal H_F}=Q^{\mathcal H_F}=\varnothing.
$$

Consequently $\mathcal H_F\models G$, with witness $a$. However, the one-element [first-order structure](../../mathematical-logic.md#first-order-structure) in which both predicates hold everywhere satisfies $F$ and falsifies $G$. Hence

$$
\boxed{\mathcal H_F\models G\quad\text{but}\quad F\not\models G.}
$$

This directly refutes the requested implication; no proof of the stated equivalence is possible. It also isolates the issue: an atom being absent from the intersection means that it is false in _some_ [Herbrand model](../../mathematical-logic.md#herbrand-model), not that it is false in every [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory).

The standard correct version assumes that $F$ is satisfiable, uses an equality-free [first-order signature](../../mathematical-logic.md#first-order-signature) with a nonempty [Herbrand universe](../../mathematical-logic.md#herbrand-universe), and requires $G^*$ to be a positive [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula): one built from atoms and truth constants using only [logical conjunction](../../mathematical-logic.md#logical-conjunction) and [logical disjunction](../../mathematical-logic.md#logical-disjunction). Under those assumptions the expected argument is as follows.

First, the intersection of the ground atoms true in all [Herbrand models](../../mathematical-logic.md#herbrand-model) is itself a [Herbrand model](../../mathematical-logic.md#herbrand-model) of $F$. To see this, read each ground [Horn clause](../../theoretical-computer-science.md#horn-clause) as $A_1\land\cdots\land A_k\to B$, where $B$ is an atom or false. If every $A_i$ is true in the intersection, every $A_i$ is true in every [Herbrand model](../../mathematical-logic.md#herbrand-model). When $B$ is an atom, all these [Herbrand models](../../mathematical-logic.md#herbrand-model) must make $B$ true, so the intersection does too. When $B$ is false, the antecedent cannot hold in any [Herbrand model](../../mathematical-logic.md#herbrand-model); since there is at least one such model, it cannot hold in the intersection either. Thus the intersection is the [least Herbrand model](../../mathematical-logic.md#least-herbrand-model).

Now let $\mathcal H_F\models G$ for positive $G^*$. There is a tuple of [ground terms](../../mathematical-logic.md#ground-term) $\bar t$ with $\mathcal H_F\models G^*(\bar t)$. Expand the positive [quantifier-free formula](../../mathematical-logic.md#quantifier-free-formula) into [disjunctive normal form](../../theoretical-computer-science.md#disjunctive-normal-form); one of its [logical conjunctions](../../mathematical-logic.md#logical-conjunction) of positive atoms is true at $\bar t$. Each of those ground atoms $A$ holds in every [Herbrand model](../../mathematical-logic.md#herbrand-model) of $F$. It also follows that $F\models A$: otherwise a [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory) of $F\land\neg A$ would, by [Herbrand's theorem](../../mathematical-logic.md#herbrand-s-theorem) for universal equality-free [first-order clauses](../../mathematical-logic.md#first-order-clause), yield a [Herbrand model](../../mathematical-logic.md#herbrand-model) of $F\land\neg A$, a contradiction. Every [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory) of $F$ therefore satisfies the same positive [logical conjunction](../../mathematical-logic.md#logical-conjunction) at the interpretations of $\bar t$, and hence satisfies $G$.

Conversely, if $F\models G$, the fact that the [least Herbrand model](../../mathematical-logic.md#least-herbrand-model) is a [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory) of $F$ immediately gives $\mathcal H_F\models G$. Thus the repaired conclusion is

$$
\boxed{\mathcal H_F\models G\ \Longleftrightarrow\ F\models G
\quad\text{for satisfiable universal Horn }F\text{ and positive existential }G.}
$$

The satisfiability qualification is separately necessary when general [Horn clauses](../../theoretical-computer-science.md#horn-clause) may have no positive conclusion. For instance, $F=\forall x(P(x)\land\neg P(x))$ is a [logical conjunction](../../mathematical-logic.md#logical-conjunction) of [Horn clauses](../../theoretical-computer-science.md#horn-clause) with no models. The intersection convention then makes every ground atom true by vacuity, yet $F$ entails even $\exists x\neg P(x)$, which that [Herbrand structure](../../mathematical-logic.md#herbrand-structure) falsifies. The earlier satisfiable example already refutes the printed claim without relying on this further defect.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Use a [first-order signature](../../mathematical-logic.md#first-order-signature) with a constant $a$ and unary predicates $P,Q$, and set

$$
F=\forall x\,[P(x)\lor Q(x)],
\qquad G=\exists x\,[P(x)\lor Q(x)].
$$

The displayed [first-order clause](../../mathematical-logic.md#first-order-clause) has two positive atoms, so it is not a [Horn clause](../../theoretical-computer-science.md#horn-clause). There is a [Herbrand model](../../mathematical-logic.md#herbrand-model) with $P(a)$ true and $Q(a)$ false, and another with the opposite values. Thus neither atom holds in all [Herbrand models](../../mathematical-logic.md#herbrand-model); the intersection construction makes both false.

Every [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory) of $F$ has a nonempty domain, and any element witnesses $G$, so $F\models G$. Nevertheless $\mathcal H_F\not\models G$. Therefore

$$
\boxed{F\models G\quad\text{but}\quad\mathcal H_F\not\models G.}
$$

This example uses a positive [existential sentence](../../mathematical-logic.md#existential-sentence), so it also shows the necessity of the [Horn clause](../../theoretical-computer-science.md#horn-clause) restriction in the repaired result from part (d). Without that restriction, the intersection of [Herbrand models](../../mathematical-logic.md#herbrand-model) need not itself be a [first-order model](../../mathematical-logic.md#model-of-a-first-order-theory) of $F$: here it fails the very disjunction that all the original [Herbrand models](../../mathematical-logic.md#herbrand-model) satisfy.

## ↑ Ancestors (8)

1. [2015](../2015.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
