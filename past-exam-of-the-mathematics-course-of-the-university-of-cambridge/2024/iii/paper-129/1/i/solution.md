<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md) says that if $A,B$ are finite nonempty subsets of an [abelian group](../../../../../../abelian-group.md) and

$$
|A+B|\le K|A|,
$$

then for all nonnegative integers $m,n$,

$$
\boxed{|mB-nB|\le K^{m+n}|A|.}
$$

Choose a nonempty $X\subseteq A$ minimizing

$$
K'=\frac{|X+B|}{|X|};
$$

then $K'\le K$. We first prove the [Petridis minimal-growth lemma](../../../../../../petridis-minimal-growth-lemma.md)

$$
|X+B+C|\le K'|X+C|
$$

for every finite $C$, by induction on $|C|$. Remove $c\in C$, write $C'=C\setminus\{c\}$, and let

$$
X'={x\in X:x+c\in X+C'}.
$$

The new points contributed to $X+C$ by $X+c$ are exactly $|X\setminus X'|$. Moreover, $X'+B+c\subseteq(X+B+c)\cap(X+B+C')$, so

$$
|X+B+C|
\le |X+B+C'|+|X+B|-|X'+B|.
$$

The induction hypothesis, the identity $|X+B|=K'|X|$, and minimality, which gives $|X'+B|\ge K'|X'|$, yield

$$
|X+B+C|\le K'|X+C'|+K'|X|-K'|X'|=K'|X+C|.
$$

Iteration with $C=(r-1)B$ gives

$$
|X+rB|\le (K')^r|X|\le K^r|X|.
$$

Finally, the [Ruzsa triangle inequality](../../../../../../ruzsa-triangle-inequality.md) gives

$$
|mB-nB|le\frac{|X+mB|\,|X+nB|}{|X|}
\le K^{m+n}|X|le K^{m+n}|A|,
$$

as required.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
