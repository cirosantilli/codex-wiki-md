<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [binary block code](../../../../../binary-block-code.md) of length $N$ is a nonempty subset $C\subseteq\mathbb F_2^N$. Its size is $|C|$, the number of distinct [codewords](../../../../../codeword.md). The [Hamming distance](../../../../../hamming-distance.md) $d(x,y)$ counts coordinates at which two words differ. The code's [minimum Hamming distance](../../../../../minimum-distance-of-a-code.md) is $\min_{x\ne y\in C}d(x,y)$ when there are at least two words. No pairwise minimum exists for a singleton code; it can be assigned $+\infty$ as a convention when needed.

A [binary linear code](../../../../../binary-linear-code.md) is a [vector subspace](../../../../../vector-subspace.md) of $\mathbb F_2^N$. If its [dimension](../../../../../dimension-vector-space.md) is $k$, a [generator matrix](../../../../../generator-matrix.md) $G$ has a basis of $C$ as its $k$ rows, giving

$$
C=\{uG:u\in\mathbb F_2^k\},\qquad |C|=2^k.
$$

To match the coordinate-row convention, take a [parity-check matrix](../../../../../parity-check-matrix.md) $P$ of size $N\times(N-k)$, with independent columns, and define

$$
C=\{x\in\mathbb F_2^N:xP=0\}.
$$

The transpose $H=P^T$ is the usual [parity-check matrix](../../../../../parity-check-matrix.md) with one column per coordinate. By [rank-nullity theorem](../../../../../rank-nullity-theorem.md), the displayed kernel has [dimension](../../../../../dimension-vector-space.md) $k$. The two constructions agree when $GP=0$: the generator's row space lies in the parity-check kernel and has the same [dimension](../../../../../dimension-vector-space.md), hence equals it. Conversely, for a given $C$, choose the columns of $P$ as a basis of its [dual code](../../../../../dual-code.md) $C^\perp$; orthogonality and the [dimension](../../../../../dimension-vector-space.md) formula give exactly $C$ as the kernel.

For a nonzero [linear code](../../../../../linear-code.md), $x-y$ is a nonzero [codeword](../../../../../codeword.md) whenever $x,y$ are distinct [codewords](../../../../../codeword.md), and $d(x,y)=\operatorname{wt}(x-y)$. Conversely compare any nonzero [codeword](../../../../../codeword.md) with zero. Thus the [minimum Hamming distance of a linear code](../../../../../minimum-hamming-distance-of-a-linear-code.md) is the least nonzero [Hamming weight](../../../../../hamming-weight.md).

Write $P_i$ for the row associated with coordinate $i$. A nonzero binary vector $x$ is a [codeword](../../../../../codeword.md) exactly when

$$
xP=\sum_{i:x_i=1}P_i=0.
$$

Its nonzero coordinate positions therefore index a [linearly dependent](../../../../../linear-dependence.md) set of rows. Conversely, a dependence among a set of rows has coefficients in $\mathbb F_2$, not all zero; putting these coefficients in the corresponding coordinates gives a nonzero [codeword](../../../../../codeword.md) of weight no greater than the number of rows in that set. Taking minima in both directions proves the [parity-check dependencies determine minimum distance](../../../../../parity-check-dependencies-determine-minimum-distance.md) criterion:

$$
\boxed{d(C)=\min\{|S|:(P_i)_{i\in S}\text{ is linearly dependent}\}}.
$$

Rows here are indexed by positions: equal row vectors at different positions are two distinct members of the indexed family. In the usual matrix convention, the same result refers to columns of $H=P^T$. For the zero code, neither a nonzero [codeword](../../../../../codeword.md) nor a dependent coordinate set exists, so both minima can consistently be interpreted as $+\infty$.

For the [Hamming code](../../../../../hamming-code.md), let $l\geq1$, set $N=2^l-1$, and let the rows of $P$ be all nonzero vectors of $\mathbb F_2^l$, each once. These rows include the standard basis, so $P$ has rank $l$ and the code has [dimension](../../../../../dimension-vector-space.md) $N-l$ and size $2^{N-l}$. There is no dependence involving one row, because no row is zero, or two rows, because no rows are equal. For $l\geq2$, any two distinct nonzero vectors $a,b$ have a distinct nonzero sum $a+b$, which is another row. These three rows sum to zero. Thus $d(C)=3$ for $l\geq2$.

The [perfectness of a Hamming code](../../../../../perfectness-of-a-hamming-code.md) also has a direct decoding proof. Given any received word $y$, its [syndrome](../../../../../syndrome.md) is $yP\in\mathbb F_2^l$. A zero [syndrome](../../../../../syndrome.md) means $y\in C$. Otherwise it equals exactly one row $P_i$. The vector $y+e_i$ then has [syndrome](../../../../../syndrome.md) zero and is the unique [codeword](../../../../../codeword.md) obtainable by changing one coordinate. There is no other [codeword](../../../../../codeword.md) at distance at most one: its necessary correction would have to have the same [syndrome](../../../../../syndrome.md), and among zero and all single-coordinate errors the [syndromes](../../../../../syndrome.md) are precisely the distinct $2^l$ vectors of $\mathbb F_2^l$. Therefore the radius-one [Hamming balls](../../../../../hamming-ball.md) about [codewords](../../../../../codeword.md) partition $\mathbb F_2^N$.

Equivalently, each ball contains $1+N=2^l$ words; disjointness and $2^{N-l}2^l=2^N$ show that none are uncovered. Hence **every nondegenerate binary Hamming code is a perfect single-error-correcting code**. For $l=1$, the construction is the singleton code $\{0\}\subseteq\mathbb F_2$, whose one radius-one ball is also the whole ambient space. This deals with the degenerate boundary without falsely claiming its minimum distance is three.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
