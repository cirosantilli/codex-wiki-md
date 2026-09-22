<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $\Omega=[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../../../space-of-infinite-subsets-of-the-natural-numbers.md), identifying a set with its increasing enumeration. If $s$ is finite and $A$ is infinite with every element of $A$ above $\max s$, set

$$
[s,A]=\{s\cup B:B\in[A]^\omega\}.
$$

For the empty stem there is no lower-bound restriction. These sets form the basis of the [Ellentuck topology](../../../../../ellentuck-topology.md), also called the [star topology](../../../../../ellentuck-topology.md). The stem $s$ is fixed, while the infinite tail may be thinned.

A [completely Ramsey set](../../../../../completely-ramsey-set.md) $E\subseteq\Omega$ is one for which every $[s,A]$ admits an infinite $B\subseteq A$ with $[s,B]\subseteq E$ or $[s,B]\cap E=\varnothing$. This keeps the same stem. A [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md) requires that every infinite $A$ admit an infinite $B\subseteq A$ with a homogeneous empty-stem cone $[B]^\omega$. It does not require preserving a nonempty finite stem.

A set is a [star-Baire set](../../../../../baire-property-in-the-ellentuck-topology.md) if it differs from a star-open set by a star-[meagre set](../../../../../meagre-set.md), equivalently $E\mathbin\triangle U$ is star-meagre for some star-open $U$. A [nowhere dense set](../../../../../nowhere-dense-set.md) has closure with empty interior, and a [meagre set](../../../../../meagre-set.md) is a countable union of such sets, with both notions interpreted in the specified topology.

For a non-Ramsey example, put $M=\{2,3,\ldots\}$ and well-order all infinite subsets of $M$ as $(A_\alpha)_{\alpha<\mathfrak c}$, where $\mathfrak c=2^{\aleph_0}$. Recursively choose two fresh points $X_\alpha,Y_\alpha\in[A_\alpha]^\omega$, not used at earlier stages. This is possible because each cone has cardinality $\mathfrak c$ and fewer than $\mathfrak c$ points have been used before any stage. Let

$$
C=\{X_\alpha:\alpha<\mathfrak c\},
$$

keeping all the $Y_\alpha$ outside $C$. Every infinite-subset cone on $M$ meets both $C$ and its complement. Thus **$C$ is not Ramsey**, even when regarded as a subset of $\Omega$: any infinite set can first be thinned to avoid $1$. This uses the [axiom of choice](../../../../../axiom-of-choice.md), rather than claiming a Borel counterexample.

Now set

$$
\boxed{E=\{\{1\}\cup X:X\in C\}.}
$$

Every infinite $A$ has an infinite subset $B$ avoiding $1$, and then $[B]^\omega\cap E=\varnothing$. Hence **$E$ is Ramsey**. But no stem-preserving thinning of $[\{1\},M]$ is homogeneous for $E$, because $C$ splits every tail cone. Hence **$E$ is not completely Ramsey**.

To prove the topological equivalence, we first establish the [Ellentuck meagre-set fusion lemma](../../../../../ellentuck-meagre-set-fusion-lemma.md): every star-meagre set can be avoided in a refinement $[s,B]$ with the original stem. Call a set [completely Ramsey-null](../../../../../completely-ramsey-null-set.md) if this avoidance holds in every $[s,A]$.

If $N$ is star-[nowhere dense](../../../../../nowhere-dense-set.md), then $U=\Omega\setminus\overline N$ is star-open and dense. By the granted complete-Ramsey property of star-open sets, every $[s,A]$ has a refinement $[s,B]$ either contained in $U$ or disjoint from $U$. The latter alternative would put a nonempty open set inside $\overline N$, contradicting density of $U$. Thus $N$ is [completely Ramsey-null](../../../../../completely-ramsey-null-set.md).

For a countable union $\bigcup_j N_j$ of [completely Ramsey-null](../../../../../completely-ramsey-null-set.md) sets, use fusion, taking care of every possible finite stem. Starting with $A_0=A$, at stage $j$ choose $b_j\in A_{j-1}$ above all previous choices. From the part of $A_{j-1}$ above $b_j$, successively thin an infinite tail for each of the finitely many subsets $t\subseteq\{b_1,\ldots,b_j\}$ so that

$$
[s\cup t,A_j]\cap N_j=\varnothing.
$$

Each thinning keeps the stem $s\cup t$ fixed; subsequent thinnings preserve earlier avoidance. Let $B=\{b_1,b_2,\ldots\}$. For any $X\in[s,B]$ and fixed $j$, put $t=(X\setminus s)\cap\{b_1,\ldots,b_j\}$. The rest of $X$ lies in $A_j$, because all later selected points do. Therefore $X\in[s\cup t,A_j]$ and $X\notin N_j$. Since $j$ was arbitrary,

$$
\boxed{[s,B]\cap\bigcup_jN_j=\varnothing.}
$$

This proves the fusion lemma. Considering all subsets $t$, not merely the single selected prefix, is essential: elements of $[s,B]$ need not use every $b_i$.

Suppose first that $E$ is star-Baire, with $E\triangle U$ star-meagre and $U$ star-open. Thin $[s,A]$ to $[s,B]$ avoiding the meagre difference by the lemma. Then apply the granted complete-Ramsey property of $U$ to find $[s,D]$ homogeneous for $U$, with $D\subseteq B$. On this refinement $E$ and $U$ agree, so it is homogeneous for $E$. Thus $E$ is completely Ramsey.

Conversely, let $E$ be completely Ramsey and let $U$ be the union of all basic neighborhoods wholly contained in $E$, namely its star-interior. Every $[s,A]$ has a homogeneous refinement. If that refinement lies in $E$, it lies in $U$; if it avoids $E$, it also avoids $E\setminus U$. Consequently every basic neighborhood contains a nonempty open refinement disjoint from $E\setminus U$. Since such a refinement is also disjoint from the closure of $E\setminus U$, this difference is star-[nowhere dense](../../../../../nowhere-dense-set.md). Thus $E\triangle U=E\setminus U$ is star-meagre, and $E$ is star-Baire. We have proved

$$
\boxed{E\text{ completely Ramsey}\iff E\text{ has the Baire property in the star topology}.}
$$

Finally, **$\Omega$ is not star-meagre**: otherwise apply the fusion lemma to its purported meagre cover inside any nonempty basic neighborhood, obtaining a nonempty $[s,B]$ disjoint from $\Omega$, a contradiction.

The printed paper does not define $\tau$. In the coarser [Ramsey cone topology](../../../../../ramsey-cone-topology.md), whose basic open sets are $[A]^\omega$ without finite stems, **$\Omega$ is $\tau$-meagre**. To prove this, let $D_j=\{X:\min X=j\}$. Its cone-topology closure is $H_j=\{X:j\in X\}$: every cone neighborhood of a point containing $j$ has a subset with least element $j$, whereas if $j\notin X$ the neighborhood $[X]^\omega$ avoids $D_j$. No nonempty cone lies in $H_j$, since its infinite ground set can be thinned to remove $j$. Therefore each $D_j$ is [nowhere dense](../../../../../nowhere-dense-set.md), but $\Omega=\bigcup_{j\geq1}D_j$. This proves [meagreness of the Ramsey cone topology](../../../../../meagreness-of-the-ramsey-cone-topology.md) and exhibits the contrast with the [star topology](../../../../../ellentuck-topology.md).

If $\tau$ instead denotes the [ordinary topology on infinite subsets](../../../../../ordinary-topology-on-infinite-subsets.md), with basic cylinders $[s]=\{X:s\text{ is an initial segment of }X\}$, the answer is **not $\tau$-meagre**. Indeed, given countably many nowhere dense sets, extend a finite increasing prefix successively so that its cylinder avoids the closure of the next set. Make the prefix longer at each step. Their union is an infinite increasing enumeration belonging to every chosen cylinder and avoiding the whole proposed cover. The same construction starts inside any nonempty cylinder, so this alternative product topology is also a [Baire space](../../../../../baire-space.md). The two conventions have different answers, so the distinction must be made explicitly rather than inferred from the symbol alone.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
