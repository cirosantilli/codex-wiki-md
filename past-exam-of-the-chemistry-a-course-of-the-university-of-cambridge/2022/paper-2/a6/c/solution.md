<h1 id="a6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the ideal [Langmuir adsorption model](../../../../../langmuir-adsorption-model.md): identical independent sites, at most one atom per site, no lateral interactions, and no additional thermally active adsorbed degrees of freedom beyond the two [spin](../../../../../spin.md) states. Treat the atoms as indistinguishable and localized after [adsorption](../../../../../adsorption.md); only site occupancy and [spin](../../../../../spin.md) choices distinguish configurations.

There are $\binom MN$ ways to select $N$ occupied sites. For any such selection, independent [spin](../../../../../spin.md) sums contribute $z^N$. Thus

$$
\boxed{Q_N=\binom MN z^N.}
$$

With $q_{\rm ads}=Mz$ as defined in part (b), this is

$$
\boxed{Q_N=q_{\rm ads}^{\,N}f(M,N),\qquad
f(M,N)=\frac{M!}{N!(M-N)!\,M^N},\quad0\leq N\leq M.}
$$

Equivalently, starting from labelled particles gives $M!/(M-N)!$ distinct assignments to different sites; division by $N!$ removes particle relabellings. The $M^{-N}$ removes the site multiplicity already included in each full one-particle function.

If $q_{\rm ads}$ denotes the one-site internal factor instead, **$f(M,N)=\binom MN$** and $Q_N=\binom MN q_{\rm ads}^{\,N}$. These are identical physical results, not different counting models. In particular, the complete-function convention gives $f(M,1)=1$ and hence $Q_1=q_{\rm ads}$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [A6](../../a6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
