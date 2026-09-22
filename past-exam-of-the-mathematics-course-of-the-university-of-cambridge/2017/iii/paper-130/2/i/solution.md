<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) by [mathematical induction](../../../../../../mathematical-induction.md) on the [alphabet](../../../../../../alphabet.md) size. A [combinatorial line](../../../../../../combinatorial-line.md) has a nonempty active coordinate set, with one common letter in all those coordinates. More generally, a $d$-dimensional [combinatorial subspace](../../../../../../combinatorial-subspace.md) has $d$ disjoint nonempty active coordinate sets, each with an independently variable letter.

First prove the [alphabet insensitivity lemma](../../../../../../alphabet-insensitivity-lemma.md), rather than assume it. Fix distinct letters $a,b\in[m]$, $k$ colors, and dimension $d$. Partition the coordinates into consecutive blocks of lengths $L_1,\ldots,L_d$, chosen from left to right. Put $S_0=0$ and choose

$$
L_i=k^{\,m^{S_{i-1}+d-i}},\qquad S_i=S_{i-1}+L_i,\qquad N=S_d.
$$

Construct the variable blocks from right to left. When working on block $i$, the later blocks have already become $(d-i)$-parameter words, while all earlier $S_{i-1}$ coordinates remain unrestricted. For each $t\in\{0,\ldots,L_i\}$, take the color vector of the word having $a^t b^{L_i-t}$ in block $i$, indexed by every earlier word and every assignment to the later parameters. There are $m^{S_{i-1}+d-i}$ entries and hence at most $L_i$ different vectors. The [pigeonhole principle](../../../../../../pigeonhole-principle.md) gives $t<s$ with identical vectors. Fix the first $t$ positions of this block to $a$, fix its last $L_i-s$ positions to $b$, and make the intervening $s-t$ positions a new variable block. Substituting $a$ or $b$ there gives exactly the two equal color vectors.

This equality holds for every earlier word and every later parameter assignment. Restricting the earlier coordinates in subsequent steps therefore preserves it. Likewise, the insensitivity already proved in a later block survives every restriction of earlier coordinates. At the end, we obtain a $d$-dimensional [combinatorial subspace](../../../../../../combinatorial-subspace.md) whose induced [finite coloring](../../../../../../finite-coloring.md) is unchanged whenever any parameter switches between $a$ and $b$, with all other parameters fixed. Multiple switches preserve the color by successive single switches. This is the [alphabet insensitivity lemma](../../../../../../alphabet-insensitivity-lemma.md) in full.

For [alphabet](../../../../../../alphabet.md) size $1$, one coordinate is already a [monochromatic](../../../../../../monochromatic-set.md) [combinatorial line](../../../../../../combinatorial-line.md). Suppose the [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) has been proved for [alphabet](../../../../../../alphabet.md) size $m-1$, and let $d=n(m-1,k)$. Apply the proved [alphabet insensitivity lemma](../../../../../../alphabet-insensitivity-lemma.md) with letters $m-1,m$ to get a $d$-dimensional [combinatorial subspace](../../../../../../combinatorial-subspace.md) in $[m]^N$. Restrict its parameter words to $[m-1]^d$. The induction hypothesis gives a [monochromatic](../../../../../../monochromatic-set.md) [combinatorial line](../../../../../../combinatorial-line.md) in these parameters. The union of its active parameter blocks is nonempty, so its image is a [combinatorial line](../../../../../../combinatorial-line.md) in the original coordinates. Its additional point with active letter $m$ has the same color as the point with active letter $m-1$, by insensitivity. Therefore all $m$ points have one color, proving

$$
\boxed{n(m,k)<\infty\quad\text{for every }m,k\geq1.}
$$

The construction supplies a finite recursive bound; optimal bounds are not needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
