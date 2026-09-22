<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Index chocolate by $a\in\{A,B,C,D\}$, day by $d$ in the three observed categories, and replicate by $r\in\{1,2\}$. The additive [two-factor normal linear model](../../../../../../two-factor-normal-linear-model.md) is

$$
Y_{adr}=\mu+\alpha_a+\gamma_d+\varepsilon_{adr},\qquad
\varepsilon_{adr}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Here $Y_{adr}$ is the board count, $\mu$ is the mean for the reference chocolate and reference day, and $\alpha_a,\gamma_d$ are chocolate and day [fixed effects](../../../../../../fixed-effect.md). With [corner-point constraints](../../../../../../corner-point-constraint.md), set $\alpha_A=0$ and $\gamma_{d_0}=0$, where $d_0$ is the first level in the day factor. The printed coefficient-free output does not determine that factor ordering; the model is unchanged by a different reference category. There is **no chocolate–day [interaction term](../../../../../../interaction-term.md) in this fit**. The six free mean [statistical parameters](../../../../../../statistical-parameter.md) consist of one baseline, three chocolate contrasts and two day contrasts; the common error [variance](../../../../../../variance-split.md) supplies a further [statistical parameter](../../../../../../statistical-parameter.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
