# Counting measure

↑ **Parent:** [Measure](measure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_measure)

[Counting measure](counting-measure.md) makes [integration](integral.md) into [summation](summation.md) by giving every measurable [singleton](singleton-mathematics.md) unit weight. On any [measurable space](measurable-space.md) $(X,\mathcal F)$, it is the [measure](measure.md) $\#$ defined by

$$
\#(A)=\begin{cases}|A|,&A\text{ is finite},\\\infty,&A\text{ is infinite},\end{cases}\qquad A\in\mathcal F.
$$

Thus $\#(\varnothing)=0$, a [finite set](finite-set.md) has its usual [cardinality](cardinality.md), and every [infinite set](infinite-set.md) has the same value $\infty$ in the [extended real number line](extended-real-number-line.md). In particular, [countably infinite sets](countably-infinite-set.md) and [uncountable sets](uncountable-set.md) are not distinguished by their [counting measure](counting-measure.md). Taking $\mathcal F$ to be the [power set](power-set.md) makes every [subset](subset.md) measurable; restricting the same rule to a smaller [sigma-algebra](sigma-algebra.md) is also allowed. [John K. Hunter, Measure Theory, Example 1.11: counting measure](https://www.math.ucdavis.edu/~hunter/measure_theory/measure_notes_ch1.pdf)

Why is this a [countably additive](countable-additivity.md) [measure](measure.md)? For pairwise disjoint [measurable sets](measurable-set.md) $A_n$,

$$
\#\left(\bigcup_{n=1}^{\infty}A_n\right)=\sum_{n=1}^{\infty}\#(A_n).
$$

If the [union](set-union.md) is finite, only finitely many $A_n$ are nonempty, and finite [cardinality](cardinality.md) adds. If the [union](set-union.md) is infinite, either one $A_n$ is infinite or infinitely many $A_n$ are nonempty; in both cases the nonnegative [series](series-mathematics.md) on the right is infinite. For example, $\{0,2\}$ and $\{1\}$ have [counting measures](counting-measure.md) $2$ and $1$, and their [union](set-union.md) has [counting measure](counting-measure.md) $3$. The [singletons](singleton-mathematics.md) $\{n\}$ for positive [natural numbers](natural-number.md) give the infinite case: $\#(\mathbb N)=\sum_{n=1}^{\infty}1=\infty$.

With the [power set](power-set.md) as [sigma-algebra](sigma-algebra.md), [counting measure](counting-measure.md) is a [finite measure](finite-measure.md) exactly when $X$ is finite, and a [sigma-finite measure](sigma-finite-measure.md) exactly when $X$ is at most [countable](countable-set.md). For the latter assertion, enumerate $X$ by measurable [singletons](singleton-mathematics.md); conversely, every finite-measure [set](set-split.md) is finite, and a [countable union](countable-union.md) of [finite sets](finite-set.md) is [countable](countable-set.md). Specifying the [sigma-algebra](sigma-algebra.md) matters: if $X=\mathbb N$ and $\mathcal F=\{\varnothing,\mathbb N\}$, [counting measure](counting-measure.md) is not a [sigma-finite measure](sigma-finite-measure.md), since the only measurable finite-measure [set](set-split.md) is the [empty set](empty-set.md).

For a finite or [countably infinite set](countably-infinite-set.md) $X$ equipped with its [power set](power-set.md), every nonnegative [function](function-split.md) is a [measurable function](measurable-function.md), and

$$
\int_X f\,d\#=\sum_{x\in X}f(x):=\sup_{F\subseteq X\text{ finite}}\sum_{x\in F}f(x).
$$

The [supremum](supremum.md) allows an infinite result and avoids choosing an order for the terms. On a [finite set](finite-set.md), expand $f$ as a [simple function](simple-function.md) using [singleton](singleton-mathematics.md) [indicator functions](indicator-function.md). On a [countably infinite set](countably-infinite-set.md), enumerate the points and apply the [monotone convergence theorem](monotone-convergence-theorem.md) to finite truncations. Real or complex [functions](function-split.md) are [integrable functions](lebesgue-integrable-function.md) for [counting measure](counting-measure.md) exactly when $\sum_{x\in X}|f(x)|<\infty$; then their [integral](integral.md) equals the absolutely convergent sum. This is the discrete counterpart of [Lebesgue integration](lebesgue-integration.md), developed further in [series as a Lebesgue integral against counting measure](series-as-a-lebesgue-integral-against-counting-measure.md). [John K. Hunter, Measure Theory, Example 4.10: absolutely convergent series as integrals](https://www.math.ucdavis.edu/~hunter/measure_theory/measure_notes_ch4.pdf)

For example, $f(n)=2^{-n}$ on the positive [natural numbers](natural-number.md) has [counting measure](counting-measure.md) [integral](integral.md) one, by the [geometric series](geometric-series.md). The [alternating harmonic series](alternating-harmonic-series.md) has a finite ordered sum but is not the [integral](integral.md) of an [integrable function](lebesgue-integrable-function.md) for [counting measure](counting-measure.md): its positive and negative parts both have infinite sums. [Absolute convergence](absolute-convergence.md) is what makes the finite [integral](integral.md) independent of enumeration. In particular, the [Lp spaces](lp-space.md) for [counting measure](counting-measure.md) on $\mathbb N$ are the [l-p sequence spaces](l-p-sequence-space.md), with their sums replacing continuous [integrals](integral.md).

Compare three [measures](measure.md) on the same [Borel sigma-algebra](borel-sigma-algebra.md) of the [real numbers](real-number.md): [counting measure](counting-measure.md) $\#$, [Dirac measure](dirac-measure.md) $\delta_1$, and [Lebesgue measure](lebesgue-measure.md) $\lambda$.

$$
\begin{array}{c|ccc}
A&\#(A)&\delta_1(A)&\lambda(A)\\\hline
\varnothing&0&0&0\\
\{0\}&1&0&0\\
\{0,1,2\}&3&1&0\\
[0,2]&\infty&1&2\\
\mathbb Q\cap[0,2]&\infty&1&0
\end{array}
$$

The [rational numbers](rational-number.md) in the last row form a [countably infinite set](countably-infinite-set.md); their [Lebesgue measure](lebesgue-measure.md) is zero by [countable additivity](countable-additivity.md) applied to [singletons](singleton-mathematics.md), even though they are [dense](dense-set.md) in the [interval](interval-mathematics.md).

<a id="image-the-same-borel-sets-have-different-sizes-under-counting-measure-dirac-measure-and-lebesgue-measure"></a>
![](counting-dirac-measures-same-sets.png)

**[Figure 6](#image-the-same-borel-sets-have-different-sizes-under-counting-measure-dirac-measure-and-lebesgue-measure). The same Borel sets have different sizes under counting measure, Dirac measure, and Lebesgue measure**. Original analytical comparison on the [real numbers](real-number.md), with the selected point $1$ marked in orange. Drawings show the finite [sets](set-split.md) and the [interval](interval-mathematics.md); the [rational numbers](rational-number.md) are named symbolically because finitely many plotted points cannot depict that infinite dense [set](set-split.md). Green zero entries mark the [null sets](null-set.md) for each column's [measure](measure.md).

These are different answers to different questions: [counting measure](counting-measure.md) asks how many points occur, [Dirac measure](dirac-measure.md) asks whether the selected point occurs, and [Lebesgue measure](lebesgue-measure.md) asks how much [length](length.md) occurs. A [null set](null-set.md) therefore depends on its [measure](measure.md). For [counting measure](counting-measure.md), the only [null set](null-set.md) is the [empty set](empty-set.md), so equality [almost everywhere](almost-everywhere.md) is equality everywhere. For $\delta_1$, a [measurable set](measurable-set.md) is a [null set](null-set.md) exactly when it misses $1$; for [Lebesgue measure](lebesgue-measure.md), even the [infinite set](infinite-set.md) $\mathbb Q\cap[0,2]$ is a [null set](null-set.md). Integrating an [indicator function](indicator-function.md) recovers each table entry through $\int\mathbf1_A\,d\mu=\mu(A)$. This lets the same [Lebesgue integral](lebesgue-integral.md) framework handle point counts, point evaluation, and geometric [length](length.md).

**Table of contents**

- [Series as a Lebesgue integral against counting measure](series-as-a-lebesgue-integral-against-counting-measure.md)

## ↑ Ancestors (7)

1. [Measure](measure.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Continuity of probability](continuity-of-probability.md)
- [Counting measure](counting-measure.md)
- [Dirac measure](dirac-measure.md)
- [Essential infimum and essential supremum](essential-infimum-and-essential-supremum.md)
- [Failure of Minkowski inequality below exponent one](failure-of-minkowski-inequality-below-exponent-one.md)
- [Hamming cube as an L1 and L2 metric](hamming-cube-as-an-l1-and-l2-metric.md)
- [Hausdorff dimension](hausdorff-dimension.md)
- [Hausdorff measure](hausdorff-measure.md)
- [Lp norm](lp-norm.md)
- [Measure](measure.md)
- [Measure theory](measure-theory-split.md)
- [Minkowski inequality](minkowski-inequality.md)
- [Minkowski inequality for finite vectors](minkowski-inequality-for-finite-vectors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-29/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/25j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/23h/c/solution.md)
- [Point process](point-process.md)
