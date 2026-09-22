<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Identify the [vertices](../../../../../../vertex-graph-theory.md) of the [Boolean hypercube](../../../../../../boolean-hypercube.md) with subsets of $[n]$. Write $N(\mathcal A)$ for the closed [vertex neighbourhood](../../../../../../vertex-neighbourhood.md) and $\partial\mathcal A=N(\mathcal A)\setminus\mathcal A$ for the [external vertex boundary](../../../../../../external-vertex-boundary.md). The [cube order](../../../../../../simplicial-order-on-the-discrete-cube.md) used here is the [simplicial order on the discrete cube](../../../../../../simplicial-order-on-the-discrete-cube.md): increasing size, then [lexicographic order](../../../../../../lexicographic-order.md), with the smallest differing coordinate belonging to the earlier set. We prove [Harper theorem](../../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) by induction on $n$; subtracting the common size of the families converts a closed-neighbourhood comparison into the required boundary comparison.

First, the closed neighbourhood of a simplicial [initial segment](../../../../../../initial-segment.md) is itself an initial segment. Such a family consists of full lower levels and a lexicographic initial part of its last level. Its next-level neighbours form the [upper shadow](../../../../../../upper-shadow.md) of that part. For a set in the next level, its lexicographically earliest lower-level subset is obtained by deleting its largest element. This map preserves the lexicographic order weakly. Membership in the upper shadow is equivalent to that earliest subset belonging to the original initial part, so the upper shadow is an initial part too. Empty and full families satisfy the assertion directly.

Assume the theorem in dimension $n-1$. Split $\mathcal A$ into two sections $\mathcal A_0,\mathcal A_1$ according to membership of coordinate $i$, deleting $i$ from the second section. Their closed-neighbourhood sections are

$$
N(\mathcal A)_0=N(\mathcal A_0)\cup\mathcal A_1,\qquad N(\mathcal A)_1=N(\mathcal A_1)\cup\mathcal A_0.
$$

Replace each section by a simplicial initial segment $I_0,I_1$ of the same size. Induction gives $|N(I_j)|\leq|N(\mathcal A_j)|$. By the preceding observation, each $N(I_j)$ is an initial segment and is nested with the other section. Consequently

$$
|N(I_0)\cup I_1|=\max\{|N(I_0)|,|I_1|\}\leq|N(\mathcal A_0)\cup\mathcal A_1|,
$$

and the analogous inequality holds for the other section. Thus [simplicial section compression](../../../../../../simplicial-section-compression.md) preserves size and cannot increase the closed neighbourhood.

Repeatedly apply a nontrivial section compression. The sum of the positions of the family members in the full simplicial order strictly decreases: the order induced on either fixed-coordinate section is precisely its lower-dimensional simplicial order. This positive integer potential makes the process terminate at a family $\mathcal B$ fixed by every section compression.

We classify such [terminal families for simplicial section compression](../../../../../../terminal-families-for-simplicial-section-compression.md). If an earlier vertex $x$ is absent while a later vertex $y$ is present, they cannot agree at any coordinate, since the corresponding section is an initial segment. Hence $y=x^c$. Every other vertex earlier than $y$ is present, and every other vertex later than $x$ is absent, since any further inverted pair would also have to be complementary. There can therefore be no vertex strictly between $x$ and $y$. Thus $\mathcal B$ either is an initial segment or is an initial segment with its last vertex replaced by the next, complementary vertex.

The complementary consecutive pairs are explicit. If $n=2r+1$, the ranks must be $r$ and $r+1$, and consecutive order positions force

$$
x=\{r+2,\ldots,2r+1\},\qquad y=\{1,\ldots,r+1\}.
$$

The corresponding initial segment $I$ contains all sets of size at most $r$, and $\mathcal B=I-\{x\}+\{y\}$. Its closed neighbourhood contains all sets of size at most $r+1$: for $r\geq1$, deletion of just one $r$-set cannot remove all the $r$-subsets of any $(r+1)$-set, and $x$ remains adjacent to one of its $(r-1)$-subsets. In addition, the $r$ supersets of $y$ of size $r+2$ enter the neighbourhood. Thus $|N(\mathcal B)|=|N(I)|+r$; the $n=1$ case gives equality directly.

If $n=2r$, the two vertices have rank $r$. Complementation reverses the lexicographic order within that rank, so consecutive complements occupy its middle two positions. These are

$$
x=\{1,r+2,\ldots,2r\},\qquad y=\{2,\ldots,r+1\}.
$$

Now $I$ contains all sets of size less than $r$ and all $r$-sets containing coordinate one. Its closed neighbourhood contains all sets of size at most $r$ and all $(r+1)$-sets containing one. For $r\geq2$, each such $(r+1)$-set has at least two $r$-subsets containing one, so exchanging $x$ for $y$ loses none of these neighbours. It adds the $r-1$ supersets of $y$ of size $r+1$ that avoid one. Hence $|N(\mathcal B)|=|N(I)|+r-1$. For $n=2$ the two neighbourhoods are both the entire cube.

In both exceptional cases the initial segment has no larger neighbourhood. The induction starts with the one-vertex zero-dimensional cube, and the compression argument now proves

$$
\boxed{|\partial\mathcal A|\geq|\partial I|\qquad(|I|=|\mathcal A|).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
