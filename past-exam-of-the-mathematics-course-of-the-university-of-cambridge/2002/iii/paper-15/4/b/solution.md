<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [compact Riemann surface](../../../../../../compact-riemann-surface.md) $X=\mathbb P^1$ and the [holomorphic vector bundle](../../../../../../holomorphic-vector-bundle.md) $E=\mathcal O_X\oplus\mathcal O_X$. For every positive integer $m$, use homogeneous coordinates $[Z_0:Z_1]$ and the map

$$
\mathcal O_X(-m)\longrightarrow\mathcal O_X^{\oplus2},\qquad
s\longmapsto(Z_0^m s,Z_1^m s).
$$

The two sections $Z_0^m,Z_1^m$ never vanish together on $\mathbb P^1$. Thus this map has rank one at every point; locally one of its two components is invertible in suitable line-bundle frames, so its image is a genuine [holomorphic subbundle](../../../../../../holomorphic-subbundle.md) and its quotient is a [locally free sheaf](../../../../../../locally-free-sheaf.md). More explicitly, there is an [exact sequence](../../../../../../exact-sequence.md)

$$
0\longrightarrow\mathcal O_X(-m)
\xrightarrow{(Z_0^m,Z_1^m)}\mathcal O_X^{\oplus2}
\xrightarrow{(-Z_1^m,Z_0^m)}\mathcal O_X(m)
\longrightarrow0.
$$

Exactness follows fibrewise from the absence of a common zero and hence also locally as a sequence of vector bundles. The image $F_m$ is isomorphic to $\mathcal O_X(-m)$ and has rank one, so

$$
\boxed{\mu(F_m)=\deg\mathcal O_X(-m)=-m\longrightarrow-\infty.}
$$

Thus **there need not be a lower bound for subbundle slopes**, even for a fixed trivial rank-two bundle. Merely multiplying a section of one fixed subline by a function with zeros would not suffice: that could give only a subsheaf with a torsion quotient. The nowhere-simultaneously-zero pair above avoids that problem and realizes [unbounded negative degrees of line subbundles](../../../../../../unbounded-negative-degrees-of-line-subbundles.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
