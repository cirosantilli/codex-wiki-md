<h1 id="17f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $G$ contains no $K_{3,2}$, every [pair](../../../../../../pair.md) of [vertices](../../../../../../vertex-graph-theory.md) has at most two [common neighbours](../../../../../../common-neighbour.md). [Double-counting](../../../../../../double-counting-proof-technique.md) a vertex together with an [unordered pair](../../../../../../unordered-pair.md) of its neighbours gives

$$
\sum_v\binom{d(v)}2\leq2\binom n2.
$$

Consequently

$$
\sum_vd(v)^2\leq2n(n-1)+2e.
$$

By Cauchy--Schwarz,

$$
\frac{4e^2}{n}\leq2n(n-1)+2e.
$$

This quadratic inequality implies $e<cn^{3/2}$ for an absolute constant $c$; for example $c=2$ works for every $n\geq1$. Thus

$$
\boxed{\operatorname{ex}(n,K_{3,2})<2n^{3/2}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
