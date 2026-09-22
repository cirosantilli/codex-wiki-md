<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) states that if $\mathcal A\subseteq[n]^{(r)}$ has the unique [binomial representation](../../../../../combinatorial-number-system.md)

$$
|\mathcal A|=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}{s},
\qquad a_r>a_{r-1}>\cdots>a_s\geq s,
$$

then its [lower shadow](../../../../../lower-shadow.md) obeys

$$
|\partial\mathcal A|\geq
\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}.
$$

An initial segment of [colexicographic order](../../../../../colexicographic-order.md) has exactly this shadow.

Here is the [UV-compression proof of the Kruskal-Katona theorem](../../../../../uv-compression-proof-of-the-kruskal-katona-theorem.md). For disjoint equal-size sets $U,V$, the [UV-compression](../../../../../uv-compression.md) $C_{U,V}$ replaces the pattern $V$ by $U$ when the image is not already in the family. If the family is not an initial colexicographic segment, choose a changing pair with $\max U<\max V$ and $|U|$ minimal. Minimality ensures that for every $x\in U$ an appropriate smaller compression $C_{U\setminus\{x\},V\setminus\{y\}}$ already fixes the family. The [Shadow lemma for UV-compressions](../../../../../shadow-lemma-for-uv-compressions.md) then gives

$$
|\partial C_{U,V}(\mathcal A)|\leq|\partial\mathcal A|.
$$

Meanwhile the binary weight $\sum_{A\in\mathcal A}\sum_{i\in A}2^i$ strictly decreases. Iterating must terminate, and a terminal family is an initial colexicographic segment. Computing that segment's shadow from its [binomial representation](../../../../../combinatorial-number-system.md) proves the theorem.

We next classify pairs that decrease the shadow for _every_ uniform family. The answer, including the identity case, is

$$
\boxed{|U|=|V|\leq1.}
$$

For $|U|=0$ the operation is the identity. For $|U|=1$, the hypotheses of the [Shadow lemma for UV-compressions](../../../../../shadow-lemma-for-uv-compressions.md) reduce to stability under the empty compression and therefore hold for every family.

To see failure for larger pairs, relabel freely. If $|U|=|V|=2$, write $U=\{u_1,u_2\}$ and $V=\{v_1,v_2\}$. The family

$$
\mathcal A=\{u_1v_1,u_1v_2,v_1v_2\}
$$

has a three-point lower shadow, whereas its compression replaces $v_1v_2$ by $u_1u_2$ and has a four-point lower shadow. If the common size is $m\geq3$, take

$$
\mathcal A=\left\{V,\ \{u_1\}\cup(V\setminus\{v_m\})\right\}.
$$

The old two shadows overlap once and have size $2m-1$. Compression replaces $V$ by $U$; the two resulting $m$-sets intersect in only $u_1$, so their lower shadows are disjoint and have size $2m$.

For the two specified pairs, the answer is **no in both cases**, even after assuming the family is [left-compressed](../../../../../left-compressed-set-family.md).

For $(U,V)=(345,126)$, take

$$
\mathcal A=\{123,124,125,126\}.
$$

This family is left-compressed. Its compression replaces $126$ by $345$. The old shadow is

$$
\{12,13,23,14,24,15,25,16,26\},
$$

of size nine, while the new shadow replaces the last two pairs by $34,35,45$ and has size ten.

For $(U,V)=(145,236)$, take the left-compressed family

$$
\mathcal A=\{123,124,125,126,134,135,136,234,235,236\}.
$$

Its shadow consists of $12,13,23$ and the nine pairs having one element in $\{1,2,3\}$ and one in $\{4,5,6\}$, so it has size twelve. Compression replaces $236$ by $145$; all twelve old shadow pairs remain and $45$ is added. The new shadow therefore has size thirteen.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
