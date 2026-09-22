# Equivalence test

↑ **Parent:** [Statistical hypothesis test](statistical-hypothesis-test-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivalence_test)

An [equivalence test](equivalence-test.md) asks whether an effect lies strictly inside a prespecified negligible-effect range, such as $(-\delta,\delta)$ for $\delta>0$. Its [null hypothesis](null-hypothesis.md) is that the effect lies outside that range, including its boundary; its [alternative hypothesis](alternative-hypothesis.md) is $-\delta<\theta<\delta$. This differs from a test with a zero-effect [null hypothesis](null-hypothesis.md): failing to reject zero does not establish that the effect is sufficiently small.

One construction performs two level-$\alpha$ [one-sided tests](one-sided-hypothesis-test.md), rejecting $\theta\le-\delta$ and rejecting $\theta\ge\delta$, and declares equivalence only if both reject. If the equivalence [null hypothesis](null-hypothesis.md) is true, at least one component null is true. The [probability](probability.md) of rejecting both cannot exceed the [probability](probability.md) of rejecting that true component, which is at most $\alpha$. Thus the combined procedure controls [Type I error](type-i-and-type-ii-errors.md) at level $\alpha$. In a continuous symmetric t-based location model with a common [standard error](standard-error.md), this is equivalent to putting the central $100(1-2\alpha)\%$ [confidence interval](confidence-interval.md) wholly inside $(-\delta,\delta)$. At $\alpha=0.05$ that is a 90% interval, not the 95% interval used for the usual two-sided zero-effect test. The margin must be chosen for substantive reasons rather than selected afterward to accommodate an observed interval.

## ↑ Ancestors (7)

1. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Equivalence test](equivalence-test.md)
- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2019/6/solution.md)
