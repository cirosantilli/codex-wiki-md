<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $C_*(X)$ be the integral [singular chain complex](../../../../../singular-chain-complex.md). Augment it by the homomorphism $C_0(X)\to\mathbb Z$ sending every point simplex to one. The [homology](../../../../../homology-split.md) of this augmented complex is [reduced homology](../../../../../reduced-homology.md): for a nonempty space, it agrees with ordinary [homology](../../../../../homology-split.md) in positive degrees and $\widetilde H_0(X)$ is the kernel of $H_0(X)\to\mathbb Z$. The [relative homology](../../../../../relative-homology.md) $H_*(X,A)$ is the [homology](../../../../../homology-split.md) of $C_*(X)/C_*(A)$; a relative cycle has boundary in $A$, and chains differing by a boundary or a chain in $A$ represent the same class.

[Excision theorem](../../../../../excision-theorem.md): if $U\subset A\subset X$ and $\overline U\subset\operatorname{int}_X A$, the inclusion $(X\setminus U,A\setminus U)\hookrightarrow(X,A)$ induces isomorphisms on all [relative homology](../../../../../relative-homology.md) groups. In particular, for a nonempty [CW subcomplex](../../../../../cw-subcomplex.md) $A$, choose a neighborhood $N$ deforming onto $A$, with the deformation fixing $A$. Such neighborhoods exist for [CW pairs](../../../../../cw-pair.md). Then $N/A$ is contractible. The [long exact sequence of a pair](../../../../../long-exact-sequence-in-relative-homology.md) gives $H_*(X,A)\cong H_*(X,N)$ and $H_*(X/A,\{*\})\cong H_*(X/A,N/A)$. Excision removes $A$ and the collapsed point respectively; the resulting pairs $(X\setminus A,N\setminus A)$ and $((X/A)\setminus\{*\},(N/A)\setminus\{*\})$ are homeomorphic. Consequently

$$
\boxed{H_*(X,A;\mathbb Z)\cong\widetilde H_*(X/A;\mathbb Z).}
$$

Here the nonempty-subcomplex condition is the usual quotient convention in this statement. If $A=\varnothing$, use the pointed cofiber $X_+$ with a disjoint basepoint; the literal unpointed quotient $X/\varnothing=X$ would not give the asserted degree-zero identity.

For one embedded circle, its [long exact sequence of a pair](../../../../../long-exact-sequence-in-relative-homology.md) reduces to

$$
0\longrightarrow\mathbb Z\longrightarrow H_2(\Sigma_g,A)\longrightarrow\mathbb Z
\xrightarrow{i_*}\mathbb Z^{2g}\longrightarrow H_1(\Sigma_g,A)\longrightarrow0,
\qquad H_0(\Sigma_g,A)=0.
$$

A separating circle bounds a subsurface, so its [homology class](../../../../../homology-class.md) is zero. A nonseparating circle has a transverse closed curve meeting it once, showing that its class is nonzero and primitive. Thus $i_*$ is either zero or an injection with torsion-free cokernel. The resulting possibilities are

$$
\boxed{\begin{array}{c|cc}
 &H_2(\Sigma_g,A)&H_1(\Sigma_g,A)\\\hline
[A]=0&\mathbb Z^2&\mathbb Z^{2g}\\
[A]\ne0&\mathbb Z&\mathbb Z^{2g-1}
\end{array}}
$$

with all other relative groups zero. These ranks determine whether the circle is [null-homologous](../../../../../null-homologous-cycle.md).

For $g\geq2$, a disk boundary and a separating circle bounding a once-punctured torus have the same relative groups. The first is [null-homotopic](../../../../../null-homotopic-map.md); the second is not. For a direct verification, use the surface-group presentation $\langle a_1,b_1,\ldots,a_g,b_g\mid\prod_i[a_i,b_i]=1\rangle$. Send $a_1,b_1$ to free generators $u,v$, send $a_2,b_2$ to $v,u$, and all remaining generators to one. The relation maps to $[u,v][v,u]=1$, so this defines a homomorphism to the [free group](../../../../../free-group.md). The separating circle represents $[a_1,b_1]$ and maps to the nonempty reduced word $uvu^{-1}v^{-1}$; it is therefore not null-homotopic. This proves the requested failure to detect nullhomotopy. There is a necessary low-genus qualification: **on $\Sigma_0$ or $\Sigma_1$, an embedded circle is nullhomologous exactly when it is nullhomotopic**. On the sphere every circle bounds a disk; on the torus every essential embedded circle is nonseparating. The printed nondetection assertion therefore needs $g\geq2$.

For two disjoint embedded circles let $r$ be the rank of their image in $H_1(\Sigma_g)$, and let $c$ be the number of connected components of the cut surface. Removing open annular neighborhoods and applying [excision](../../../../../excision-theorem.md) gives the compact cut surface $W$ relative to its boundary. [Poincare-Lefschetz duality](../../../../../lefschetz-duality.md) gives $H_2(W,\partial W)\cong H^0(W)=\mathbb Z^c$ and $H_1(W,\partial W)\cong H^1(W)$, which is free. Thus there is no hidden torsion. The long exact sequence gives $c=3-r$, and the [Euler characteristic](../../../../../euler-characteristic.md) of the pair is $2-2g$, giving

$$
\boxed{H_2(\Sigma_g,A)=\mathbb Z^{3-r},\qquad H_1(\Sigma_g,A)=\mathbb Z^{2g+1-r},\qquad H_j=0\ (j\ne1,2).}
$$

The possibilities are $r=0,1,2$: two separating circles give zero; a nonseparating circle with a disk boundary, or two parallel essential circles, give one; circles around two different handles give two. For genus zero only $r=0$ occurs; for genus one $r=0,1$ occur; for every genus at least two all three occur. This is [relative homology of a surface modulo disjoint circles](../../../../../relative-homology-of-a-surface-modulo-disjoint-circles.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
