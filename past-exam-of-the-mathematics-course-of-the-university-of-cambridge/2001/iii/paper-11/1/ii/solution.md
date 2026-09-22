<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $q=1-p=1/b$ and $L=\log_b n$. For $s=\lceil2L\rceil$, the expected number of independent $s$-sets is

$$
\mathbb EX_s=\binom ns q^{\binom s2}
\le\left(\frac{en}{s}\right)^s b^{-s(s-1)/2}.
$$

Taking logarithms gives $\log\mathbb EX_s\le-c_p\log n\log\log n$ for all sufficiently large $n$: the two quadratic-order terms cancel to within $O_p(\log n)$, leaving the negative term $-s\log s$. By the [first moment method](../../../../../../first-moment-method.md), with [probability](../../../../../../probability.md) tending to one $\alpha(G)\le s-1<2L$. Hence

$$
\boxed{\chi(G)\ge\frac{n}{2\log_b n}.}
$$

For the upper bound, an explicit greedy exposure rule suffices; the sharper factor two is not needed here. Set

$$
m_0=\left\lceil\frac{n}{(\log n)^2}\right\rceil,
\qquad r=\left\lfloor L-8\log_b\log n\right\rfloor,
\qquad \eta=1/\log n.
$$

While at least $m_0$ [vertices](../../../../../../vertex-graph-theory.md) remain, construct a [colour class](../../../../../../colour-class.md) by choosing a candidate, retaining its non-neighbours as candidates, and repeating for $r$ choices. Expose only [edges](../../../../../../edge-of-a-graph.md) incident to chosen [vertices](../../../../../../vertex-graph-theory.md). They will all be removed with this [colour class](../../../../../../colour-class.md). By [deferred edge exposure in greedy independent-set colouring](../../../../../../deferred-edge-exposure-in-greedy-independent-set-colouring.md), the remaining internal [edges](../../../../../../edge-of-a-graph.md) are still independent Bernoulli [edges](../../../../../../edge-of-a-graph.md) conditional on the history. This assertion depends on this particular rule; it is not true for an arbitrary adaptively selected remainder.

If $M_j$ candidates remain after $j$ choices, then conditionally

$$
M_{j+1}\sim\operatorname{Bin}(M_j-1,q).
$$

The [Chernoff bound](../../../../../../chernoff-bound.md) gives, for $M_j\ge1/\eta$,

$$
\Pr\bigl(M_{j+1}<q(1-2\eta)M_j\mid\text{history}\bigr)
\le\exp(-c_p\eta^2M_j).
$$

On the event that these lower bounds hold, a class started from $m\ge m_0$ has

$$
M_j\ge m[q(1-2\eta)]^j\ge c_p(\log n)^6\qquad(0\le j\le r).
$$

Indeed $q^r\ge n^{-1}(\log n)^8$, while $(1-2/\log n)^r$ is bounded below by a positive constant depending on $p$. Thus each conditional failure [probability](../../../../../../probability.md) is at most $\exp[-c_p(\log n)^4]$. A [union bound](../../../../../../boole-s-inequality.md) over at most $nr$ candidate steps shows that all these classes can be formed with [probability](../../../../../../probability.md) tending to one. Colour the final fewer than $m_0$ [vertices](../../../../../../vertex-graph-theory.md) individually. The number of colours is at most

$$
\frac nr+m_0=\frac{n}{\log_b n}(1+o(1)).
$$

Together this proves

$$
\boxed{\frac{n}{2\log_b n}\le\chi(G(n,p))\le\frac{n}{\log_b n}(1+o(1)).}
$$

The failure estimates are summable in $n$. Thus they give both the usual asymptotically-almost-sure assertion and, on any common [probability](../../../../../../probability.md) space carrying the sequence, eventual almost-sure validity by the first [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
