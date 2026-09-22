<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

All groups in the first calculation have integral coefficients. Let $U=S^n\setminus j(W)$ and $V=S^n\setminus\operatorname{int}j(W)$. A two-sided [tubular neighborhood](../../../../../tubular-neighborhood.md) of $j(\partial W)$ identifies $V$ as a compact [manifold with boundary](../../../../../manifold-with-boundary.md), with interior $U$. Pushing its boundary inward in a [collar neighborhood](../../../../../collar-neighbourhood.md) gives a [homotopy equivalence](../../../../../homotopy-equivalence.md) $U\simeq V$. After thickening across the same collar, [excision](../../../../../excision-theorem.md) identifies the relative groups

$$
H_r(S^n,V)\cong H_r(W,\partial W).
$$

The orientation of $S^n$ gives $W$ an orientation. The [Poincare-Lefschetz duality](../../../../../lefschetz-duality.md) isomorphism therefore gives

$$
H_r(S^n,V)\cong H^{n-r}(W).
$$

Each component of $W$ has boundary: a closed component would have open image by the local embedding condition and closed image by compactness, hence would occupy the whole connected sphere, leaving no room for the components with boundary. In particular $U$ is nonempty, and $H^n(W)=0$.

Apply the [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) of $(S^n,V)$, using [reduced homology](../../../../../reduced-homology.md) for the absolute terms. Away from the top-dimensional homology of the sphere, it identifies

$$
\widetilde H_i(U)\cong H^{n-i-1}(W).
$$

The exceptional map is

$$
H_n(S^n)=\mathbb Z\longrightarrow H_n(W,\partial W)=H^0(W)\cong\mathbb Z^r,
$$

where $r$ is the number of components of $W$. Local compatibility of the orientations sends $1$ to $(1,\ldots,1)$, the relative [fundamental classes](../../../../../fundamental-class.md) of all the components. Its kernel is zero and its cokernel is $\widetilde H^0(W)$. Thus the exceptional term has exactly the reduced form required, and all higher groups vanish. We obtain the [Alexander duality](../../../../../alexander-duality.md) formula

$$
\boxed{\widetilde H_i(S^n\setminus j(W);\mathbb Z)
\cong\widetilde H^{n-i-1}(W;\mathbb Z)\quad(i\geq0),}
$$

with negative-index cohomology zero. Ordinary degree zero is recovered by

$$
\boxed{H_0(S^n\setminus j(W);\mathbb Z)\cong
\mathbb Z\oplus\widetilde H^{n-1}(W;\mathbb Z).}
$$

Both formulas depend on the abstract manifold $W$, so they establish the requested independence up to group isomorphism. They make no claim that the complements themselves are homeomorphic or have isomorphic [fundamental groups](../../../../../fundamental-group.md). The argument also covers $n=1$, when the diagonal map handles the degree-zero exception. This is the [complement homology of a compact codimension-zero submanifold](../../../../../complement-homology-of-a-compact-codimension-zero-submanifold.md).

For the second calculation write $F=\mathbb F_2$, $C=S^n\setminus i(M)$ and $c=n-k$. First suppose $c>0$, with $n\geq1$. The rank-$c$ [normal bundle](../../../../../normal-bundle.md) has a mod-two [Thom class](../../../../../thom-class.md), regardless of orientability. A [tubular neighborhood](../../../../../tubular-neighborhood.md), [excision](../../../../../excision-theorem.md) and the homological [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) identify

$$
H_j(S^n,C;F)\cong H_{j-c}(M;F).
$$

The [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) becomes the [Gysin sequence of an embedding](../../../../../gysin-sequence-of-an-embedding.md):

$$
\cdots\longrightarrow H_j(C;F)\longrightarrow H_j(S^n;F)
\xrightarrow{\gamma}H_{j-c}(M;F)
\longrightarrow H_{j-1}(C;F)\longrightarrow\cdots.
$$

The map $\gamma$ takes the mod-two [fundamental class](../../../../../fundamental-class.md) of $S^n$ to that of $M$: restricting to each normal fiber evaluates the Thom class as $1$. Since $M$ is closed and connected, the degree-$n$ map

$$
F=H_n(S^n;F)\longrightarrow H_k(M;F)=F
$$

is an isomorphism. This cancels the exceptional top term and gives $H_i(C;F)=0$ for $i\geq n-1$ when $i>0$. In all the intervening degrees the sphere groups vanish. In degree zero, the remaining $F$ is removed by the augmentation. Consequently the [mod-two homology of a submanifold complement](../../../../../mod-two-homology-of-a-submanifold-complement.md) is

$$
\boxed{\widetilde H_i(C;F)\cong
\begin{cases}
H_{i+k+1-n}(M;F),&0\leq i\leq n-2,\\
0,&i\geq n-1,
\end{cases}}
$$

where negative-index homology of $M$ is zero. To recover ordinary homology, add one copy of $F$ in degree zero and change nothing in positive degrees. For $n=1$ the first range is empty, so the complement of a connected zero-manifold has the homology of a point. For example, codimension at least two gives $H_0(C;F)=F$, while codimension one gives $H_0(C;F)=F^2$ when $n\geq2$.

If $k=n\geq1$, an embedding of the closed connected manifold has image both open and closed in $S^n$, hence is onto; its complement is empty and all its ordinary homology groups vanish. The positive-codimension formula is not asserted in that case. The standard sphere calculations here assume $n\geq1$; in ambient dimension zero the complement of the embedded connected point in $S^0$ is the other point.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
