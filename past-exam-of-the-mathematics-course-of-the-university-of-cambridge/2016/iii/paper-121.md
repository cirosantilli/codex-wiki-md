# Paper 121

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_121.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_121.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [i](#5/e/i)
      - [Solution](#5/e/i/solution)
    - [ii](#5/e/ii)
      - [Solution](#5/e/ii/solution)

## 1

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For an infinite [cardinal number](../../../set-theory.md#cardinal-number) $\kappa$, the [gimel function](../../../set-theory.md#gimel-function) is

$$
\boxed{\gimel(\kappa)=\kappa^{\operatorname{cf}(\kappa)}}.
$$

The [singular cardinals hypothesis](../../../set-theory.md#singular-cardinals-hypothesis) asserts that for every infinite [singular cardinal](../../../set-theory.md#singular-cardinal) $\kappa$,

$$
\boxed{2^{\operatorname{cf}(\kappa)}<\kappa
\ \Longrightarrow\ \gimel(\kappa)=\kappa^+.}
$$

Here $\kappa^+$ is the [successor cardinal](../../../set-theory.md#successor-cardinal). Equivalently, for every infinite [singular cardinal](../../../set-theory.md#singular-cardinal),

$$
\kappa^{\operatorname{cf}(\kappa)}
=\max\{\kappa^+,2^{\operatorname{cf}(\kappa)}\}.
$$

To see why the second formulation adds nothing in the other case, put $\theta=\operatorname{cf}(\kappa)$. If $\kappa\leq2^\theta$, then $2^\theta\leq\kappa^\theta\leq(2^\theta)^\theta=2^\theta$ by [infinite cardinal arithmetic](../../../set-theory.md#infinite-cardinal-arithmetic). Equality $\kappa=2^\theta$ is impossible here: the [König theorem for cardinal numbers](../../../set-theory.md#konig-s-theorem-set-theory) gives $\operatorname{cf}(2^\theta)>\theta$, whereas $\operatorname{cf}(\kappa)=\theta$. Thus in this case $2^\theta\geq\kappa^+$, as required by the maximum formula. For a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) that is singular, the hypothesis also yields $2^\kappa=\kappa^+$: restrictions of a subset of $\kappa$ to a cofinal sequence of smaller cardinals give $2^\kappa\leq\kappa^\theta$, while the reverse inequality is immediate. The quantified implication above is the precise general statement.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $\mathfrak c=2^{\aleph_0}$. Its [cofinality](../../../set-theory.md#cofinality) is $\aleph_1$, so choose a strictly increasing sequence of infinite [cardinal numbers](../../../set-theory.md#cardinal-number) $(\kappa_\xi)_{\xi<\omega_1}$ below $\mathfrak c$ with supremum $\mathfrak c$. Such a sequence is obtained by refining a cofinal sequence and choosing larger cardinals recursively; $\mathfrak c$ is a [singular cardinal](../../../set-theory.md#singular-cardinal), hence a [limit cardinal](../../../set-theory.md#limit-cardinal).

By the [axiom of choice](../../../set-theory.md#axiom-of-choice), fix a [bijection](../../../function.md#bijection) $b:\mathfrak c\to\mathbb R$. Set

$$
A_\xi=b[\kappa_\xi],\qquad
\boxed{\mathcal A=\{A_\xi:\xi<\omega_1\}}.
$$

Every $A_\xi$ is infinite, $|A_\xi|=\kappa_\xi<\mathfrak c$, and distinct indices give distinct [cardinalities](../../../set-theory.md#cardinality). The [cofinality](../../../set-theory.md#cofinality) of the sequence ensures

$$
\bigcup_{\xi<\omega_1}A_\xi=b\left[\bigcup_{\xi<\omega_1}\kappa_\xi\right]=b[\mathfrak c]=\mathbb R.
$$

Thus $|\mathcal A|=\aleph_1$. Pairwise different sizes means different sizes for distinct members; without that qualification the parenthetical condition would contradict the case $A=B$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The least index is $\boxed{\alpha=\omega_1}$, with

$$
\boxed{\sigma_{\omega_1}=\aleph_{\omega_1},\qquad
\operatorname{cf}(\sigma_{\omega_1})=\aleph_1}.
$$

Indeed, for every nonzero [limit ordinal](../../../set-theory.md#limit-ordinal) $\beta$, continuity of the [aleph number](../../../set-theory.md#aleph-number) enumeration and the [cofinality of an increasing ordinal supremum](../../../set-theory.md#cofinality-of-an-increasing-ordinal-supremum) give

$$
\operatorname{cf}(\aleph_\beta)=\operatorname{cf}(\beta).
$$

If $\beta<\omega_1$ is a nonzero [limit ordinal](../../../set-theory.md#limit-ordinal), this [cofinality](../../../set-theory.md#cofinality) is $\omega$, so $\aleph_\beta$ is a [singular cardinal](../../../set-theory.md#singular-cardinal). The other infinite [cardinal numbers](../../../set-theory.md#cardinal-number) below $\aleph_{\omega_1}$ are successor-indexed or $\aleph_0$, and are [regular cardinals](../../../set-theory.md#regular-cardinal). For a [successor cardinal](../../../set-theory.md#successor-cardinal) $\mu^+$, a cofinal sequence of length at most $\mu$ would express $\mu^+$ as a union of at most $\mu$ sets of size at most $\mu$, contradicting [infinite cardinal arithmetic](../../../set-theory.md#infinite-cardinal-arithmetic).

There are $\aleph_1$ nonzero countable [limit ordinals](../../../set-theory.md#limit-ordinal), and each countable initial segment contains only countably many. In increasing order they therefore have [order type](../../../set-theory.md#order-type) $\omega_1$. These are precisely the indices of the uncountable [singular cardinals](../../../set-theory.md#singular-cardinal) below $\aleph_{\omega_1}$. Hence every $\sigma_\alpha$ with $\alpha<\omega_1$ has countable [cofinality](../../../set-theory.md#cofinality), and the next one is $\aleph_{\omega_1}$, whose [cofinality](../../../set-theory.md#cofinality) is $\omega_1<\aleph_{\omega_1}$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**Yes.** A [cardinal fixed point of the singular cardinal enumeration](../../../set-theory.md#cardinal-fixed-point-of-the-singular-cardinal-enumeration) is obtained by countable iteration. Start with $\kappa_0=\aleph_0$ and put

$$
\kappa_{n+1}=\sigma_{\kappa_n}.
$$

The [singular cardinal enumeration](../../../set-theory.md#singular-cardinal-enumeration) is strictly increasing and satisfies $\sigma_\alpha\geq\alpha$ for every [ordinal](../../../set-theory.md#ordinal) $\alpha$; the latter follows by [transfinite induction](../../../set-theory.md#transfinite-induction) for any strictly increasing ordinal-valued enumeration. If equality occurs at some $\kappa_n$, that [cardinal number](../../../set-theory.md#cardinal-number) is already a witness. Otherwise the sequence is strictly increasing. Put $\kappa=\sup_{n<\omega}\kappa_n$. This is an uncountable [singular cardinal](../../../set-theory.md#singular-cardinal) of [cofinality](../../../set-theory.md#cofinality) $\omega$.

For every $\alpha<\kappa$, some $n$ has $\alpha<\kappa_n$, and therefore

$$
\sigma_\alpha<\sigma_{\kappa_n}=\kappa_{n+1}<\kappa.
$$

Also $\sup_n\sigma_{\kappa_n}=\kappa$, so $\sup_{\alpha<\kappa}\sigma_\alpha=\kappa$. At a [limit ordinal](../../../set-theory.md#limit-ordinal) index, if the supremum of all preceding enumerated cardinals is itself singular, it is exactly the next member: every smaller singular cardinal already has a preceding index. Thus

$$
\boxed{\sigma_\kappa=\kappa}.
$$

This argument uses continuity only at a singular supremum; the enumeration need not be continuous at a [weakly inaccessible cardinal](../../../set-theory.md#weakly-inaccessible-cardinal).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

It suffices to obtain a [model of ZFC without weakly inaccessible cardinals](../../../set-theory.md#model-of-zfc-without-weakly-inaccessible-cardinals). Starting with any model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), pass to its [constructible universe](../../../definable-power-set.md#constructible-universe), which satisfies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) and the [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis). If it has no [inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal), use that model. Otherwise pass to its rank segment at its least [inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) $\delta$. This segment satisfies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), retains the [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis), and has no [inaccessible cardinals](../../../set-theory.md#strongly-inaccessible-cardinal). Under the [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis), every [weakly inaccessible cardinal](../../../set-theory.md#weakly-inaccessible-cardinal) is strongly inaccessible: if $\lambda<\kappa$ and $\kappa$ is a [limit cardinal](../../../set-theory.md#limit-cardinal), then $2^\lambda=\lambda^+<\kappa$. Thus in either case the resulting model $N$ has no [weakly inaccessible cardinals](../../../set-theory.md#weakly-inaccessible-cardinal).

Work inside $N$. If $\alpha$ is a nonzero [limit ordinal](../../../set-theory.md#limit-ordinal), let $\lambda=\sup_{\beta<\alpha}\sigma_\beta$. It is an uncountable [limit cardinal](../../../set-theory.md#limit-cardinal). If it were regular, it would be a [weakly inaccessible cardinal](../../../set-theory.md#weakly-inaccessible-cardinal), which is impossible in $N$. It is therefore singular, and the [singular cardinal enumeration](../../../set-theory.md#singular-cardinal-enumeration) is continuous at this index:

$$
\sigma_\alpha=\sup_{\beta<\alpha}\sigma_\beta.
$$

The [cofinality of an increasing ordinal supremum](../../../set-theory.md#cofinality-of-an-increasing-ordinal-supremum) now gives

$$
\boxed{\operatorname{cf}(\sigma_\alpha)=\operatorname{cf}(\alpha)}
$$

for every nonzero [limit ordinal](../../../set-theory.md#limit-ordinal) $\alpha$ in $N$. Hence $N$ satisfies the negation of the proposed existential assertion. By the [soundness theorem for first-order logic](../../../mathematical-logic.md#soundness-theorem-for-first-order-logic), consistency of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) prevents [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) from proving that assertion. The model construction is a relative-consistency argument; it does not assume that consistency alone supplies a [countable transitive model](../../../forcing.md#countable-transitive-model). Here, as usual, a [limit ordinal](../../../set-theory.md#limit-ordinal) excludes zero.

## 2

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Freiling axiom of symmetry](../../../set-theory.md#freiling-axiom-of-symmetry) is

$$
\boxed{\forall f:\mathbb R\to[\mathbb R]^{<\omega_1}\quad
\exists x,y\in\mathbb R\quad
x\notin f(y)\ \land\ y\notin f(x).}
$$

The values of $f$ are countable [subsets](../../../set.md#subset) of the [real numbers](../../../arithmetic.md#real-number), including finite ones. One may require $x\ne y$ without changing the axiom: apply the displayed version to $x\mapsto f(x)\cup\{x\}$.

The [Generalized continuum hypothesis](../../../set-theory.md#generalized-continuum-hypothesis) states

$$
\boxed{\forall\text{ infinite cardinals }\kappa,\quad2^\kappa=\kappa^+.}
$$

Here $\kappa^+$ is the [successor cardinal](../../../set-theory.md#successor-cardinal); equivalently $2^{\aleph_\alpha}=\aleph_{\alpha+1}$ for every [ordinal](../../../set-theory.md#ordinal) $\alpha$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Freiling theorem](../../../set-theory.md#freiling-theorem) gives

$$
\boxed{A_{<\omega_1}(\mathbb R)\ \Longleftrightarrow\ \neg\mathrm{CH}}.
$$

First assume the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis) and fix a [well-order](../../../set.md#well-order) $(r_\alpha)_{\alpha<\omega_1}$ of the [real numbers](../../../arithmetic.md#real-number). Define $f(r_\alpha)=\{r_\beta:\beta\leq\alpha\}$. Each value is countable. For any pair, one index is at most the other, so at least one of $x\in f(y)$ or $y\in f(x)$ holds. The same holds for $x=y$, since $x\in f(x)$. This violates the [Freiling axiom of symmetry](../../../set-theory.md#freiling-axiom-of-symmetry).

Conversely, assume $|\mathbb R|>\aleph_1$ and let $f$ assign a countable set to each real. Choose $X\subseteq\mathbb R$ of [cardinality](../../../set-theory.md#cardinality) $\aleph_1$. By [infinite cardinal arithmetic](../../../set-theory.md#infinite-cardinal-arithmetic),

$$
\left|X\cup\bigcup_{x\in X}f(x)\right|\leq\aleph_1<|\mathbb R|.
$$

Choose $y$ outside this union. Since $f(y)$ is countable and $X$ is uncountable, choose $x\in X\setminus f(y)$. Then $y\notin f(x)$ and $x\notin f(y)$, with $x\ne y$. This proves the [Freiling axiom of symmetry](../../../set-theory.md#freiling-axiom-of-symmetry) and completes both implications.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The construction gives a [Lusin set](../../../topological-analysis.md#lusin-set) $\boxed{A=\{x_\alpha:\alpha<\omega_1\}}$ with all $x_\alpha$ distinct.

Every [meagre set](../../../topological-analysis.md#meagre-set) is contained in a meagre $F_\sigma$ set: replace each [nowhere dense set](../../../topological-analysis.md#nowhere-dense-set) in a countable covering by its closure. There are at most $2^{\aleph_0}$ such covers, since each closed subset of $\mathbb R$ is determined by a countable rational basis for its open complement, and a countable sequence of such codes is again coded by a real. Under the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis), enumerate all meagre $F_\sigma$ sets as $(M_\alpha)_{\alpha<\omega_1}$, allowing repetitions.

By [transfinite recursion](../../../set-theory.md#transfinite-recursion), choose

$$
x_\alpha\in\mathbb R\setminus\left(\bigcup_{\beta\leq\alpha}M_\beta\ \cup\ \{x_\beta:\beta<\alpha\}\right).
$$

For each $\alpha<\omega_1$, the excluded union is a [meagre set](../../../topological-analysis.md#meagre-set): it is a countable union of [meagre sets](../../../topological-analysis.md#meagre-set) and singletons. The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) ensures that it does not cover $\mathbb R$, so the choice is possible. The resulting $A$ is uncountable. If $M$ is meagre, choose $\gamma$ with $M\subseteq M_\gamma$. Every $x_\alpha$ with $\alpha\geq\gamma$ avoids $M_\gamma$, hence

$$
A\cap M\subseteq\{x_\alpha:\alpha<\gamma\},
$$

which is countable. Thus $A$ has precisely the [Lusin set](../../../topological-analysis.md#lusin-set) property. Enumerating covers rather than all [meagre sets](../../../topological-analysis.md#meagre-set) avoids an unjustified claim that there are only continuum many arbitrary meagre subsets.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [cardinal bound for an increasing chain of countable sets](../../../set-theory.md#cardinal-bound-for-an-increasing-chain-of-countable-sets) is $\boxed{|X|\leq\aleph_1}$. If $X$ is countable, there is nothing to prove. Otherwise choose $Y\subseteq X$ with $|Y|=\aleph_1$, and for every $y\in Y$ choose an index $i(y)$ such that $y\in X_{i(y)}$.

For any $i\in I$, its countable $X_i$ cannot contain all of $Y$, so choose $y\in Y\setminus X_i$. Since $I$ is a [linear order](../../../algebra.md#linear-order), comparison of $i$ and $i(y)$ forces $i<i(y)$: the other direction would imply $y\in X_i$. Therefore $X_i\subseteq X_{i(y)}$. The selected family is cofinal among the original sets, and

$$
X=\bigcup_{y\in Y}X_{i(y)}.
$$

By [infinite cardinal arithmetic](../../../set-theory.md#infinite-cardinal-arithmetic), this union of $\aleph_1$ countable sets has [cardinality](../../../set-theory.md#cardinality) at most $\aleph_1$. No [well-order](../../../set.md#well-order) or [cofinality](../../../set-theory.md#cofinality) assumption on $I$ was used; a [linear increasing union of countable sets](../../../set-theory.md#increasing-chain-of-countable-sets) has the same bound even for an arbitrary linear index order.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**The continuum hypothesis holds.** Let $A$ be the assumed [Lusin set](../../../topological-analysis.md#lusin-set) of [cardinality](../../../set-theory.md#cardinality) $\mathfrak c=2^{\aleph_0}$. If $\mathfrak c>\aleph_1$, choose $B\subseteq A$ with $|B|=\aleph_1$. The size assumption makes $B$ a [meagre set](../../../topological-analysis.md#meagre-set), but then $A\cap B=B$ is uncountable, contradicting the [Lusin set](../../../topological-analysis.md#lusin-set) property. Thus

$$
\boxed{2^{\aleph_0}=\aleph_1}.
$$

One can also use (d) directly: [well-order](../../../set.md#well-order) $A$ in type $\mathfrak c$. Each proper initial segment has size below $\mathfrak c$, so is meagre and consequently countable, since it is a subset of the [Lusin set](../../../topological-analysis.md#lusin-set). These initial segments form a [linear increasing union of countable sets](../../../set-theory.md#increasing-chain-of-countable-sets) equal to $A$. The bound in (d) gives $\mathfrak c\leq\aleph_1$.

## 3

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix a regular uncountable [cardinal number](../../../set-theory.md#cardinal-number) $\kappa$. A [club set](../../../set-theory.md#club-set) $C\subseteq\kappa$ is unbounded in $\kappa$ and closed under suprema below $\kappa$ of nonempty increasing sequences with no last term. Equivalently, every [limit ordinal](../../../set-theory.md#limit-ordinal) $\delta<\kappa$ with $\sup(C\cap\delta)=\delta$ belongs to $C$. The [club filter](../../../set-theory.md#club-filter) is

$$
\boxed{\mathcal D_\kappa=\{A\subseteq\kappa:\exists C\subseteq A\text{ with }C\text{ club in }\kappa\}}.
$$

It consists of all sets containing a [club set](../../../set-theory.md#club-set), not only the club sets themselves.

An [omega-measurable cardinal](../../../set-theory.md#omega-measurable-cardinal) is a [cardinal number](../../../set-theory.md#cardinal-number) carrying a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) closed under countable intersections, that is, a [countably complete ultrafilter](../../../set-theory.md#countably-complete-ultrafilter). Such a cardinal must be uncountable: on a countable set the intersection of the complements of all singletons would be empty.

A [measurable cardinal](../../../set-theory.md#measurable-cardinal) is an uncountable [cardinal number](../../../set-theory.md#cardinal-number) $\kappa$ carrying a nonprincipal $\kappa$-complete [ultrafilter](../../../set-theory.md#ultrafilter). A [kappa-complete filter](../../../set-theory.md#kappa-complete-filter) is closed under intersections of every family of size strictly below $\kappa$. Thus for an [omega-measurable cardinal](../../../set-theory.md#omega-measurable-cardinal) the completeness required is countable completeness, not merely closure under finitely many intersections.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A uniform example is $\boxed{A=\kappa\setminus\{\omega\}}$. It contains the final segment $[\omega+1,\kappa)$, a [club set](../../../set-theory.md#club-set). Therefore $A$ belongs to the [club filter](../../../set-theory.md#club-filter). Every two [club sets](../../../set-theory.md#club-set) in a regular uncountable cardinal intersect: alternately choose larger points from each and take the countable supremum, which remains below $\kappa$ and lies in both by closure. Hence every member of the [club filter](../../../set-theory.md#club-filter) is a [stationary set](../../../set-theory.md#stationary-set), so $A$ is stationary.

However, every finite [ordinal](../../../set-theory.md#ordinal) belongs to $A$, and their increasing supremum $\omega$ does not. Thus $A$ is not closed and is not a [club set](../../../set-theory.md#club-set). This is a [stationary nonclosed member of the club filter](../../../set-theory.md#stationary-nonclosed-member-of-the-club-filter) for every regular uncountable $\kappa$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [club filter completeness](../../../set-theory.md#club-filter-completeness) argument works for every regular uncountable $\kappa$. Let $\mu<\kappa$ and let $C_i$ be a [club set](../../../set-theory.md#club-set) for each $i<\mu$. Their intersection is closed. To prove it unbounded, start above any prescribed $\beta<\kappa$ and choose an increasing sequence $(\delta_n)_{n<\omega}$ so that $\delta_{n+1}$ lies above a chosen point of every $C_i$ greater than $\delta_n$. $\kappa$ is a [regular cardinal](../../../set-theory.md#regular-cardinal), so the supremum of these $\mu$ choices remains below $\kappa$. The resulting countable supremum $\delta=\sup_n\delta_n$ likewise remains below $\kappa$. For each $i$, the chosen $C_i$ points are cofinal in $\delta$, so closure gives $\delta\in C_i$. Thus the intersection is a [club set](../../../set-theory.md#club-set). Intersecting fewer than $\kappa$ members of the [club filter](../../../set-theory.md#club-filter) still contains such an intersection of clubs. In particular, $\boxed{\mathcal D_{\omega_2}\text{ is }\aleph_2\text{-complete}}$.

It is not an [ultrafilter](../../../set-theory.md#ultrafilter). For a regular infinite $\theta<\kappa$, the set

$$
S_\theta^\kappa=\{\delta<\kappa:\operatorname{cf}(\delta)=\theta\}
$$

is stationary. Given a [club set](../../../set-theory.md#club-set) $C$, build in $C$ a strictly increasing continuous sequence of length $\theta$ and take its supremum $\delta<\kappa$. Closure gives $\delta\in C$, and the [cofinality of an increasing ordinal supremum](../../../set-theory.md#cofinality-of-an-increasing-ordinal-supremum) gives $\operatorname{cf}(\delta)=\theta$. This proves the [stationarity of ordinals of prescribed cofinality](../../../set-theory.md#stationarity-of-ordinals-of-prescribed-cofinality).

At $\kappa=\omega_2$, the disjoint sets $S_\omega^{\omega_2}$ and $S_{\omega_1}^{\omega_2}$ are both stationary. A club contained in either $S_\omega^{\omega_2}$ or its complement would miss one of these stationary sets. Thus neither $S_\omega^{\omega_2}$ nor its complement belongs to $\mathcal D_{\omega_2}$, and

$$
\boxed{\mathcal D_{\omega_2}\text{ is not an ultrafilter}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

**Weakly inaccessible cardinals are unbounded below the given cardinal.** In fact, they form a [stationary set](../../../set-theory.md#stationary-set) there. Let $\kappa$ be the [weakly Mahlo cardinal](../../../set-theory.md#weakly-mahlo-cardinal), so it is a regular uncountable [limit cardinal](../../../set-theory.md#limit-cardinal) and the set $R=\{\alpha<\kappa:\alpha=\operatorname{cf}(\alpha)\}$ is stationary.

The set $C$ of uncountable [limit cardinals](../../../set-theory.md#limit-cardinal) below $\kappa$ is a [club set](../../../set-theory.md#club-set). For unboundedness, above any starting point choose a strictly increasing countable sequence of [cardinal numbers](../../../set-theory.md#cardinal-number) below $\kappa$; its supremum remains below $\kappa$ by regularity and is an uncountable [limit cardinal](../../../set-theory.md#limit-cardinal). For closure, a limit of such limit cardinals is again a [limit cardinal](../../../set-theory.md#limit-cardinal).

Every $\alpha\in R\cap C$ is an uncountable [regular cardinal](../../../set-theory.md#regular-cardinal) and a [limit cardinal](../../../set-theory.md#limit-cardinal), hence a [weakly inaccessible cardinal](../../../set-theory.md#weakly-inaccessible-cardinal). The intersection of a [stationary set](../../../set-theory.md#stationary-set) with a [club set](../../../set-theory.md#club-set) is stationary, because its intersection with any further club is nonempty. Therefore

$$
\boxed{\{\lambda<\kappa:\lambda\text{ is weakly inaccessible}\}\text{ is stationary, hence unbounded}.}
$$

This proves the stronger form of the requested conclusion.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Take the least [omega-measurable cardinal](../../../set-theory.md#omega-measurable-cardinal) $\kappa$, with a [countably complete ultrafilter](../../../set-theory.md#countably-complete-ultrafilter) $U$ on $\kappa$ that is nonprincipal. We prove that $U$ is $\kappa$-complete. This will give $\boxed{\kappa\text{ is measurable}}$.

Suppose $\mu<\kappa$, $A_i\in U$ for $i<\mu$, and $\bigcap_{i<\mu}A_i\notin U$. Then $B=\kappa\setminus\bigcap_{i<\mu}A_i$ belongs to $U$. For $x\in B$ let $g(x)$ be the least $i<\mu$ with $x\notin A_i$. The [pushforward ultrafilter](../../../set-theory.md#pushforward-ultrafilter)

$$
W=\{E\subseteq\mu:g^{-1}[E]\in U\}
$$

is a countably complete [ultrafilter](../../../set-theory.md#ultrafilter) on $\mu$; this uses $B\in U$, so $U$ restricts to an ultrafilter on $B$. For each $i$, the fibre $g^{-1}[\{i\}]$ is contained in $\kappa\setminus A_i$, hence is not in $U$. Thus $W$ is nonprincipal. If $\mu$ is finite or countable, countable completeness already rules this out. Otherwise $|\mu|<\kappa$ would be an [omega-measurable cardinal](../../../set-theory.md#omega-measurable-cardinal), contradicting minimality of $\kappa$.

Therefore every intersection of fewer than $\kappa$ members of $U$ lies in $U$. Since $\kappa$ is uncountable, it is a [measurable cardinal](../../../set-theory.md#measurable-cardinal). This proves that the [least omega-measurable cardinal is measurable](../../../set-theory.md#least-omega-measurable-cardinal-is-measurable), even if the originally supplied cardinal carried only a countably complete ultrafilter.

## 4

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Von Neumann hierarchy](../../../set-theory.md#von-neumann-hierarchy) and the [constructible hierarchy](../../../definable-power-set.md#constructible-hierarchy) are defined by [transfinite recursion](../../../set-theory.md#transfinite-recursion):

$$
\boxed{V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad
V_\lambda=\bigcup_{\alpha<\lambda}V_\alpha},
$$



$$
\boxed{L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\qquad
L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha}.
$$

The union clauses apply to nonzero [limit ordinals](../../../set-theory.md#limit-ordinal). The [definable power set](../../../definable-power-set.md) $\operatorname{Def}(L_\alpha)$ consists of subsets definable over $(L_\alpha,\in)$ by a [first-order formula](../../../mathematical-logic.md#first-order-formula) with finitely many parameters from $L_\alpha$. Definability over that structure is essential; it is not unrestricted definability in the ambient universe. The full [constructible universe](../../../definable-power-set.md#constructible-universe) is $L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha$.

For an infinite [cardinal number](../../../set-theory.md#cardinal-number) $\kappa$, the [hereditarily small set](../../../set-theory.md#hereditarily-small-set) collection is

$$
\boxed{H_\kappa=\{x:|\operatorname{tc}(\{x\})|<\kappa\}},
$$

where $\operatorname{tc}$ is [transitive closure](../../../set-theory.md#transitive-closure). Using $\operatorname{tc}(x)$ instead gives the same size criterion for infinite $\kappa$. This bounds the whole membership ancestry, not just $|x|$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

One can take $\boxed{\alpha=\omega+1}$. Finite induction gives $L_n=V_n$ for every finite $n$: every subset of a finite level is definable using its finitely many elements as parameters. Hence $L_\omega=V_\omega$, the set of [hereditarily finite sets](../../../set-theory.md#hereditarily-finite-set).

Now reason inside the [constructible universe](../../../definable-power-set.md#constructible-universe) $L$, a model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). The set $L_\omega$ is countable there, and there are countably many [first-order formulas](../../../mathematical-logic.md#first-order-formula) and finite parameter tuples. Thus $L_{\omega+1}=\operatorname{Def}(L_\omega)$ is countable in $L$. But the [constructible power set](../../../definable-power-set.md#constructible-power-set) $\mathcal P^L(\omega)$ is uncountable in $L$ by the [Cantor theorem](../../../set.md#cantor-s-theorem). Choose

$$
r\in\mathcal P^L(\omega)\setminus L_{\omega+1}.
$$

This $r$ is constructible and a subset of $\omega$, so $r\subseteq V_\omega$ and $r\in V_{\omega+1}$. Therefore

$$
\boxed{r\in L\cap V_{\omega+1}\setminus L_{\omega+1}}.
$$

All comparisons were made inside $L$; this avoids assuming that the constructible reals are uncountable in the ambient universe. The witness remains valid externally because the two structures use the same $r$, the same $V_\omega$, and the same constructible level. Thus [constructible sets of low rank can appear at later stages](../../../definable-power-set.md#constructible-sets-of-low-rank-can-appear-at-later-stages).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Use the [Lévy hierarchy](../../../set-theory.md#levy-hierarchy), with [bounded formulas in set theory](../../../set-theory.md#bounded-formula-in-set-theory) as the quantifier-free level for this purpose. Let $\operatorname{Ord}(\kappa)$ be the bounded ordinal predicate, and let $\operatorname{Bij}(f,\alpha,\kappa)$ be the bounded predicate saying that $f$ is a graph of a [bijection](../../../function.md#bijection) from $\alpha$ onto $\kappa$. Then cardinalhood is expressed by

$$
\boxed{\operatorname{Ord}(\kappa)\ \land\
\forall f\,\forall\alpha\in\kappa\ \neg\operatorname{Bij}(f,\alpha,\kappa).}
$$

All quantifiers in $\operatorname{Ord}$ and $\operatorname{Bij}$ are bounded by the displayed sets and the graph. Ordered-pair membership, graph functionality, injectivity and surjectivity have bounded expansions using the usual set coding of [ordered pairs](../../../set.md#ordered-pair). The only unbounded quantifier shown is universal over $f$. The formula is therefore $\Pi_1$ and in particular a [Pi-one formula modulo ZF](../../../set-theory.md#pi-one-formula-modulo-zf).

In [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory), a [cardinal number](../../../set-theory.md#cardinal-number) is an [ordinal](../../../set-theory.md#ordinal) not in bijection with any smaller ordinal, so this formula has exactly the required meaning. Thus [cardinalhood is Pi-one definable](../../../set-theory.md#cardinalhood-is-pi-one-definable); the argument does not use the [axiom of choice](../../../set-theory.md#axiom-of-choice).

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Let $\operatorname{Map}(f,\delta,\kappa)$ be the bounded graph predicate for a function $\delta\to\kappa$. For an infinite [cardinal number](../../../set-theory.md#cardinal-number), regularity is expressed by

$$
\boxed{\operatorname{InfCard}(\kappa)\ \land\
\forall f\,\forall\delta\in\kappa\left(
\operatorname{Map}(f,\delta,\kappa)\ \Longrightarrow\
\exists\beta\in\kappa\ \forall\xi\in\delta\ f(\xi)<\beta\right).}
$$

The predicate $\operatorname{InfCard}$ is the cardinal predicate in (i), conjoined with the bounded condition that $\kappa$ is a nonzero [limit ordinal](../../../set-theory.md#limit-ordinal). For an infinite [cardinal number](../../../set-theory.md#cardinal-number), this latter condition holds automatically; it excludes the finite cardinals. The expression $f(\xi)<\beta$ abbreviates bounded graph membership with the output lying in $\beta$.

Every quantifier after $\forall f$ is bounded, and the cardinal predicate is already $\Pi_1$. Their conjunction can be placed in universal form, so this is a [Pi-one formula modulo ZF](../../../set-theory.md#pi-one-formula-modulo-zf). Its mathematical content is that no function from a smaller ordinal is cofinal in $\kappa$. By the definition of [cofinality](../../../set-theory.md#cofinality), that is equivalent to $\operatorname{cf}(\kappa)=\kappa$. Hence [regular cardinalhood is Pi-one definable](../../../set-theory.md#regular-cardinalhood-is-pi-one-definable). This uses the standard convention that a [regular cardinal](../../../set-theory.md#regular-cardinal) is infinite.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

A witness to failure of the [Axiom of power set](../../../set-theory.md#axiom-of-power-set) is $\boxed{\omega_1\in H_{\omega_2}}$. Every subset $A\subseteq\omega_1$ belongs to $H_{\omega_2}$, since its [transitive closure](../../../set-theory.md#transitive-closure) has [cardinality](../../../set-theory.md#cardinality) at most $\aleph_1$. If some $p\in H_{\omega_2}$ were the internal [power set](../../../set.md#power-set) of $\omega_1$, transitivity and bounded subsethood would force $p$ to contain every ambient subset of $\omega_1$, and only those subsets. Thus it would be the full $\mathcal P(\omega_1)$.

By the [Cantor theorem](../../../set.md#cantor-s-theorem),

$$
|p|=2^{\aleph_1}\geq\aleph_2.
$$

Its [transitive closure](../../../set-theory.md#transitive-closure) contains all its members, so $|\operatorname{tc}(\{p\})|\geq|p|\geq\aleph_2$. This contradicts $p\in H_{\omega_2}$. Therefore

$$
\boxed{H_{\omega_2}\not\models\mathrm{PowerSet}}.
$$

The [power-set failure in hereditarily small sets](../../../set-theory.md#power-set-failure-in-hereditarily-small-sets) needs no assumption about the [Continuum hypothesis](../../../set-theory.md#continuum-hypothesis).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Let $T$ be [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) together with the assertion of unboundedly many [inaccessible cardinals](../../../set-theory.md#strongly-inaccessible-cardinal). Given a model of $T$, if it has no [inaccessible limit of inaccessibles](../../../set-theory.md#inaccessible-limit-of-inaccessibles), it already witnesses the required nonimplication. Otherwise let $\iota$ be its least [inaccessible limit of inaccessibles](../../../set-theory.md#inaccessible-limit-of-inaccessibles) and pass to its rank segment $V_\iota$.

Because $\iota$ is an [inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal), $V_\iota$ satisfies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Its [ordinals](../../../set-theory.md#ordinal) are precisely those below $\iota$, and below $\iota$ the inaccessible cardinals are unbounded by the choice of $\iota$. Inaccessibility of any smaller ordinal is absolute to this segment: it has the same subsets and functions on all smaller ordinals, as in [strong-inaccessibility absoluteness from rank agreement](../../../set-theory.md#strong-inaccessibility-absoluteness-from-rank-agreement). Thus $V_\iota$ satisfies the unbounded-inaccessibles assertion.

No smaller ordinal can be an [inaccessible limit of inaccessibles](../../../set-theory.md#inaccessible-limit-of-inaccessibles), by minimality of $\iota$ and the same absoluteness. Also $\iota$ is not an ordinal of $V_\iota$ itself. Consequently

$$
\boxed{V_\iota\models T+\neg\mathrm{ILI}}.
$$

This [rank cutoff at the first inaccessible limit of inaccessibles](../../../set-theory.md#rank-cutoff-at-the-first-inaccessible-limit-of-inaccessibles) proves $\operatorname{Con}(T)\Rightarrow\operatorname{Con}(T+\neg\mathrm{ILI})$. The [soundness theorem for first-order logic](../../../mathematical-logic.md#soundness-theorem-for-first-order-logic) then gives $T\not\vdash\mathrm{ILI}$ if $T$ is consistent. This is a model-theoretic relative-consistency argument, and does not infer external transitivity from mere consistency.

## 5

↑ **Parent:** [Paper 121](paper-121.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use [standard notation for forcing](../../../forcing.md#standard-notation-for-forcing): $q\leq p$ means that $q$ is stronger than $p$. A [closed forcing](../../../forcing.md#closed-forcing) order is $\lambda$-closed when every decreasing sequence $\langle p_\xi:\xi<\delta\rangle$ with $\delta<\lambda$ has a common lower bound:

$$
\boxed{\forall\delta<\lambda\ \forall\text{ decreasing }(p_\xi)_{\xi<\delta}\ \exists q\ \forall\xi<\delta\ (q\leq p_\xi).}
$$

The [chain condition for forcing](../../../forcing.md#chain-condition-for-forcing) is

$$
\boxed{\text{every antichain in }\mathbb P\text{ has cardinality strictly below }\lambda.}
$$

An [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) consists of pairwise [incompatible forcing conditions](../../../forcing.md#incompatible-forcing-conditions); incompatibility means having no common stronger extension. In particular, the $\aleph_1$-chain condition is the [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing). These properties and their sequences or antichains are computed inside the ground model $M$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

**False as printed: separativity alone does not guarantee a new generic filter.** A [separative forcing order](../../../forcing.md#separative-forcing-order) means that if $p\not\leq q$, some $r\leq p$ is incompatible with $q$. The one-point order $\mathbb P=\{p\}$ is separative vacuously. Its only [generic filter](../../../forcing.md#generic-filter) is $\{p\}=\mathbb P$, and this belongs to $M$. Thus no $G\notin M$ exists in this example.

The natural missing hypothesis is that the nonempty order is an [atomless forcing order](../../../forcing.md#atomless-forcing-order). Under that hypothesis the intended argument works. Since $M$ is a [countable transitive model](../../../forcing.md#countable-transitive-model), enumerate externally its dense subsets as $D_0,D_1,\ldots$. Choose $p_{n+1}\leq p_n$ with $p_{n+1}\in D_n$. Then

$$
G=\{q\in\mathbb P:\exists n\ p_n\leq q\}
$$

is a directed upward-closed [filter in an ordered set](../../../set.md#filter-mathematics) and meets every $D_n$. This is the [Rasiowa–Sikorski lemma](../../../forcing.md#rasiowa-sikorski-lemma), giving a [generic filter](../../../forcing.md#generic-filter) over $M$.

If $G\in M$, the [set difference](../../../set.md#set-difference) $D=\mathbb P\setminus G$ would belong to $M$. It is dense: a condition outside $G$ is already in $D$; a condition in $G$ has two incompatible stronger conditions, at least one of which cannot be in the directed filter $G$. Genericity would require $G\cap D\ne\varnothing$, a contradiction. Thus

$$
\boxed{\text{with atomlessness, a generic }G\text{ exists and }G\notin M.}
$$

This uses [generic filter for an atomless order is new](../../../forcing.md#generic-filter-for-an-atomless-order-is-new). A [forcing atom](../../../forcing.md#forcing-atom) is precisely the obstruction illustrated by the counterexample; separativity does not remove it.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

With the condition-first name convention used here, [evaluation of a forcing name](../../../forcing.md#evaluation-of-a-forcing-name) is

$$
\eta_G=\{\sigma_G:\exists p\in G\ ((p,\sigma)\in\eta)\}.
$$

Since a [generic filter](../../../forcing.md#generic-filter) is nonempty, there is a condition in $G$. In the given [paired forcing name](../../../forcing.md#paired-forcing-name), every condition is paired with both $\tau$ and $\tau'$, and there are no other lower-rank names. Therefore

$$
\boxed{\nu(\tau,\tau')_G=\{\tau_G,\tau'_G\}}.
$$

This is the **unordered pair** of the two interpreted sets. If the interpretations coincide, it is a singleton. It is neither an [ordered pair](../../../set.md#ordered-pair) nor the [set union](../../../set.md#set-union) of those interpretations. Reversing the two components in the name-pair convention changes only the syntax of the same recursive evaluation.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

**Closure preserves the ground-model cardinal $\lambda$.** We use the stronger fact that [closed forcing adds no short ordinal sequences](../../../forcing.md#closed-forcing-adds-no-short-ordinal-sequences). Fix an ordinal $\mu<\lambda$ in $M$ and a [forcing name](../../../forcing.md#forcing-name) $\dot h$ that a condition $p$ forces to be an ordinal-valued function with domain $\mu$.

Inside $M$, recursively strengthen $p$ to decide each value $\dot h(\xi)$, for $\xi<\mu$. At a limit stage take a lower bound of the previously chosen descending sequence; its length is below $\lambda$, so $\lambda$-closure supplies one. After all $\mu$ values have been decided, closure supplies a common lower bound $q$. The decided values form a function $h\in M$ by the [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement), and

$$
q\Vdash\dot h=\check h.
$$

The recursion is carried out within $M$ using the definable [forcing theorem](../../../forcing.md#forcing-theorem) and a ground-model choice of deciding extensions, so every sequence to which closure is applied belongs to $M$. Repeating the construction below any stronger condition shows that such full-decision conditions are [dense below a forcing condition](../../../forcing.md#dense-below-a-forcing-condition) $p$. The [dense-below generic meeting lemma](../../../forcing.md#dense-below-generic-meeting-lemma) ensures that a [generic filter](../../../forcing.md#generic-filter) containing $p$ meets them. Thus the interpreted function is in $M$.

If $\lambda$ ceased to be a [cardinal number](../../../set-theory.md#cardinal-number) in $M[G]$, there would be a surjection $\mu\to\lambda$ for some ordinal $\mu<\lambda$. The [forcing theorem](../../../forcing.md#forcing-theorem) gives a name and a condition in $G$ forcing this. The argument above makes its interpretation a ground-model function, but $M$ regards $\lambda$ as a [cardinal number](../../../set-theory.md#cardinal-number) and admits no such surjection. Therefore

$$
\boxed{M[G]\models\text{“}\lambda\text{ is a cardinal”}}.
$$

No regularity of $\lambda$ is required; every recursion used has length strictly below $\lambda$. Finite cardinals are preserved automatically. This is [cardinal preservation by closed forcing](../../../forcing.md#cardinal-preservation-by-closed-forcing).

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/i">i</h4>

↑ **Parent:** [E](#5/e)

<h5 id="5/e/i/solution">Solution</h5>

↑ **Parent:** [I](#5/e/i)

The [Fn forcing](../../../forcing.md#fn-forcing) here is $\operatorname{Fn}(\alpha_2\times\omega,2,\omega)$; larger partial functions are stronger conditions. This translates the inclusion description into [standard notation for forcing](../../../forcing.md#standard-notation-for-forcing) as $q\leq p$ when $q\supseteq p$. Compatible members of the [generic filter](../../../forcing.md#generic-filter) agree wherever both are defined, so

$$
F=\bigcup G
$$

is a function. For every $(\xi,n)\in\alpha_2\times\omega$, the conditions whose domains contain that coordinate form a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order). This requirement belongs to $M$, and the [generic filter](../../../forcing.md#generic-filter) meets it. Consequently $F:\alpha_2\times\omega\to2$ is total.

Define the [generic coordinate reals for finite-function forcing](../../../forcing.md#generic-coordinate-reals-for-finite-function-forcing) by

$$
a_\xi=\{n<\omega:F(\xi,n)=1\}.
$$

For distinct $\xi,\eta<\alpha_2$, the conditions assigning opposite bits to those rows at some column form a [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order). Given any finite condition, choose a column absent from both rows and extend by assigning zero to one coordinate and one to the other. Genericity supplies such a condition in $G$, so $a_\xi\ne a_\eta$.

The function $\xi\mapsto a_\xi$ is formed inside $M[G]$ by separation and replacement from $F$. Hence

$$
\boxed{M[G]\models\text{“}\xi\mapsto a_\xi\text{ is an injection }\alpha_2\to\mathcal P(\omega)\text{”}}.
$$

This constructs an [injective function](../../../algebra.md#injective-function) on the ground-model ordinal $\alpha_2$; preservation of its cardinal status is a separate issue.

<h4 id="5/e/ii">ii</h4>

↑ **Parent:** [E](#5/e)

<h5 id="5/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/e/ii)

Inside $M$, the finite-function order has the [countable chain condition for finite-function forcing](../../../forcing.md#countable-chain-condition-for-finite-function-forcing). In an uncountable family of binary conditions there are uncountably many distinct finite domains, since each domain supports only finitely many conditions. These domains would have an uncountable [Delta-system](../../../set-theory.md#delta-system) subfamily by the [Delta-system lemma](../../../set-theory.md#delta-system-lemma). There are only finitely many assignments to the common finite root, so thin further to an uncountable family agreeing there. Any two such conditions have a union that is again a function and is a common stronger extension. Thus no uncountable [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) exists.

Here is the relevant preservation argument, rather than an appeal to the condition alone. Fix $p\in G$ forcing that a [forcing name](../../../forcing.md#forcing-name) $\dot h$ is a function $\omega\to\alpha_1$. For each $n$, choose inside $M$ a maximal [antichain in a forcing order](../../../forcing.md#antichain-in-a-forcing-order) below $p$ deciding $\dot h(n)$. By the [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing), this antichain is countable in $M$, so the possible values form a countable $B_n\subseteq\alpha_1$. The union $B=\bigcup_nB_n$ is countable in $M$, hence bounded below its regular $\omega_1=\alpha_1$. The interpreted $h$ has range contained in $B$, by maximality and the [dense-below generic meeting lemma](../../../forcing.md#dense-below-generic-meeting-lemma). It therefore cannot be a surjection onto $\alpha_1$.

If $\alpha_1$ were not a [cardinal number](../../../set-theory.md#cardinal-number) in $M[G]$, it would be equinumerous with a smaller ordinal, which was countable already in $M$; composing with that ground-model enumeration would give a surjection $\omega\to\alpha_1$. This is impossible. Therefore

$$
\boxed{M[G]\models\text{“}\alpha_1\text{ is a cardinal”}}.
$$

This is the [possible-values lemma for chain-condition forcing](../../../forcing.md#possible-values-lemma-for-chain-condition-forcing) specialized to $\omega_1$. Countability and regularity in this proof are computed inside $M$, not inferred from the external countability of $M$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
