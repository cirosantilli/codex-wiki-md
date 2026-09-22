<h1 id="9/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Four groups have $\binom42=6$ pairwise comparisons. Testing each at [test size](../../../../../size-of-a-statistical-test.md) $\alpha=0.05$ without adjustment generally increases the [familywise error rate](../../../../../familywise-error-rate.md), the chance of at least one [type I error](../../../../../type-i-and-type-ii-errors.md). If the six rejection events were independent, that chance would be $1-(1-0.05)^6\simeq0.265$; shared samples make the actual comparisons dependent, so this expression is illustrative rather than exact.

A single omnibus [ANOVA](../../../../../analysis-of-variance.md) tests equality of all four means with one stated [test size](../../../../../size-of-a-statistical-test.md), avoiding that six-test inflation for the global question. If the aim is to identify differing pairs, follow with suitably adjusted comparisons, such as [Bonferroni correction](../../../../../bonferroni-correction.md) or a simultaneous pairwise method. A significant omnibus test does not automatically license six unadjusted claims. The benefit concerns control of [type I error](../../../../../type-i-and-type-ii-errors.md), rather than a guarantee that the model's independence and common-variance assumptions hold.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
