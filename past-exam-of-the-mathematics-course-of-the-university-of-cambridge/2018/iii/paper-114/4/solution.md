<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For connected oriented [closed manifolds](../../../../../closed-manifold.md) of dimension $n$, the [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) is the integer determined by

$$
\boxed{f_*[M]=(\deg f)[N]\quad\text{in }H_n(N;\mathbb Z),}
$$

where the brackets are the chosen [fundamental classes](../../../../../fundamental-class.md). Functoriality gives $\deg(g\circ f)=\deg g\,\deg f$.

Give $S^n$ its boundary orientation as the boundary of the unit ball in $\mathbb R^{n+1}$. The [antipodal map](../../../../../antipodal-map.md) is the restriction of $-I$. Its ambient determinant is $(-1)^{n+1}$, and it takes the outward normal at $x$ to the outward normal at $-x$. Thus its effect on the boundary orientation has this same sign, giving

$$
\boxed{\deg A=(-1)^{n+1}.}
$$

The original PDF has $A:S^n\to S^n$, correcting the extra prime on the target in the TeX transcription.

For even dimension $n=2k\geq2$, [cellular homology of real projective space](../../../../../cellular-homology-of-real-projective-space.md) gives $H_n(\mathbb{RP}^n;\mathbb Z)=0$. Thus the composite map on top homology factors through zero, and

$$
\boxed{\deg h=0\quad\text{if }h:S^{2k}\to S^{2k}\text{ factors through }\mathbb{RP}^{2k},\ k\geq1.}
$$

Zero is attained by constant maps.

For odd dimension $n=2k+1\geq3$, [Real projective space](../../../../../real-projective-space.md) is orientable: the antipodal deck transformation has degree $+1$. Orient it so that the double [covering map](../../../../../covering-space.md) $q:S^n\to\mathbb{RP}^n$ has degree $2$. Since $S^n$ is simply connected, the [lifting criterion for a covering space](../../../../../lifting-criterion-for-a-covering-space.md) gives $f=q\circ\widetilde f$ for a map $\widetilde f:S^n\to S^n$. Hence

$$
\deg(g\circ f)=2\deg g\,\deg\widetilde f,
$$

which is even. Every even integer occurs: collapse the complement of an oriented embedded disk in $\mathbb{RP}^n$ to obtain a degree-one map $g:\mathbb{RP}^n\to S^n$, and choose $\widetilde f$ of any prescribed integer degree $m$. Maps of all integer degrees on spheres are obtained, for example, by suspending the circle maps $z\mapsto z^m$. Setting $f=q\circ\widetilde f$ gives degree $2m$. Thus

$$
\boxed{\{\deg h\}=2\mathbb Z\quad\text{in odd dimensions }2k+1\geq3.}
$$

These are the [degrees of maps factoring through real projective space](../../../../../degrees-of-maps-factoring-through-real-projective-space.md). If $k=0$ is permitted in the odd-dimensional clause, there is an exception: $\mathbb{RP}^1\cong S^1$, so every integer degree occurs. The lifting argument requires dimension at least two. The initial connected-manifold degree definition excludes $S^0$; with the usual reduced-homology definition for self-maps of $S^0$, a factorization through the one-point $\mathbb{RP}^0$ has degree zero.

Finally suppose $\deg f=p$ is prime. Fix any prime $q\ne p$ and work over $F=\mathbb F_q$. We claim that $f^*:H^r(N;F)\to H^r(S^n;F)$ is injective. If $a\ne0$, [Poincare duality](../../../../../poincare-duality.md) supplies $b\in H^{n-r}(N;F)$ with $\langle a\smile b,[N]_F\rangle\ne0$. Naturality of the [cup product](../../../../../cup-product.md) and evaluation gives

$$
\langle f^*a\smile f^*b,[S^n]_F\rangle
=p\,\langle a\smile b,[N]_F\rangle\ne0,
$$

because $p$ is invertible in $F$. Hence $f^*a\ne0$, proving [cohomological injectivity of a map of invertible degree](../../../../../cohomological-injectivity-of-a-map-of-invertible-degree.md).

The intermediate cohomology of the sphere is zero, so $H^r(N;F)=0$ for $0<r<n$. Over a field, the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) identifies this with the dual of $H_r(N;F)$, so these homology groups vanish as well. The [universal coefficient theorem for homology](../../../../../universal-coefficient-theorem-for-homology.md) then gives

$$
H_r(N;\mathbb Z)\otimes\mathbb F_q=0\quad(0<r<n,\ q\ne p).
$$

Each integral group is a [finitely generated abelian group](../../../../../finitely-generated-abelian-group.md), by the permitted finite [CW complex](../../../../../cw-complex.md) model. Its decomposition can have no free summand, since that would survive modulo $q$, and no torsion summand divisible by any prime $q\ne p$. Thus it is a finite $p$-primary group. There are only finitely many intermediate degrees, so the exponents of their finite cyclic summands have a common bound $p^a$. Taking $a\geq1$ also covers the case in which all the groups vanish. Therefore

$$
\boxed{\exists a>0:\quad p^a x=0\quad\text{for every }x\in H_r(N;\mathbb Z),\ 0<r<n.}
$$

This proves that a [prime-degree sphere map forces primary torsion](../../../../../prime-degree-sphere-map-forces-primary-torsion.md), including one uniform exponent for all the degrees.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
