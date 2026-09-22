<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) states that, for nonnegative measurable $f_n$ on a [Lebesgue measurable set](../../../../../lebesgue-measurable-set.md) $E$ with $f_n\uparrow f$ [almost everywhere](../../../../../almost-everywhere.md),

$$
\int_Ef_n\uparrow\int_Ef,
$$

allowing infinity. [Fatou's lemma](../../../../../fatou-s-lemma.md) states that, for nonnegative measurable $f_n$,

$$
\int_E\liminf_nf_n\leq\liminf_n\int_Ef_n.
$$

Now write $C=\sup_n\int_E|g_n|<\infty$. A pointwise [limit superior](../../../../../limit-superior.md) of measurable functions is measurable, and it agrees with $g$ off the exceptional [null set](../../../../../null-set.md). By [completeness of Lebesgue measure](../../../../../completeness-of-lebesgue-measure.md), assigning any values on that null set preserves measurability. Therefore $g$ is measurable. Since $|g_n|\to|g|$ almost everywhere, Fatou's lemma gives

$$
\boxed{\int_E|g|\leq\liminf_n\int_E|g_n|\leq C<\infty.}
$$

Thus $g$ is finite almost everywhere and is a [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md). This is an [almost-everywhere limit under a uniform L1 bound](../../../../../almost-everywhere-limit-under-a-uniform-l1-bound.md). The argument proves integrability of the limit, not convergence in [L1 space](../../../../../l1-space.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
