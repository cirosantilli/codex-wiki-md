<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [pair of partitions for a generalized Specht module](../../../../../pair-of-partitions-for-a-generalized-specht-module.md) convention appropriate to [generalized Specht modules](../../../../../generalized-specht-module.md). Put $a=\mu^\sharp$ and $b=\mu$. Here $b=(b_1,b_2,\ldots)$ is a sequence of nonnegative row lengths of total $n$, and $a$ is a proper [partition of an integer](../../../../../partition-of-an-integer.md) satisfying $0\le a_i\le b_i$ and $a_{i+1}\le a_i$. The row-length sequence $b$ is allowed to be a composition; it need not decrease. The first $a_i$ cells of row $i$ are marked. This construction is not an arbitrary pair of unrelated [partitions of an integer](../../../../../partition-of-an-integer.md) and is not simply a skew diagram $b/a$.

A word has type $b$ if it contains $b_i$ occurrences of $i$. Read it from left to right. Every occurrence of $1$ is good; an occurrence of $i+1$ is good exactly when there have so far been more good occurrences of $i$ than good occurrences of $i+1$. Otherwise it is bad. Define

$$
s(a,b)=\{w:\operatorname{type}(w)=b,\ \#\text{good occurrences of }i\ge a_i\text{ for every }i\}.
$$

Thus $s(0,b)$ is the set of all words of type $b$, and $s(b,b)$ consists of [lattice words](../../../../../lattice-word.md) when $b$ is a proper [partition of an integer](../../../../../partition-of-an-integer.md). Marking the whole first row makes no difference because every $1$ is good.

For a [Young tableau](../../../../../young-tableau.md) $T$ with row lengths $b$, let $C_T^a$ permute labels within each column of its marked subdiagram, fixing all unmarked labels. Its generalized [polytabloid](../../../../../polytabloid.md) and [generalized Specht module](../../../../../generalized-specht-module.md) are

$$
\boxed{e_T^{a,b}=\sum_{g\in C_T^a}\operatorname{sgn}(g)\{gT\},\qquad
S^{a,b}=\operatorname{span}_F\{e_T^{a,b}\}\subseteq M^b.}
$$

In particular $S^{0,b}=M^b$ and $S^{b,b}=S^b$. The [Young tableau](../../../../../young-tableau.md) shape in this definition must be the row sequence $b$.

We give the filtration argument, keeping its combinatorial and module-theoretic steps separate. Normalize $a_1=b_1$, and if $a\ne b$ choose the first row $c>1$ with $a_c<b_c$. Then $a_{c-1}=b_{c-1}$. Define $A_c(a,b)=(a+e_c,b)$ if $a_{c-1}>a_c$; otherwise the add branch is empty. Define $R_c(a,b)=(a,b')$ by moving the unmarked tail of row $c$ into row $c-1$:

$$
b'_c=a_c,\qquad b'_{c-1}=b_{c-1}+b_c-a_c,
$$

with other row lengths unchanged. Re-normalize the first marked row if necessary. The Basic Combinatorial Theorem supplies the counting and formal-character recursions

$$
|s(a,b)|=|s(A_c(a,b))|+|s(R_c(a,b))|,\qquad
[0]^{[a,b]}=[0]^{[A_c(a,b)]}+[0]^{[R_c(a,b)]}.
$$

At a terminal pair $(\nu,\nu)$ the formal term is $[\nu]$. Thus the second recursion specifies the Specht multiplicities by the terminal leaves, with repeated leaves counted separately.

Define an equivariant map $\psi:M^b\to M^{b'}$ by summing, on each [tabloid](../../../../../tabloid.md), over all choices of the $a_c$ labels retained in row $c$, moving the remaining labels to row $c-1$. Column cancellation gives

$$
\psi(S^{a,b})=S^{R_c(a,b)},\qquad
S^{A_c(a,b)}\subseteq S^{a,b}\cap\ker\psi.
$$

For the first identity, terms that put two marked labels of one column in the raised row cancel in pairs; the surviving marked antisymmetrizer is the one for the raised pair, and every target generator has a preimage. For the second, the extra marked cell makes such a collision unavoidable, so the sum vanishes. Also antisymmetrizing the extra cell expresses its generator as a sum of old generators, proving containment in $S^{a,b}$.

There is a characteristic-independent lower bound $\dim S^{a,b}\ge|s(a,b)|$. Given a word in $s(a,b)$, place the label $j$ in its letter's row: good occurrences fill that row from the left and bad occurrences fill it from the right. The marked cells form increasing column chains because each good $i+1$ has an earlier unmatched good $i$. Its generalized [polytabloid](../../../../../polytabloid.md) has the original row-assignment [tabloid](../../../../../tabloid.md) with coefficient one; every other term changes an earlier member of a marked chain. Ordering these row assignments gives a triangular coefficient matrix. The resulting vectors are independent over every [field](../../../../../field.md).

Start with $(0,v)$, where equality holds because the [tabloid](../../../../../tabloid.md) basis is indexed by all words of type $v$. Any pair is reached from such a pair by a sequence of add and raise operations: reverse a raise by splitting a raised tail, and reverse an add by unmarking a cell; row by row these recover an entirely unmarked composition. Suppose equality holds at a pair. The map and [kernel](../../../../../kernel-of-a-linear-map.md) containment above give

$$
|s(a,b)|=\dim S^{a,b}\ge\dim S^{A_c(a,b)}+\dim S^{R_c(a,b)}
\ge|s(A_c(a,b))|+|s(R_c(a,b))|=|s(a,b)|.
$$

Every inequality is therefore equality. In particular the containment is the whole [kernel](../../../../../kernel-of-a-linear-map.md), and

$$
0\longrightarrow S^{A_c(a,b)}\longrightarrow S^{a,b}\longrightarrow S^{R_c(a,b)}\longrightarrow0
$$

is exact. The process terminates because each add marks an extra cell and each raise decreases the total row index of unmarked cells. Induction from the terminal [Specht modules](../../../../../specht-module.md), splicing their filtrations through these exact sequences, proves **a [Specht series](../../../../../specht-filtration.md) with factors precisely $[0]^{[\mu^\sharp,\mu]}$**. No splitting of these sequences in positive [characteristic](../../../../../characteristic-of-a-field.md) is asserted.

Applying the same marking, raising and straightening procedure to the two sets of [column antisymmetrizers](../../../../../column-antisymmetrizer-of-a-young-tableau.md) in $(S^\mu\boxtimes S^\lambda)\uparrow^{S_{r+s}}$, where $|\mu|=r$, $|\lambda|=s$, leaves the cells of $\mu$ fixed and records the added cells by their row labels from $\lambda$. The column relations require strict increase down columns, the row relations weak increase along rows, and the [good-letter matching in a tableau word](../../../../../good-letter-matching-in-a-tableau-word.md) test requires a [lattice word](../../../../../lattice-word.md). Thus the surviving terminal multiplicity is the number $c_{\mu\lambda}^\nu$ of [Semistandard Young tableaux](../../../../../semistandard-young-tableau.md) of [skew shape](../../../../../skew-young-diagram.md) of shape $\nu/\mu$ and content $\lambda$ whose word, read right-to-left along successive rows from top to bottom, has at least as many $i$'s as $(i+1)$'s in every prefix. The same triangular leading-tabloid argument identifies each quotient with $S^\nu$. Consequently the [Littlewood–Richardson rule](../../../../../littlewood-richardson-rule.md) is

$$
\boxed{[\mu][\lambda]=\sum_{\nu\vdash r+s}c_{\mu\lambda}^\nu[\nu].}
$$

It describes ordinary [irreducible](../../../../../irreducible-representation.md) constituents in [characteristic](../../../../../characteristic-of-a-field.md) zero and [Specht filtration](../../../../../specht-filtration.md) factors over arbitrary $F$.

For induction by one letter, content $(1)$ permits exactly one added cell and each multiplicity is one. A [Specht series](../../../../../specht-filtration.md) for the requested induced [module](../../../../../module-mathematics.md) has successive quotients, ordered by addable nodes from bottom to top,

$$
\boxed{S^{(4,2,2,1,1)},\quad S^{(4,2,2,2)},\quad S^{(4,3,2,1)},\quad S^{(5,2,2,1)}.}
$$

Equivalently there is $0=N_0\subset N_1\subset N_2\subset N_3\subset N_4=S^{(4,2,2,1)}\uparrow^{S_{10}}$ with these four quotients in order. Their [dimensions](../../../../../dimension-vector-space.md) $567,300,768,525$ sum to $2160=10\cdot216$, the [dimension](../../../../../dimension-vector-space.md) of the induced [module](../../../../../module-mathematics.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
