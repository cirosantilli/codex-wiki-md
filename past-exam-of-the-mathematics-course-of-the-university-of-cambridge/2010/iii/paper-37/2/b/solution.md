<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Y_{agpq}$ be the premium at age $a\in\{21,30,40\}$, gender $g\in\{F,M\}$, policy $p\in\{\mathrm{3rd},\mathrm{comp}\}$, and points $q\in\{0,3,6,9\}$, for the combinations actually observed. The additive [normal linear model](../../../../../../normal-linear-model.md) is

$$
Y_{agpq}=\mu+\alpha_a+\gamma_g+\delta_p+\eta_q+\varepsilon_{agpq},\qquad \varepsilon_{agpq}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Its [corner-point constraints](../../../../../../corner-point-constraint.md) are $\alpha_{21}=\gamma_F=\delta_{\mathrm{3rd}}=\eta_0=0$. Thus $\mu$ is the reference-category mean; the other coefficients are additive contrasts. The model assumes a common variance and excludes all [interactions](../../../../../../interaction-statistics.md). It has $1+2+1+1+3=8$ estimable mean parameters and $32-8=24$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md). The variance estimate is

$$
\boxed{\hat\sigma^2=19512/24=813.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
