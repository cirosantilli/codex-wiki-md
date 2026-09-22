<h1 id="o/o5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [significance level](../../../../../significance-level.md) of a test is a bound $\alpha$ on its probability of rejecting a true null; for a composite null the bound is uniform over its parameter values. Its power at an alternative parameter is its rejection probability under that parameter.

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) concerns a simple null density $f_0$ and a simple alternative density $f_1$ for the whole sample. Among tests of size at most $\alpha$, a most powerful test rejects where $f_1>kf_0$, accepts where $f_1<kf_0$, and if necessary randomizes on equality so that its size is $\alpha$. Let its rejection probability function be $\phi_*$, with $0\leq\phi_*\leq1$, and let $\phi$ be any competing test of size at most $\alpha$.

Pointwise,

$$
(\phi_* -\phi)(f_1-kf_0)\geq0:
$$

on the rejection side both factors are nonnegative, and on the acceptance side both are nonpositive. Integrating gives

$$
\int\phi_*f_1-\int\phi f_1
\geq k\left(\int\phi_*f_0-\int\phi f_0\right)\geq0.
$$

Thus the likelihood-ratio test has at least as much power as any competitor. Even when the sample has a continuous density, the [likelihood ratio](../../../../../likelihood-ratio.md) can have an atom, so boundary randomization may still be necessary in the general statement. For the exponential test below the statistic has a continuous distribution and no randomization is needed.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
