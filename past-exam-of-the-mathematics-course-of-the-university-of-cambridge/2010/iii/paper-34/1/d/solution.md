<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There is an apparent reversal, but not a mathematical contradiction. The crude [odds ratio](../../../../../../odds-ratio.md) averages over the actual background distribution in each group, whereas the adjusted [logistic regression](../../../../../../logistic-regression.md) compares groups at the same fitted background values. Strong [confounding](../../../../../../confounding.md) could make those distributions very different: for example, elective patients might disproportionately come from low-risk backgrounds or clinics, while the reference patients come from higher-risk backgrounds. The [Simpson paradox](../../../../../../simpson-s-paradox.md) can then reverse the marginal comparison even when every conditional comparison favours the same direction.

The [noncollapsibility of the odds ratio](../../../../../../noncollapsibility-of-the-odds-ratio.md) can also make marginal and conditional odds ratios differ in magnitude. It does not, by itself, explain a sign reversal if both groups have the same covariate distribution and the common conditional effect has one sign: if $p(1,x)>p(0,x)$ for every $x$, averaging over the same distribution of $x$ still gives a larger exposed risk. A genuine reversal therefore requires differing background distributions, heterogeneous effects or another change in what is being compared. The observed reversal is a reason to investigate these issues, not proof of a programming error.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
