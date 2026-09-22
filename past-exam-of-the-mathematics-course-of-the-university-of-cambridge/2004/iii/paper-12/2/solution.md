<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a finite alphabet $K$, a [combinatorial line](../../../../../combinatorial-line.md) in $K^N$ has a nonempty active set $J\subseteq\{1,\ldots,N\}$, fixed letters outside $J$, and the same variable letter at every coordinate in $J$. The [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) states that for every alphabet size $k\ge1$ and number of colours $r\ge1$, some $N$ makes every r-colouring of $\{1,\ldots,k\}^N$ contain a [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md).

We first prove the [alphabet insensitivity lemma](../../../../../alphabet-insensitivity-lemma.md) with a concrete bound. Fix two distinct letters $a,b$, a desired dimension $d$, and a colouring $\chi:K^N\to\{1,\ldots,r\}$. A [combinatorial subspace](../../../../../combinatorial-subspace.md) of dimension $d$ has disjoint nonempty active blocks $J_1,\ldots,J_d$ and fixed other coordinates. It is $(a,b)$-insensitive when exchanging $a,b$ in any one variable leaves the colour unchanged, whatever the other variable letters are.

Choose consecutive blocks of lengths $L_1,\ldots,L_d$ recursively by

$$
P_i=\sum_{j<i}L_j,\qquad L_i=r^{\,k^{P_i+d-i}},\qquad N=\sum_{i=1}^dL_i.
$$

Process these blocks from right to left. When block $i$ is reached, the later blocks already have one variable each; the earlier $P_i$ coordinates are still entirely unrestricted. For each of the $L_i+1$ words $a^t b^{L_i-t}$ in block $i$, form its complete [colour profile](../../../../../colour-profile-of-a-finite-block.md) over all $k^{P_i}$ earlier words and all $k^{d-i}$ assignments to the later variables. There are at most $r^{k^{P_i+d-i}}=L_i$ profiles. The [pigeonhole principle](../../../../../pigeonhole-principle.md) gives $s<t$ with equal profiles. Fix the first $s$ coordinates of this block to $a$, the coordinates after $t$ to $b$, and make the interval from $s+1$ to $t$ variable. Substitution of $b$ gives the chain word indexed by $s$, and substitution of $a$ gives the one indexed by $t$; they have identical profiles. Thus this variable is insensitive to $a,b$ for every remaining context. Previously constructed later variables remain insensitive, because their colour equalities held for every possible earlier word. After all $d$ blocks, we have the required insensitive [combinatorial subspace](../../../../../combinatorial-subspace.md). This proves the [explicit block bound for alphabet insensitivity](../../../../../explicit-block-bound-for-alphabet-insensitivity.md).

Now induct on $k$, simultaneously for every $r$. The case $k=1$ is immediate with $N=1$. For $k\ge2$, assume the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) for the alphabet of size $k-1$, and take $d$ large enough for that theorem with $r$ colours. Apply the proved [alphabet insensitivity lemma](../../../../../alphabet-insensitivity-lemma.md) to the letters $k-1,k$, obtaining a d-dimensional [combinatorial subspace](../../../../../combinatorial-subspace.md) $\phi:K^d\to K^N$. On $\{1,\ldots,k-1\}^d$, the induced colouring $\chi\circ\phi$ has a [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md). Its value at letter $k$ has the same colour as its value at $k-1$: change the active variables one at a time and use insensitivity. The [union](../../../../../set-union.md) of their nonempty active blocks is the active set of a [combinatorial line](../../../../../combinatorial-line.md) in the original word space. All its k points have one colour, completing the induction and the proof.

To deduce the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md), take $K=\{0,\ldots,m-1\}$ and pull a colouring of the [positive integers](../../../../../positive-integer.md) back through

$$
\pi(w)=1+\sum_{j=1}^Nw_j.
$$

A [combinatorial line](../../../../../combinatorial-line.md) with active set $J$ maps to

$$
a,a+d,\ldots,a+(m-1)d,\qquad
 a=1+\sum_{j\notin J}w_j,\quad d=|J|>0.
$$

Hence **every [finite colouring](../../../../../finite-coloring.md) has a [monochromatic](../../../../../monochromatic-set.md) [arithmetic progression](../../../../../arithmetic-progression.md) of every prescribed finite length**. In finite form, if $H(k,r)$ is a word-length bound for the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md), then $W(r,m)\le1+(m-1)H(m,r)$ is a valid interval bound.

The [Strengthened Van der Waerden theorem](../../../../../strengthened-van-der-waerden-theorem.md) also puts the [common difference](../../../../../common-difference.md) in the colour class:

$$
\boxed{\{d,a,a+d,\ldots,a+(m-1)d\}\text{ is monochromatic for some }a,d>0.}
$$

Here is a finite proof by induction on the number $r$ of colours. For $m=1$ choose $a=d=1$. For $r=1$ choose $a=d=1$ in $[m]$. For $m\ge2,r\ge2$, let $M$ be a bound for the strengthened theorem with $r-1$ colours, put $L=(m-1)M+1$, and let $W=W(r,L)$ be an ordinary [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) bound. Work in $[MW]$. Its first $W$ points contain a [monochromatic](../../../../../monochromatic-set.md) progression

$$
a,a+d,\ldots,a+(L-1)d
$$

of colour $c$. Every $jd$, $1\le j\le M$, lies in $[MW]$. If some $jd$ has colour $c$, then $a,a+jd,\ldots,a+(m-1)jd$, together with its difference $jd$, gives the answer. Otherwise the colouring of $\{d,2d,\ldots,Md\}$ uses only $r-1$ colours. Pull it back to $[M]$ and apply the induction hypothesis to get a [monochromatic](../../../../../monochromatic-set.md) set $\{e,b,b+e,\ldots,b+(m-1)e\}$. Multiplication by $d$ gives the required configuration in the original colouring. This proves the strengthened theorem, including finite bounds.

The [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md) states that every [finite colouring](../../../../../finite-coloring.md) of $\mathbb Z^h$ contains a [monochromatic](../../../../../monochromatic-set.md) [homothetic copy](../../../../../homothetic-copy-of-a-finite-configuration.md) $u+tF$ of every prescribed finite nonempty pattern $F\subseteq\mathbb Z^h$, where $t$ is a [positive integer](../../../../../positive-integer.md). The positive-lattice version holds for finite $F\subseteq\mathbb N^h$ as well. Write $F=\{v_1,\ldots,v_k\}$ and colour $w\in\{1,\ldots,k\}^N$ by the colour of

$$
\pi(w)=b+\sum_{j=1}^Nv_{w_j}.
$$

A [monochromatic](../../../../../monochromatic-set.md) [combinatorial line](../../../../../combinatorial-line.md) maps to $u+|J|F$, with $u=b+\sum_{j\notin J}v_{w_j}$. Thus the [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) supplies the copy, with nonzero dilation $|J|$. Choosing $b$ large and positive places all these word sums in the positive lattice if required. This [sum map from words to homothetic copies](../../../../../sum-map-from-words-to-homothetic-copies.md) also proves the real-vector-space version: replace $\mathbb Z^h$ by $\mathbb R^h$ and allow an arbitrary finite real pattern, while retaining [positive integer](../../../../../positive-integer.md) dilations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
