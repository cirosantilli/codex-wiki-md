<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Unless a coefficient group is displayed, use integral [singular cohomology](../../../../../singular-cohomology.md). The standard [CW complex](../../../../../cw-complex.md) structure on [infinite-dimensional real projective space](../../../../../infinite-dimensional-real-projective-space.md) has one cell in each nonnegative dimension. Its [cellular chain complex](../../../../../cellular-chain-complex.md) has boundary $d_j=2$ for positive even $j$ and $d_j=0$ for odd $j$. The [cellular cohomology](../../../../../cellular-cohomology.md) differential $\delta^j$ is therefore zero for even $j$ and multiplication by two for odd $j$. Consequently

$$
\boxed{H^j(\mathbb{RP}^{\infty};\mathbb Z)=\begin{cases}\mathbb Z,&j=0,\\\mathbb Z/2,&j>0\text{ even},\\0,&j\text{ odd}.\end{cases}}
$$

More generally, for an [abelian group](../../../../../abelian-group.md) $A$, the positive odd groups are $A[2]=\{a:2a=0\}$ and the positive even groups are $A/2A$. In particular $H^j(\mathbb{RP}^{\infty};\mathbb Z_2)=\mathbb Z_2$ in every nonnegative degree.

For the required [Bockstein homomorphism](../../../../../bockstein-homomorphism.md), use the [short exact sequence](../../../../../short-exact-sequence.md)

$$
0\longrightarrow\mathbb Z_m\overset{\iota}{\longrightarrow}\mathbb Z_{m^2}\overset{q}{\longrightarrow}\mathbb Z_m\longrightarrow0,
\qquad\iota([a])=[ma],\quad q([b])=[b]\pmod m.
$$

Here $m\geq2$; for $m=1$ all three coefficient groups are zero. Since [singular chains](../../../../../singular-chain.md) are free [abelian groups](../../../../../abelian-group.md), applying cochains gives a [short exact sequence](../../../../../short-exact-sequence.md) of [cochain complexes](../../../../../cochain-complex.md). Its [connecting homomorphism](../../../../../connecting-homomorphism.md) defines $\beta$ and its [long exact sequence](../../../../../long-exact-sequence.md) is precisely the required one, with the other maps induced by $\iota$ and $q$.

Explicitly, represent a class by a [cocycle](../../../../../cocycle.md) $u\in C^n(X;\mathbb Z_m)$ and choose a lift $\widetilde u\in C^n(X;\mathbb Z_{m^2})$. Since $q(\delta\widetilde u)=0$, there is a unique cochain $v$ with $\iota(v)=\delta\widetilde u$. Injectivity of $\iota$ and $\delta^2=0$ show $\delta v=0$. Define

$$
\boxed{\beta([u])=[v].}
$$

Changing the lift by $\iota(w)$ changes $v$ by the [coboundary](../../../../../coboundary.md) $\delta w$. Changing the representative $u$ by a [coboundary](../../../../../coboundary.md) can be lifted by a coboundary as well and leaves the resulting class unchanged. Thus this is a well-defined [group homomorphism](../../../../../group-homomorphism.md), and the standard cochain lifting argument gives exactness.

Compute the [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) on [infinite-dimensional real projective space](../../../../../infinite-dimensional-real-projective-space.md) using its [cellular cohomology](../../../../../cellular-cohomology.md) complex. A generator with coefficients $\mathbb Z_2$ is represented by $1$ in degree $n$, lifted to $1\in\mathbb Z_4$. Its coboundary is $0$ for even $n$ and $2$ for odd $n$. Dividing via $\iota(1)=2$ gives

$$
\boxed{\beta=0\text{ for even }n,\qquad\beta=\mathrm{id}_{\mathbb Z_2}\text{ for odd }n.}
$$

Thus the odd-degree maps are **isomorphisms**. The comparison between [cellular cohomology](../../../../../cellular-cohomology.md) and [singular cohomology](../../../../../singular-cohomology.md) is natural with respect to coefficient maps, so this computes the same [connecting homomorphism](../../../../../connecting-homomorphism.md) constructed above.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
