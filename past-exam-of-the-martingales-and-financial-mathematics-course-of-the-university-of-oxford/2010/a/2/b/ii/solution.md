<h1 id="a/2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each positive integer $m$, the events $\{|X_n|\geq mn\}$ are independent and have divergent total probability by part (i). The [Borel-Cantelli second lemma](../../../../../../borel-cantelli-second-lemma.md) makes them occur infinitely often. Taking the countable intersection over $m$ gives

$$
\boxed{\limsup_n|X_n|/n=\infty\quad\text{almost surely}.}
$$

If $\limsup_n|S_n|/n$ were finite along any such sample path, then for some finite path-dependent $C$, $|S_n|\leq Cn$ eventually. But $X_n=S_n-S_{n-1}$ would give $|X_n|/n\leq C+C(n-1)/n\leq2C$ eventually, a contradiction. Therefore

$$
\boxed{\limsup_n|S_n|/n=\infty\quad\text{almost surely}.}
$$

This is the [divergence of normalized iid partial sums without a first absolute moment](../../../../../../divergence-of-normalized-iid-partial-sums-without-a-first-absolute-moment.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
