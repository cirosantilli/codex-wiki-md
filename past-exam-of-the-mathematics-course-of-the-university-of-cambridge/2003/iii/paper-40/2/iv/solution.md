<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $u_m=d_m/r_m$. The [Taylor series](../../../../../../taylor-series.md) of the logarithm gives the [small-jump comparison of cumulative hazard estimators](../../../../../../small-jump-comparison-of-cumulative-hazard-estimators.md):

$$
-\log(1-u_m)=u_m+\frac{u_m^2}{2}+\frac{u_m^3}{3}+\cdots.
$$

Consequently, if $\max_m u_m\le\varepsilon<1$, the two [integrated hazard](../../../../../../cumulative-hazard-function.md) estimates obey

$$
0\le\widehat H_{\rm KM}-\widehat H_{\rm NA}\le\frac1{2(1-\varepsilon)}\sum_m u_m^2\le\frac{\varepsilon}{2(1-\varepsilon)}\widehat H_{\rm NA}.
$$

**They are close when every event fraction is small.** In particular, with distinct single failures and large [risk sets](../../../../../../risk-set.md), $u_m=1/r_m$ is small. With tied data, large [risk sets](../../../../../../risk-set.md) alone are insufficient if a substantial fraction of the [risk set](../../../../../../risk-set.md) fails together.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
