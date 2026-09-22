<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**Euler number and self-intersection.** Orient the rank-two [normal bundle](../../../../../normal-bundle.md) $\nu_S$ by the orientations of $S$ and $M$: the ordered tangent and normal spaces have the ambient orientation. Choose a smooth normal section $s$ transverse to the zero section. Its zeros are isolated, and their signed number is the evaluation $\langle e(\nu_S),[S]\rangle$ of the [Euler class](../../../../../euler-class-of-a-vector-bundle.md) on the [fundamental class](../../../../../fundamental-class.md). Scale the section sufficiently small to lie in a [tubular neighborhood](../../../../../tubular-neighborhood.md). Its graph is a push-off $S'$ isotopic to $S$.

The intersections of $S$ with $S'$ occur exactly at the zeros of $s$. In a positively oriented local splitting $TS\oplus\nu_S$, the basis formed from the tangent spaces to $S$ and to the graph has block matrix

$$
\begin{pmatrix}I&I\\0&Ds\end{pmatrix}.
$$

Its [determinant](../../../../../determinant.md) is $\det Ds$, so the local intersection sign is precisely the local zero index of the section. Summing proves the [Euler number equals self-intersection](../../../../../euler-number-equals-self-intersection.md) identity

$$
\boxed{\langle e(\nu_S),[S]\rangle=S\cdot S'=[S]\cdot[S].}
$$

**The conic.** The given map is the degree-two [Veronese map](../../../../../veronese-map.md) $[u:v]\mapsto[u^2:uv:v^2]$ followed by the [projective linear transformation](../../../../../projective-linear-transformation.md)

$$
A=\begin{pmatrix}1&0&1\\0&1&0\\1&0&-1\end{pmatrix},
\qquad \det A=-2\ne0.
$$

The [Veronese map](../../../../../veronese-map.md) is injective with nonvanishing differential: on the chart $u\ne0$ its coordinates are $[1:t:t^2]$, and on $v\ne0$ they are $[s^2:s:1]$. It is therefore a [smooth embedding](../../../../../smooth-embedding.md), and $S$ is a [smooth plane conic](../../../../../smooth-plane-conic.md) diffeomorphic to $\mathbb{CP}^1\cong S^2$. Its equation in the given coordinates is $z_0^2-z_2^2=4z_1^2$.

Let $L$ be a projective line, with its complex orientation. The [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md) gives $[L]\cdot[L]=1$ in $\mathbb{CP}^2$. The hyperplane $z_1=0$ meets $S$ at $[u:v]=[1:0]$ and $[0:1]$. The zeros of $uv$ are simple in the respective local coordinates, and complex intersections have positive signs. Hence $[S]\cdot[L]=2$, so $[S]=2[L]$. The [self-intersection number](../../../../../self-intersection-number.md) and the normal [Euler class](../../../../../euler-class-of-a-vector-bundle.md) are

$$
\boxed{[S]\cdot[S]=4,\qquad e(\nu_S)=4u,}
$$

where $u\in H^2(S^2;\mathbb Z)$ has $\langle u,[S^2]\rangle=1$.

**The boundary of the tubular neighborhood.** Write $N=\nu(S)$ for the closed disk [tubular neighborhood](../../../../../tubular-neighborhood.md) and $E=\partial N$ for its boundary. This distinguishes the disk neighborhood $N$ from the vector [normal bundle](../../../../../normal-bundle.md) $\nu_S$. The space $E$ is the oriented [circle bundle](../../../../../circle-bundle.md) of $\nu_S$, with [Euler class](../../../../../euler-class-of-a-vector-bundle.md) $4u$. The [Gysin sequence](../../../../../gysin-sequence-of-a-sphere-bundle.md) contains

$$
0\to H^1(E;\mathbb Z)\to H^0(S^2;\mathbb Z)
\xrightarrow{\;\smile\,4u\;}H^2(S^2;\mathbb Z)
\to H^2(E;\mathbb Z)\to0.
$$

The middle map is multiplication by four, yielding $H^1(E;\mathbb Z)=0$ and $H^2(E;\mathbb Z)=\mathbb Z/4$. The same [Gysin sequence](../../../../../gysin-sequence-of-a-sphere-bundle.md) gives $H^0(E;\mathbb Z)=H^3(E;\mathbb Z)=\mathbb Z$. The total space is a closed connected oriented three-manifold, so [Poincare duality](../../../../../poincare-duality.md) gives

$$
\boxed{H_k(\partial\nu(S);\mathbb Z)\cong
\begin{cases}
\mathbb Z,&k=0,3,\\
\mathbb Z/4,&k=1,\\
0,&\text{otherwise}.
\end{cases}}
$$

**The exterior.** Work first with $W=\mathbb{CP}^2\setminus\operatorname{int}N$. A [collar neighborhood](../../../../../collar-neighbourhood.md) of $\partial W$ shows that its interior, the requested $\mathbb{CP}^2\setminus N$, has the same [homotopy equivalence](../../../../../homotopy-equivalence.md) type: push the boundary a small positive distance into the collar. The [Excision theorem](../../../../../excision-theorem.md) and [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) identify

$$
H_k(\mathbb{CP}^2,W;\mathbb Z)
\cong H_k(N,E;\mathbb Z)
\cong H_{k-2}(S^2;\mathbb Z).
$$

Only degrees two and four are nonzero, each a copy of $\mathbb Z$.

In degree four the map $H_4(\mathbb{CP}^2;\mathbb Z)\to H_4(N,E;\mathbb Z)$ sends the ambient [fundamental class](../../../../../fundamental-class.md) to the relative [fundamental class](../../../../../fundamental-class.md) of $N$. Under the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) this becomes $[S]$. Thus this map is multiplication by **one** with compatible orientations. The [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) gives

$$
0\to H_4(W;\mathbb Z)\to\mathbb Z
\xrightarrow{\;1\;}\mathbb Z\to H_3(W;\mathbb Z)\to0,
$$

so $H_4(W)=H_3(W)=0$.

In degree two, the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) identifies the map $H_2(\mathbb{CP}^2)\to H_0(S^2)$ with intersection against $[S]$. A projective line intersects the conic twice, so this map is multiplication by **two**. The [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) is

$$
0\to H_2(W;\mathbb Z)\to\mathbb Z
\xrightarrow{\;2\;}\mathbb Z\to H_1(W;\mathbb Z)\to0.
$$

It yields $H_2(W)=0$ and $H_1(W)=\mathbb Z/2$. In degree zero the relative groups vanish, so $H_0(W)\cong H_0(\mathbb{CP}^2)\cong\mathbb Z$. This computes the [homology of the complement of a smooth conic](../../../../../homology-of-the-complement-of-a-smooth-conic.md):

$$
\boxed{H_k(\mathbb{CP}^2\setminus\nu(S);\mathbb Z)\cong
\begin{cases}
\mathbb Z,&k=0,\\
\mathbb Z/2,&k=1,\\
0,&k\geq2.
\end{cases}}
$$

The normal Euler number $4$, the degree-two intersection map and the degree-four restriction map $1$ play different roles; distinguishing them explains why the boundary has first [homology](../../../../../homology-split.md) $\mathbb Z/4$ while the exterior has first [homology](../../../../../homology-split.md) $\mathbb Z/2$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
