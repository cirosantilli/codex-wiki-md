<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose [orientations](../../../../../orientation-of-a-simplex.md) on the two [sphere](../../../../../sphere.md) factors whose product is the specified [orientation](../../../../../orientation-of-a-simplex.md) of $X$. Give the four factors of $Y=(S^2)^4$ the corresponding [orientations](../../../../../orientation-of-a-simplex.md) in the order $1,2,3,4$. The [Künneth theorem](../../../../../kunneth-theorem.md) has no [Tor functor](../../../../../tor-functor.md) terms here and gives

$$
\boxed{H_j(Y;\mathbb Z)=
\begin{cases}
\mathbb Z,&j=0,8,\\
\mathbb Z^4,&j=2,6,\\
\mathbb Z^6,&j=4,\\
0,&\text{otherwise}.
\end{cases}}
$$

Let $u_i\in H^2(Y;\mathbb Z)$ be the pullback of the positively normalized [cohomology](../../../../../cohomology-split.md) class from factor $i$. The [cohomology ring](../../../../../cohomology-ring.md) is

$$
H^*(Y;\mathbb Z)=\mathbb Z[u_1,u_2,u_3,u_4]/(u_1^2,u_2^2,u_3^2,u_4^2),
\qquad |u_i|=2,
$$

with $\langle u_1u_2u_3u_4,[Y]\rangle=1$. Its generators commute by [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md).

Fix a point in each [sphere](../../../../../sphere.md). For each pair $i<j$, let $S_{ij}$ be the four-dimensional [submanifold](../../../../../submanifold.md) in which factors $i,j$ vary and the remaining factors equal their fixed points. Orient $S_{ij}$ by the ordered factors $i,j$. The six [homology classes](../../../../../homology-class.md)

$$
[S_{12}],\ [S_{13}],\ [S_{14}],\ [S_{23}],\ [S_{24}],\ [S_{34}]
$$

give a [coordinate sphere intersection basis](../../../../../coordinate-sphere-intersection-basis.md) by the [homology cross product](../../../../../homology-cross-product.md) description in the [Künneth theorem](../../../../../kunneth-theorem.md). Moving a fixed point in one of the other two factors produces a disjoint homologous representative of each $S_{ij}$. Hence every basis element has zero [self-intersection number](../../../../../self-intersection-number.md).

More precisely, the [intersection pairing](../../../../../intersection-pairing.md) is

$$
[S_{ij}]\mathbin{\cdot}[S_{kl}]=
\begin{cases}
1,&\{i,j\}\sqcup\{k,l\}=\{1,2,3,4\},\\
0,&\text{otherwise}.
\end{cases}
$$

For complementary pairs the representatives intersect transversely at one point. The sign is positive because swapping two-dimensional factors contributes $(-1)^{2\cdot2}=1$. For pairs with a common index, a factor fixed in both representatives can be displaced to make them disjoint. In the paired order $(12,34),(13,24),(14,23)$, the [intersection form](../../../../../intersection-form.md) is three copies of $\begin{pmatrix}0&1\\1&0\end{pmatrix}$.

For the [diagonal map](../../../../../diagonal-map.md) $\delta:X\to Y$, write $a,b\in H^2(X;\mathbb Z)$ for the two [sphere](../../../../../sphere.md) generators. Then

$$
\delta^*u_1=\delta^*u_3=a,\qquad
\delta^*u_2=\delta^*u_4=b,
\qquad a^2=b^2=0,\quad\langle ab,[X]\rangle=1.
$$

The coefficient of $[S_{ij}]$ in $[\Delta]$ is $\langle u_iu_j,[\Delta]\rangle$. Pullback and the preceding [cup product](../../../../../cup-product.md) relations show that these coefficients are one for $12,14,23,34$ and zero for $13,24$. Therefore

$$
\boxed{[\Delta]=[S_{12}]+[S_{14}]+[S_{23}]+[S_{34}].}
$$

There are exactly two complementary pairings among these four terms, each counted twice in the square. Thus

$$
\boxed{[\Delta]\mathbin{\cdot}[\Delta]=2(1+1)=4.}
$$

This computes both the explicit [homology class](../../../../../homology-class.md) and its [intersection pairing](../../../../../intersection-pairing.md), including all [orientation](../../../../../orientation-of-a-simplex.md) signs.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
