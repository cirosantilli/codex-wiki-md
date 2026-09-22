<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**(A)** For a finite point set $P$ and a family $\mathcal C$ of distinct unit circles in $\mathbb R^2$, the [Szemerédi–Trotter theorem for unit circles](../../../../../szemeredi-trotter-theorem-for-unit-circles.md) states

$$
\boxed{I(P,\mathcal C)\le C\bigl(|P|^{2/3}|\mathcal C|^{2/3}+|P|+|\mathcal C|\bigr)}
$$

with an absolute constant $C$. Here $I$ counts point-circle incidences. Distinctness matters: repeated copies of the same circle are not separate members of this geometric family. A dilation gives the same bound for circles of any one fixed positive radius, with the same constant.

**(B)** Write $N=|P|$ and $D=|\Delta(P)\setminus\{0\}|$. The comparison is a bound on the cardinality of the [distinct-distance set](../../../../../distinct-distance-set.md), rather than on the set itself. For each positive distance $\rho$, take the $N$ circles of radius $\rho$ centred at points of $P$. Their [incidences between points and curves](../../../../../incidences-between-points-and-curves.md) count exactly the ordered pairs $(p,q)$ at distance $\rho$. After dilation by $1/\rho$, part (A) bounds this number by

$$
C(N^{4/3}+2N)\le C_1N^{4/3}\qquad(N\ge1).
$$

Every ordered pair of distinct points contributes to exactly one of these counts. Thus the [unit-circle method for a distinct-distance lower bound](../../../../../unit-circle-method-for-a-distinct-distance-lower-bound.md) gives

$$
N(N-1)\le C_1D N^{4/3}.
$$

For $N\ge2$, $N-1\ge N/2$, so

$$
\boxed{|\Delta(P)|\ge D\ge \frac1{2C_1}N^{2/3}.}
$$

For $N=1$ the distance set is $\{0\}$ and the conclusion holds after adjusting the absolute constant; the empty set causes no difficulty.

**(C)** A direct [incidence bound from two-point multiplicity](../../../../../incidence-bound-from-two-point-multiplicity.md) suffices. Put $M=|\mathcal L|=N^2$ and $k_\gamma=|P\cap\gamma|$. Count unordered pairs of distinct points on each curve. By [double counting](../../../../../double-counting-proof-technique.md),

$$
\sum_{\gamma\in\mathcal L}\binom{k_\gamma}{2}
=\sum_{\{p,q\}\subset P}|\{\gamma:p,q\in\gamma\}|
\le\sqrt N\,\binom N2.
$$

Writing $I=\sum_\gamma k_\gamma$, this gives

$$
\sum_\gamma k_\gamma^2
=I+2\sum_\gamma\binom{k_\gamma}{2}
\le I+N^{1/2}N(N-1).
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) now yields

$$
I^2\le M\sum_\gamma k_\gamma^2
\le N^2I+N^{9/2}.
$$

If $x^2\le ax+b$ with $x,a,b\ge0$, then $x\le a+\sqrt b$. Consequently

$$
\boxed{I(P,\mathcal L)\le N^2+N^{9/4}\le2N^{5/2}\qquad(N\ge1).}
$$

In fact the argument proves the stronger $O(N^{9/4})$ bound. The two-point multiplicity hypothesis alone controls these [incidences between points and curves](../../../../../incidences-between-points-and-curves.md); the algebraic degree bound is not needed for the requested estimate.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
