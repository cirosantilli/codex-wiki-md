<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [randomized complete block design](../../../../../randomized-complete-block-design.md) groups similar [experimental units](../../../../../experimental-unit.md) into [experimental blocks](../../../../../blocks-in-experimental-design.md) and places every [treatment](../../../../../treatment.md) once in each [experimental block](../../../../../blocks-in-experimental-design.md), independently randomizing [treatment](../../../../../treatment.md) allocation within [experimental blocks](../../../../../blocks-in-experimental-design.md). Blocking removes background between-block variation from within-block [treatment](../../../../../treatment.md) comparisons. A [balanced incomplete block design](../../../../../balanced-incomplete-block-design.md) has $v$ [treatments](../../../../../treatment.md) and $b$ [experimental blocks](../../../../../blocks-in-experimental-design.md) of size $k<v$, with each [treatment](../../../../../treatment.md) occurring in $r$ [experimental blocks](../../../../../blocks-in-experimental-design.md) and every distinct [treatment](../../../../../treatment.md) pair together in $\lambda$ [experimental blocks](../../../../../blocks-in-experimental-design.md). Counting [treatment](../../../../../treatment.md) occurrences and co-occurrences gives $vr=bk$ and $r(k-1)=\lambda(v-1)$.

A [Latin square](../../../../../latin-square.md) of order $q$ places each of $q$ [treatment](../../../../../treatment.md) symbols once in every row and every column of a $q\times q$ array. This controls two nuisance directions. A [Graeco-Latin square](../../../../../graeco-latin-square.md) superposes two [mutually orthogonal Latin squares](../../../../../mutually-orthogonal-latin-squares.md): each square is Latin, and each ordered pair of symbols from the two squares occurs exactly once. The two symbol factors can then be fitted together with row and column effects. Random permutations of row labels, column labels and [treatment](../../../../../treatment.md) symbols provide a suitable randomized allocation without destroying these balances.

For the operator experiment, fit the additive [normal linear model](../../../../../normal-linear-model.md)

$$
Y_{ij}=\mu+r_i+c_j+\tau_{o(i,j)}+\epsilon_{ij},
\qquad\sum_ir_i=\sum_jc_j=\sum_o\tau_o=0,
\qquad\epsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Here $r_i,c_j$ account for the two fabric directions, and $\tau_o$ is the operator effect. Additivity, independent equal-variance errors and the [normal](../../../../../normal-distribution.md) assumption supply the exact [F-test](../../../../../f-test.md); there is only one observation per cell, so an unrestricted [interaction](../../../../../interaction-statistics.md) model is not available.

In the [analysis of variance for a Latin square](../../../../../analysis-of-variance-for-a-latin-square.md), the three centered factor spaces each have dimension $4-1=3$. Together with the [intercept](../../../../../regression-intercept.md) the model has [rank](../../../../../rank-one-quadratic-form.md) ten, leaving $16-10=6$ residual [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The corrected total has $16-1=15$. The completed calculation is

$$
\begin{array}{c|r|r|r}
\text{source}&\text{df}&\text{SS}&\text{MS}\\\hline
\text{row}&3&5.00&5/3\\
\text{column}&3&8.50&8.5/3\\
\text{operator}&3&18.25&18.25/3\\
\text{residual}&6&17.25&17.25/6=2.875\\
\text{corrected total}&15&49.00&
\end{array}
$$

Under the [null hypothesis](../../../../../null-hypothesis.md) $\tau_1=\cdots=\tau_4=0$, the operator [F-statistic](../../../../../f-statistic.md) is

$$
\boxed{F=\frac{18.25/3}{17.25/6}\simeq2.116.}
$$

The upper five-percent critical value for $F_{3,6}$ is $4.76$, so **the operator effect is not significant at five percent** in this model.

The decision is independent of the order of fitting rows, columns and operators. To prove the required [orthogonality](../../../../../orthogonal-vectors.md), let $u_i$ be any centered row coefficients and $w_o$ any centered operator coefficients. Their observation-space [inner product](../../../../../inner-product.md) is $\sum_{i,j}u_iw_{o(i,j)}=\sum_i u_i\sum_o w_o=0$, since every operator occurs once in each row. The same calculation applies to columns and operators, and all row-column pairs occur once as well. Thus the three centered spaces are mutually [orthogonal](../../../../../orthogonal-vectors.md); their projections commute and sequential sums of squares equal adjusted sums of squares in every fitting order.

With machines included, the layout is a [Graeco-Latin square](../../../../../graeco-latin-square.md): the machine symbols are Latin, and all sixteen operator-machine pairs occur exactly once. Fit

$$
Y_{ij}=\mu+r_i+c_j+\tau_{o(i,j)}+\eta_{m(i,j)}+\epsilon_{ij},
\qquad\sum_m\eta_m=0
$$

in addition to the earlier constraints. The machine space contributes three new [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) and is [orthogonal](../../../../../orthogonal-vectors.md) to the previous factor spaces, so the operator sum of squares remains $18.25$. The residual sum of squares and [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) become

$$
\operatorname{SSE}_{\mathrm{new}}=17.25-16.50=0.75,
\qquad\nu_{\mathrm{new}}=6-3=3.
$$

Hence

$$
\boxed{F_{\mathrm{operator}}=\frac{18.25/3}{0.75/3}=\frac{73}{3}\simeq24.333.}
$$

This exceeds $F_{3,3}(0.05)=9.28$ but not $F_{3,3}(0.01)=29.46$. Therefore **the operator effect is now significant at five percent, but not at one percent**. Adjustment for machines has removed substantial residual variation without altering the operator numerator. This illustrates why a balanced nuisance factor can change precision and significance even when it does not change the estimated [treatment](../../../../../treatment.md) [contrasts](../../../../../contrast-statistics.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
