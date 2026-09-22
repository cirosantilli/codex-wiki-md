<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $Y_{ijkl}$ be the flight distance in millimetres for paper level $i$, launch-angle level $j$, design level $k$ and replicate $l$, where $i,j,k\in\{1,2\}$ and $l\in\{1,2\}$. The full [factorial design](../../../../../factorial-design.md) is fitted by the [normal linear model](../../../../../normal-linear-model.md)

$$
Y_{ijkl}=\mu+P_i+A_j+D_k+(PA)_{ij}+(PD)_{ik}+(AD)_{jk}+(PAD)_{ijk}+\varepsilon_{ijkl},\qquad
\varepsilon_{ijkl}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The assumptions are independent errors with a common [variance](../../../../../variance-split.md) and [normal distribution](../../../../../normal-distribution.md), and the displayed factor-combination mean structure. The [corner-point constraints](../../../../../corner-point-constraint.md) are

$$
P_1=A_1=D_1=0,\quad
(PA)_{1j}=(PA)_{i1}=(PD)_{1k}=(PD)_{i1}=(AD)_{1k}=(AD)_{j1}=0,
$$

and $(PAD)_{ijk}=0$ whenever at least one index equals $1$. Thus the eight free mean coefficients are $\mu,P_2,A_2,D_2,(PA)_{22},(PD)_{22},(AD)_{22},(PAD)_{222}$. These [treatment coding](../../../../../treatment-coding.md) coefficients are comparisons at the other factors' reference levels, rather than necessarily averaged main effects.

To test the three-factor [interaction term](../../../../../interaction-term.md), compare the full model with the model retaining all main effects and all two-factor [interactions](../../../../../interaction-statistics.md). The [null hypothesis](../../../../../null-hypothesis.md) is $(PAD)_{222}=0$, against a nonzero value. Removing it increases the [residual sum of squares](../../../../../residual-sum-of-squares.md) by $21025$ and removes one parameter. With eight residual [degrees of freedom](../../../../../degree-of-freedom.md), the [nested-model F-test](../../../../../nested-model-f-test.md) gives

$$
\boxed{F=\frac{21025/1}{8392178/8}=0.02004,\qquad F\mid H_0\sim F_{1,8},\qquad p=0.8909.}
$$

There is no evidence that this three-factor [interaction](../../../../../interaction-statistics.md) is needed. This does not establish that all two-factor [interactions](../../../../../interaction-statistics.md) vanish: the paper-design interaction is substantial.

The `stepAIC` command performs [stepwise selection by the Akaike information criterion](../../../../../stepwise-selection-by-the-akaike-information-criterion.md). Its upper scope is the full factorial model and its lower scope is the intercept-only model. Starting from the full model, it compares admissible additions and deletions, preserving the hierarchy of [interaction terms](../../../../../interaction-term.md), and chooses changes that reduce the [Akaike information criterion](../../../../../akaike-information-criterion.md). With the supplied scope its default search permits both directions. For these Gaussian fits the displayed criterion, up to constants common to all models, is $16\log(\mathrm{RSS}/16)+2k$, where $k$ counts mean coefficients. The first deletion changes it from $226.72$ to $224.76$: the small increase in [residual sum of squares](../../../../../residual-sum-of-squares.md) is outweighed by removing a parameter. This is a greedy [model selection](../../../../../model-selection.md) procedure, not an exhaustive search or a sequence of fixed-level [hypothesis tests](../../../../../statistical-hypothesis-test.md). The command's arguments are described in [the MASS documentation](https://stat.ethz.ch/R-manual/R-devel/library/MASS/html/stepAIC.html).

For the selected model, let $p=\mathbf1_{\{i=2\}}$ and $d=\mathbf1_{\{k=2\}}$. Then

$$
Y=\beta_0+\beta_Pp+\beta_Dd+\beta_{PD}pd+\varepsilon,\qquad \varepsilon\sim N(0,\sigma^2)
$$

independently between flights. It has no angle term. The [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) of its mean coefficients are also obtained by [ordinary least squares](../../../../../ordinary-least-squares.md):

$$
\begin{array}{c|rr}
\text{coefficient}&\text{estimate}&\text{standard error}\\\hline
\beta_0&2303.8&446.3\\
\beta_P&3073.5&631.2\\
\beta_D&2107.5&631.2\\
\beta_{PD}&-4836.0&892.6
\end{array}
$$

For example, the four fitted means are just the four paper-design cell means, each averaging four flights over the angle levels. With $s^2=\mathrm{RSS}/12$, the [variance-covariance matrix](../../../../../covariance-matrix.md) of the coefficient estimates is $s^2(X^TX)^{-1}$. Its diagonal gives the displayed [standard errors](../../../../../standard-error.md); their ratios are $s/2,s/\sqrt2,s/\sqrt2,s$, with $s=892.6$ mm.

The final line of `summary(model2.lm)` is the joint [nested-model F-test](../../../../../nested-model-f-test.md) of $H_0:\beta_P=\beta_D=\beta_{PD}=0$, comparing this four-parameter model with a common mean. Its statistic is

$$
\frac{(\mathrm{RSS}_{\mathrm{null}}-\mathrm{RSS}_{\mathrm{selected}})/3}{\mathrm{RSS}_{\mathrm{selected}}/12}=10.66,
$$

with [F-distribution](../../../../../f-distribution.md) $F_{3,12}$ under the fixed-model null and [P-value](../../../../../p-value.md) $0.001057$. Thus the selected paper-design terms jointly improve the fit substantially. The [coefficient of determination](../../../../../coefficient-of-determination.md) $0.7272$ means they account for about $72.7\%$ of the observed centred variation. These nominal inferential summaries do not adjust for the preceding [model selection](../../../../../model-selection.md) on the same data.

Using the unrounded fitted means gives

$$
\begin{array}{c|rr}
&\text{high-performance design}&\text{simple design}\\\hline
80\ \mathrm{g/m^2}&2303.75&4411.25\\
50\ \mathrm{g/m^2}&5377.25&2648.75
\end{array}
$$

in millimetres. Hence **choose the high-performance design with the lighter paper; the fitted model leaves both launch angles tied**, with expected distance about $5377$ mm. A preference for one angle is not supported by this selected model. The strong paper-design [interaction](../../../../../interaction-statistics.md) reverses the design comparison: the simple design is better on heavy paper, whereas the high-performance design is better on light paper. Consequently a single design effect averaged over paper types would conceal the main result. There is little evidence here for an angle effect, and considerable flight-to-flight variability remains.

Before fitting, inspect raw-distance dot plots for all eight factor combinations, and [interaction plots](../../../../../interaction-plot.md) of cell means against design, with separate lines for paper and panels for angle. With only two replicates per cell, showing individual observations is more informative than elaborate box plots. These reveal reversals, spread and possible unusual flights. Afterwards inspect a [residual-versus-fitted plot](../../../../../residual-versus-fitted-plot.md), a [Q-Q plot](../../../../../q-q-plot.md) of residuals, a [scale-location plot](../../../../../scale-location-plot.md), residuals against each factor and, if recorded, flight order, and [Cook's distance](../../../../../cook-s-distance.md) for influential observations. Residual patterns by angle would question its deletion, while unequal spread or departures from the [normal distribution](../../../../../normal-distribution.md) would question the error assumptions rather than merely demand another mean term.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
