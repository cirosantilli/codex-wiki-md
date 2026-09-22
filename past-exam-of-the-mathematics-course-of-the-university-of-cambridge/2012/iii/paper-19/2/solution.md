<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [integral homology](../../../../../integral-homology.md) throughout. The [singular chain group](../../../../../singular-chain-group.md) $C_k(X)$ is free on the [continuous maps](../../../../../continuous-map.md) from the standard $k$-simplex to $X$. Since the [boundary operator](../../../../../boundary-operator.md) preserves chains lying in $A$, these form a [chain subcomplex](../../../../../chain-subcomplex.md). The [relative chain complex](../../../../../relative-chain-complex.md) and its [relative homology](../../../../../relative-homology.md) are

$$
C_k(X,A)=C_k(X)/C_k(A),\qquad
\boxed{H_k(X,A)=\ker(\partial:C_k(X,A)\to C_{k-1}(X,A))/\operatorname{im}(\partial:C_{k+1}(X,A)\to C_k(X,A)).}
$$

The [short exact sequence of chain complexes](../../../../../short-exact-sequence-of-chain-complexes.md) gives the [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md).

A sufficient hypothesis for the quotient comparison is a nonempty [good pair](../../../../../good-pair.md): $A$ is closed and has an open neighbourhood $U$ which admits a [deformation retraction](../../../../../deformation-retraction.md) onto $A$ while fixing $A$ throughout. A [CW pair](../../../../../cw-pair.md) is another standard sufficient setting. These hypotheses hold for a simple closed curve in the surface here, using its annular [collar neighbourhood](../../../../../collar-neighbourhood.md). The induced [quotient map](../../../../../quotient-map.md) $q:X\to Y=X/A$ collapses $A$ to a point $a$.

Here is the proof of the [collapsing a pair theorem](../../../../../collapsing-a-pair-theorem.md). Put $V=U/A\subset Y$. The [deformation retraction](../../../../../deformation-retraction.md) makes $H_*(U,A)=0$, so the [long exact sequence](../../../../../long-exact-sequence.md) of the triple gives $H_*(X,A)\cong H_*(X,U)$. It also contracts $V$ onto $a$, giving $H_*(Y,\{a\})\cong H_*(Y,V)$. Because $A$ is closed inside the open neighbourhood $U$, [excision](../../../../../excision-theorem.md) gives

$$
H_*(X,U)\cong H_*(X\setminus A,U\setminus A).
$$

Similarly, [excision](../../../../../excision-theorem.md) of the closed point $a$ in the open set $V$ gives

$$
H_*(Y,V)\cong H_*(Y\setminus\{a\},V\setminus\{a\}).
$$

The [quotient map](../../../../../quotient-map.md) restricts to a [homeomorphism](../../../../../homeomorphism.md) between the two punctured pairs, so these are the same groups and the identifications commute with $q_*$. Finally $H_*(Y,\{a\})\cong\widetilde H_*(Y)$, including degree zero. Thus

$$
\boxed{q_*:H_k(X,A)\xrightarrow{\sim}\widetilde H_k(X/A).}
$$

The neighbourhood condition is part of the result; the quotient assertion is not made for arbitrary bad pairs.

For the genus-two [closed orientable surface](../../../../../closed-orientable-surface.md) with its chosen [orientation](../../../../../orientation-of-a-simplex.md), $H_0(X)=\mathbb Z$, $H_1(X)=\mathbb Z^4$, $H_2(X)=\mathbb Z$, with higher groups zero. The curve has $H_0(A)=H_1(A)=\mathbb Z$. Its relevant [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) is

$$
0\longrightarrow\mathbb Z\longrightarrow H_2(X,A)
\longrightarrow\mathbb Z\xrightarrow{i_*}\mathbb Z^4
\longrightarrow H_1(X,A)\longrightarrow\mathbb Z\xrightarrow{\sim}\mathbb Z\longrightarrow0.
$$

The final map is an [isomorphism](../../../../../isomorphism.md) because both spaces are connected. Consequently $H_1(X,A)=\operatorname{coker}i_*$ and $H_0(X,A)=0$; all relative groups above degree two vanish. The [quotient topological space](../../../../../quotient-topological-space.md) is connected, so its unreduced $H_0$ is $\mathbb Z$.

In the separating case, the curve is the oriented boundary of one of the two subsurfaces. Its [homology class](../../../../../homology-class.md) in $X$ is therefore zero, so $i_*=0$. The [exact sequence](../../../../../exact-sequence.md) becomes

$$
0\to\mathbb Z\to H_2(X,A)\to\mathbb Z\to0,
\qquad H_1(X,A)=\mathbb Z^4.
$$

The first sequence splits since its quotient is a free [abelian group](../../../../../abelian-group.md). Hence the [homology after collapsing a separating surface curve](../../../../../homology-after-collapsing-a-separating-surface-curve.md) is

$$
\boxed{H_k(X/A;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0,\\
\mathbb Z^4,&k=1,\\
\mathbb Z^2,&k=2,\\
0,&k\geq3.
\end{cases}}
$$

Geometrically, collapsing the boundary of each once-punctured [torus](../../../../../torus.md) fills its puncture with a cone on the [circle](../../../../../circle.md), which is a disk. The quotient is a [wedge sum](../../../../../wedge-sum.md) of two tori at the collapsed point. Their two independent [fundamental classes](../../../../../fundamental-class.md) explain the extra second-homology generator.

In the nonseparating case, join the two new boundary components of the cut surface by an arc. Upon regluing, this supplies a closed curve meeting $A$ once transversely. The signed [intersection pairing on an oriented surface](../../../../../intersection-pairing-on-an-oriented-surface.md) therefore provides an integer homomorphism $H_1(X)\to\mathbb Z$ taking $[A]$ to $\pm1$. Thus $[A]$ is a nonzero [primitive homology class](../../../../../primitive-homology-class.md), and $i_*:\mathbb Z\to\mathbb Z^4$ is an injection onto a direct summand. Its kernel is zero and its cokernel is $\mathbb Z^3$. The same [exact sequence](../../../../../exact-sequence.md) gives $H_2(X,A)\cong H_2(X)\cong\mathbb Z$. Therefore the [homology after collapsing a nonseparating surface curve](../../../../../homology-after-collapsing-a-nonseparating-surface-curve.md) is

$$
\boxed{H_k(X/A;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0,2,\\
\mathbb Z^3,&k=1,\\
0,&k\geq3.
\end{cases}}
$$

Another description starts from the genus-one surface with two boundary circles. Collapse those two circles separately to obtain a closed [torus](../../../../../torus.md) with two marked points, then identify the two points. Identifying two distinct points in a connected [CW complex](../../../../../cw-complex.md) adds a loop up to [homotopy](../../../../../homotopy.md), so this quotient has the [homotopy type](../../../../../homotopy-type.md) of $T^2\vee S^1$. The preceding [relative homology](../../../../../relative-homology.md) calculation proves the groups without requiring that [homotopy](../../../../../homotopy.md) description.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
