<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [random alteration method](../../../../../../random-alteration-method.md). Take arbitrarily large $n$ divisible by $2k$, and sample a [binomial random graph](../../../../../../binomial-random-graph.md) with [edge](../../../../../../edge-of-a-graph.md) [probability](../../../../../../probability.md) $p=n^{-1+1/(2g)}$. Let $Z$ count [cycles](../../../../../../permutation-cycle.md) of lengths $3,\ldots,g-1$. For each length $\ell$, its expected count is at most $(np)^\ell/(2\ell)$, so

$$
\mathbb EZ\le\sum_{\ell=3}^{g-1}\frac{n^{\ell/(2g)}}{2\ell}=o(n).
$$

The sum is empty if $g=3$. By the [Markov inequality](../../../../../../markov-inequality.md), $Z\le n/2$ with [probability](../../../../../../probability.md) tending to one.

Set $s=n/(2k)$. The expected number of independent $s$-vertex sets is

$$
\binom ns(1-p)^{\binom s2}
\le2^n\exp\left(-\frac{p s(s-1)}2\right)\longrightarrow0,
$$

because the negative exponent has order $n^{1+1/(2g)}$, dominating the term of order $n$. Thus with [probability](../../../../../../probability.md) tending to one there is no [independent set](../../../../../../independent-set-graph-theory.md) of size $s$.

Choose a realization having both properties. Delete one [vertex](../../../../../../vertex-graph-theory.md) from each of its short [cycles](../../../../../../permutation-cycle.md), using at most $Z$ deletions. The induced remaining [graph](../../../../../../graph-split.md) $H$ has at least $n/2$ [vertices](../../../../../../vertex-graph-theory.md) and [girth](../../../../../../girth.md) at least $g$. Deletion cannot create a new [independent set](../../../../../../independent-set-graph-theory.md), so $\alpha(H)\le s-1$. Every [colour class](../../../../../../colour-class.md) is independent, giving

$$
\chi(H)\ge\frac{|V(H)|}{\alpha(H)}\ge\frac{n/2}{s-1}>k.
$$

In particular **a [graph](../../../../../../graph-split.md) of the required [girth](../../../../../../girth.md) and [chromatic number](../../../../../../chromatic-number.md) exists**. This proves [graphs of arbitrarily high girth and chromatic number](../../../../../../graphs-of-arbitrarily-high-girth-and-chromatic-number.md) rather than invoking that existence theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
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
