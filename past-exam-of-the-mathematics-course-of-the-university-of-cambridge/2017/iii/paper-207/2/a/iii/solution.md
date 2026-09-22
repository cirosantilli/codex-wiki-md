<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Bonferroni correction](../../../../../../../bonferroni-correction.md) compares every [p-value](../../../../../../../p-value.md) with $0.05/100000=5\times10^{-7}$. Only the first two displayed values lie below that threshold; all undisplayed values are at least the tenth displayed value. Hence

$$
\boxed{R_{\mathrm{Bonferroni}}=2.}
$$

For the [Benjamini-Hochberg procedure](../../../../../../../benjamini-hochberg-procedure.md) at [false discovery rate](../../../../../../../false-discovery-rate.md) level $q=0.1$, the rank-$i$ threshold is $qi/100000=i\times10^{-6}$. The first nine displayed ranks meet their thresholds, while rank ten does not: $1.1\times10^{-5}>10^{-5}$. Consequently **nine is the intended count if every later rank also fails its threshold**. The rule is a step-up rule, however:

$$
k=\max\{i:p_{(i)}\leq qi/100000\},\qquad R_{\mathrm{BH}}=k.
$$

It does not stop at the first failed comparison. The full rejection count is therefore not determined by ten order statistics. For example, completing the list with $99990$ values equal to $1$ gives $k=9$, whereas completing it with $99990$ values equal to $0.02$ gives $k=100000$, since $p_{(100000)}=0.02\leq0.1$. Both completions respect the printed ten smallest [p-values](../../../../../../../p-value.md). Thus **at least nine are rejected; exactly nine requires an extra assumption about the undisplayed ranks**. In the second completion even the tenth marker is rejected, despite failing its own rank threshold. The [false discovery rate](../../../../../../../false-discovery-rate.md) guarantee also requires the usual validity and [independence](../../../../../../../independent-random-variables.md) or appropriate positive-dependence assumptions, unlike the arbitrary-dependence [Bonferroni correction](../../../../../../../bonferroni-correction.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
