<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the initial [normal linear model](../../../../../normal-linear-model.md), the [design matrix](../../../../../design-matrix.md) has rows $(1,x_1,x_2,x_3)$. The eight factorial corners have balanced signs and [orthogonal](../../../../../orthogonal-vectors.md) coordinate columns; the six centre points contribute only to the intercept. Consequently

$$
X^TX=\operatorname{diag}(14,8,8,8).
$$

Using the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) gives the [least-squares estimator](../../../../../ordinary-least-squares-estimators.md)

$$
\boxed{\begin{aligned}
\widehat\beta_0&=\frac1{14}\sum_{i=1}^{14}y_i,\\
\widehat\beta_1&=\frac{-y_1-y_2-y_3-y_4+y_5+y_6+y_7+y_8}{8},\\
\widehat\beta_2&=\frac{-y_1-y_2+y_3+y_4-y_5-y_6+y_7+y_8}{8},\\
\widehat\beta_3&=\frac{-y_1+y_2-y_3+y_4-y_5+y_6-y_7+y_8}{8}.
\end{aligned}}
$$

It is a linear transformation of independent normal responses, so its [sampling distribution](../../../../../sampling-distribution.md) is

$$
\boxed{\widehat\beta\sim N_4\!\left(\beta,\sigma^2
\operatorname{diag}(1/14,1/8,1/8,1/8)\right).}
$$

The four estimated coefficients are [independent](../../../../../independent-random-variables.md), since they are jointly normal with diagonal [covariance matrix](../../../../../covariance-matrix.md).

Adding the axial settings produces a [central composite design](../../../../../central-composite-design.md): eight factorial corners, six axial points and six replicated centre points. The axial distance $1.682$ is the rounded value of $8^{1/4}=1.6817928\ldots$. With that exact distance it is a [rotatable design](../../../../../rotatable-design.md) for a full quadratic model. Indeed, sign symmetry annihilates odd moments, all coordinates have the same second moment, and the fourth moments satisfy

$$
\sum x_j^4=8+2\alpha^4,\qquad
\sum x_j^2x_l^2=8\quad(j\ne l).
$$

Rotational symmetry requires the first to be three times the second, giving $\alpha^4=8$. Using the printed rounded distance makes rotatability approximate, rather than mathematically exact.

The full [quadratic regression](../../../../../quadratic-regression.md) mean has ten coefficients:

$$
y=\beta_0+\sum_{j=1}^3\beta_jx_j+
\sum_{j=1}^3\beta_{jj}x_j^2+
\beta_{12}x_1x_2+\beta_{13}x_1x_3+\beta_{23}x_2x_3+\varepsilon.
$$

The expanded [design matrix](../../../../../design-matrix.md) has rank ten. To verify this rather than just count parameters, suppose such a quadratic vanishes at every setting. Its centre value sets its constant term to zero; subtracting the values at opposite axial points sets every linear coefficient to zero, and adding them then sets every squared-coordinate coefficient to zero. On the factorial corners, [orthogonality](../../../../../orthogonal-vectors.md) of the three pair-product columns forces their coefficients to zero as well. Thus all ten columns are independent, leaving $20-10=10$ residual [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md).

There are $15$ distinct settings: eight corners, six axial points and the centre. The six centre replicates give the only [pure error](../../../../../pure-error.md), with $6-1=5$ degrees and sum of squares $859.33$. The saturated setting-mean model has $15$ parameters, so the [lack of fit](../../../../../lack-of-fit.md) beyond the quadratic model has $15-10=5$ degrees. For any setting $r$ with $n_r$ replicates, the identity

$$
\sum_j(y_{rj}-\widehat y_r)^2
=\sum_j(y_{rj}-\bar y_r)^2+n_r(\bar y_r-\widehat y_r)^2
$$

splits the [residual sum of squares](../../../../../residual-sum-of-squares.md) into [pure error](../../../../../pure-error.md) and [lack of fit](../../../../../lack-of-fit.md); the cross term vanishes because the deviations from the setting mean sum to zero. Summing gives

$$
\mathrm{SS}_{\mathrm{LOF}}=1860.98-859.33=1001.65.
$$

Under a correct quadratic mean with independent errors of constant normal [variance](../../../../../variance-split.md), the pure-error and lack-of-fit projections are [orthogonal](../../../../../orthogonal-vectors.md), hence their sums of squares are independent with respective distributions $\sigma^2\chi^2_5$ and $\sigma^2\chi^2_5$. The [Lack-of-fit F-test](../../../../../lack-of-fit-f-test.md) therefore uses

$$
\boxed{F=\frac{1001.65/5}{859.33/5}=1.1656,\qquad F\sim F_{5,5}\text{ under the null}.}
$$

This is below the given $10\%$ and $5\%$ critical values $3.45$ and $5.05$. **There is no significant lack of fit at either level.** That is failure to reject this quadratic mean, not proof that it is exact or that a maximum has already been located. The pure-error denominator also assumes the error variance at the centre represents the common variance throughout the experiment.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
