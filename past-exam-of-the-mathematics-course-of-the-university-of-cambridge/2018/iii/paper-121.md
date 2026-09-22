# Paper 121

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_121.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_121.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [a](#1/iv/a)
      - [Solution](#1/iv/a/solution)
    - [b](#1/iv/b)
      - [Solution](#1/iv/b/solution)
    - [c](#1/iv/c)
      - [Solution](#1/iv/c/solution)
  - [v](#1/v)
    - [a](#1/v/a)
      - [Solution](#1/v/a/solution)
    - [b](#1/v/b)
      - [Solution](#1/v/b/solution)
    - [c](#1/v/c)
      - [Solution](#1/v/c/solution)
  - [vi](#1/vi)
    - [a](#1/vi/a)
      - [Solution](#1/vi/a/solution)
    - [b](#1/vi/b)
      - [Solution](#1/vi/b/solution)
    - [c](#1/vi/c)
      - [Solution](#1/vi/c/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [a](#2/ii/a)
      - [Solution](#2/ii/a/solution)
    - [b](#2/ii/b)
      - [Solution](#2/ii/b/solution)
    - [c](#2/ii/c)
      - [Solution](#2/ii/c/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
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
  - [v](#3/v)
    - [Solution](#3/v/solution)

## 1

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test) says that $(M,\in)$ is an [elementary substructure](../../../mathematical-logic.md#elementary-substructure) of $(N,\in)$ if and only if every existential statement true in $N$ with parameters from $M$ has a witness in $M$ that satisfies its matrix in $N$. Explicitly, for every [first-order formula](../../../mathematical-logic.md#first-order-formula) $\psi(x,\bar y)$ and every parameter tuple $\bar a\in M^{|\bar y|}$, require

$$
\boxed{N\models\exists x\,\psi(x,\bar a)\quad\Longrightarrow\quad\exists b\in M\;N\models\psi(b,\bar a).}
$$

The truth of the matrix in this test is evaluated in the larger structure $N$. Under this criterion, $(M,\in)\prec(N,\in)$ means that all [first-order formulas](../../../mathematical-logic.md#first-order-formula) with parameters from $M$ have identical truth values in the two structures.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) applies when $E$ is a [well-founded relation](../../../set-theory.md#well-founded-relation) and an [extensional relation](../../../set-theory.md#extensional-relation) on the set $M$. Extensionality here means that different points have different sets of $E$-predecessors. There is then a unique [transitive set](../../../set-theory.md#transitive-set) $T$ and a unique [bijection](../../../function.md#bijection) $\pi:M\to T$ such that

$$
\boxed{x\,E\,y\iff\pi(x)\in\pi(y).}
$$

The collapsing map is characterized by [well-founded relation](../../../set-theory.md#well-founded-relation) recursion:

$$
\pi(x)=\{\pi(y):y\in M,\ y\,E\,x\}.
$$

Thus $(M,E)$ is isomorphic to $(T,\in)$. Both well-foundedness and extensionality are hypotheses of the theorem; well-foundedness alone does not make the recursive map injective.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

A [cardinal number](../../../set-theory.md#cardinal-number) is identified with an [initial ordinal](../../../set-theory.md#initial-ordinal), namely an [ordinal](../../../set-theory.md#ordinal) not in [bijection](../../../function.md#bijection) with any smaller ordinal. An [inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal), in the strong sense used here, is an uncountable [regular cardinal](../../../set-theory.md#regular-cardinal) that is also a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal). Thus

$$
\boxed{\kappa>\aleph_0,\qquad\operatorname{cf}(\kappa)=\kappa,\qquad 2^\lambda<\kappa\text{ for every cardinal }\lambda<\kappa.}
$$

A [worldly cardinal](../../../set-theory.md#worldly-cardinal) is a [cardinal number](../../../set-theory.md#cardinal-number) whose level of the [Von Neumann hierarchy](../../../set-theory.md#von-neumann-hierarchy) satisfies all of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice):

$$
\boxed{(V_\kappa,\in)\models\mathsf{ZFC}.}
$$

Worldliness is this model-theoretic condition; regularity is not part of its definition. The original PDF asks for these two notions; the extra comma in the local TeX makes “cardinal” look like a separate requested item.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/a">a</h4>

↑ **Parent:** [Iv](#1/iv)

<h5 id="1/iv/a/solution">Solution</h5>

↑ **Parent:** [A](#1/iv/a)

For every tuple of parameters $\bar a\in M^n$, a [downward absolute formula](../../../set-theory.md#downward-absolute-formula) transfers truth from the larger structure to the smaller one:

$$
\boxed{(N,\in)\models\varphi(\bar a)\quad\Longrightarrow\quad(M,\in)\models\varphi(\bar a).}
$$

The condition concerns every parameter tuple from $M$, not merely parameter-free sentences.

<h4 id="1/iv/b">b</h4>

↑ **Parent:** [Iv](#1/iv)

<h5 id="1/iv/b/solution">Solution</h5>

↑ **Parent:** [B](#1/iv/b)

For every tuple of parameters $\bar a\in M^n$, an [upward absolute formula](../../../set-theory.md#upward-absolute-formula) transfers truth from the smaller structure to the larger one:

$$
\boxed{(M,\in)\models\varphi(\bar a)\quad\Longrightarrow\quad(N,\in)\models\varphi(\bar a).}
$$

These definitions of directional [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) do not themselves require the structures to be transitive.

<h4 id="1/iv/c">c</h4>

↑ **Parent:** [Iv](#1/iv)

<h5 id="1/iv/c/solution">Solution</h5>

↑ **Parent:** [C](#1/iv/c)

A formula has [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness) between these structures when both directions hold for every $\bar a\in M^n$:

$$
\boxed{(M,\in)\models\varphi(\bar a)\quad\Longleftrightarrow\quad(N,\in)\models\varphi(\bar a).}
$$

Equivalently, it is both a [downward absolute formula](../../../set-theory.md#downward-absolute-formula) and an [upward absolute formula](../../../set-theory.md#upward-absolute-formula) between them.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/a">a</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/a/solution">Solution</h5>

↑ **Parent:** [A](#1/v/a)

We construct the two [transitive models](../../../set-theory.md#transitive-model) together, taking care that the later collapse really retains the earlier model. First, a [worldly cardinal](../../../set-theory.md#worldly-cardinal) $\kappa$ is greater than $\omega_1$: [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) in $V_\kappa$ contains the full [power set](../../../set.md#power-set) $\mathcal P(\omega)$, and the [axiom of choice](../../../set-theory.md#axiom-of-choice) there gives a [bijection](../../../function.md#bijection) between it and an ordinal $\gamma<\kappa$. That power set is externally uncountable by [Cantor theorem](../../../set.md#cantor-s-theorem), so $\gamma\geq\omega_1$. Infinity rules out the finite cardinals and $\omega$ before this argument is applied.

By the [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem), choose a countable [elementary substructure](../../../mathematical-logic.md#elementary-substructure) $X\prec(V_\kappa,\in)$. Its inherited membership is a [well-founded relation](../../../set-theory.md#well-founded-relation), and elementarity transfers extensionality from $V_\kappa$. Apply the [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) to obtain a [countable transitive model](../../../forcing.md#countable-transitive-model) $M$ of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Because $M$ is a countable [transitive set](../../../set-theory.md#transitive-set), it is a [hereditarily countable set](../../../set-theory.md#hereditarily-countable-set) and its [rank of a set](../../../set-theory.md#rank-of-a-set) is below $\omega_1$. In particular, $M\in V_\kappa$.

Now take the [Skolem hull](../../../mathematical-logic.md#skolem-hull) in $V_\kappa$ of the seed

$$
S=\omega_1\cup M\cup\{\omega_1,M\}.
$$

Call it $H$. The seed has external cardinality $\aleph_1$ and lies inside $V_\kappa$. The hull is an [elementary substructure](../../../mathematical-logic.md#elementary-substructure) of $V_\kappa$ with $|H|=\aleph_1$: closure under countably many finitary Skolem functions gives the upper bound, and $\omega_1\subseteq H$ gives the lower bound. Let $\pi:H\to N$ be its [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) map. Then $N$ is a [transitive model](../../../set-theory.md#transitive-model) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice).

The [transitive collapse fixes transitive subsets](../../../set-theory.md#transitive-collapse-fixes-transitive-subsets) lemma gives $\pi(m)=m$ for every $m\in M$, since $M\subseteq H$ is transitive. Since also $M\in H$, the collapse sends that element to $M$ itself. Thus $M\in N$, and transitivity of $N$ yields the required inclusion:

$$
\boxed{M\in N\quad\text{and hence}\quad M\subseteq N.}
$$

This is the construction of [nested transitive models from a worldly cardinal](../../../set-theory.md#nested-transitive-models-from-a-worldly-cardinal); the next two parts verify its size and ordinal requirements.

<h4 id="1/v/b">b</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/b/solution">Solution</h5>

↑ **Parent:** [B](#1/v/b)

For the model $M$ constructed in part (a), the collapsing map $X\to M$ is a [bijection](../../../function.md#bijection). The [Downward Lowenheim-Skolem theorem](../../../mathematical-logic.md#downward-lowenheim-skolem-theorem) supplied countable $X$, so $M$ is externally countable. It is infinite because it satisfies the [axiom of infinity](../../../set-theory.md#axiom-of-infinity). Consequently

$$
\boxed{|M|=\aleph_0.}
$$

This is external [cardinality](../../../set-theory.md#cardinality). A [countable transitive model](../../../forcing.md#countable-transitive-model) still regards many of its own sets and ordinals as uncountable, because external enumerations need not belong to it.

<h4 id="1/v/c">c</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/c/solution">Solution</h5>

↑ **Parent:** [C](#1/v/c)

The collapse $\pi:H\to N$ is a [bijection](../../../function.md#bijection), so $|N|=|H|=\aleph_1$. Every $\alpha<\omega_1$ and every element of $\alpha$ belong to $H$. The [transitive collapse fixes transitive subsets](../../../set-theory.md#transitive-collapse-fixes-transitive-subsets) lemma therefore gives $\pi(\alpha)=\alpha$, so every ambient [countable ordinal](../../../set-theory.md#countable-ordinal) belongs to $N$.

Moreover, $V_\kappa$ correctly regards each such $\alpha$ as countable. An injection $\alpha\to\omega$ has rank below $\max(\alpha,\omega)+\omega<\kappa$, so a witness belongs to $V_\kappa$. Elementarity gives $H\models$ “$\alpha$ is a countable ordinal”. Transporting this statement across the collapse, which fixes $\alpha$, gives the same statement in $N$.

The collapse also fixes the element $\omega_1\in H$. No injection $\omega_1\to\omega$ exists externally, hence none belongs to $V_\kappa$; together with the countability witnesses below it, this shows that $V_\kappa$ correctly identifies $\omega_1$ as its first uncountable ordinal. Elementarity and the collapse preserve that identification. Thus the construction gives

$$
\boxed{|N|=\aleph_1,\quad\alpha\in N\text{ and }N\models\text{“}\alpha\text{ is countable”}\ (\alpha<\omega_1),\quad(\omega_1)^N=\omega_1.}
$$

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/a">a</h4>

↑ **Parent:** [Vi](#1/vi)

<h5 id="1/vi/a/solution">Solution</h5>

↑ **Parent:** [A](#1/vi/a)

Take the formula saying that a set is transitive:

$$
\boxed{\varphi_1(x):\quad\forall u\in x\;\forall v\in u\;(v\in x).}
$$

This is a [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory). If $x\in M$, transitivity of $M$ ensures that every $u\in x$ and every $v\in u$ is already in $M$, and the same holds in $N$. Both structures therefore run through exactly the same bounded witnesses and use the same actual membership relation. They agree on $\varphi_1(x)$ for every $x\in M$, proving [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness).

<h4 id="1/vi/b">b</h4>

↑ **Parent:** [Vi](#1/vi)

<h5 id="1/vi/b/solution">Solution</h5>

↑ **Parent:** [B](#1/vi/b)

Let $C(x)$ be the formula expressing [cardinal number](../../../set-theory.md#cardinal-number) status:

$$
\boxed{\varphi_2(x)=C(x):\quad x\text{ is an ordinal}\ \land\ \forall\alpha\in x\;\neg\exists f\;(f\text{ is a bijection }\alpha\to x).}
$$

Ordinalhood and the assertion that a given set is a [bijection](../../../function.md#bijection) between fixed sets are each expressible by a [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory). If $M$ regarded $x$ as a non-cardinal ordinal, a witnessing smaller ordinal and bijection would remain present and valid in $N$. Ordinalhood itself is absolute between the [transitive models](../../../set-theory.md#transitive-model). Thus $N\models C(x)$ implies $M\models C(x)$: this is [downward absoluteness of cardinalhood](../../../set-theory.md#downward-absoluteness-of-cardinalhood).

For failure in the other direction, put $\beta=(\omega_1)^M$. This ordinal belongs to $M$, and $M\models C(\beta)$ with $\beta>\omega$. Externally $\beta$ is countable, since $\beta\subseteq M$ and $M$ is countable. By the construction of $N$, it contains a countability witness for $\beta$, and hence a bijection $\omega\to\beta$. Therefore $N\models\neg C(\beta)$. This formula is downward absolute and fails to be upward absolute.

<h4 id="1/vi/c">c</h4>

↑ **Parent:** [Vi](#1/vi)

<h5 id="1/vi/c/solution">Solution</h5>

↑ **Parent:** [C](#1/vi/c)

Use the cardinalhood formula $C$ from part (b), and let a finite flag choose between it and its negation:

$$
\boxed{\varphi_3(x,i):\quad(i=0\land C(x))\lor(i=1\land\neg C(x)).}
$$

Here $0,1$ abbreviate their parameter-free definitions as [Finite von Neumann ordinals](../../../set-theory.md#finite-von-neumann-ordinal), and both belong to $M$. This is one [first-order formula](../../../mathematical-logic.md#first-order-formula) with two free variables.

For $\beta=(\omega_1)^M$, part (b) proved $M\models C(\beta)$ and $N\models\neg C(\beta)$. The shared parameters $(\beta,0)$ therefore make $\varphi_3$ true in $M$ and false in $N$, disproving upward [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness). The shared parameters $(\beta,1)$ make it false in $M$ and true in $N$, disproving downward [set-theoretic absoluteness](../../../set-theory.md#set-theoretic-absoluteness). Hence the same formula fails both directions, with explicit witnesses to each failure.

## 2

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [constructible hierarchy](../../../definable-power-set.md#constructible-hierarchy) is defined by [transfinite recursion](../../../set-theory.md#transfinite-recursion) using the [definable power set](../../../definable-power-set.md). With parameters permitted in the internal definitions, write $\operatorname{Def}(A,1)$ for the definable subsets of $A$. Then

$$
\boxed{L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha,1),\qquad L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha\quad(\lambda\text{ a nonzero limit ordinal}).}
$$

Its class union is the [constructible universe](../../../definable-power-set.md#constructible-universe) $L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha$. Only subsets definable over $(L_\alpha,\in)$ using a [first-order formula](../../../mathematical-logic.md#first-order-formula) and finitely many parameters from $L_\alpha$ enter at a successor stage.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/a">a</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/ii/a)

We prove simultaneously that each $L_\alpha$ is a [transitive set](../../../set-theory.md#transitive-set) and that $L_\alpha\subseteq L_{\alpha+1}$. The key observation is that if $A$ is transitive and $x\in A$, then $x\subseteq A$ and

$$
x=\{y\in A:(A,\in)\models y\in x\}.
$$

This is an internal definition with parameter $x$, so $x\in\operatorname{Def}(A,1)$. Hence $A\subseteq\operatorname{Def}(A,1)$. Every $z\in\operatorname{Def}(A,1)$ is a subset of $A$; if $y\in z$, then $y\in A\subseteq\operatorname{Def}(A,1)$. Thus the definable power set is transitive too.

Start with the empty set. At successor stages the observation proves transitivity and inclusion. At a limit stage the union of the earlier transitive sets is transitive, and the same observation then proves its inclusion in its own definable power set. This completes the [transfinite induction](../../../set-theory.md#transfinite-induction) and gives

$$
\boxed{\forall\alpha\quad L_\alpha\text{ is transitive}.}
$$

<h4 id="2/ii/b">b</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/ii/b)

The argument in part (a) established $L_\alpha\subseteq L_{\alpha+1}$ for every ordinal $\alpha$. A [transfinite induction](../../../set-theory.md#transfinite-induction) on $\beta$ now proves that every earlier level is contained in $L_\beta$. If $\beta=\gamma+1$, use the inductive inclusions into $L_\gamma$ followed by $L_\gamma\subseteq L_{\gamma+1}$. At a limit stage, every earlier level is one of the sets in the defining union. Equality of indices is trivial. Thus

$$
\boxed{\alpha\leq\beta\quad\Longrightarrow\quad L_\alpha\subseteq L_\beta.}
$$

The [constructible hierarchy](../../../definable-power-set.md#constructible-hierarchy) is a [nondecreasing family of sets](../../../set.md#nondecreasing-family-of-sets).

<h4 id="2/ii/c">c</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#2/ii/c)

Induct on $\alpha$ using the transitivity and inclusion already established. The zero stage is immediate. Suppose $L_\alpha\cap\operatorname{Ord}=\alpha$. Being an [ordinal](../../../set-theory.md#ordinal) is expressible by a [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory), for example transitivity, transitivity of all members, and membership comparability. It is therefore absolute for the transitive set $L_\alpha$. The subset of its elements that are ordinals is internally definable, so

$$
\alpha=\{x\in L_\alpha:x\text{ is an ordinal}\}\in\operatorname{Def}(L_\alpha,1)=L_{\alpha+1}.
$$

By inclusion, all smaller ordinals are present as well. Conversely, if an ordinal $\gamma$ belongs to $L_{\alpha+1}$, then $\gamma\subseteq L_\alpha$, since every member of a [definable power set](../../../definable-power-set.md) is a subset of the preceding domain. All members of $\gamma$ are ordinals, so $\gamma\subseteq L_\alpha\cap\operatorname{Ord}=\alpha$ and $\gamma\leq\alpha$. Hence the ordinal part of the successor level is exactly $\alpha+1$.

At a nonzero limit ordinal $\lambda$,

$$
L_\lambda\cap\operatorname{Ord}=\bigcup_{\alpha<\lambda}(L_\alpha\cap\operatorname{Ord})=\bigcup_{\alpha<\lambda}\alpha=\lambda.
$$

Thus

$$
\boxed{L_\alpha\cap\operatorname{Ord}=\alpha\quad\text{for every ordinal }\alpha.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Let $\theta=M\cap\operatorname{Ord}$ be the [ordinal height of a model of set theory](../../../set-theory.md#ordinal-height-of-a-model-of-set-theory). First $\theta\geq\omega_1$. Indeed, if $\theta$ were countable, the internal [axiom of choice](../../../set-theory.md#axiom-of-choice) would give, for every $x\in M$, a bijection in $M$ between $x$ and some ordinal below $\theta$. Such a bijection is also valid externally, making $x$ externally countable. In particular every internal rank $V_\xi^M$, $\xi<\theta$, would be countable. Every element of $M$ lies in one of these internal ranks, so

$$
M=\bigcup_{\xi<\theta}V_\xi^M
$$

would be a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets), a contradiction. This is why an [uncountable transitive set model has uncountable ordinal height](../../../set-theory.md#uncountable-transitive-set-model-has-uncountable-ordinal-height).

For $\xi<\theta$, [absoluteness of constructible levels](../../../definable-power-set.md#absoluteness-of-constructible-levels) gives $L_\xi^M=L_\xi$, and that level is an element of $M$. The reason is that satisfaction in a fixed set structure uses the same domain and finite formulas in both universes, so successor definitions agree; [transfinite recursion](../../../set-theory.md#transfinite-recursion) then also makes limit stages agree. Transitivity consequently gives

$$
L_{\omega_1}\subseteq L_\theta\subseteq M.
$$

It remains to locate a countability witness. Given an ambient [countable ordinal](../../../set-theory.md#countable-ordinal) $\alpha$, choose an injection $f:\alpha\to\omega$. Since $V=L$, it belongs to the [constructible universe](../../../definable-power-set.md#constructible-universe). Its [transitive closure](../../../set-theory.md#transitive-closure), together with $f$ itself, is countable. Choose a countable [elementary substructure](../../../mathematical-logic.md#elementary-substructure) $X\prec L_\eta$ of a sufficiently large limit level containing this closure pointwise. The [condensation lemma for the constructible universe](../../../definable-power-set.md#condensation-lemma-for-the-constructible-universe) identifies the collapse with $L_\beta$ for some countable $\beta$. The collapse fixes $f$, since all its hereditary members were included. Thus $f\in L_\beta\subseteq L_{\omega_1}\subseteq M$.

The ordinal $\alpha$ itself is in $M$, since $\alpha<\omega_1\leq\theta$. Being an injection between these fixed sets is a [bounded formula in set theory](../../../set-theory.md#bounded-formula-in-set-theory), so $M$ recognizes $f$ as a countability witness. This proves [countable-ordinal correctness under constructibility](../../../set-theory.md#countable-ordinal-correctness-under-constructibility):

$$
\boxed{\alpha\in M\quad\text{and}\quad M\models\text{“}\alpha\text{ is countable”}\qquad(\alpha<\omega_1).}
$$

The use of condensation supplies a witness below the height of $M$; merely knowing that $f$ belongs somewhere to $L$ would not be sufficient.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

We give a relative-consistency argument using a [finite-function collapse to countable size](../../../forcing.md#finite-function-collapse-to-countable-size). The assumed consistency implies that [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) is consistent. Passing to the [constructible universe](../../../definable-power-set.md#constructible-universe) gives consistency of $\mathsf{ZFC}+V=L$, which also satisfies the [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis). Work in this ground theory, let $\delta=\omega_1^L$, and force with finite [partial functions](../../../function.md#partial-function) $\omega\rightharpoonup\delta$, ordered by reverse inclusion.

The union of a [generic filter](../../../forcing.md#generic-filter) $H$ is a total surjection $h:\omega\to\delta$: prescribing a new domain coordinate is dense, and putting any specified $\gamma<\delta$ into the range is dense. Hence $\delta$ becomes countable. Set forcing preserves ordinals, and [absoluteness of constructible levels](../../../definable-power-set.md#absoluteness-of-constructible-levels) implies that the extension has the same constructible universe as the ground model. Its $\omega_1^L$ is therefore still the old $\delta$, so it satisfies the stated [countability of constructible omega-one](../../../definable-power-set.md#countability-of-constructible-omega-one) condition.

We must also verify GCH after the collapse. The order has ground-model size $\delta$, hence the $\delta^+$-chain condition. By [cardinal preservation by chain-condition forcing](../../../forcing.md#cardinal-preservation-by-chain-condition-forcing), all old cardinals at least $\delta^+$ survive. Every old ordinal below $\delta^+$ has size at most $\delta$ and becomes countable, so the old $\delta^+$ is exactly the new $\omega_1$.

A name for a subset of a fixed ground-model ordinal $\lambda$ can be chosen as a set of pairs $(\check\xi,p)$ with $\xi<\lambda$ and $p$ a condition: use an antichain deciding membership at each coordinate. Thus the number of such names in the ground model is at most $2^{|\lambda\times\mathbb P|}$. For subsets of $\omega$ this is $2^\delta=\delta^+$ by ground-model GCH. In the extension it gives $2^{\aleph_0}\leq\delta^+=\aleph_1$, and [Cantor theorem](../../../set.md#cantor-s-theorem) gives the reverse lower bound. For every old cardinal $\lambda\geq\delta^+$ the bound is

$$
2^{\lambda\cdot\delta}=2^\lambda=\lambda^+
$$

in the ground model. Both $\lambda$ and $\lambda^+$ remain cardinals, so again the upper bound and [Cantor theorem](../../../set.md#cantor-s-theorem) give the extension's equality $2^\lambda=\lambda^+$. These are all its uncountable cardinals. This proves [GCH preservation by a finite-function collapse](../../../forcing.md#gch-preservation-by-a-finite-function-collapse) in the required case.

The forcing relative-consistency theorem now yields

$$
\boxed{\operatorname{Con}(\mathsf{ZFC}+\mathrm{NC})\ \Longrightarrow\ \operatorname{Con}(\mathsf{ZFC}+\mathrm{NC}+\mathrm{GCH}).}
$$

The construction in fact only needs consistency of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). This argument uses the formal inner-model and forcing consistency theorems; it does not infer the existence of a [countable transitive model](../../../forcing.md#countable-transitive-model) merely from consistency.

## 3

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use [standard notation for forcing](../../../forcing.md#standard-notation-for-forcing), so $q\leq p$ means that $q$ is stronger. Let $\check p$ be the [canonical forcing name](../../../forcing.md#canonical-forcing-name) for the ground-model condition $p$. Define

$$
\boxed{\tau=\{(\check p,q):p,q\in\mathbb P,\ q\perp p\}.}
$$

Here $q\perp p$ means that they are [incompatible forcing conditions](../../../forcing.md#incompatible-forcing-conditions). The checks and their collection are formed by recursion and [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) in $M$, and the displayed set is selected by [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification), so this is a [forcing name](../../../forcing.md#forcing-name) in $M$.

By [evaluation of a forcing name](../../../forcing.md#evaluation-of-a-forcing-name),

$$
\operatorname{val}(\tau,G)=\{p\in\mathbb P:\exists q\in G\ (q\perp p)\}.
$$

If $p\in G$, directedness of the [generic filter](../../../forcing.md#generic-filter) gives a common stronger condition for $p$ and each $q\in G$, so $p$ is absent from this value.

Conversely, for fixed $p\in\mathbb P$ the set

$$
D_p=\{q\in\mathbb P:q\leq p\text{ or }q\perp p\}
$$

is a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order) belonging to $M$. A condition incompatible with $p$ is already in it, and one compatible with $p$ has a common extension below $p$. Genericity supplies $q\in G\cap D_p$. If $p\notin G$, upward closure of $G$ rules out $q\leq p$, hence $q\perp p$. Therefore

$$
\boxed{\operatorname{val}(\tau,G)=\mathbb P\setminus G.}
$$

This [forcing name for the complement of a generic filter](../../../forcing.md#forcing-name-for-the-complement-of-a-generic-filter) works without a separativity assumption on the order.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/a">a</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/ii/a)

We prove the implication from existence of a witness in the extension to a condition forcing the existential statement. If $M[G]\models\exists x\,\varphi(x)$, choose a witness $a\in M[G]$ and a [forcing name](../../../forcing.md#forcing-name) $\sigma\in M$ with $\operatorname{val}(\sigma,G)=a$. The assumed instance of the truth lemma supplies $p\in G$ with

$$
M\models p\Vdash^*\varphi(\sigma).
$$

The [syntactic forcing relation](../../../forcing.md#syntactic-forcing-relation) is monotone under stronger conditions, so every $q\leq p$ also forces this same named instance. In particular, the conditions below $p$ having some forced witness are [dense below a forcing condition](../../../forcing.md#dense-below-a-forcing-condition) $p$. The [existential clause of syntactic forcing](../../../forcing.md#existential-clause-of-syntactic-forcing) therefore gives

$$
\boxed{M[G]\models\exists x\,\varphi(x)\quad\Longrightarrow\quad\exists p\in G\;M\models p\Vdash^*\exists x\,\varphi(x).}
$$

Only the truth lemma assumed for individual named instances and the recursive existential clause were used.

<h4 id="3/ii/b">b</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/ii/b)

For the reverse implication, suppose $p\in G$ and $M\models p\Vdash^*\exists x\,\varphi(x)$. By the [existential clause of syntactic forcing](../../../forcing.md#existential-clause-of-syntactic-forcing), the set

$$
D=\{q\leq p:M\models\exists\sigma\;(q\Vdash^*\varphi(\sigma))\}
$$

is dense below $p$; the existential quantifier ranges over [forcing names](../../../forcing.md#forcing-name) of $M$. Definability of the [syntactic forcing relation](../../../forcing.md#syntactic-forcing-relation) and [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) put $D$ in $M$.

To apply genericity, augment it to the globally dense set

$$
D'=D\cup\{q\in\mathbb P:q\perp p\}.
$$

A condition compatible with $p$ has an extension below $p$, then one in $D$, and an incompatible condition already lies in $D'$. Thus $D'$ is a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order) in $M$. The [generic filter](../../../forcing.md#generic-filter) meets it. Since $p\in G$, directedness prevents $G$ from containing a condition incompatible with $p$, so some $q\in G\cap D$ exists.

There is consequently a name $\sigma\in M$ with $M\models q\Vdash^*\varphi(\sigma)$. The assumed truth lemma gives $M[G]\models\varphi(\operatorname{val}(\sigma,G))$, and hence

$$
\boxed{\exists p\in G\;M\models p\Vdash^*\exists x\,\varphi(x)\quad\Longrightarrow\quad M[G]\models\exists x\,\varphi(x).}
$$

Together with part (a), this completes the existential step of the [forcing theorem](../../../forcing.md#forcing-theorem) without assuming the desired existential truth lemma in advance.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

A [Delta-system](../../../set-theory.md#delta-system) is a family $\mathcal A$ of sets with a fixed root $r$ such that

$$
\boxed{A\cap B=r\qquad\text{whenever }A,B\in\mathcal A\text{ are distinct}.}
$$

The [Delta-system lemma](../../../set-theory.md#delta-system-lemma) says that every uncountable family of finite sets has an uncountable subfamily forming a [Delta-system](../../../set-theory.md#delta-system). The root may be empty. Finiteness is a hypothesis on the family to which this lemma is applied, rather than a requirement in the general definition of a [Delta-system](../../../set-theory.md#delta-system).

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/a">a</h4>

↑ **Parent:** [Iv](#3/iv)

<h5 id="3/iv/a/solution">Solution</h5>

↑ **Parent:** [A](#3/iv/a)

A [cardinal-preserving forcing](../../../forcing.md#cardinal-preserving-forcing) over $M$ leaves every ground-model [cardinal number](../../../set-theory.md#cardinal-number) a cardinal in every [generic extension](../../../forcing.md#generic-extension). In the present notation, for every $M$-generic filter $G$ and every ordinal $\kappa\in M$,

$$
\boxed{M\models\text{“}\kappa\text{ is a cardinal”}\quad\Longrightarrow\quad M[G]\models\text{“}\kappa\text{ is a cardinal”}.}
$$

Set [forcing](../../../forcing.md) preserves ordinals, and an old bijection witnessing that an ordinal is not a cardinal remains available. Thus this condition also means that the two models have exactly the same cardinals. Cardinality here is computed inside the respective models, not from their external sizes.

<h4 id="3/iv/b">b</h4>

↑ **Parent:** [Iv](#3/iv)

<h5 id="3/iv/b/solution">Solution</h5>

↑ **Parent:** [B](#3/iv/b)

The [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing) says that every [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) is a [countable set](../../../set-theory.md#countable-set). Equivalently,

$$
\boxed{\text{There is no uncountable set of pairwise incompatible conditions.}}
$$

In this question the assertion is evaluated inside $M$. Although every subset of the countable set $M$ is externally countable, that observation does not establish the internal chain condition: $M$ need not contain an enumeration of an antichain.

<h4 id="3/iv/c">c</h4>

↑ **Parent:** [Iv](#3/iv)

<h5 id="3/iv/c/solution">Solution</h5>

↑ **Parent:** [C](#3/iv/c)

Assume $M$ satisfies the [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing). We prove [cardinal preservation by chain-condition forcing](../../../forcing.md#cardinal-preservation-by-chain-condition-forcing) using the [possible-values lemma for chain-condition forcing](../../../forcing.md#possible-values-lemma-for-chain-condition-forcing), and give the argument explicitly for ccc.

Let $\kappa$ be an uncountable cardinal of $M$. If it ceased to be a cardinal, some ordinal $\mu<\kappa$ would admit a surjection onto $\kappa$ in an extension. By the [forcing theorem](../../../forcing.md#forcing-theorem), there would be a condition $p$ and a [forcing name](../../../forcing.md#forcing-name) $\dot f$ such that

$$
p\Vdash\dot f:\check\mu\twoheadrightarrow\check\kappa.
$$

Inside $M$, for each $\xi<\mu$ choose a maximal [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) below $p$ deciding the ordinal value of $\dot f(\xi)$. Conditions deciding that value are dense below $p$. The chain condition makes the chosen antichain countable in $M$, so the corresponding set $B_\xi\subseteq\kappa$ of possible decided values is countable in $M$.

A [generic filter](../../../forcing.md#generic-filter) containing $p$ meets the downward closure of every such maximal antichain, so its value $f(\xi)$ belongs to $B_\xi$. Therefore its whole range lies in the ground-model set

$$
B=\bigcup_{\xi<\mu}B_\xi,\qquad |B|^M\leq|\mu|^M\cdot\aleph_0<\kappa.
$$

The last inequality is [infinite cardinal arithmetic](../../../set-theory.md#infinite-cardinal-arithmetic) and uses only that $\kappa$ is uncountable and $\mu<\kappa$; no regularity of $\kappa$ is needed. Some ordinal in $\kappa\setminus B$ exists already in $M$ and cannot occur in the range, contradicting the forced surjectivity.

Finite cardinals cannot collapse, and $\omega$ cannot become finite: a finite domain has finite image, and transitive models agree on the [natural numbers](../../../arithmetic.md#natural-number). Old non-cardinals cannot become cardinals because their old bijections persist. Thus

$$
\boxed{\mathbb P\text{ is ccc in }M\quad\Longrightarrow\quad\operatorname{Card}^{M[G]}=\operatorname{Card}^{M}.}
$$

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Let $s_p$ be the finite stem of a condition $p=(n_p,s_p,A_p)$, and define

$$
f=\bigcup_{p\in G}s_p.
$$

The stems of two conditions in the [generic filter](../../../forcing.md#generic-filter) agree on their common domain, because they have a common stronger extension. Hence this union is a function. For every $\ell\in\omega$, the set of conditions with $n_p\geq\ell$ is dense: append values from the nonempty infinite reservoir until the desired length is reached. Genericity therefore makes $f$ total on $\omega$. The generic stems, and thus their union, are available in $M[G]$.

Fix $g\in M\cap\omega^\omega$ and $K\in\omega$. In $M$ form the set

$$
D_{g,K}=\{(n,s,A):\exists k\ (K\leq k<n\ \land\ g(k)<s(k))\}.
$$

We show that it is a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order). Given $p=(n,s,A)$, put $k=\max(n,K)$. Fill the new positions $n,\ldots,k-1$ with any fixed element of $A$, and choose $a\in A$ with $a>g(k)$ for the new position $k$. This is possible because an infinite subset of $\omega$ is unbounded. Let $t$ be the resulting stem of length $k+1$, and keep the reservoir $A$ unchanged. Then

$$
q=(k+1,t,A)\leq p,\qquad q\in D_{g,K}.
$$

Every new stem value came from the old reservoir, exactly as required by the extension relation. The construction is performed in $M$, so $D_{g,K}\in M$ and is internally dense.

Genericity gives a condition in $G\cap D_{g,K}$. Its witnessing coordinate remains fixed in every later stem and hence in $f$, so some $k\geq K$ satisfies $g(k)<f(k)$. Since this holds for every $K$, there are infinitely many such $k$. As $g$ was arbitrary,

$$
\boxed{f\in\omega^\omega\cap M[G],\qquad\forall g\in M\cap\omega^\omega\;\exists^\infty k\;(g(k)<f(k)).}
$$

Thus this [infinite-reservoir stem forcing](../../../forcing.md#infinite-reservoir-stem-forcing) produces an [unbounded real over a model](../../../forcing.md#unbounded-real-over-a-model), which is precisely the stipulated meaning of bounding $M$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
