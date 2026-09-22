<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret each mechanism for a fixed missingness pattern $r$: the observed and missing response components are the coordinates selected by that pattern, and the [covariates](../../../../../../covariate.md) $X$ are assumed fully recorded.

For [missing completely at random](../../../../../../missing-completely-at-random.md), missingness depends on neither response values nor [covariates](../../../../../../covariate.md):

$$
\boxed{f(r\mid Y^o,Y^m,X)=f(r).}
$$

For [covariate-dependent missing completely at random](../../../../../../covariate-dependent-missing-completely-at-random.md), response observation may depend on $X$ but not on the response after conditioning on $X$:

$$
\boxed{f(r\mid Y^o,Y^m,X)=f(r\mid X).}
$$

This is [conditional independence](../../../../../../conditional-independence.md) $R\perp Y\mid X$ and can still produce a marginal association between response and missingness.

For [covariate-dependent missing at random](../../../../../../covariate-dependent-missing-at-random.md), the observation probability may use observed response components and [covariates](../../../../../../covariate.md), but not the values missing under that pattern:

$$
\boxed{f(r\mid Y^o,Y^m,X)=f(r\mid Y^o,X).}
$$

For [missing not at random](../../../../../../missing-not-at-random.md), there remains dependence on $Y^m$ after conditioning on $Y^o,X$; the displayed simplification is not valid. For example, refusal could depend on the unreported response itself, even among individuals sharing all recorded [covariates](../../../../../../covariate.md). These mechanisms concern the reason for nonobservation, not whether the incomplete records merely look irregular. Their distinction is not generally identifiable from the observed responses alone.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
