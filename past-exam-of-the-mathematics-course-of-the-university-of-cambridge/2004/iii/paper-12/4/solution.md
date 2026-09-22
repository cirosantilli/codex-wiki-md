<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../../../space-of-infinite-subsets-of-the-natural-numbers.md), with each [subset](../../../../../subset.md) identified with its increasing enumeration. In the homogeneous-cone convention, a family $\mathcal A\subseteq[\mathbb N]^\omega$ is a [Ramsey family in the homogeneous-cone sense](../../../../../ramsey-family-in-the-homogeneous-cone-sense.md) when some infinite $M$ satisfies

$$
[M]^\omega\subseteq\mathcal A\quad\text{or}\quad[M]^\omega\cap\mathcal A=\varnothing.
$$

The stronger [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md) convention asks for such an infinite $M\subseteq A$ inside every given infinite ground set $A$. We will prove the open-set assertion in this stronger form, and our Ramsey-but-not-completely-Ramsey example will satisfy it as well. Thus the distinction in conventions does not affect any of the conclusions below.

For a non-Ramsey example, declare $X\sim Y$ if their [symmetric difference](../../../../../symmetric-difference.md) is finite, and choose a representative $R$ from each [equivalence class](../../../../../equivalence-class.md) using the [axiom of choice](../../../../../axiom-of-choice.md). Set

$$
\varepsilon(X)=|X\triangle R|\pmod2
$$

for the representative of the class of $X$. Removing one point reverses this colour, because its [symmetric difference](../../../../../symmetric-difference.md) with $R$ changes by exactly one point. Consequently every cone $[M]^\omega$ contains the oppositely coloured sets $M$ and $M\setminus\{\min M\}$. Either colour class of this [finite-symmetric-difference parity colouring](../../../../../finite-symmetric-difference-parity-colouring.md) is not a [Ramsey family in the homogeneous-cone sense](../../../../../ramsey-family-in-the-homogeneous-cone-sense.md). No definability is claimed for the representative selection.

The [ordinary topology on infinite subsets](../../../../../ordinary-topology-on-infinite-subsets.md), denoted $\tau$, has basic cylinders $[s]=\{X:s\sqsubset X\}$, where $s$ is a [finite stem](../../../../../finite-stem-of-an-infinite-subset.md) of the increasing enumeration. Let $O$ be a $\tau$-open family and fix an arbitrary infinite ground set $A$. We give a complete fusion proof of a homogeneous cone inside $A$.

Use the convention $\max\varnothing=0$. For finite $s$ and an infinite reservoir $B$ above $\max s$, say that $B$ accepts $s$ if $[s,B]\subseteq O$, where

$$
[s,B]=\{s\cup X:X\in[B]^\omega\}.
$$

Say that $B$ rejects $s$ if no infinite [subset](../../../../../subset.md) of $B$ accepts $s$. There is always a refinement deciding $s$: choose an accepting subreservoir if one exists, and otherwise retain $B$, which rejects. Both decisions persist under further thinning.

A first fusion produces an infinite $H\subseteq A$ deciding every finite $s\subseteq H$ on its tail $H/s=\{h\in H:h>\max s\}$. First decide the empty stem. Choose the first point, and thin the remaining reservoir successively to decide every [subset](../../../../../subset.md) of the selected prefix. Repeat after choosing each new point. There are finitely many [subsets](../../../../../subset.md) to decide at each stage. The diagonal sequence of chosen points has the required property, since its tail after the largest point of any stem lies in the reservoir where that stem was decided. The empty-stem decision persists too. This is [deciding all finite stems by fusion](../../../../../deciding-all-finite-stems-by-fusion.md).

If $H$ accepts the empty stem, $[H]^\omega\subseteq O$ and we are done. Suppose it rejects. For a rejected finite $s\subseteq H$, only finitely many $h\in H/s$ can have $H/h$ accepting $s\cup\{h\}$. Otherwise let $D$ be their [infinite set](../../../../../infinite-set.md). Every infinite $X\subseteq D$ starts with some such $h$, and its remaining tail lies in $H/h$, so $s\cup X\in O$. Then $D$ accepts $s$, contradicting rejection. This proves [finitely many accepting extensions of a rejected stem](../../../../../finitely-many-accepting-extensions-of-a-rejected-stem.md).

A second fusion constructs $K\subseteq H$ whose every finite [subset](../../../../../subset.md) is rejected. If a finite prefix of chosen points has been selected, all its [subsets](../../../../../subset.md) are rejected by induction. Avoid the [union](../../../../../set-union.md) of their finitely many accepting successor sets when choosing the next point. The first fusion already decides every successor, so every new [subset](../../../../../subset.md) is rejected. An infinite reservoir remains after each finite exclusion.

If some $X\in[K]^\omega$ belonged to $O$, openness would give an [initial segment](../../../../../initial-segment.md) $s\sqsubset X$ with $[s]\subseteq O$. Its reservoir $H/s$ would then accept $s$, contradicting the second fusion. Therefore $[K]^\omega\cap O=\varnothing$. In either case we have a homogeneous cone inside the arbitrary ground set $A$. **Every $\tau$-open family is a [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md)**, under both conventions.

A [completely Ramsey set](../../../../../completely-ramsey-set.md) requires more: for every finite $s$ and infinite reservoir $A$ above $\max s$, there is an infinite $B\subseteq A$ such that

$$
[s,B]\subseteq\mathcal A\quad\text{or}\quad[s,B]\cap\mathcal A=\varnothing.
$$

The [finite stem](../../../../../finite-stem-of-an-infinite-subset.md) must be kept fixed. These $[s,A]$ are the basic [neighbourhoods](../../../../../neighbourhood-mathematics.md) of the [Ellentuck topology](../../../../../ellentuck-topology.md), also called the [star topology](../../../../../ellentuck-topology.md).

Let $E$ be the even [positive integers](../../../../../positive-integer.md), and construct the [finite-symmetric-difference parity colouring](../../../../../finite-symmetric-difference-parity-colouring.md) $\varepsilon$ on $[E]^\omega$. Define

$$
\mathcal R=\{\{1\}\cup X:X\in[E]^\omega,\ \varepsilon(X)=0\}.
$$

For any infinite ground set $A$, the set $A\setminus\{1\}$ is still infinite and its whole cone misses $\mathcal R$. Thus $\mathcal R$ is a [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md) even in the stronger convention. But inside $[\{1\},E]$, every infinite refinement $B\subseteq E$ gives the two sets $\{1\}\cup B$ and $\{1\}\cup(B\setminus\{\min B\})$ of opposite colours. Hence no such refinement is homogeneous. **The family $\mathcal R$ is Ramsey but not [completely Ramsey](../../../../../completely-ramsey-set.md).** The [stem-supported Ramsey family need not be completely Ramsey](../../../../../stem-supported-ramsey-family-need-not-be-completely-ramsey.md) construction explains this example: forgetting the stem $\{1\}$ is precisely what loses the obstruction.

Finally take $D=[E]^\omega$. It is nonempty and star-open, since it equals $[\varnothing,E]$. It is $\tau$-closed: if an [infinite set](../../../../../infinite-set.md) contains an odd [integer](../../../../../integer.md), an [initial segment](../../../../../initial-segment.md) witnessing that [integer](../../../../../integer.md) has a cylinder disjoint from $D$. Its $\tau$-interior is empty: after any [finite stem](../../../../../finite-stem-of-an-infinite-subset.md) of even [integers](../../../../../integer.md), append an arbitrarily large odd [integer](../../../../../integer.md) and then infinitely many further points. Thus

$$
\boxed{D\text{ is nonempty and star-open, but }\tau\text{-nowhere dense}.}
$$

This is the [cone on an infinite coinfinite ground set](../../../../../cone-on-an-infinite-coinfinite-ground-set.md). Choose its [subset](../../../../../subset.md) $Y=\{X\in[E]^\omega:\varepsilon(X)=0\}$. Since $\overline Y^{\,\tau}\subseteq D$, $Y$ is also $\tau$-nowhere dense. Nevertheless every $[\varnothing,B]$ with infinite $B\subseteq E$ contains both $B$ and $B\setminus\{\min B\}$, of opposite colours. Hence $Y$ is not [completely Ramsey](../../../../../completely-ramsey-set.md). We have proved explicitly that [ordinarily nowhere-dense sets need not be completely Ramsey](../../../../../ordinarily-nowhere-dense-sets-need-not-be-completely-ramsey.md); the [topology](../../../../../topology-split.md) in the nowhere-dense hypothesis cannot be silently changed to the [star topology](../../../../../ellentuck-topology.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
