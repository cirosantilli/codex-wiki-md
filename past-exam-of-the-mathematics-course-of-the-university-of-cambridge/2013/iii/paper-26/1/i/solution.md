<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [self-avoiding walk](../../../../../../self-avoiding-walk.md) is a finite sequence of [graph vertices](../../../../../../vertex-graph-theory.md) $v_0,\ldots,v_n$ in which successive vertices are adjacent and no [graph vertex](../../../../../../vertex-graph-theory.md) is repeated; its length is $n$, the number of [edges](../../../../../../edge-of-a-graph.md). Include the zero-length walk.

Split a length-$m+n$ walk from $v$ into its first $m$ [edges](../../../../../../edge-of-a-graph.md) and remaining $n$ [edges](../../../../../../edge-of-a-graph.md). After fixing the first segment, the number of possible suffixes is at most $\sigma_n$, since forgetting the prohibition on revisiting its earlier vertices can only increase that number. Thus $\sigma_{m+n}(v)\leq\sigma_m(v)\sigma_n$, and taking the supremum gives

$$
\boxed{\sigma_{m+n}\leq\sigma_m\sigma_n}.
$$

Every finite-radius ball is finite because degrees are bounded. An infinite connected [graph](../../../../../../graph-split.md) has vertices arbitrarily far from each root, so shortest paths give $\sigma_n(v)\geq1$. Also $\sigma_n\leq\Delta(\Delta-1)^{n-1}$ for $n\geq1$: after the first [edge](../../../../../../edge-of-a-graph.md), an immediate reversal is forbidden. In particular $\Delta\geq2$ and these suprema are finite.

Apply the [Fekete lemma](../../../../../../fekete-s-lemma.md): a real [subadditive sequence](../../../../../../subadditive-sequence.md) $a_{m+n}\leq a_m+a_n$ satisfies $\lim a_n/n=\inf_{n\geq1}a_n/n$, allowing negative infinity. Here $a_n=\log\sigma_n\geq0$, so the limit is finite. The [uniform connective constant of a bounded-degree graph](../../../../../../uniform-connective-constant-of-a-bounded-degree-graph.md) is therefore

$$
\boxed{\mu=\lim_{n\to\infty}\sigma_n^{1/n}=\inf_{n\geq1}\sigma_n^{1/n},\qquad1\leq\mu\leq\Delta-1}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
