<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The finite-dimensional implication again follows from equivalence of [norms](../../../../../../norm.md) and the [Heine-Borel theorem](../../../../../../heine-borel-theorem.md). In an infinite-dimensional [Banach space](../../../../../../banach-space-split.md), inductively apply [Riesz lemma](../../../../../../riesz-s-lemma.md) to the proper closed finite-dimensional [linear span](../../../../../../linear-span.md) $Y_n=\operatorname{span}(f_1,\ldots,f_n)$ to obtain a unit vector $f_{n+1}$ with $\operatorname{dist}(f_{n+1},Y_n)>1/2$. Therefore $\|f_n-f_m\|>1/2$ for distinct indices, precluding a [Cauchy subsequence](../../../../../../cauchy-subsequence.md).

For completeness, [Riesz lemma](../../../../../../riesz-s-lemma.md) here follows by taking $z\notin Y$, setting $d=\operatorname{dist}(z,Y)>0$, choosing $y\in Y$ with $\|z-y\|<2d$, and putting $f=(z-y)/\|z-y\|$. Its distance from $Y$ exceeds $1/2$. This proves **the closed unit ball is norm compact if and only if the Banach space is finite-dimensional**. The printed hint's equality of all pairwise distances is unnecessary; the separation inequality is what the argument supplies.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
