<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $X=[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../../../space-of-infinite-subsets-of-the-natural-numbers.md), and $[M]^\omega$ for all infinite subsets of an infinite $M$. A family $Y\subseteq X$ is a [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md) if for every infinite $M$ there is an infinite $L\subseteq M$ with either $[L]^\omega\subseteq Y$ or $[L]^\omega\cap Y=\varnothing$.

A non-[Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md) is obtained by [finite-symmetric-difference parity colouring](../../../../../finite-symmetric-difference-parity-colouring.md). Declare $A\sim B$ when their [symmetric difference](../../../../../symmetric-difference.md) is finite, and use the [axiom of choice](../../../../../axiom-of-choice.md) to select a representative $R$ for each [equivalence class](../../../../../equivalence-class.md). Put

$$
\varepsilon(A)=|A\mathbin{\triangle}R|\pmod2,\qquad Y=\{A\in X:\varepsilon(A)=0\}.
$$

For every infinite $L$, both $L$ and $L\setminus\{\min L\}$ belong to $[L]^\omega$ and have the same representative. Toggling one element changes the parity of the finite [symmetric difference](../../../../../symmetric-difference.md), so these two sets have opposite colors. Thus no $[L]^\omega$ is homogeneous, and **$Y$ is not a [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md)**. Only finite differences are counted; no parity is being assigned to an infinite cardinal.

We use the [Ellentuck topology](../../../../../ellentuck-topology.md) for the star notation. Its basic neighborhoods are

$$
[s,A]=\{s\cup B:B\in[A]^\omega\},
$$

where $s$ is a finite stem (the [initial segment](../../../../../initial-segment.md) of each member of the neighborhood) and every element of the infinite reservoir $A$ exceeds $\max s$; the empty stem is allowed. A star-[nowhere dense set](../../../../../nowhere-dense-set.md) $N$ has star-[closure](../../../../../closure-topology.md) with empty star-[interior](../../../../../interior-topology.md); a star-[meagre set](../../../../../meagre-set.md) is a [countable](../../../../../countable-set.md) union of star-[nowhere dense sets](../../../../../nowhere-dense-set.md).

We need the following stem-preserving open-set conclusion: a star-[open set](../../../../../open-set.md) $G$ has, in every $[s,A]$, an infinite $B\subseteq A$ such that $[s,B]\subseteq G$ or $[s,B]\cap G=\varnothing$. Here is the [fusion proof for open Ellentuck sets](../../../../../fusion-proof-for-open-ellentuck-sets.md), so that the precise form being used is explicit. A reservoir $T$ accepts a finite extension $t$ of $s$ when $[t,T]\subseteq G$, and rejects it when no infinite subreservoir accepts it. Every reservoir can be thinned to decide a prescribed stem: take an accepting subreservoir if one exists, and otherwise it already rejects. Acceptance and rejection are hereditary under further infinite thinning.

First thin $A$ to decide $s$. If it accepts, we have finished. Otherwise, choose successive points $b_0<b_1<\cdots$, thinning the unused tail after each selection to decide every stem $s\cup t$ with $t$ a subset of the finitely many points already selected. Each stage requires only finitely many decisions. The final set $B$ therefore decides every such finite extension, using the tail above its largest point. It rejects $s$.

For any rejected stem $s\cup t$, only finitely many possible next points $b$ of $B$ have accepting tails for $s\cup t\cup\{b\}$. Otherwise collect infinitely many such points into $C$. Every member of $[s\cup t,C]$ starts with some such $b$, and its remaining points lie in the accepting tail above $b$. Hence $[s\cup t,C]\subseteq G$, contradicting rejection. A second selection now gives $C\subseteq B$ all of whose finite extensions of $s$ are rejected: at each stage avoid the finitely many forbidden next points for each subset of the chosen prefix. Previous rejections persist on thinning. If $Z\in[s,C]\cap G$, star-openness gives an initial stem $s\cup t$ of $Z$ and an infinite tail of $Z$ whose entire neighborhood lies in $G$. This is an accepting subreservoir for a stem we made rejected, a contradiction. Thus $[s,C]\cap G=\varnothing$, proving the needed open-set conclusion.

Apply this conclusion to $G=X\setminus\overline N^{\,*}$ when $N$ is star-[nowhere dense](../../../../../nowhere-dense-set.md). This $G$ is star-[open](../../../../../open-set.md) and star-[dense](../../../../../dense-set.md). The alternative $[s,B]\cap G=\varnothing$ would give a nonempty star-[open set](../../../../../open-set.md) inside $\overline N^{\,*}$, contradicting empty [interior](../../../../../interior-topology.md). Consequently **every star-[nowhere dense set](../../../../../nowhere-dense-set.md) can be avoided without extending the finite stem**.

Now let $N=\bigcup_{j\geq0}N_j$, each $N_j$ star-[nowhere dense](../../../../../nowhere-dense-set.md), and fix $[s,A]$. Construct $b_0<b_1<\cdots$ with nested infinite unused reservoirs. At stage $j$, let $P_j=\{b_0,\ldots,b_{j-1}\}$. For every $t\subseteq P_j$, in turn, thin the current reservoir using the preceding avoidance property until

$$
[s\cup t,C_j]\cap N_j=\varnothing\qquad(t\subseteq P_j).
$$

There are only finitely many such $t$, and subsequent thinning preserves all previous avoidances. Choose $b_j=\min C_j$ and retain the part of $C_j$ above $b_j$ for the next stage. Put $B=\{b_j:j\geq0\}$. For any $Z\in[s,B]$ and any $j$, the finite part $t=(Z\setminus s)\cap P_j$ is one of the stems tested at stage $j$, and the rest of $Z\setminus(s\cup t)$ lies in $C_j$. Hence $Z\in[s\cup t,C_j]$ and $Z\notin N_j$. This proves $[s,B]\cap N=\varnothing$.

The final $[s,B]$ is star-[open](../../../../../open-set.md) and disjoint from $N$, so it is also disjoint from the star-[closure](../../../../../closure-topology.md) of $N$. Every basic neighborhood therefore has a nonempty open refinement missing that closure. This [Ellentuck meagre-set fusion lemma](../../../../../ellentuck-meagre-set-fusion-lemma.md) proves

$$
\boxed{\text{star-meagre}\ \Longrightarrow\ \text{star-nowhere dense}.}
$$

Indeed, we obtained the stronger [completely Ramsey-null](../../../../../completely-ramsey-null-set.md) property. Testing all subsets of the selected prefix was essential; testing just the entire prefix would not cover every infinite subset of $B$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
