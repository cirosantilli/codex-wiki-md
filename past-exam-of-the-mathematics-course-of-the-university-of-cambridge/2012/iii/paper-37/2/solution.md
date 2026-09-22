<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [regression factor](../../../../../regression-factor.md) is a [categorical predictor](../../../../../regression-factor.md) represented by level indicators and contrasts. Treating year as a [regression factor](../../../../../regression-factor.md) permits arbitrary differences between the three yearly means, reflecting conditions such as weather, rather than imposing a linear time trend.

Let $Y_{ijk}$ be the yield for seed variety $i\in\{1,2\}$, fertiliser level $j\in\{L,H\}$, and year $k\in\{2004,2005,2006\}$. A treatment-coded [two-factor normal linear model](../../../../../two-factor-normal-linear-model.md) with additive year effects is

$$
Y_{ijk}=\beta_0+a\mathbf1_{\{i=2\}}+b\mathbf1_{\{j=H\}}+c_k+d\mathbf1_{\{i=2,j=H\}}+\varepsilon_{ijk},\qquad c_{2004}=0,
$$

with independent $N(0,\sigma^2)$ errors. The unrestricted coefficients are $\beta_0,a,b,c_{2005},c_{2006},d$: six parameters for twelve observations. Equivalently use baseline-zero variety, fertiliser, and interaction arrays. There are no year-treatment interactions in this fit.

Dividing each sum of squares by its [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) gives the completed [analysis of variance](../../../../../analysis-of-variance.md):

$$
\begin{array}{l|rrrrr}
\text{source}&\mathrm{df}&\mathrm{SS}&\mathrm{MS}&F&p\\\hline
\text{seed}&1&5.3868&5.3868&11.3748&0.014993\\
\text{fertiliser}&1&0.0768&0.0768&0.1622&0.701122\\
\text{year}&2&6.2883&3.14415&6.6392&0.030146\\
\text{seed:fertiliser}&1&16.0083&16.0083&33.803&0.001137\\
\text{residual}&6&2.8414&0.4735667&&
\end{array}
$$

In particular, the missing interaction statistic is $16.0083/(2.8414/6)\simeq33.803$. Its [null hypothesis](../../../../../null-hypothesis.md) is $H_0:d=0$, against $H_1:d\ne0$: the change in mean yield from high fertiliser is the same for both varieties. Under the [null hypothesis](../../../../../null-hypothesis.md) and the independent homoscedastic [normal linear model](../../../../../normal-linear-model.md), this [nested-model F-test](../../../../../nested-model-f-test.md) has distribution $F_{1,6}$. The printed $p$-value 0.001137 strongly rejects no interaction.

**Do not drop fertiliser just because its main-effect ANOVA row has $p=0.7011$.** In this balanced factorial design that row measures a fertiliser effect averaged over varieties; large opposite effects can cancel. The strongly supported interaction requires retaining its associated main effects by [regression model hierarchy](../../../../../principle-of-marginality.md). Seed and year also have evidence of effects in their ANOVA rows, so this table alone gives no compelling simplification of the fitted terms.

The [interaction contrast](../../../../../interaction-contrast.md) is $-4.6200$, with [standard error](../../../../../standard-error.md) 0.7946. The fitted high-minus-low fertiliser effect is $+2.4700$ for variety 1 but $2.4700-4.6200=-2.1500$ for variety 2. The fitted variety-2-minus-variety-1 contrast is $+3.6500$ under low fertiliser and $3.6500-4.6200=-0.9700$ under high fertiliser. Thus **variety 2 performs best under low fertiliser, while high fertiliser benefits variety 1 and reduces variety 2's fitted yield.** The marginal fertiliser effect is only $(2.4700-2.1500)/2=0.1600$.

The four fitted means in the baseline year are $5.5050,7.9750,9.1550,7.0050$ for $(1,L),(1,H),(2,L),(2,H)$ respectively. Add $1.5775$ in 2005 and $0.0875$ in 2006 to every fitted mean. The 2005 coefficient has $p=0.017646$ under a $t_6$ test of a zero contrast with 2004; the analogous 2006 contrast has $p=0.863216$. The latter is lack of evidence for a difference, not proof that the yearly means coincide. [Standard errors](../../../../../standard-error.md) for the combined contrasts require the coefficient [covariance matrix](../../../../../covariance-matrix.md). The experiment is small: [residual standard error](../../../../../residual-standard-error.md) is 0.6882 on only six [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). If the same fields were reused, possible within-field dependence and field allocation would need checking before treating the fitted error independence as established.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
