<h1 id="8/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The $m$ red positions form a uniformly chosen [subset](../../../../../../subset.md) of size $m$, so there are $\binom{m+n}{m}$ equally likely colour patterns. A contiguous red block can start at positions $1,2,\ldots,n+1$, giving exactly $n+1$ favourable patterns. Therefore

$$
\boxed{\mathbb P(\text{all reds together})=\frac{n+1}{\binom{m+n}{m}}.}
$$

If the cards are regarded as individually labelled, each colour pattern corresponds to $m!n!$ [permutations](../../../../../../permutation.md), so the same counting argument still applies. In the edge case $m=1$, the formula correctly gives [probability](../../../../../../probability.md) one.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
