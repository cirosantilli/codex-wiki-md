# Stirling numbers of the second kind

↑ **Parent:** [Set partition](set-partition.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stirling_numbers_of_the_second_kind)

For [nonnegative integers](natural-number.md) $n,k$, the [Stirling number of the second kind](stirling-numbers-of-the-second-kind.md)

$$
S(n,k)=\left\{\begin{matrix}n\\k\end{matrix}\right\}
$$

counts the [set partitions](set-partition.md) of an $n$-element [finite set](finite-set.md) into exactly $k$ unlabelled [blocks of a set partition](block-of-a-set-partition.md). Set $S(0,0)=1$, $S(n,0)=0$ for $n>0$, and $S(n,k)=0$ for $k>n$. Also $S(n,1)=S(n,n)=1$ for $n\geq1$. Grassl and Levin develop these counts through explicit [set partitions](set-partition.md) and a [recurrence relation](recurrence-relation.md). [Grassl and Levin, More Discrete Mathematics via Graph Theory, section 3.1: counting partitions](https://discrete.openmathbooks.org/more/mdm/sec_adv-partitions.html)

**Insert one distinguished element.** For $n\geq1$ and $1\leq k\leq n$, the [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md) obey

$$
S(n,k)=kS(n-1,k)+S(n-1,k-1).
$$

**Proof outline.** Inspect the [block of a set partition](block-of-a-set-partition.md) containing $n$. If it contains another element, removing $n$ leaves a [set partition](set-partition.md) into $k$ [blocks of a set partition](block-of-a-set-partition.md); conversely, insert $n$ into any of those $k$ [blocks of a set partition](block-of-a-set-partition.md). If $n$ is alone, remove its [singleton set](singleton-mathematics.md) and obtain a [set partition](set-partition.md) into $k-1$ [blocks of a set partition](block-of-a-set-partition.md). The cases cannot overlap, and deletion reverses each construction. This explains the factor $k$ even though the [blocks of a set partition](block-of-a-set-partition.md) have no names. [Grassl and Levin, More Discrete Mathematics via Graph Theory, section 3.4: Stirling recurrence](https://discrete.openmathbooks.org/more/mdm/sec_adv-stirling.html)

For $n=4,k=2$, start with the three two-block [set partitions](set-partition.md) of $\{1,2,3\}$. Inserting $4$ into either [block of a set partition](block-of-a-set-partition.md) gives six possibilities. The remaining possibility is $\{\{1,2,3\},\{4\}\}$, obtained by making $4$ a [singleton set](singleton-mathematics.md). Hence $S(4,2)=2\cdot3+1=7$. The seven [set partitions](set-partition.md) in the diagram comprise four with sizes $3+1$ and three with sizes $2+2$; this grouping by sizes independently gives $4+3=7$.

<a id="image-exact-construction-of-all-seven-two-block-set-partitions-of-1-2-3-4-six-insert-4-into-an-existing-block-of-a-set-partition-and-one-creates-a-singleton-set"></a>
![](set-partitions-stirling-insert-four.png)

**[Figure 16](#image-exact-construction-of-all-seven-two-block-set-partitions-of-1-2-3-4-six-insert-4-into-an-existing-block-of-a-set-partition-and-one-creates-a-singleton-set). Exact construction of all seven two-block set partitions of $\{1,2,3,4\}$: six insert $4$ into an existing block of a set partition, and one creates a singleton set**.

**Three different counting questions.** The [binomial coefficient](binomial-coefficient.md) $\binom nk$ selects one $k$-element [subset](subset.md). The [Stirling number of the second kind](stirling-numbers-of-the-second-kind.md) $S(n,k)$ groups all $n$ distinct elements into $k$ nonempty unnamed [blocks of a set partition](block-of-a-set-partition.md). The power $k^n$ counts all [functions](function-split.md) to a specified $k$-element [finite set](finite-set.md), allowing some destination labels to go unused. At $n=4,k=2$, these counts are respectively $6$, $7$, and $16$. Choosing two people, making two unnamed nonempty teams, and assigning each person a red or blue label are different tasks.

**When the destinations have labels.** For fixed [finite sets](finite-set.md) $X,Y$ of sizes $n,k$, respectively, the number of [surjective functions](surjective-function.md) $X\to Y$ is

$$
\#\{f:X\to Y\mid f\text{ is surjective}\}=k!S(n,k).
$$

Here every element of $Y$ must be used. Each [surjective function](surjective-function.md) gives a [set partition](set-partition.md) of $X$ into its nonempty [preimages](preimage.md) $f^{-1}(\{y\})$. Conversely, assign the $k$ distinct destination labels to the $k$ [blocks of a set partition](block-of-a-set-partition.md) in $k!$ ways, where $k!$ is a [factorial](factorial.md). For two labelled teams of four people this gives $2!\cdot7=14$: of the $2^4=16$ assignments, exactly two use only one label. Dividing arbitrary [function](function-split.md) counts by $k!$ fails in general because unused labels can be permuted without changing a [function](function-split.md). For example, $3^4/3!=13.5$ cannot count [set partitions](set-partition.md). The empty-to-empty [function](function-split.md) is a [surjection](surjective-function.md), consistent with $0!S(0,0)=1$. Stanley gives the [bijection](bijection.md) underlying this qualification.[section 1.9: Twelvefold Way entry 3](enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley.md)

For example, the [inclusion-exclusion principle](inclusion-exclusion-principle.md) counts the [surjections](surjective-function.md) from four elements to three labelled destinations as $3^4-3\cdot2^4+3\cdot1^4=36$. Thus $S(4,3)=36/3!=6$. An independent check chooses the only two-element [block of a set partition](block-of-a-set-partition.md) in $\binom42=6$ ways; the other two elements form [singleton sets](singleton-mathematics.md).

**Why these numbers also occur in algebra.** Classifying all [functions](function-split.md) to an $m$-element [finite set](finite-set.md) by the size $k$ of their [image](image-of-a-function.md) gives

$$
m^n=\sum_{k=0}^n S(n,k)(m)_k,\qquad (m)_k=m(m-1)\cdots(m-k+1),\quad (m)_0=1.
$$

For a fixed [set partition](set-partition.md), the [falling factorial](falling-factorial.md) $(m)_k$ counts assignments of distinct labels to its $k$ [blocks of a set partition](block-of-a-set-partition.md), and is zero when $k>m$. At $n=3,m=4$, this reads $64=1\cdot4+3\cdot12+1\cdot24$. Replacing $m$ by $x$ yields a [polynomial](polynomial-split.md) identity: both sides agree at every [nonnegative integer](natural-number.md). Thus the [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md) translate powers into [falling factorials](falling-factorial.md). Grouping by equal values turns a counting rule into an algebraic change of coordinates. Summing $S(n,k)$ without destination labels instead gives the [Bell number](bell-number.md).

**Table of contents**

- [Bell number](bell-number.md)
- [Graphical Stirling number](graphical-stirling-number.md)

## ↑ Ancestors (5)

1. [Set partition](set-partition.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bell number](bell-number.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
