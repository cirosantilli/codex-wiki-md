<h1 id="d/d1/solution">Solution</h1>

↑ **Parent:** [D1](../d1.md)

A [sigma-algebra](../../../../sigma-algebra.md) $\mathcal F$ on $\Omega$ contains $\Omega$, is closed under complements relative to $\Omega$, and is closed under countable unions. Consequently it contains the empty set and is closed under countable intersections. A [measure space](../../../../measure-space.md) is a triple $(\Omega,\mathcal F,\mu)$ with a map $\mu:\mathcal F\to[0,\infty]$ satisfying $\mu(\varnothing)=0$ and [countable additivity](../../../../countable-additivity.md) on pairwise disjoint measurable sets.

For the increasing sequence, set $C_1=A_1$ and $C_n=A_n\setminus A_{n-1}$ for $n\geq2$. These measurable sets are disjoint, their union is $A$, and $A_N=\bigcup_{n=1}^NC_n$. Thus [countable additivity](../../../../countable-additivity.md) and finite additivity give

$$
\boxed{\mu(A)=\sum_{n=1}^{\infty}\mu(C_n)
=\lim_{N\to\infty}\sum_{n=1}^N\mu(C_n)
=\lim_{N\to\infty}\mu(A_N).}
$$

The identity permits the value infinity; it uses no subtraction of infinite measures. This is [continuity from below of a measure](../../../../continuity-from-below-of-a-measure.md).

For a decreasing sequence, the analogous assertion is **not always true**. On $\Omega=\mathbb N$ with the [counting measure](../../../../counting-measure.md), take $B_n=\{n,n+1,\ldots\}$. Then $\bigcap_nB_n=\varnothing$, so $\mu(B)=0$, whereas $\mu(B_n)=\infty$ for every $n$ and their limit is infinity.

A sufficient extra condition for [continuity from above of a measure](../../../../continuity-from-above-of-a-measure.md) is $\mu(B_1)<\infty$. Indeed $B_1\setminus B_n$ increases to $B_1\setminus B$, and the increasing-sequence result gives

$$
\mu(B_n)=\mu(B_1)-\mu(B_1\setminus B_n)\longrightarrow\mu(B).
$$

More generally it suffices that one of the $B_n$ has finite measure. The missing finiteness assumption is exactly what the counterexample violates.

## ↑ Ancestors (12)

1. [D1](../d1.md)
2. [D](../../d.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
