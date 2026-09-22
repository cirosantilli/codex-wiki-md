<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [singular simplex](../../../../../singular-simplex.md) $\sigma:\Delta^i\to Y$, there are exactly $n$ lifts to $X$: choose any of the $n$ points above one vertex, then use the lifting property, since the simplex is [simply connected](../../../../../simply-connected-space.md). Define

$$
T_i(\sigma)=\sum_{\widetilde\sigma:\ f\widetilde\sigma=\sigma}\widetilde\sigma
$$

and extend $R$-linearly to [singular chains](../../../../../singular-chain.md). The restrictions of these lifts to any face are exactly the $n$ lifts of that face, each appearing once. Indeed a lift is determined uniquely by its value at any point of that face, and every possible value in the corresponding fiber extends to a lift of the whole simplex. Therefore $\partial T_i=T_{i-1}\partial$, so $T$ is a [chain map](../../../../../chain-map.md) and induces the [homological transfer for a finite covering](../../../../../homological-transfer-for-a-finite-covering.md), denoted $f^*$ in the question.

On chains, every lifted simplex projects back to the original simplex. Thus $f_\#T_i=n\,\mathrm{id}$, and on [homology](../../../../../homology-split.md) this gives

$$
\boxed{f_*f^*(u)=nu.}
$$

Over $\mathbb Q$, the map $n^{-1}f^*$ is a right inverse of $f_*$, proving **surjectivity in every degree**. Consequently each rational [Betti number](../../../../../betti-number.md) of the covering space is at least that of its base. This transfer goes in the opposite direction to the usual homological pushforward and is not the ordinary cohomological pullback.

For equality, use the connected double [covering space](../../../../../covering-space.md) $S^1\to S^1$, $z\mapsto z^2$. Both spaces have $b_0=b_1=1$ and all other [Betti numbers](../../../../../betti-number.md) zero. For strict increase, take a connected double [covering space](../../../../../covering-space.md) of the genus-two [closed orientable surface](../../../../../closed-orientable-surface.md), whose existence was proved in 1(b). The [genus of a finite cover of a closed orientable surface](../../../../../genus-of-a-finite-cover-of-a-closed-orientable-surface.md) gives covering genus $1+2(2-1)=3$. Its first [Betti number](../../../../../betti-number.md) is six, whereas that of the genus-two base is four; their zeroth and second [Betti numbers](../../../../../betti-number.md) are both one. Thus **a connected double cover can preserve every Betti number or strictly increase some of them**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
