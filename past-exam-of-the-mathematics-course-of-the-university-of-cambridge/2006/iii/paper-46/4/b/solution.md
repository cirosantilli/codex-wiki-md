<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A metric dissimilarity $d$ must satisfy nonnegativity, separation, symmetry and the triangle inequality:

$$
\boxed{d(x,y)\geq0;\quad d(x,y)=0\iff x=y;\quad d(x,y)=d(y,x);\quad d(x,z)\leq d(x,y)+d(y,z).}
$$

The underlying objects must be specified: here they are binary measurement profiles, rather than labels attached to individuals.

Let $n_{11},n_{00},n_{10},n_{01}$ count coordinate pairs of the indicated types. The [simple matching coefficient](../../../../../../simple-matching-coefficient.md) is $S=(n_{11}+n_{00})/4$, so its complementary dissimilarity is $(n_{10}+n_{01})/4$. Counting mismatches in every pair gives the [dissimilarity matrix](../../../../../../dissimilarity-matrix.md)

$$
\boxed{D_S=\begin{pmatrix}
0&3/4&1/4&3/4\\
3/4&0&1/2&1/2\\
1/4&1/2&0&1/2\\
3/4&1/2&1/2&0
\end{pmatrix}.}
$$

For the [Jaccard coefficient](../../../../../../jaccard-index.md), joint absences are excluded: $J=n_{11}/(n_{11}+n_{10}+n_{01})$. Thus the [Jaccard distance](../../../../../../jaccard-distance.md) is $1-J$, giving

$$
\boxed{D_J=\begin{pmatrix}
0&3/4&1/4&3/4\\
3/4&0&1/2&2/3\\
1/4&1/2&0&1/2\\
3/4&2/3&1/2&0
\end{pmatrix}.}
$$

Only the pair of individuals two and four has a joint absence. Their profiles have one shared presence, two mismatched presences and one joint absence, giving dissimilarities $2/4$ and $2/3$, respectively. All other pairs have a presence in at least one profile at every coordinate, so the two denominators coincide.

For the requested [metric property of simple matching dissimilarity](../../../../../../metric-property-of-simple-matching-dissimilarity.md), write a general pair of $p$-coordinate binary profiles as $x,y$. Then

$$
d_S(x,y)=1-S(x,y)=\frac1p\sum_{j=1}^p\mathbf1_{\{x_j\ne y_j\}},
$$

which is the [normalized Hamming distance](../../../../../../normalized-hamming-distance.md). It is nonnegative and symmetric, and equals zero exactly when all coordinates match. For each coordinate, a mismatch between $x_j$ and $z_j$ forces a mismatch between $x_j,y_j$ or between $y_j,z_j$. Therefore

$$
\mathbf1_{\{x_j\ne z_j\}}\leq\mathbf1_{\{x_j\ne y_j\}}+\mathbf1_{\{y_j\ne z_j\}}.
$$

Summing and dividing by $p$ proves the triangle inequality, establishing all four metric properties. **Simple matching dissimilarity is a metric on binary profiles.** If two separately labelled individuals have identical profiles, it gives zero distance between them, so on those labels it is only a [pseudometric](../../../../../../pseudometric.md). The four profiles here are distinct, so this distinction does not prevent $D_S$ from defining a metric on the given sample.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
