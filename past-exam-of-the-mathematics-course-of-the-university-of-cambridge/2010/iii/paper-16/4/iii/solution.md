<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $X$ is an [affine scheme](../../../../../../affine-scheme.md), each reduced [irreducible component](../../../../../../irreducible-component.md) is a [closed subscheme](../../../../../../closed-subscheme.md), hence an [affine scheme](../../../../../../affine-scheme.md). We prove the converse by explicit [affine gluing along closed subschemes](../../../../../../affine-gluing-along-closed-subschemes.md).

First suppose $X$ is the scheme-theoretic union of two [closed subschemes](../../../../../../closed-subscheme.md) which are [affine schemes](../../../../../../affine-scheme.md) $Y$ and $Z$: their defining [ideal sheaves](../../../../../../ideal-sheaf-of-a-closed-subscheme.md) have zero intersection. Their scheme-theoretic intersection $W$ is a [closed subscheme](../../../../../../closed-subscheme.md) of both, hence an [affine scheme](../../../../../../affine-scheme.md). Write

$$
Y=\operatorname{Spec}A,\qquad Z=\operatorname{Spec}B,\qquad W=\operatorname{Spec}C.
$$

The two maps $A\to C$ and $B\to C$ are surjective. Form the [fiber product of rings](../../../../../../fiber-product-of-rings.md)

$$
R=A\times_CB=\{(a,b):a|_W=b|_W\}.
$$

Both projections are surjective. Let $I=\ker(R\to A)$ and $J=\ker(R\to B)$. Then

$$
I\cap J=IJ=0,\qquad R/I=A,\qquad R/J=B,\qquad R/(I+J)=C.
$$

For the last equality, the common image map $R\to C$ is surjective, and its [kernel of a ring homomorphism](../../../../../../kernel-of-a-ring-homomorphism.md) consists exactly of pairs whose two coordinates map to zero. Therefore $\operatorname{Spec}R$ has closed pieces isomorphic to $Y$ and $Z$, with intersection $W$. They cover it because each [prime ideal](../../../../../../prime-ideal.md) contains $I$ or $J$, as $IJ=0$.

A finite closed cover determines the topology: a subset is closed if and only if its intersections with both closed pieces are closed. The identifications of $Y,Z,W$ therefore give a homeomorphism between $X$ and $\operatorname{Spec}R$. To check the [structure sheaf](../../../../../../structure-sheaf-of-a-scheme.md), on $X$ the elementary ideal-intersection sequence gives

$$
0\longrightarrow\mathcal O_X\longrightarrow i_*\mathcal O_Y\oplus j_*\mathcal O_Z\xrightarrow{(a,b)\mapsto a|_W-b|_W}k_*\mathcal O_W\longrightarrow0.
$$

It is exact on [stalks](../../../../../../stalk-of-a-sheaf.md), by $\mathcal I_Y\cap\mathcal I_Z=0$. The same sequence holds on $\operatorname{Spec}R$, using $I\cap J=0$. Under the homeomorphism, the two middle [sheaves](../../../../../../sheaf-mathematics.md) and their restriction maps identify, so their kernels identify as [sheaves](../../../../../../sheaf-mathematics.md) of [rings](../../../../../../ring.md). This identifies the [structure sheaves](../../../../../../structure-sheaf-of-a-scheme.md), giving an isomorphism of [schemes](../../../../../../scheme.md) $X\simeq\operatorname{Spec}R$. The intersection $W$ need not be reduced.

Now a [Noetherian scheme](../../../../../../noetherian-scheme.md) has finitely many [irreducible components](../../../../../../irreducible-component.md) $Y_1,\ldots,Y_r$. Induct on $r$. For $r=1$, the reduced [scheme](../../../../../../scheme.md) is its single reduced [irreducible component](../../../../../../irreducible-component.md), so is an [affine scheme](../../../../../../affine-scheme.md). For $r>1$, let $Y=Y_1$ and let $Z$ be the reduced union of the remaining [irreducible components](../../../../../../irreducible-component.md). Its components are the corresponding $Y_i$, so $Z$ is an [affine scheme](../../../../../../affine-scheme.md) by induction. The defining [ideal sheaves](../../../../../../ideal-sheaf-of-a-closed-subscheme.md) of $Y$ and $Z$ have zero intersection: their intersection is the [ideal sheaf](../../../../../../ideal-sheaf-of-a-closed-subscheme.md) of the reduced union of all components, which is zero because $X$ is reduced. The two-piece argument proves that $X$ is an [affine scheme](../../../../../../affine-scheme.md). The empty [scheme](../../../../../../scheme.md) is $\operatorname{Spec}0$ and causes no exception. Hence

$$
\boxed{X\text{ affine}\ \Longleftrightarrow\ \text{every reduced irreducible component of }X\text{ is affine}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
