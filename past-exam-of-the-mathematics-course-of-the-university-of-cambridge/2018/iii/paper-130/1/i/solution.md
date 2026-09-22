<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Hales–Jewett and the arithmetic-progression consequence.** For a finite [alphabet](../../../../../../alphabet.md) $[m]$ and a positive integer $r$, the [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) gives an integer $N$ such that every $r$-color [finite coloring](../../../../../../finite-coloring.md) of $[m]^N$ contains a [monochromatic](../../../../../../monochromatic-set.md) [combinatorial line](../../../../../../combinatorial-line.md). A [combinatorial line](../../../../../../combinatorial-line.md) has a nonempty active coordinate set: all those coordinates receive the same freely varying letter, and the remaining coordinates are fixed.

We first prove the [alphabet insensitivity lemma](../../../../../../alphabet-insensitivity-lemma.md). Fix two letters $a,b\in[m]$, with $m\geq2$, and a desired dimension $d$. There is a [combinatorial subspace](../../../../../../combinatorial-subspace.md) of dimension $d$ on which changing $a$ to $b$ in any variable coordinate, with all other variable coordinates arbitrary, preserves the color.

For the construction, divide the coordinates into $d$ consecutive blocks. Choose their lengths from left to right by

$$
P_i=\sum_{j<i}L_j,\qquad L_i=r^{\,m^{P_i+d-i}}.
$$

Process the blocks from right to left. When processing block $i$, the later blocks already form a $(d-i)$-dimensional [combinatorial subspace](../../../../../../combinatorial-subspace.md). Color each word in block $i$ by the vector of its original colors for every prefix word of length $P_i$ and every assignment to those later variables. There are $m^{P_i+d-i}$ contexts, and at most $r^{m^{P_i+d-i}}=L_i$ such color vectors.

The $L_i+1$ words $a^j b^{L_i-j}$, $0\leq j\leq L_i$, contain two, indexed by $u<v$, with the same vector by the [pigeonhole principle](../../../../../../pigeonhole-principle.md). Fix the first $u$ coordinates to $a$, the coordinates after $v$ to $b$, and make coordinates $u+1,\ldots,v$ the active set of one new variable. Its values $a,b$ now have identical colors for every prefix and later-variable context. The active set is nonempty. Insensitivity already obtained in later blocks survives, because it held for every unrestricted earlier prefix. After all $d$ blocks have been processed, changing $a,b$ in any of the $d$ variables preserves the color. This proves the lemma.

Now induct on $m$. For $m=1$, a one-coordinate [combinatorial line](../../../../../../combinatorial-line.md) is automatically [monochromatic](../../../../../../monochromatic-set.md). For $m\geq2$, let $d$ be a length supplied by the theorem for [alphabet](../../../../../../alphabet.md) $[m-1]$ and $r$ colors. Apply the [alphabet insensitivity lemma](../../../../../../alphabet-insensitivity-lemma.md) for the letters $m-1,m$ to obtain a $d$-dimensional [combinatorial subspace](../../../../../../combinatorial-subspace.md). Restrict its variables to $[m-1]$. Induction gives a [monochromatic](../../../../../../monochromatic-set.md) [combinatorial line](../../../../../../combinatorial-line.md) in those variables. Its values $1,\ldots,m-1$ have the same color, and its value $m$ has the same color as its value $m-1$ by successively switching the active variables. Lifting this line to the original coordinates proves

$$
\boxed{\text{every finite coloring of a sufficiently long word space has a monochromatic line}.}
$$

For the [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md), fix a progression length $k\geq2$ and use the [alphabet](../../../../../../alphabet.md) $\{0,\ldots,k-1\}$. Pull back an $r$-color [finite coloring](../../../../../../finite-coloring.md) of $\{1,\ldots,1+(k-1)N\}$ along

$$
(x_1,\ldots,x_N)\longmapsto1+\sum_{j=1}^N x_j.
$$

A [combinatorial line](../../../../../../combinatorial-line.md) with active set $S$ maps to the [arithmetic progression](../../../../../../arithmetic-progression.md) $a,a+q,\ldots,a+(k-1)q$, where $a\geq1$ and its [common difference](../../../../../../common-difference.md) is $q=|S|>0$. The [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) makes this progression [monochromatic](../../../../../../monochromatic-set.md). Length one is trivial, so every [finite coloring](../../../../../../finite-coloring.md) of the [positive integers](../../../../../../positive-integer.md) contains [monochromatic](../../../../../../monochromatic-set.md) [arithmetic progressions](../../../../../../arithmetic-progression.md) of every finite length.

**The active-coordinate obstruction.** Color a word red when its first coordinate is $1$, and blue otherwise. Any [combinatorial line](../../../../../../combinatorial-line.md) whose active coordinate set contains $1$ has a red word at variable value $1$ and a blue word at variable value $2$, since $m>1$. Thus

$$
\boxed{\{S\subseteq[n]:1\in S\}\text{ is not adequate}.}
$$

Here adequacy is the [adequate family of active coordinate sets](../../../../../../adequate-family-of-active-coordinate-sets.md) property; an active coordinate set is always nonempty.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
