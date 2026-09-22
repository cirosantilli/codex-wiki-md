<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [combinatorial line](../../../../../combinatorial-line.md) in $[k]^N$ fixes all coordinates outside a nonempty set $J$ and puts the same variable letter in every coordinate of $J$. The [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) asserts that **for every $k,r\ge1$, some $N$ forces a [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md) in every $r$-colouring of $[k]^N$**. We prove it by [mathematical induction](../../../../../mathematical-induction.md) on $k$, using an explicit [alphabet insensitivity lemma](../../../../../alphabet-insensitivity-lemma.md).

A $d$-dimensional [combinatorial subspace](../../../../../combinatorial-subspace.md) fixes some coordinates and has $d$ disjoint nonempty variable blocks. It is $(a,b)$-insensitive if changing any parameter from $a$ to $b$ or back leaves the colour unchanged. For $k\ge2$, fixed $a\ne b\in[k]$, $r$ colours and any required dimension $d$, we now construct such a subspace without assuming the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md).

Choose consecutive blocks of lengths $L_1,\ldots,L_d$ by

$$
P_i=\sum_{j<i}L_j,\qquad
L_i=r^{\,k^{P_i+d-i}},\qquad N=\sum_{i=1}^dL_i.
$$

Process blocks from right to left. When processing block $i$, the later blocks already have their variable templates. For each $0\le t\le L_i$, consider $a^tb^{L_i-t}$ in block $i$. Record its [colour profile](../../../../../colour-profile-of-a-finite-block.md) for every earlier word in $[k]^{P_i}$ and every assignment of the $d-i$ later parameters. There are $k^{P_i+d-i}$ contexts and at most $r^{k^{P_i+d-i}}=L_i$ profiles. The $L_i+1$ chain words therefore contain two equal profiles by the [pigeonhole principle](../../../../../pigeonhole-principle.md).

If their indices are $s<t$, replace the block by the variable template

$$
a^s\,v^{t-s}\,b^{L_i-t},\qquad v\in[k].
$$

Its active block is nonempty. The values $v=a,b$ recover those two equal-profile words, so the colour is unchanged by interchanging $a,b$, for every earlier word and every later parameter assignment. Insensitivity already established in a later block persists, since it was established uniformly over all earlier words, including every subsequent restriction of block $i$. Continuing leftward gives the promised $d$-dimensional [combinatorial subspace](../../../../../combinatorial-subspace.md). This proves the [explicit block bound for alphabet insensitivity](../../../../../explicit-block-bound-for-alphabet-insensitivity.md) and its required uniformity.

The one-letter case of the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) is immediate: take $N=1$. Suppose it is proved for $k-1$ letters and every number of colours. Let $d$ be a dimension guaranteed for $k-1$ letters and $r$ colours. Obtain a $d$-dimensional $(k-1,k)$-insensitive [combinatorial subspace](../../../../../combinatorial-subspace.md) by the lemma. Restrict its parameter alphabet to $[k-1]$ and apply the induction hypothesis. The resulting [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md) uses some nonempty set of parameters. Its extra $k$-letter point has the same colour as its $(k-1)$-letter point: interchange $k-1,k$ in those parameters one at a time. The union of their active blocks is nonempty, so the extended line is a genuine [combinatorial line](../../../../../combinatorial-line.md) in the original word space. This completes the [letter-merging proof of the Hales-Jewett theorem](../../../../../letter-merging-proof-of-the-hales-jewett-theorem.md).

To deduce the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md), take alphabet $\{0,\ldots,m-1\}$ and pull a [finite colouring](../../../../../finite-coloring.md) of the positive integers back by

$$
\pi(w)=1+\sum_{j=1}^Nw_j.
$$

A [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md) with active set $J$ maps to

$$
a,\ a+d,\ldots,a+(m-1)d,\qquad
 a=1+\sum_{j\notin J}w_j>0,\quad d=|J|>0.
$$

Thus **every [finite colouring](../../../../../finite-coloring.md) of the positive integers contains a [monochromatic](../../../../../monochromatic-set.md) [arithmetic progression](../../../../../arithmetic-progression.md) of each prescribed finite length**. Since the map only uses $[1,1+N(m-1)]$, this also gives the finite interval version, with an interval bound $W(r,m)$.

The [Strengthened Van der Waerden theorem](../../../../../strengthened-van-der-waerden-theorem.md) requires the [common difference](../../../../../common-difference.md) to have the same colour: for every $r,m$ some finite interval forces a [monochromatic](../../../../../monochromatic-set.md) set

$$
\boxed{\{d,a,a+d,\ldots,a+(m-1)d\},\qquad a,d>0.}
$$

For $m=1$, take $a=d=1$. For $m\ge2$, prove the assertion by [mathematical induction](../../../../../mathematical-induction.md) on $r$, writing $B(r,m)$ for a sufficient interval bound. The one-colour case has $a=d=1$ and $B(1,m)=m$. Suppose $M=B(r-1,m)$ is known. Apply the ordinary [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) to find a [monochromatic](../../../../../monochromatic-set.md) progression

$$
a,a+d,\ldots,a+(L-1)d,\qquad L=(m-1)M+1,
$$

in $[N]$, where $N=W(r,L)$; call its colour $\gamma$. As $(L-1)d<N$, every point $td$ with $1\le t\le M$ also lies in $[N]$.

If one such $td$ has colour $\gamma$, the $m$ points $a,a+td,\ldots,a+(m-1)td$ lie in the original progression and have that colour, together with their difference $td$. Otherwise the pulled-back [finite colouring](../../../../../finite-coloring.md) $t\mapsto\chi(td)$ on $[M]$ uses at most $r-1$ colours. By the induction hypothesis it contains $\{e,b,b+e,\ldots,b+(m-1)e\}$ of one colour. Multiplication by $d$ gives the required set with starting point $bd$ and [common difference](../../../../../common-difference.md) $ed$. This proves the strengthened theorem with

$$
B(r,m)=W\bigl(r,(m-1)B(r-1,m)+1\bigr)\quad(r\ge2,m\ge2).
$$

This is the colour-count argument behind the [Brauer progression theorem](../../../../../brauer-progression-theorem.md).

The [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md) states that **every [finite colouring](../../../../../finite-coloring.md) of $\mathbb N^d$ contains a [monochromatic](../../../../../monochromatic-set.md) [homothetic copy](../../../../../homothetic-copy-of-a-finite-configuration.md) of each finite lattice pattern**. More precisely, for finite $S\subseteq\mathbb Z^d$ there exist $q\in\mathbb N$ and $b\in\mathbb Z^d$ with $b+qS\subseteq\mathbb N^d$ [monochromatic](../../../../../monochromatic-set.md). For $S\subseteq\mathbb N^d$, the translation vector can also be chosen positive.

The empty pattern is trivial. Otherwise first translate the pattern so its points $v_1,\ldots,v_k$ have nonnegative coordinates. Pull the given [finite colouring](../../../../../finite-coloring.md) back to words through the [sum map from words to homothetic copies](../../../../../sum-map-from-words-to-homothetic-copies.md)

$$
\Phi(w)=\mathbf1+\sum_{j=1}^Nv_{w_j}\in\mathbb N^d.
$$

By the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md), some [combinatorial line](../../../../../combinatorial-line.md) with active set $J$ is [monochromatic](../../../../../monochromatic-set.md). Its images are

$$
\mathbf1+\sum_{j\notin J}v_{w_j}+|J|v_i,\qquad 1\le i\le k.
$$

They are a [homothetic copy](../../../../../homothetic-copy-of-a-finite-configuration.md) with positive integer dilation $|J|$. Undoing the preliminary translation merely changes the translation vector; the actual copy still lies in the positive lattice. This derives [Gallai's theorem](../../../../../gallai-theorem-for-an-integer-lattice.md) from the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md), and justifies the version used in Question 1.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
