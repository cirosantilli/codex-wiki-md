<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The two Ramsey properties and the topologies.** Write $[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../../../../space-of-infinite-subsets-of-the-natural-numbers.md), and $[A]^\omega$ for the infinite subsets of $A$. The [positive integers](../../../../../../positive-integer.md) are used throughout. A [Ramsey set of infinite subsets](../../../../../../ramsey-set-of-infinite-subsets.md) $E$ has the property that every infinite $A$ contains an infinite $B$ for which $[B]^\omega$ lies wholly in $E$ or wholly in $E^c$.

For finite $s$ and infinite $A$ above $\max s$, let

$$
[s,A]=\{s\cup B:B\in[A]^\omega\},\qquad\max\varnothing=0.
$$

These are the basic [neighbourhoods](../../../../../../neighbourhood-mathematics.md) of the [Ellentuck topology](../../../../../../ellentuck-topology.md), denoted $*$ in the question. They form a basis: if $X$ belongs to two such sets, their stems are comparable [initial segments](../../../../../../initial-segment.md) of $X$; take the longer stem and the intersection of the two tails beyond that stem. This intersection contains the infinite remaining tail of $X$ and yields a basic set contained in both.

A [completely Ramsey set](../../../../../../completely-ramsey-set.md) $E$ allows such a homogeneous refinement $[s,B]$ inside every $[s,A]$, with $B\subseteq A$ infinite and the stem $s$ kept fixed. Taking $s=\varnothing$ shows that complete Ramseyness implies Ramseyness. The [ordinary topology on infinite subsets](../../../../../../ordinary-topology-on-infinite-subsets.md) $\tau$ has basic cylinders

$$
[s]=\{X:s\text{ is an initial segment of }X\}
=[s,\{n:n>\max s\}].
$$

It is the usual [product topology](../../../../../../product-topology.md) on increasing enumerations and is coarser than the [Ellentuck topology](../../../../../../ellentuck-topology.md).

**Examples distinguishing the properties.** A non-Ramsey example uses the [axiom of choice](../../../../../../axiom-of-choice.md). Let $\kappa=2^{\aleph_0}$ and enumerate all infinite sets as $(A_\alpha)_{\alpha<\kappa}$. Each $[A_\alpha]^\omega$ has [cardinality](../../../../../../cardinality.md) $\kappa$: an enumeration of $A_\alpha$ gives the upper bound, and choosing one element from each of infinitely many disjoint pairs gives an injection from all binary sequences for the lower bound.

By [transfinite recursion](../../../../../../transfinite-recursion.md), choose two distinct, previously unused elements $X_\alpha,Y_\alpha\in[A_\alpha]^\omega$ at each stage. Fewer than $\kappa$ elements have been used at stage $\alpha<\kappa$, so this is possible without any assumption on the [Continuum hypothesis](../../../../../../continuum-hypothesis.md). Put $R=\{X_\alpha:\alpha<\kappa\}$. All the $Y_\alpha$ remain outside $R$, since subsequent choices also avoid previously chosen elements. Every $[A]^\omega$ contains one $X_\alpha$ and one $Y_\alpha$, so $R$ is not a [Ramsey set of infinite subsets](../../../../../../ramsey-set-of-infinite-subsets.md). This is the [non-Ramsey set from transfinite selection](../../../../../../non-ramsey-set-from-transfinite-selection.md) construction.

Perform the same construction on $T=\mathbb N\setminus\{1\}$, giving a non-Ramsey set $R_T\subseteq[T]^\omega$, and put

$$
E=\{\{1\}\cup X:X\in R_T\}.
$$

For any infinite $A$, the infinite set $B=A\setminus\{1\}$ has $[B]^\omega\cap E=\varnothing$, so $E$ is a [Ramsey set of infinite subsets](../../../../../../ramsey-set-of-infinite-subsets.md). But no $[\{1\},B]$ with infinite $B\subseteq T$ is homogeneous, because $[B]^\omega$ meets both $R_T$ and its complement. Therefore $E$ is not a [completely Ramsey set](../../../../../../completely-ramsey-set.md).

**Every star-open set is completely Ramsey.** We give the full [fusion proof for open Ellentuck sets](../../../../../../fusion-proof-for-open-ellentuck-sets.md), without quoting an infinite Ramsey theorem. Fix a star-[open set](../../../../../../open-set.md) $O$ and a basic set $[s,A]$. For finite $a\subseteq A$ and an infinite tail $D\subseteq A$ above $\max a$, say $D$ accepts $a$ if $[s\cup a,D]\subseteq O$; it rejects $a$ if no infinite subset of $D$ accepts $a$. Both properties persist under passing to infinite subsets. Every infinite tail can be thinned to decide $a$: take an accepting subset if one exists, and otherwise the original tail rejects it.

First thin $A$ to decide $a=\varnothing$. If it accepts, the required homogeneous neighborhood has already been found. Otherwise keep a rejecting tail. We now fuse to an infinite set $B$ deciding every finite $a\subseteq B$, where the decision for $a$ is made by $B/a=\{b\in B:b>\max a\}$.

To do this, choose $b_1<b_2<\cdots$ successively from an infinite current tail. After choosing $b_j$, thin the tail above $b_j$ to decide each of the finitely many subsets of $\{b_1,\ldots,b_j\}$, one after another, before choosing the next element. For any finite $a\subseteq B$, at the stage when its largest element is selected, the current tail decides $a$ and contains every later selected element. Heredity therefore gives a decision on $B/a$. For $a=\varnothing$, rejection persists from the initial tail.

If $B/a$ rejects $a$, only finitely many $n\in B/a$ can have $B/n$ accepting $a\cup\{n\}$. Otherwise let $D$ be the infinite set of those $n$. Every member of $[s\cup a,D]$ has a first new element $n$, and its remaining tail lies in $B/n$. It therefore belongs to $O$ by acceptance of $a\cup\{n\}$. This would make $D$ accept $a$, contradicting rejection.

Thin $B$ a second time to $C=\{c_1<c_2<\cdots\}$ so that every finite $a\subseteq C$ is rejected. Start with the rejected empty set. At a finite stage, all subsets of the selected elements are rejected. For each of these finitely many subsets, avoid its finitely many next elements that would give an accepted extension, and choose the next $c_j$ beyond all excluded elements. Since $B$ decides every finite extension, each new extension is rejected. Induction gives the asserted property of $C$.

We claim $[s,C]\cap O=\varnothing$. If $X\in[s,C]\cap O$, openness provides a basic set $[t,D]\subseteq O$ containing $X$. Extend $t$, if necessary, to an [initial segment](../../../../../../initial-segment.md) $u$ of $X$ containing $s$. Write $u=s\cup a$ with finite $a\subseteq C$. The infinite tail $X\setminus u$ lies in $B/a$ and

$$
[s\cup a,X\setminus u]\subseteq[t,D]\subseteq O.
$$

It is therefore an accepting subtail for $a$, contradicting rejection. We have found either an accepting neighborhood or a neighborhood disjoint from $O$. Thus

$$
\boxed{O\text{ star-open }\Longrightarrow O\text{ completely Ramsey}.}
$$

**Basic neighborhoods are clopen.** Consider $[s,A]$ and a point $X$ outside it. If $s$ is not an [initial segment](../../../../../../initial-segment.md) of $X$, take an [initial segment](../../../../../../initial-segment.md) $t$ of $X$ of length at least $|s|$; its ordinary cylinder $[t]$ cannot meet $[s,A]$. Otherwise some element of $X\setminus s$ is outside $A$; take $t$ through that element, and again $[t]$ is disjoint from $[s,A]$.

Thus the complement of $[s,A]$ is already [open](../../../../../../open-set.md) in the [ordinary topology on infinite subsets](../../../../../../ordinary-topology-on-infinite-subsets.md), and hence in the finer [Ellentuck topology](../../../../../../ellentuck-topology.md). A basic [neighbourhood](../../../../../../neighbourhood-mathematics.md) is [open](../../../../../../open-set.md) by definition, so

$$
\boxed{[s,A]\text{ is star-clopen, and is also }\tau\text{-closed}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
