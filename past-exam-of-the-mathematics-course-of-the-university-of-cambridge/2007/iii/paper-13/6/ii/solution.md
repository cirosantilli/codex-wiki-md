<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $T$ be the [torus graph](../../../../../../torus-graph.md) $(\mathbb Z/(5n)\mathbb Z)^2$, with independent bond density $p$. For $n$ large, all rectangles below are too small to identify any of their own vertices or edges. Let $E_n$ be the event that somewhere in $T$ there is a horizontal open crossing of a $4n$ by $n$ rectangle or a vertical open crossing of an $n$ by $4n$ rectangle. It is increasing and invariant under translations and a quarter turn. These symmetries act transitively on all $50n^2$ bonds, including both orientations. Thus it is a [transitive increasing event](../../../../../../transitive-increasing-event.md).

A fixed $4n$ by $n$ rectangle has its ordinary planar distribution, so the supplied lower bound gives $\mathbb P_{1/2}^T(E_n)>c_4$. Choose any $0<\eta<\min(c_4,1/2)$. Since $p-1/2>0$ is fixed and $\log(50n^2)\to\infty$, the [Friedgut-Kalai sharp threshold theorem](../../../../../../friedgut-kalai-sharp-threshold-theorem.md) implies $\mathbb P_p^T(E_n)>1-\eta$ for all sufficiently large $n$. As $\eta$ is arbitrary,

$$
\mathbb P_p^T(E_n)\longrightarrow1.
$$

It remains to transfer this symmetric statement to a fixed rectangle, without a growing union-bound loss. On each circular coordinate take the ten positions $a_j=\lfloor jn/2\rfloor$, $0\leq j<10$. Consecutive circular gaps are at most $\lceil n/2\rceil$. Use the one hundred $3n$ by $2n$ rectangles starting at pairs $(a_i,a_j)$ and their one hundred quarter-turn images. Every crossed $4n$ by $n$ rectangle contains the full horizontal width of one of the first family, with its vertical span contained in that rectangle's height-$2n$ span: the permissible starting intervals in each coordinate have length $n$, so the chosen positions always supply a suitable start. The crossing, restricted between those two vertical sides, gives a crossing of the chosen $3n$ by $2n$ rectangle. The analogous assertion holds in the rotated family.

Consequently $E_n$ implies at least one of these two hundred increasing crossing events. Their common success probability is $a_n=h_p(3n,2n)$. The [nth root trick](../../../../../../square-root-trick-for-positively-associated-events.md) gives

$$
(1-a_n)^{200}\leq\mathbb P_p^T(E_n^c),\qquad\text{hence}\qquad a_n\longrightarrow1.
$$

Only two hundred translates are used, independently of scale. This bounded exponent is the essential [finite-torus crossing amplification](../../../../../../finite-torus-crossing-amplification.md) step.

For a requested height $N$, set $s=\lfloor N/2\rfloor$. Glue $k$ width-$3s$, height-$2s$ rectangles, each successive pair overlapping in a square of side $2s$. Their horizontal crossings and the $k-1$ vertical overlap crossings imply a crossing of the union, which has width $(k+2)s$. An overlap square has crossing probability at least $a_s=h_p(3s,2s)$. Thus the [Harris lemma](../../../../../../harris-inequality.md) gives

$$
h_p((k+2)s,2s)\geq a_s^{2k-1}\longrightarrow1.
$$

Choose $k$ fixed and large enough that $(k+2)s\geq\lambda N$ for all sufficiently large $N$. Increasing height and shortening width can only help, so uniformly for $m\leq\lambda N$,

$$
\boxed{h_p(m,N)\longrightarrow1\quad(N\to\infty).}
$$

In particular it exceeds $1-\varepsilon$ for every sufficiently large $N$, with the bound depending only on $p,\lambda,\varepsilon$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
