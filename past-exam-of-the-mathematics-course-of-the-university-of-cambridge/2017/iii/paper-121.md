# Paper 121

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_121.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_121.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [a](#3/ii/a)
      - [Solution](#3/ii/a/solution)
    - [b](#3/ii/b)
      - [Solution](#3/ii/b/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [a](#3/iv/a)
      - [Solution](#3/iv/a/solution)
    - [b](#3/iv/b)
      - [Solution](#3/iv/b/solution)
    - [c](#3/iv/c)
      - [Solution](#3/iv/c/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)

## 1

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For parameters $a_1,\ldots,a_n\in M$, [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) means agreement of the two membership [first-order structures](../../../mathematical-logic.md#first-order-structure):

$$
\boxed{(M,\in)\models\varphi(a_1,\ldots,a_n)\ \Longleftrightarrow\ (N,\in)\models\varphi(a_1,\ldots,a_n).}
$$

This must hold for every such parameter tuple. Equivalently, [formula relativization to a class](../../../set-theory.md#formula-relativization-to-a-class) produces two formulas $\varphi^M$ and $\varphi^N$ whose truth values agree on tuples from $M$. Agreement for parameters only in $N\setminus M$ is not part of the definition. For a proper [class in set theory](../../../set-theory.md#class-set-theory), this notation is understood separately for each fixed [first-order formula](../../../mathematical-logic.md#first-order-formula), rather than as an unrestricted truth predicate for the entire universe.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A syntactically [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory) is built from the atomic [first-order formulas](../../../mathematical-logic.md#first-order-formula) $u=v$ and $u\in v$ using [Boolean operations](../../../computer-science.md#boolean-operation) and bounded quantifiers $\exists u\in v$ and $\forall u\in v$. These abbreviate $\exists u(u\in v\land\cdots)$ and $\forall u(u\in v\Rightarrow\cdots)$, with $u$ different from the bounding variable $v$.

The superscript in the question allows provable equivalence: a [ZF-equivalent bounded formula](../../../set-theory.md#zf-equivalent-bounded-formula) is any [first-order formula](../../../mathematical-logic.md#first-order-formula) $\varphi(\vec v)$ for which some syntactically [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory) $\psi(\vec v)$ satisfies

$$
\boxed{\mathsf{ZF}\vdash\forall\vec v\,(\varphi(\vec v)\leftrightarrow\psi(\vec v)).}
$$

Thus $\Delta_0^{\mathrm{ZF}}$ is the class of [first-order formulas](../../../mathematical-logic.md#first-order-formula) equivalent over [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) to a syntactic $\Delta_0$ [first-order formula](../../../mathematical-logic.md#first-order-formula). If a convention uses $\Delta_0^{\mathrm{ZF}}$ just for syntactically bounded set-theoretic [first-order formulas](../../../mathematical-logic.md#first-order-formula), it is the smaller syntactic class; the subsequent [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) proof works for both conventions.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [Von Neumann hierarchy](../../../set-theory.md#von-neumann-hierarchy) is the following [transfinite recursion](../../../set-theory.md#transfinite-recursion) on the [ordinals](../../../set-theory.md#ordinal):

$$
\boxed{V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad V_\lambda=\bigcup_{\beta<\lambda}V_\beta\ \text{for nonzero limit }\lambda.}
$$

Here $\mathcal P$ denotes the full [power set](../../../set.md#power-set). The levels are increasing [transitive sets](../../../set-theory.md#transitive-set), and the construction is continuous at [limit ordinals](../../../set-theory.md#limit-ordinal). [Transfinite induction](../../../set-theory.md#transfinite-induction) proves these properties: transitivity at a successor follows because a member of a [subset](../../../set.md#subset) of $V_\alpha$ already belongs to $V_\alpha\subseteq\mathcal P(V_\alpha)$; at a limit it follows from the [set union](../../../set.md#set-union) of increasing [transitive sets](../../../set-theory.md#transitive-set). In [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory), [Axiom of foundation](../../../set-theory.md#axiom-of-regularity) and [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) ensure that every [set](../../../set.md) belongs to some $V_\alpha$. In terms of the [rank of a set](../../../set-theory.md#rank-of-a-set), $x\in V_\alpha$ exactly when $\operatorname{rank}(x)<\alpha$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

First prove [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) for syntactically [bounded formulas in set theory](../../../set-theory.md#bounded-formula-in-set-theory) by induction on their construction. Atomic equality and membership use the actual equality and membership relations in both [transitive classes](../../../set-theory.md#transitive-class). [Boolean operations](../../../computer-science.md#boolean-operation) preserve agreement.

For the bounded existential step, take $a\in M$ and suppose $N\models\exists u\in a\,\psi(u,\vec b)$. Its witness $c$ is an actual member of $a$. Since $M$ is a [transitive class](../../../set-theory.md#transitive-class), $c\in M$; the induction hypothesis then gives $M\models\psi(c,\vec b)$. The converse uses the same witness in $N$. The bounded universal step follows similarly because both structures quantify over exactly the actual members of $a$, or follows by [negation](../../../computer-science.md#negation) from the existential step. Hence

$$
\boxed{\psi^M(\vec b)\leftrightarrow\psi^N(\vec b)\qquad\text{for every syntactic }\Delta_0\text{ formula and }\vec b\in M.}
$$

No [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms are needed for this syntactic statement beyond the ambient meaning of a [transitive class](../../../set-theory.md#transitive-class). For a [ZF-equivalent bounded formula](../../../set-theory.md#zf-equivalent-bounded-formula) $\varphi$, choose a bounded equivalent $\psi$. The assumption that both structures model [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) gives $\varphi^M\leftrightarrow\psi^M$ and $\varphi^N\leftrightarrow\psi^N$. Combining these with the displayed equivalence proves the asserted [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) of $\Delta_0^{\mathrm{ZF}}$.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The essential fact is [absoluteness of cardinalhood in limit ranks](../../../set-theory.md#absoluteness-of-cardinalhood-in-limit-ranks). Let $\alpha\leq\beta$ be [limit ordinals](../../../set-theory.md#limit-ordinal) and $x\in V_\alpha$. Being an [ordinal](../../../set-theory.md#ordinal) is absolute between these [transitive sets](../../../set-theory.md#transitive-set), so a non-ordinal is a [cardinal number](../../../set-theory.md#cardinal-number) in neither structure. For an [ordinal](../../../set-theory.md#ordinal) $\delta\in V_\alpha$, we have $\delta<\alpha$.

If $\delta$ is not an ambient [cardinal number](../../../set-theory.md#cardinal-number), there is an [ordinal](../../../set-theory.md#ordinal) $\gamma<\delta$ and a [bijection](../../../function.md#bijection) $f:\gamma\to\delta$. With [Kuratowski ordered pairs](../../../set.md#kuratowski-ordered-pair), its graph has [rank of a set](../../../set-theory.md#rank-of-a-set) at most $\delta+3$. Since $\alpha$ is a [limit ordinal](../../../set-theory.md#limit-ordinal), $\delta+3<\alpha$, so $f\in V_\alpha$. The assertion that $f$ is such a [bijection](../../../function.md#bijection) is a [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory) and is therefore evaluated correctly by each rank. Conversely, any internal [bijection](../../../function.md#bijection) witnessing failure of [cardinal number](../../../set-theory.md#cardinal-number) status is an actual one by the same [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness). Consequently

$$
\boxed{V_\alpha\models\text{``}\delta\text{ is a cardinal''}\ \Longleftrightarrow\ \delta\text{ is an ambient cardinal}\ \Longleftrightarrow\ V_\beta\models\text{``}\delta\text{ is a cardinal''.}}
$$

Unlike arbitrary [transitive models](../../../set-theory.md#transitive-model), these rank-initial structures contain every sufficiently low-rank witness. That witness availability is what upgrades the usual [downward absoluteness of cardinalhood](../../../set-theory.md#downward-absoluteness-of-cardinalhood) to agreement in both directions.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

Use the standard convention that a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) is uncountable, regular and strong limit. **The printed explanatory definition omits uncountability**: literally it also admits $\kappa=\omega$, for which no finite cardinal is a [worldly cardinal](../../../set-theory.md#worldly-cardinal). Thus that omission makes the requested conclusion false under the literal abbreviated definition. The proof below applies to the usual, intended [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) convention $\kappa>\omega$.

First $|V_\gamma|<\kappa$ for every $\gamma<\kappa$. At successor stages this follows from the [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) property, and at limits from the [regular cardinal](../../../set-theory.md#regular-cardinal) property. Consequently $V_\kappa\models\mathsf{ZFC}$. In particular, for [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement), a domain $a\in V_\kappa$ has size less than $\kappa$, so its functional image has fewer than $\kappa$ elements, so the supremum of the [rank of a set](../../../set-theory.md#rank-of-a-set) over its elements is below $\kappa$ by [regular cardinal](../../../set-theory.md#regular-cardinal) structure. All other axioms, including [axiom of choice](../../../set-theory.md#axiom-of-choice), have their witnesses at bounded ranks below $\kappa$; uncountability supplies [axiom of infinity](../../../set-theory.md#axiom-of-infinity).

Enumerate the [first-order formulas](../../../mathematical-logic.md#first-order-formula) as $\varphi_0,\varphi_1,\ldots$. For each finite collection, reflection inside the set structure $V_\kappa$ gives a [closed unbounded subset](../../../set-theory.md#club-set) of $\kappa$ of agreeing ranks. To see why the witness bounds stay below $\kappa$, there are fewer than $\kappa$ parameter tuples at each $V_\gamma$, and the supremum of their least witness ranks remains below $\kappa$ by [regular cardinal](../../../set-theory.md#regular-cardinal) structure. Closing under these bounds and taking increasing countable limits gives the usual [reflection theorem for definable hierarchies](../../../set-theory.md#reflection-theorem-for-definable-hierarchies) argument. The countable intersection of these [closed unbounded subsets](../../../set-theory.md#club-set) is still [closed unbounded](../../../set-theory.md#club-set) because $\kappa$ is regular and uncountable. At each resulting $\alpha$,

$$
(V_\alpha,\in)\prec(V_\kappa,\in),\qquad V_\alpha\models\mathsf{ZFC}.
$$

The infinite [cardinal numbers](../../../set-theory.md#cardinal-number) below $\kappa$ also form a [closed unbounded subset](../../../set-theory.md#club-set): they are unbounded because $\lambda^+\leq2^\lambda<\kappa$ for infinite $\lambda<\kappa$, and a supremum of increasing [cardinal numbers](../../../set-theory.md#cardinal-number) is a [cardinal number](../../../set-theory.md#cardinal-number). Intersect the two [closed unbounded subsets](../../../set-theory.md#club-set). Every member of the intersection is a [worldly cardinal](../../../set-theory.md#worldly-cardinal), and an unbounded [subset](../../../set.md#subset) of a [regular cardinal](../../../set-theory.md#regular-cardinal) $\kappa$ has size $\kappa$. Hence

$$
\boxed{\left|\{\alpha<\kappa:\alpha\text{ is a cardinal and }V_\alpha\models\mathsf{ZFC}\}\right|=\kappa.}
$$

In fact this proves the stronger [worldly cardinals below an inaccessible cardinal](../../../set-theory.md#worldly-cardinals-below-an-inaccessible-cardinal) result that these [worldly cardinals](../../../set-theory.md#worldly-cardinal) contain a [closed unbounded subset](../../../set-theory.md#club-set) of $\kappa$.

## 2

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [definable continuous hierarchy](../../../set-theory.md#definable-continuous-hierarchy) is a definable class function $\alpha\mapsto H_\alpha$ on the [ordinals](../../../set-theory.md#ordinal), with set-valued levels, such that $H_\alpha\subseteq H_\beta$ for $\alpha<\beta$ and

$$
H_\lambda=\bigcup_{\alpha<\lambda}H_\alpha
$$

for nonzero [limit ordinals](../../../set-theory.md#limit-ordinal). Its union is a definable [class in set theory](../../../set-theory.md#class-set-theory) $H$. Often the definition additionally requires every level to be a [transitive set](../../../set-theory.md#transitive-set); the following statement also works without that requirement.

The [reflection theorem for definable hierarchies](../../../set-theory.md#reflection-theorem-for-definable-hierarchies) says that for any finite collection $\mathcal F$ of [first-order formulas](../../../mathematical-logic.md#first-order-formula), there is a [closed unbounded](../../../set-theory.md#club-set) class of [ordinals](../../../set-theory.md#ordinal) $\alpha$ such that, for every $\varphi\in\mathcal F$ and every parameter tuple from $H_\alpha$,

$$
\boxed{(H_\alpha,\in)\models\varphi(\vec a)\ \Longleftrightarrow\ (H,\in)\models\varphi(\vec a).}
$$

A useful justification is the witness-closure proof. Close $\mathcal F$ under subformulas. At each level and for each existential subformula, bound the least level containing a witness for each parameter tuple for which a witness exists in $H$. [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) bounds these indices. Iterating the finitely many bounds through $\omega$ produces a limit level containing all required witnesses. Induction on the [first-order formulas](../../../mathematical-logic.md#first-order-formula), equivalently the finite-formula version of the [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test), yields agreement. Continuity gives closedness of the reflecting class, and starting above any prescribed [ordinal](../../../set-theory.md#ordinal) gives unboundedness. This is finite reflection, not a claim that all [first-order formulas](../../../mathematical-logic.md#first-order-formula) reflect simultaneously in an arbitrary hierarchy.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Fix the base convention $L_0(X)=X$. For a [transitive set](../../../set-theory.md#transitive-set) $X$, the [relative constructible hierarchy](../../../definable-power-set.md#relative-constructible-hierarchy) is

$$
\boxed{L_0(X)=X,\qquad L_{\alpha+1}(X)=\operatorname{Def}(L_\alpha(X)),\qquad L_\lambda(X)=\bigcup_{\alpha<\lambda}L_\alpha(X),\qquad L(X)=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha(X).}
$$

Here the [definable power set](../../../definable-power-set.md) is

$$
\operatorname{Def}(A)=\{\{u\in A:(A,\in)\models\varphi(u,\vec a)\}:\varphi\text{ a first-order formula},\ \vec a\in A^{<\omega}\}.
$$

The [satisfaction for a set structure](../../../mathematical-logic.md#satisfaction-for-a-set-structure) in this definition is a definable set-theoretic relation, obtained by finite syntax coding and recursion on a [first-order formula](../../../mathematical-logic.md#first-order-formula). The [transfinite recursion](../../../set-theory.md#transfinite-recursion) therefore defines a class in [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory).

Each level is a [transitive set](../../../set-theory.md#transitive-set). For transitive $A$, every $a\in A$ is a [subset](../../../set.md#subset) of $A$ definable using the parameter $a$, so $A\subseteq\operatorname{Def}(A)$; also $A\in\operatorname{Def}(A)$ using the always-true [first-order formula](../../../mathematical-logic.md#first-order-formula). Thus the levels increase and $X\in L_1(X)$. Starting instead with $X\cup\{X\}$ is another common indexing convention, but it is not the convention used here. The relative universe need not satisfy [axiom of choice](../../../set-theory.md#axiom-of-choice): arbitrary $X$ need not have an internally available [well-order](../../../set.md#well-order).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Use [relative constructible level recognition](../../../definable-power-set.md#relative-constructible-level-recognition). The finite coding conditions matter here: merely writing “every set is relatively constructible” inside an arbitrary [transitive set](../../../set-theory.md#transitive-set) does not ensure that its computations are correct.

Let $\mathsf A$ be a single finite conjunction expressing [finite relation closure for set-theoretic coding](../../../definable-power-set.md#finite-relation-closure-for-set-theoretic-coding). Concretely require the empty [set](../../../set.md), pairing, [set union](../../../set.md#set-union), [set difference](../../../set.md#set-difference), [Cartesian products](../../../set-theory.md#cartesian-product), and the following uniform relation operations: for each finite [ordinal](../../../set-theory.md#ordinal) $n$ and each [set](../../../set.md) $A$, the set $A^n$ of finite tuples exists; relations on these tuple domains can be complemented, intersected, projected along a coordinate and pulled back along finite coordinate maps; the equality and membership relations restricted to $A^2$ exist. These are finitely many first-order closure assertions with $n$ quantified, not an axiom schema. Each operation is specified by its usual elementwise membership equivalence. Transitivity makes the operations correct externally. Finite tuple domains are also correct: every individual finite tuple is already present by pairing and union.

These conditions make [satisfaction for a set structure](../../../mathematical-logic.md#satisfaction-for-a-set-structure) absolute. For a fixed coded [first-order formula](../../../mathematical-logic.md#first-order-formula), compute its truth relations on $A^n$ by induction: equality and membership give the atomic cases, [relative complement](../../../set.md#set-difference) gives [negation](../../../computer-science.md#negation), intersection gives [logical conjunction](../../../mathematical-logic.md#logical-conjunction), and projection gives existential quantification. All required truth tables exist by $\mathsf A$ and agree with the actual ones. Thus the first-order assertion $B=\operatorname{Def}(A)$ is absolute whenever $A,B$ belong to a transitive structure satisfying $\mathsf A$: require that each member of $B$ has such a finite formula-and-parameter definition, and that each coded definition contributes a member of $B$. Codes are finite objects; no truth predicate for the ambient universe is being used.

Write $S_x(\xi,B)$ for the [coded relative constructible stage](../../../definable-power-set.md#coded-relative-constructible-stage) assertion: $\xi$ is an [ordinal](../../../set-theory.md#ordinal) and there is a function $f$ with domain $\xi+1$, with $f(0)=x$, $f(\eta+1)=\operatorname{Def}(f(\eta))$, $f(\lambda)=\bigcup_{\eta<\lambda}f(\eta)$ at nonzero [limit ordinals](../../../set-theory.md#limit-ordinal), and $f(\xi)=B$. Under $\mathsf A$, any such internal code is correct by [transfinite induction](../../../set-theory.md#transfinite-induction). Restrictions of a code to shorter domains exist by the relation operations. Define the one-free-variable [first-order formula](../../../mathematical-logic.md#first-order-formula)

$$
\boxed{\begin{aligned}
\Phi(x):={}&\mathsf A\ \land\ x\text{ is transitive}\\
&\land\ \forall y\,\exists\xi\,\exists B\,(S_x(\xi,B)\land y\in B)\\
&\land\ \forall\xi\,\forall B\,(S_x(\xi,B)\Rightarrow\exists\eta\,\exists C\,(\xi<\eta\land S_x(\eta,C))).
\end{aligned}}
$$

All displayed abbreviations expand into [first-order formulas](../../../mathematical-logic.md#first-order-formula) of the membership language.

Suppose $M$ is transitive, $X\in M$, and $M\models\Phi(X)$. Let $I$ be the externally defined set of indices of stage codes in $M$. It contains $0$, is downward closed by restricting codes, and has no largest member by the last conjunct. Thus $I$ is a nonzero [limit ordinal](../../../set-theory.md#limit-ordinal) $\alpha$. Correctness of stage codes gives $L_\xi(X)\in M$ for $\xi<\alpha$, hence $L_\xi(X)\subseteq M$ by transitivity. Conversely the exhaustion conjunct puts every $y\in M$ in some such level. Therefore

$$
M=\bigcup_{\xi<\alpha}L_\xi(X)=L_\alpha(X).
$$

For the converse, every $L_\alpha(X)$ with nonzero limit $\alpha$ satisfies $\mathsf A$: each listed operation on parameters from one level is definable at finitely many later levels, still below $\alpha$. Moreover [stage histories appear below every limit constructible level](../../../definable-power-set.md#stage-histories-appear-below-every-limit-constructible-level). Here is the essential limit step of that lemma. If the histories $f_\eta$ for $\eta<\lambda$ are available in $L_\lambda(X)$, the correct predicate $S_X$ defines their graph of endpoints as a subset of $L_\lambda(X)$. No endpoint $L_\eta(X)$ with $\eta\geq\lambda$ can belong to $L_\lambda(X)$, because $L_\lambda(X)\subseteq L_\eta(X)$ would then give $L_\eta(X)\in L_\eta(X)$, contradicting [Axiom of foundation](../../../set-theory.md#axiom-of-regularity). The defined graph therefore has domain exactly $\lambda$. Adjoining its final pair $(\lambda,L_\lambda(X))$ takes finitely many more stages. Together with finite successor extensions, this proves by [transfinite induction](../../../set-theory.md#transfinite-induction) that every $f_\xi$ belongs to $L_{\xi+k}(X)$ for some finite $k$.

Thus all histories for $\xi<\alpha$ belong to $L_\alpha(X)$. Exhaustion follows from continuity, and $\xi+1<\alpha$ supplies a larger represented stage. Hence $L_\alpha(X)\models\Phi(X)$, proving both directions without assuming [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) for the arbitrary input structure $M$.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

A suitable [relative condensation lemma](../../../definable-power-set.md#relative-condensation-lemma) fixes the base pointwise. Let $\alpha$ be a nonzero [limit ordinal](../../../set-theory.md#limit-ordinal), and let $Y\prec(L_\alpha(X),\in)$ be an [elementary substructure](../../../mathematical-logic.md#elementary-substructure) with

$$
X\cup\{X\}\subseteq Y.
$$

Then the [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) gives an isomorphism $\pi:Y\to T$ onto a [transitive set](../../../set-theory.md#transitive-set), and

$$
\boxed{T=L_\beta(X)\quad\text{for a nonzero limit ordinal }\beta\leq\alpha,\qquad\pi\!\upharpoonright X=\operatorname{id}_X.}
$$

For the collapse to apply, the restricted membership relation is well-founded because it is actual membership. It is extensional: if two members of $Y$ differ, an element distinguishing them in $L_\alpha(X)$ can be chosen in $Y$ by [elementary substructure](../../../mathematical-logic.md#elementary-substructure) structure. Since $X$ is transitive and all its members are in $Y$, [transfinite induction](../../../set-theory.md#transfinite-induction) on their [rank of a set](../../../set-theory.md#rank-of-a-set) shows that $\pi$ fixes every member of $X$, and then $\pi(X)=X$.

By the preceding [relative constructible level recognition](../../../definable-power-set.md#relative-constructible-level-recognition), $L_\alpha(X)\models\Phi(X)$. [Elementary substructure](../../../mathematical-logic.md#elementary-substructure) agreement transfers this to $Y$, and the collapse isomorphism transfers it to $T$. Thus $T\models\Phi(X)$ and $T=L_\beta(X)$ for a nonzero [limit ordinal](../../../set-theory.md#limit-ordinal) $\beta$.

For the bound, let $\rho=X\cap\operatorname{Ord}$. The [relative constructible hierarchy](../../../definable-power-set.md#relative-constructible-hierarchy) has ordinal height $L_\gamma(X)\cap\operatorname{Ord}=\rho+\gamma$: at a successor the [definable power set](../../../definable-power-set.md) adds exactly the previous ordinal height as a new [ordinal](../../../set-theory.md#ordinal), and at limits take unions. The order type of $Y\cap\operatorname{Ord}$ is at most $\rho+\alpha$, so $\rho+\beta\leq\rho+\alpha$; strict increase of [ordinal addition](../../../set-theory.md#ordinal-addition) in the right argument gives $\beta\leq\alpha$. The requirement $X\subseteq Y$ is essential to this version: merely having $X\in Y$ need not make the collapse fix the base.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

The assumed [beth number](../../../set-theory.md#beth-number) equality $\beth_1=\aleph_2$ means $2^{\aleph_0}=\aleph_2$ in the ambient universe. Put $W=L(X)$ with $X=\mathcal P(\omega)$, using the [relative constructible hierarchy](../../../definable-power-set.md#relative-constructible-hierarchy) defined above.

The base $X$ is transitive because every member of a member of $X$ is a finite [ordinal](../../../set-theory.md#ordinal), hence itself a [subset](../../../set.md#subset) of $\omega$. Moreover $X\subseteq W$ and $X\in W$, and $W$ is an [inner model](../../../set-theory.md#inner-model) of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory). The latter standard fact follows from the hierarchy and reflection: bounded-rank witnesses give pairing and union; reflection gives separation and replacement; ambient replacement bounds the stages of all relatively constructible [subsets](../../../set.md#subset) of any fixed [set](../../../set.md), giving power set. It does not require [axiom of choice](../../../set-theory.md#axiom-of-choice) inside $W$. Since no new [subsets](../../../set.md#subset) of $\omega$ can appear in an inner class,

$$
\mathcal P^W(\omega)=X=\mathcal P(\omega).
$$

Since [inner models with all reals preserve omega-one](../../../definable-power-set.md#inner-models-with-all-reals-preserve-omega-one), it suffices to check that their real-code argument applies to $W$. Every ambient countably infinite [ordinal](../../../set-theory.md#ordinal) has a [well-order code](../../../definable-power-set.md#well-order-code) on $\omega$, coded by a [subset](../../../set.md#subset) of $\omega$ in $X$. Finite [ordinals](../../../set-theory.md#ordinal) and $\omega$ are already shared. This code belongs to $W$, is well-founded there, and its [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) interpretation inside $W$ is the same [ordinal](../../../set-theory.md#ordinal) as outside. Hence the [ordinal](../../../set-theory.md#ordinal) is countable in $W$. Conversely, any countability witness in $W$ remains a witness in the ambient universe. Thus $\omega_1^W=\omega_1$.

If $W$ satisfied the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis) in its usual well-orderable formulation, it would contain a [bijection](../../../function.md#bijection) from $\omega_1^W$ onto its [power set](../../../set.md#power-set) of $\omega$. The same [bijection](../../../function.md#bijection) would exist externally from $\omega_1$ onto $X$, contradicting $|X|=\aleph_2$. Therefore

$$
\boxed{L(\mathcal P(\omega))\models\neg\mathsf{CH}.}
$$

This proof uses agreement on all reals and on $\omega_1$, not an unwarranted assertion that $L(X)$ satisfies [axiom of choice](../../../set-theory.md#axiom-of-choice) or computes every higher [cardinal number](../../../set-theory.md#cardinal-number) correctly.

## 3

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use [standard notation for forcing](../../../forcing.md#standard-notation-for-forcing): $q\leq p$ means that $q$ is stronger. A [generic filter](../../../forcing.md#generic-filter) is nonempty, upward closed and downward directed, and meets every [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order) in the ground model. Names below are [forcing names](../../../forcing.md#forcing-name) in $M$, with pairs ordered as $(\text{name},\text{condition})$.

The [semantic forcing relation](../../../forcing.md#semantic-forcing-relation) is

$$
\boxed{p\Vdash\varphi(\tau_1,\ldots,\tau_n)\ \Longleftrightarrow\ \text{for every }M\text{-generic }K\ni p,\ M[K]\models\varphi(\tau_1^K,\ldots,\tau_n^K).}
$$

Here $\tau^K=\operatorname{val}(\tau,K)$ is the [evaluation of a forcing name](../../../forcing.md#evaluation-of-a-forcing-name). Countability of $M$ supplies such [generic filters](../../../forcing.md#generic-filter) through every condition by the [Rasiowa–Sikorski lemma](../../../forcing.md#rasiowa-sikorski-lemma).

Define the [syntactic forcing relation](../../../forcing.md#syntactic-forcing-relation) by mutual well-founded recursion on the [forcing names](../../../forcing.md#forcing-name) for the atomic cases, then induction on the [first-order formula](../../../mathematical-logic.md#first-order-formula). Its membership clause is

$$
p\Vdash^*\sigma\in\tau\ \Longleftrightarrow\ \forall q\leq p\ \exists s\leq q\ \exists(\rho,r)\in\tau\ (s\leq r\ \land\ s\Vdash^*\sigma=\rho).
$$

For equality, first abbreviate

$$
p\Vdash^*\sigma\subseteq\tau\ \Longleftrightarrow\ \forall(\rho,r)\in\sigma\ \forall q\,(q\leq p\land q\leq r\Rightarrow q\Vdash^*\rho\in\tau),
$$

and set $p\Vdash^*\sigma=\tau$ exactly when both inclusions hold. Each recursive call lowers the rank of at least one [forcing name](../../../forcing.md#forcing-name) without raising the other. This makes the mutual recursion well-founded.

For a basis of connectives consisting of [logical conjunction](../../../mathematical-logic.md#logical-conjunction), [negation](../../../computer-science.md#negation) and existential quantification, the remaining clauses are

$$
\begin{aligned}
p\Vdash^*(\varphi\land\psi)&\Longleftrightarrow(p\Vdash^*\varphi\ \land\ p\Vdash^*\psi),\\
p\Vdash^*\neg\varphi&\Longleftrightarrow\text{no }q\leq p\text{ satisfies }q\Vdash^*\varphi,\\
p\Vdash^*\exists v\,\varphi(v)&\Longleftrightarrow\forall q\leq p\ \exists s\leq q\ \exists\rho\in M^{\mathbb P}\ (s\Vdash^*\varphi(\rho)).
\end{aligned}
$$

The last line is the [existential clause of syntactic forcing](../../../forcing.md#existential-clause-of-syntactic-forcing); witnesses need only occur densely, rather than be forced by $p$ itself with one preselected name. Other connectives are defined by logical abbreviations. The recursion gives a definable relation inside $M$ for each fixed [first-order formula](../../../mathematical-logic.md#first-order-formula), with quantification over the class of its names. If $\mathbb P$ has no greatest element, use [canonical forcing names](../../../forcing.md#canonical-forcing-name) $\check a=\{(\check b,p):b\in a,\ p\in\mathbb P\}$, which still evaluate to $a$. It also proves monotonicity: strengthening a condition preserves what it forces. The [forcing theorem](../../../forcing.md#forcing-theorem) identifies the two relations and supplies the truth lemma.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/a">a</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/ii/a)

This is the forward implication of the [atomic membership truth lemma for forcing](../../../forcing.md#atomic-membership-truth-lemma-for-forcing). Suppose $\sigma^G\in\tau^G$. By the [evaluation of a forcing name](../../../forcing.md#evaluation-of-a-forcing-name), choose $(\rho,r)\in\tau$ with $r\in G$ and $\sigma^G=\rho^G$. The assumed equality truth lemma supplies $s\in G$ with $s\Vdash^*\sigma=\rho$.

Directedness of the [generic filter](../../../forcing.md#generic-filter) gives $p\in G$ with $p\leq r,s$. For every $q\leq p$, monotonicity of the [syntactic forcing relation](../../../forcing.md#syntactic-forcing-relation) gives $q\Vdash^*\sigma=\rho$, and $q\leq r$. Thus $q$ itself witnesses the required membership density below $p$. Hence

$$
\boxed{\sigma^G\in\tau^G\ \Longrightarrow\ \exists p\in G\ (p\Vdash^*\sigma\in\tau).}
$$

Only the equality truth lemma stipulated in the source and the recursive membership clause have been used.

<h4 id="3/ii/b">b</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/ii/b)

Conversely, suppose $p\in G$ and $p\Vdash^*\sigma\in\tau$. The [syntactic forcing relation](../../../forcing.md#syntactic-forcing-relation) says that

$$
D=\{s\leq p:\exists(\rho,r)\in\tau\ (s\leq r\land s\Vdash^*\sigma=\rho)\}
$$

is [dense below a forcing condition](../../../forcing.md#dense-below-a-forcing-condition) $p$. This is a [set](../../../set.md) in $M$ by definability of forcing and [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification). The [dense-below generic meeting lemma](../../../forcing.md#dense-below-generic-meeting-lemma) gives $s\in G\cap D$: augment $D$ by all [incompatible forcing conditions](../../../forcing.md#incompatible-forcing-conditions) with $p$ to obtain a globally dense ground-model [set](../../../set.md), and use $p\in G$ to exclude the incompatible part.

Choose the witnessing $(\rho,r)\in\tau$. Since $s\leq r$ and $s\in G$, upward closure gives $r\in G$. The assumed equality truth lemma gives $\sigma^G=\rho^G$, while $r\in G$ gives $\rho^G\in\tau^G$. Combining both directions,

$$
\boxed{\sigma^G\in\tau^G\ \Longleftrightarrow\ \exists p\in G\ (p\Vdash^*\sigma\in\tau).}
$$

This completes the [atomic membership truth lemma for forcing](../../../forcing.md#atomic-membership-truth-lemma-for-forcing); no separate assumption of the membership truth lemma was made.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

We prove [power set in a generic extension](../../../forcing.md#power-set-in-a-generic-extension) by bounding possible subnames in the ground model, rather than presupposing the desired [power set](../../../set.md#power-set) in $M[G]$. Let $x=\tau^G$, and let $S=\{\rho:\exists r\,((\rho,r)\in\tau)\}$. In $M$ form

$$
U=\{(\rho,p)\in S\times\mathbb P:\exists r\,((\rho,r)\in\tau\land p\leq r)\},\qquad B=\mathcal P^M(U).
$$

Every $\nu\in B$ is a [forcing name](../../../forcing.md#forcing-name). Its value is a [subset](../../../set.md#subset) of $x$: an active pair $(\rho,p)\in\nu$ has $p\leq r$ for some $(\rho,r)\in\tau$, so $p\in G$ implies $r\in G$ and $\rho^G\in x$.

Now take any $y\in M[G]$ with $y\subseteq x$, and choose a [forcing name](../../../forcing.md#forcing-name) $\sigma\in M$ with $\sigma^G=y$. By [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) and definability of the [syntactic forcing relation](../../../forcing.md#syntactic-forcing-relation),

$$
\nu_\sigma=\{(\rho,p)\in U:p\Vdash^*\rho\in\sigma\}\in B.
$$

The [atomic membership truth lemma for forcing](../../../forcing.md#atomic-membership-truth-lemma-for-forcing) shows $\nu_\sigma^G=y$. One inclusion follows immediately from its soundness direction. For the other, if $a\in y\subseteq x$, choose $(\rho,r)\in\tau$ with $r\in G$ and $\rho^G=a$. The truth direction supplies $p\in G$ forcing $\rho\in\sigma$; strengthen within $G$ below $p$ and $r$ to obtain an active pair in $\nu_\sigma$ representing $a$.

Finally the ground-model [forcing name](../../../forcing.md#forcing-name)

$$
\Pi_\tau=\{(\nu,p):\nu\in B,\ p\in\mathbb P\}
$$

exists by [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) and the ground-model [power set](../../../set.md#power-set) axiom. Since $G$ is nonempty, all $\nu\in B$ contribute their values, and

$$
\boxed{\Pi_\tau^G=\{y\in M[G]:y\subseteq\tau^G\}=\mathcal P^{M[G]}(x).}
$$

This [set](../../../set.md) belongs to $M[G]$ by the definition of a [generic extension](../../../forcing.md#generic-extension). The construction uses all conditions in the outer pairs and therefore does not require a greatest condition in $\mathbb P$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/a">a</h4>

↑ **Parent:** [Iv](#3/iv)

<h5 id="3/iv/a/solution">Solution</h5>

↑ **Parent:** [A](#3/iv/a)

For the [product forcing](../../../forcing.md#product-forcing) order, let $G_0$ and $G_1$ be the coordinate projections of $H$:

$$
G_0=\{p:\exists q\ ((p,q)\in H)\},\qquad G_1=\{q:\exists p\ ((p,q)\in H)\}.
$$

These are nonempty upward-closed, directed [filters in an ordered set](../../../set.md#filter-mathematics). Clearly $H\subseteq G_0\times G_1$. If $p\in G_0$ and $q\in G_1$, choose $(p,q')\in H$ and $(p',q)\in H$. Directedness supplies $(r,s)\in H$ below both, so $(r,s)\leq(p,q)$. Upward closure of $H$ gives $(p,q)\in H$. Therefore the [projection of a product-generic filter](../../../forcing.md#projection-of-a-product-generic-filter) satisfies

$$
\boxed{H=G_0\times G_1.}
$$

No greatest conditions in the factors are required for this argument.

<h4 id="3/iv/b">b</h4>

↑ **Parent:** [Iv](#3/iv)

<h5 id="3/iv/b/solution">Solution</h5>

↑ **Parent:** [B](#3/iv/b)

Let $D\in M$ be a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order) $\mathbb P$. Then $D\times\mathbb Q\in M$ is dense in the [product forcing](../../../forcing.md#product-forcing) order: below $(p,q)$, choose $p'\leq p$ in $D$ and retain $q$. The [generic filter](../../../forcing.md#generic-filter) $H$ meets it, so its first projection $G_0$ meets $D$. Together with the filter properties proved above, this gives

$$
\boxed{G_0\text{ is }\mathbb P\text{-generic over }M.}
$$

The same argument proves that $G_1$ is $\mathbb Q$-generic over $M$, but genericity over the larger [generic extension](../../../forcing.md#generic-extension) $M[G_0]$ needs the next argument.

<h4 id="3/iv/c">c</h4>

↑ **Parent:** [Iv](#3/iv)

<h5 id="3/iv/c/solution">Solution</h5>

↑ **Parent:** [C](#3/iv/c)

We prove [mutual genericity for product forcing](../../../forcing.md#mutual-genericity-for-product-forcing). Let $D\in M[G_0]$ be a dense [subset](../../../set.md#subset) of $\mathbb Q$, and take a [forcing name](../../../forcing.md#forcing-name) $\dot D\in M$ evaluating to $D$. By the [forcing theorem](../../../forcing.md#forcing-theorem), some $p_0\in G_0$ forces that $\dot D$ is a dense [subset](../../../set.md#subset) of the [canonical forcing name](../../../forcing.md#canonical-forcing-name) for $\mathbb Q$.

In $M$ define

$$
E=\{(p,q):p\perp p_0\}\ \cup\ \{(p,q):p\leq p_0\text{ and }p\Vdash\check q\in\dot D\}.
$$

This [set](../../../set.md) is dense in the [product forcing](../../../forcing.md#product-forcing) order. Given $(p,q)$, the incompatible case is immediate. Otherwise first strengthen $p$ below $p_0$. The forced density assertion and the [existential clause of syntactic forcing](../../../forcing.md#existential-clause-of-syntactic-forcing) supply a further $r\leq p,p_0$ and a ground-model $q'\leq q$ with $r\Vdash\check q'\in\dot D$. To justify choosing a ground-model $q'$, a name forced to lie in $\check{\mathbb Q}$ can densely be made equal to some $\check q'$ by the atomic membership clause; strengthen to that equality and use the forced order comparison. Thus $(r,q')\in E$ lies below $(p,q)$.

The [generic filter](../../../forcing.md#generic-filter) $H$ meets $E$. It cannot meet the first part, because its first projection contains $p_0$ and is directed. Hence there is $(p,q)\in H$ with $p\in G_0$ and $p\Vdash\check q\in\dot D$. Soundness of the [forcing theorem](../../../forcing.md#forcing-theorem) gives $q\in D$, and the projection gives $q\in G_1$. Since every such $D$ is met,

$$
\boxed{G_1\text{ is }\mathbb Q\text{-generic over }M[G_0].}
$$

This establishes the stronger property, rather than merely meeting dense ground-model [subsets](../../../set.md#subset).

## 4

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A [forcing atom](../../../forcing.md#forcing-atom) is a condition $p\in\mathbb P$ such that any two strengthenings of $p$ are [compatible forcing conditions](../../../forcing.md#compatible-forcing-conditions):

$$
p\text{ is an atom}\ \Longleftrightarrow\ \forall q,r\leq p\ \exists s\in\mathbb P\ (s\leq q,r).
$$

An [atomless forcing order](../../../forcing.md#atomless-forcing-order) has no such condition; equivalently,

$$
\boxed{\forall p\in\mathbb P\ \exists q,r\leq p\ (q\perp r).}
$$

The meaning of $q\perp r$ is that there is no common stronger condition. For an arbitrary [partial order](../../../set.md#partially-ordered-set), an atom need not be a minimal element: the definition concerns compatibility below it. This distinction prevents a minimal-element definition from misclassifying an order with descending but mutually compatible conditions.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The two-argument version of [Fn forcing](../../../forcing.md#fn-forcing) consists of finite [partial functions](../../../function.md#partial-function):

$$
\boxed{\operatorname{Fn}(I,J)=\{p:p\text{ is a function},\ \operatorname{dom}p\subseteq I,\ \operatorname{ran}p\subseteq J,\ |\operatorname{dom}p|<\omega\},\qquad q\leq p\ \Longleftrightarrow\ q\supseteq p.}
$$

Thus a stronger condition specifies more values. The empty [partial function](../../../function.md#partial-function) is the greatest condition. Two conditions are [compatible forcing conditions](../../../forcing.md#compatible-forcing-conditions) exactly when they agree on their common domain; if they do, their [set union](../../../set.md#set-union) is a common strengthening. This is $\operatorname{Fn}(I,J,\omega)$ in the three-argument convention for [Fn forcing](../../../forcing.md#fn-forcing). If $I$ or $J$ is empty, only the empty condition exists. For infinite $I$ and at least two elements in $J$, assigning two different values at a fresh coordinate proves that this is an [atomless forcing order](../../../forcing.md#atomless-forcing-order).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Suppose, towards a contradiction, that $G\in M$. Then $D=\mathbb P\setminus G$ is a ground-model [set](../../../set.md) by [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification). It is dense. If $p\notin G$, it already lies in $D$. If $p\in G$, [atomless forcing order](../../../forcing.md#atomless-forcing-order) structure gives [incompatible forcing conditions](../../../forcing.md#incompatible-forcing-conditions) $q,r\leq p$. Both cannot belong to the directed filter $G$, so at least one is a strengthening of $p$ in $D$.

All compatibility and extension quantifiers range over the same ground-model [set](../../../set.md) $\mathbb P$, so this density argument is also valid internally in the [transitive model](../../../set-theory.md#transitive-model) $M$. Genericity requires $G\cap D\ne\varnothing$, contradicting the definition of $D$. Therefore a [generic filter for an atomless order is new](../../../forcing.md#generic-filter-for-an-atomless-order-is-new):

$$
\boxed{G\notin M.}
$$

The assumption is essential: [a forcing atom determines a ground-model generic filter](../../../forcing.md#a-forcing-atom-determines-a-ground-model-generic-filter). For an atom $p$, the conditions compatible with $p$ form a [generic filter](../../../forcing.md#generic-filter) $G_p\in M$: two such conditions have strengthenings below $p$, which have a common strengthening by the atom property; every dense [set](../../../set.md) has a member below $p$. In a general [partial order](../../../set.md#partially-ordered-set), $G_p$ need not be the [principal filter](../../../set.md#principal-filter-in-an-ordered-set) above $p$.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Put $\kappa=\aleph_2^M$ and let $F=\bigcup G$. Conditions from [Fn forcing](../../../forcing.md#fn-forcing) agree on common coordinates because $G$ is directed, so $F$ is a function. For each $(\xi,n)\in\kappa\times\omega$, the ground-model [set](../../../set.md)

$$
D_{\xi,n}=\{p:(\xi,n)\in\operatorname{dom}p\}
$$

is dense: add a value at that coordinate if necessary. The [generic filter](../../../forcing.md#generic-filter) meets all these [sets](../../../set.md), making $F:\kappa\times\omega\to2$ total.

For distinct $\xi,\eta<\kappa$, the ground-model [set](../../../set.md)

$$
D_{\xi,\eta}=\{p:\exists n\ ((\xi,n),(\eta,n)\in\operatorname{dom}p\text{ and }p(\xi,n)\ne p(\eta,n))\}
$$

is dense. Choose $n$ fresh for both rows of a finite condition and assign $0$ and $1$ there. Genericity therefore makes the rows pairwise different. The [generic coordinate reals for finite-function forcing](../../../forcing.md#generic-coordinate-reals-for-finite-function-forcing) are $c_\xi=\{n\in\omega:F(\xi,n)=1\}$, and in the [generic extension](../../../forcing.md#generic-extension)

$$
\boxed{\xi\longmapsto c_\xi\text{ is an injection }\aleph_2^M\hookrightarrow\mathcal P^{M[G]}(\omega).}
$$

The family is a [set](../../../set.md) in $M[G]$, for example by collecting the ground-model names $\dot c_\xi=\{(\check n,p):p(\xi,n)=1\}$ and evaluating the corresponding name for their indexed family. This argument only needs $\kappa$ as the specified ground-model [ordinal](../../../set-theory.md#ordinal); it does not silently assume a [cardinal preservation by chain-condition forcing](../../../forcing.md#cardinal-preservation-by-chain-condition-forcing) result.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

The [Rasiowa–Sikorski lemma](../../../forcing.md#rasiowa-sikorski-lemma) constructs a [generic filter](../../../forcing.md#generic-filter) $G_i$ over each $M_i$. Every resulting [generic extension](../../../forcing.md#generic-extension) remains a [countable transitive model](../../../forcing.md#countable-transitive-model) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice): there are only countably many ground-model names externally. The order $\mathbb P$ has the same elements and ordering at every stage, and [atomless forcing order](../../../forcing.md#atomless-forcing-order) structure is absolute because all its quantifiers are bounded to $\mathbb P$. Hence the [generic filter for an atomless order is new](../../../forcing.md#generic-filter-for-an-atomless-order-is-new) result gives $G_i\notin M_i$ for every $i$.

The increasing union $N=\bigcup_{i<\omega}M_i$ is transitive and contains $\mathbb P$. If it satisfied [Axiom of power set](../../../set-theory.md#axiom-of-power-set) for $\mathbb P$, there would be a [set](../../../set.md) $A\in N$ with

$$
N\models\forall z\,(z\subseteq\mathbb P\leftrightarrow z\in A).
$$

Choose $i$ with $A\in M_i$. The next-stage [generic filter](../../../forcing.md#generic-filter) $G_i$ belongs to $M_{i+1}\subseteq N$ and is an actual [subset](../../../set.md#subset) of $\mathbb P$. This subset assertion is absolute for the [transitive set](../../../set-theory.md#transitive-set) $N$, so $G_i\in A$. Transitivity of $M_i$ and $A\in M_i$ then give $G_i\in M_i$, a contradiction. Thus the [power-set failure in an increasing union of generic extensions](../../../forcing.md#power-set-failure-in-an-increasing-union-of-generic-extensions) occurs already at the fixed ground-model order:

$$
\boxed{N\not\models\mathsf{PowerSet}\quad\text{because no }\mathcal P^N(\mathbb P)\text{ belongs to }N.}
$$

The stages form an increasing chain, not an elementary chain, so the [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem) does not assert [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) for their union.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
