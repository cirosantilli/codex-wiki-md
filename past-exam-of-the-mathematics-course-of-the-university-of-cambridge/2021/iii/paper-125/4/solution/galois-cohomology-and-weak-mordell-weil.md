<h1 id="4/solution/galois-cohomology-and-weak-mordell-weil">Galois cohomology and weak Mordell-Weil</h1>

↑ **Parent:** [Solution](../solution.md)

For a discrete module $M$ over the absolute Galois group $G_K$, the first [Galois cohomology](../../../../../../galois-cohomology.md) group is

$$
H^1(K,M)=Z^1(G_K,M)/B^1(G_K,M),
$$

where a one-cocycle satisfies $c(\sigma\tau)=c(\sigma)+\sigma c(\tau)$ and a coboundary has the form $c(\sigma)=\sigma m-m$.

For an integer $n\geq2$, the [Kummer exact sequence of an elliptic curve](../../../../../../kummer-exact-sequence-of-an-elliptic-curve.md)

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)
\xrightarrow{[n]}E(\overline K)\longrightarrow0
$$

produces the injective [Kummer map of an elliptic curve](../../../../../../kummer-map-of-an-elliptic-curve.md)

$$
\delta:E(K)/nE(K)\hookrightarrow H^1(K,E[n]).
$$

Explicitly, if $nQ=P$, then $\delta(P)$ is represented by $\sigma\mapsto\sigma Q-Q$.

For every completion $K_v$ there is a local Kummer map. The [n-Selmer group](../../../../../../n-selmer-group.md) is

$$
\operatorname{Sel}^{(n)}(E/K)
=\{c\in H^1(K,E[n]):c_v\in\operatorname{im}\delta_v\text{ for every }v\}.
$$

It fits into

$$
0\longrightarrow E(K)/nE(K)
\longrightarrow\operatorname{Sel}^{(n)}(E/K)
\longrightarrow\operatorname{Sha}(E/K)[n]
\longrightarrow0,
$$

where $\operatorname{Sha}(E/K)$ is the [Tate–Shafarevich group](../../../../../../tate-shafarevich-group.md).

Only finitely many places divide $n$, are places of bad reduction, or are Archimedean. Outside this finite set $S$, every Selmer class is unramified. Since the finite Galois module $E[n]$ has finite order, there are only finitely many $E[n]$-valued cohomology classes unramified outside $S$; equivalently, the relevant finite extensions have bounded degree and ramification, and their number is finite by the [Hermite–Minkowski theorem](../../../../../../hermite-minkowski-theorem.md). Hence $\operatorname{Sel}^{(n)}(E/K)$ is finite, and its subgroup $E(K)/nE(K)$ is finite. This is the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md). Combined with height descent, which chooses representatives of bounded height in the finitely many cosets modulo $nE(K)$, it yields the finite generation asserted by the [Mordell-Weil theorem](../../../../../../mordell-weil-group.md).

## ↑ Ancestors (11)

1. [Solution](../solution.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
