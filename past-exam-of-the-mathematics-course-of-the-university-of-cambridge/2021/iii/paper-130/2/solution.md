<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) says that, for every finite alphabet $A$ and number of colors $r$, there is $N$ such that every $r$-coloring of $A^N$ contains a monochromatic [combinatorial line](../../../../../combinatorial-line.md).

We use the standard insensitivity lemma. Assuming the Hales-Jewett theorem for alphabets of size $m-1$, fix two letters $a,b$ in an $m$-letter alphabet. For every $r$ and $d$, there is $N$ such that each $r$-coloring of $A^N$ has a $d$-dimensional [combinatorial subspace](../../../../../combinatorial-subspace.md) on which changing any selection of variable coordinates from $a$ to $b$, or from $b$ to $a$, leaves the color unchanged.

Here is the finite fusion proof of the lemma. Choose the sizes of $d$ successive coordinate blocks backwards. On the last block, omit $b$ and color a word over $A\setminus\{b\}$ by the vector of all colors obtained after filling the previously chosen blocks in every possible way and then replacing any chosen occurrences of $a$ by $b$. This is a finite derived coloring. The induction hypothesis supplies a combinatorial line on which that entire vector is constant. Treat its active coordinates as one new variable block and repeat. After $d$ repetitions, each replacement of $a$ by $b$ can be pushed into the last block where it was created, and equality of the derived color vectors shows that it does not alter the original color. This proves the insensitivity lemma.

Now induct on $m=|A|$. The case $m=1$ is immediate. For $m>1$, choose the target dimensions backwards and apply the insensitivity lemma successively to the pairs

$$
(a_m,a_1),\ldots,(a_m,a_{m-1}).
$$

At every step pass to the resulting nested combinatorial subspace, so the insensitivities already obtained are retained. On the final positive-dimensional subspace, replacing $a_m$ by any other letter does not change the color. Any two words can be connected by such replacements, so the whole subspace is monochromatic. It contains a combinatorial line, completing the induction and the proof.

The [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md) says that, for every finite $S\subseteq\mathbb N^d$ and every finite coloring of $\mathbb N^d$, there are $u\in\mathbb N^d$ and $q\geq1$ such that the homothetic copy

$$
u+qS=\{u+qs:s\in S\}
$$

is monochromatic.

Write $S=\{s_1,\ldots,s_m\}$ and apply the Hales-Jewett theorem to the alphabet $[m]$. Color a word $w\in[m]^N$ by the color of

$$
\Phi(w)=t+\sum_{j=1}^Ns_{w_j},
$$

where a fixed positive vector $t$ keeps the image in $\mathbb N^d$ under either convention for the natural numbers. On a monochromatic combinatorial line, let $I$ be the active coordinate set. The fixed coordinates contribute a vector $u-t$, while the word whose active letter is $i$ maps to

$$
u+|I|s_i.
$$

These points form a monochromatic copy $u+|I|S$, proving Gallai's theorem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
