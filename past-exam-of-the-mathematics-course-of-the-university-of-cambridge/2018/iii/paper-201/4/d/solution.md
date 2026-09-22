<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix an integer $k\geq1$ and consider the [independent increments](../../../../../../independent-increments.md)

$$
\Delta_{j,k}=B_{(j+1)/k}-B_{j/k},\qquad j=0,1,2,\ldots.
$$

For fixed $k$ these are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with the [normal distribution](../../../../../../normal-distribution.md) $N(0,1/k)$, so $p_k=\mathbb P(|\Delta_{j,k}|>1)>0$. The second [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) gives $|\Delta_{j,k}|>1$ for infinitely many $j$, [almost surely](../../../../../../almost-sure-convergence.md). Intersecting these probability-one [events](../../../../../../event.md) over the countably many $k$ preserves probability one.

On any path in this intersection, [uniform continuity](../../../../../../uniform-continuity.md) on $[0,\infty)$ would give some $\delta>0$ such that $|B_t-B_s|<1$ whenever $|t-s|<\delta$. Choosing $k$ with $1/k<\delta$ contradicts the existence of an increment $|\Delta_{j,k}|>1$. Therefore [Brownian paths are not uniformly continuous on the half-line](../../../../../../brownian-paths-are-not-uniformly-continuous-on-the-half-line.md):

$$
\boxed{\mathbb P\bigl(B\text{ is uniformly continuous on }[0,\infty)\bigr)=0.}
$$

The event is measurable: for [continuous paths](../../../../../../continuous-path.md), [uniform continuity](../../../../../../uniform-continuity.md) can be tested by countably many pairs of nonnegative [rational numbers](../../../../../../rational-number.md) and tolerances $1/m$. **[Brownian motion](../../../../../../brownian-motion-split.md) has [uniform continuity](../../../../../../uniform-continuity.md) on every compact time interval, but [almost surely](../../../../../../almost-sure-convergence.md) fails it on the whole half-line.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
