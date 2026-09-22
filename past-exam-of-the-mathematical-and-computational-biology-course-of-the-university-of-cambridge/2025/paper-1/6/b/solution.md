<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [beta distribution](../../../../../beta-distribution.md) [prior density](../../../../../prior-density.md) is proportional to $p^{a-1}(1-p)^{b-1}$. By [Bayes' theorem](../../../../../bayes-theorem.md), its product with the [likelihood function](../../../../../likelihood-function.md) gives the [posterior density](../../../../../posterior-density.md)

$$
\pi(p\mid x)\propto p^{a+n-1}(1-p)^{b+S-n-1}.
$$

This is again a [beta distribution](../../../../../beta-distribution.md), namely

$$
\boxed{p\mid x\sim\operatorname{Beta}(a+n,b+S-n)}.
$$

Thus the beta family is a [conjugate prior](../../../../../conjugate-prior.md) family for the [geometric distribution](../../../../../geometric-distribution.md). The update is an instance of [beta-geometric conjugacy](../../../../../beta-geometric-conjugacy.md): counts of observed successes and failures are added to the two beta parameters.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
