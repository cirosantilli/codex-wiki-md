<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $[M]^\omega$ for the infinite subsets of an infinite $M\subseteq\mathbb N$. A [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md) $Y\subseteq[\mathbb N]^\omega$ has an infinite homogeneous set $M$: either $[M]^\omega\subseteq Y$ or $[M]^\omega\cap Y=\varnothing$. The proof below actually supplies homogeneous refinements within every infinite reservoir, and with any fixed initial finite stem; this stronger property is that of a [completely Ramsey set](../../../../../completely-ramsey-set.md).

For a non-Ramsey example, identify two infinite sets when their [symmetric difference](../../../../../symmetric-difference.md) is finite, and choose one representative $R$ for each equivalence class. Define a two-colouring by

$$
\varepsilon(A)=|A\mathbin\triangle R|\pmod2,
$$

where $R$ is the representative of $A$'s class. Removing one point changes this parity. Thus, for every infinite $M$, the two subsets $M$ and $M\setminus\{\min M\}$ have opposite colours. The zero-colour family meets every $[M]^\omega$ and so does its complement. Hence **the zero-colour family is not Ramsey**. This [finite-symmetric-difference parity colouring](../../../../../finite-symmetric-difference-parity-colouring.md) uses a choice of representatives; no definability or regularity is being claimed for that first example.

To prove the open-set assertion, for a finite increasing set $s$ and an infinite tail $A$ above $\max s$ define

$$
[s,A]=\{s\cup B:B\in[A]^\omega\}.
$$

The [star topology](../../../../../ellentuck-topology.md), or [Ellentuck topology](../../../../../ellentuck-topology.md), has these sets as basic open sets. For an empty stem there is no lower-bound restriction. More generally $[s,A]$ always uses only the points of $A$ above $\max s$. The [ordinary topology on infinite subsets](../../../../../ordinary-topology-on-infinite-subsets.md), denoted $\tau$, has cylinders $[s]=\{B:s\text{ is an initial segment of }B\}$ as a basis. The two topologies must not be confused.

Fix any family $Y$, initially without any openness assumption. An infinite $A$ accepts a stem $s$ if $[s,A]\subseteq Y$, and rejects it if no infinite subset of its tail accepts $s$. Every infinite reservoir has an infinite refinement deciding $s$: take an accepting refinement if one exists, and otherwise the reservoir itself rejects. Acceptance and rejection are both inherited by infinite refinements. These facts follow from the definitions, giving [acceptance and rejection of finite stems](../../../../../acceptance-and-rejection-of-finite-stems.md).

First refine the initial reservoir to decide the empty stem. If it accepts, its infinite subsets already lie in $Y$. Otherwise start from an infinite reservoir rejecting the empty stem. Choose an increasing point $a_1$, then thin its remaining tail finitely many times to decide all subsets of $\{a_1\}$. Having chosen $a_1,\ldots,a_n$, choose $a_{n+1}$ from the current tail and refine the remaining tail to decide all subsets of $\{a_1,\ldots,a_{n+1}\}$. Each stage has only finitely many stems to handle. Let $L=\{a_1,a_2,\ldots\}$.

For every finite $s\subset L$, at the stage of its largest point the reservoir was made to decide $s$, and all later chosen points remain inside that reservoir. Heredity therefore makes the tail of $L$ decide $s$. Moreover $L$ still rejects the empty stem. This proves [deciding all finite stems by fusion](../../../../../deciding-all-finite-stems-by-fusion.md) without assuming a separate fusion theorem.

Suppose $L$ rejects a finite $s\subset L$. There are only finitely many $a\in L$ above $\max s$ for which $L$'s tail above $a$ accepts $s\cup\{a\}$. For if there were infinitely many, collect them into $C$. Every infinite $B\subset C$ has least point $a$ of this kind, and its remaining tail lies in the accepting tail of $L$. Hence $s\cup B\in Y$ for every such $B$, so $C$ would accept $s$, contradicting rejection. This proves [finitely many accepting extensions of a rejected stem](../../../../../finitely-many-accepting-extensions-of-a-rejected-stem.md).

Now choose increasing $b_1,b_2,\ldots$ from $L$ so that every subset of the chosen finite prefix is rejected by the appropriate tail of $L$. The empty prefix is rejected. At the next step, for each of the finitely many already chosen subsets $s$, avoid the finitely many accepting successors just identified. All other successors are rejected, since the previous fusion made every finite stem in $L$ decided. Thus one can choose the next point beyond the finite forbidden union. With $M=\{b_1,b_2,\ldots\}$, every finite $s\subset M$ is rejected.

Now assume $Y$ is star-open. If some infinite $B\subset M$ lay in $Y$, there would be a basic neighbourhood $[s,A]\subseteq Y$ containing $B$. Here $s$ is a finite initial segment of $B$, and its infinite tail $C=B\setminus s$ lies in $A$ and in the relevant tail of $L$. Then $[s,C]\subseteq[s,A]\subseteq Y$, so $C$ accepts $s$, contradicting rejection. Therefore $[M]^\omega\cap Y=\varnothing$. In the earlier acceptance case, $[M]^\omega\subseteq Y$. We have proved

$$
\boxed{\text{every star-open set is Ramsey}.}
$$

The construction works with any infinite starting reservoir. Keeping an initial finite stem fixed and applying the same acceptance/rejection argument to its tails proves the [completely Ramsey set](../../../../../completely-ramsey-set.md) conclusion as well. This supplies the full [fusion proof for open Ellentuck sets](../../../../../fusion-proof-for-open-ellentuck-sets.md); no unproved course combinatorial lemma has been used.

For the final request, a family has the [Baire property in the ordinary infinite-subset topology](../../../../../baire-property-in-the-ordinary-infinite-subset-topology.md) if it differs from a $\tau$-open family by a $\tau$-meagre set. We construct a non-Ramsey family which is already $\tau$-nowhere dense. Let

$$
D=\{A=\{a_1<a_2<\cdots\}:a_{n+1}>2a_n\text{ for every }n\}.
$$

The [gap-doubling closed family of infinite subsets](../../../../../gap-doubling-closed-family-of-infinite-subsets.md) $D$ is $\tau$-closed: a violation is witnessed by a finite initial segment, whose whole cylinder lies outside $D$. It is [nowhere dense](../../../../../nowhere-dense-set.md): inside any cylinder, extend the stem by two sufficiently large consecutive integers $k,k+1$; the resulting smaller cylinder violates the gap inequality and is disjoint from $D$.

For every infinite $M$, the set $D\cap[M]^\omega$ has cardinality $\mathfrak c=2^{\aleph_0}$. To prove the lower bound, build a binary tree of finite gap-doubling sequences using points of $M$, choosing two distinct next points above twice the previous point at every node. Distinct infinite binary branches give distinct increasing sets. The upper bound follows because all these sets are subsets of the countable set $\mathbb N$.

Well-order all infinite subsets as $(M_\alpha)_{\alpha<\mathfrak c}$, using the initial ordinal of that cardinality. At stage $\alpha$, choose two previously unused sets

$$
R_\alpha,B_\alpha\in D\cap[M_\alpha]^\omega,
$$

and reserve both permanently. There are fewer than $\mathfrak c$ previously reserved sets but $\mathfrak c$ candidates, so this recursion always continues. This argument does not assume that the continuum is a regular cardinal. Set $X=\{R_\alpha:\alpha<\mathfrak c\}$. Every cone $[M_\alpha]^\omega$ contains its red choice in $X$ and its blue choice outside $X$; the blue choices can never become later red choices. Therefore $X$ is not Ramsey.

But $X\subseteq D$, and $D$ is closed nowhere dense, so the closure of $X$ also has empty interior. Thus $X$ is nowhere dense, hence [meagre](../../../../../meagre-set.md), and $X\mathbin\triangle\varnothing=X$ proves its ordinary Baire property. We have obtained a [meagre set meeting every Ramsey cone in both colours](../../../../../meagre-set-meeting-every-ramsey-cone-in-both-colours.md):

$$
\boxed{X\text{ is }\tau\text{-Baire but not Ramsey}.}
$$

This explains why ordinary Baire regularity cannot replace the star-topology regularity in the open-set theorem. A family supported only on the infinite subsets of a fixed sparse set would not suffice for this counterexample: another infinite set could give an entirely disjoint cone. The gap-doubling family used here instead meets every cone in continuum many candidates.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
