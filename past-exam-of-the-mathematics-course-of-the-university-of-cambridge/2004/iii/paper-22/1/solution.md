<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use rational coefficients and finite [singular chains](../../../../../singular-chain.md). For an $N$-dimensional [stratified pseudomanifold](../../../../../stratified-pseudomanifold.md) with filtration $X_j$, the [lower middle perversity](../../../../../lower-middle-perversity.md) is

$$
\boxed{\bar m(k)=\left\lfloor\frac{k-2}{2}\right\rfloor\quad(k\ge2).}
$$

A [singular simplex](../../../../../singular-simplex.md) $\sigma:\Delta^i\to X$ is an [allowable singular simplex](../../../../../allowable-singular-simplex.md) when, for every $k\ge2$, $\sigma^{-1}(X_{N-k})$ lies in the $(i-k+\bar m(k))$-skeleton of $\Delta^i$; negative-dimensional skeletons are empty. Let $A_i$ be the span of these simplices in $S_i(X;\mathbb Q)$. The [intersection chains](../../../../../intersection-chains.md) are

$$
IS_i(X)=\{c\in A_i:\partial c\in A_{i-1}\}.
$$

The condition on $\partial c$ is imposed after combining equal simplices and cancelling coefficients: the faces of an allowable simplex need not themselves be allowable. If $c\in IS_i$, then $\partial c\in A_{i-1}$ and $\partial(\partial c)=0$, so $\partial c\in IS_{i-1}$. Thus $IS_*$ is a [chain subcomplex](../../../../../chain-subcomplex.md) of $S_*$, and $IH_i(X)=H_i(IS_*)$ defines [intersection homology](../../../../../intersection-homology.md).

Write $v$ for the vertex of $cY$. Its codimension is $2n$, so the vertex condition for an allowable $i$-simplex is

$$
\sigma^{-1}(v)\subseteq (\Delta^i)^{(i-n-1)}.
$$

In particular all simplices of degree at most $n$ avoid $v$. For $i<n$, both the degree-$i$ chains and the degree-$(i+1)$ chains that can bound them lie in $cY\setminus\{v\}=Y\times(0,1)$. The two [chain complexes](../../../../../chain-complex.md) therefore have the same cycles and boundaries in degree $i$, proving the low-degree isomorphism.

For $i\ge n$, let $z$ be an allowable $i$-cycle. Cone every simplex of $z$ radially to $v$, using the cone on $\Delta^i$ as $\Delta^{i+1}$, and write the resulting chain as $cz$. At the vertex, coning an old inverse image in the $(i-n-1)$-skeleton gives a subset of the $(i-n)$-skeleton, and the new cone vertex also lies in this skeleton because $i-n\ge0$. For every other singular stratum, coning the inverse image increases its permitted skeleton dimension by one, exactly as increasing the simplex dimension does. Thus $cz$ is allowable. The usual cone identity is $\partial(cz)=z-c(\partial z)=z$; since $z$ is allowable, the boundary condition for [intersection chains](../../../../../intersection-chains.md) holds as well. Every cycle is consequently a boundary. This proves the [intersection homology cone formula](../../../../../intersection-homology-cone-formula.md) here:

$$
\boxed{IH_i(cY)=\begin{cases}IH_i(Y\times(0,1)),&i<n,\\0,&i\ge n.\end{cases}}
$$

The assumption $\dim Y=2n-1$ entails $n\ge1$, so no augmented degree-zero exception arises in this coning argument.

For the [suspension of a topological space](../../../../../suspension-topology.md), the two endpoints are collapsed separately, giving two distinct vertices. Use the following standard computational facts for [intersection homology](../../../../../intersection-homology.md): a product with an interval has the same [intersection homology](../../../../../intersection-homology.md) as the original [stratified space](../../../../../stratified-space.md), via the projection and its stratum-preserving homotopy inverse; and an open cover has a [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) whose overlap map is the signed pair of inclusion maps. Cover the suspension by its two open cones. Their overlap is $Y\times(-\varepsilon,\varepsilon)$. Below degree $n$, the overlap map is, under the interval identifications, $a\mapsto(a,-a)$ in $IH_i(Y)\oplus IH_i(Y)$, hence is injective with cokernel $IH_i(Y)$. In degree $n$ both cone groups vanish and the next overlap map, in degree $n-1$, is still injective. Above degree $n$ both adjacent cone groups vanish. Exactness therefore gives

$$
\boxed{IH_i(\operatorname{Susp}Y)=\begin{cases}IH_i(Y),&i<n,\\0,&i=n,\\IH_{i-1}(Y),&i>n.\end{cases}}
$$

This differs from ordinary reduced suspension homology: below the cutoff the cycles cannot use either vertex, and in the middle degree coning kills them. If $Y$ is a compact oriented [Witt space](../../../../../witt-space.md), its [Poincare duality](../../../../../poincare-duality.md) pairs $IH_i(Y)$ with $IH_{2n-1-i}(Y)$. The displayed groups of the suspension are correspondingly paired in complementary degrees $i$ and $2n-i$, while its middle group is zero. The new vertices have even codimension $2n$ and thus impose no additional [Witt space](../../../../../witt-space.md) condition; the suspension is again Witt. Its middle [intersection form](../../../../../intersection-form.md) has zero rank and, when its dimension is divisible by four, zero [signature](../../../../../signature-of-a-quadratic-form.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
