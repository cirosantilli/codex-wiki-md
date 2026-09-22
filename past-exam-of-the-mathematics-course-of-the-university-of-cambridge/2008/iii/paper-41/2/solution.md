<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $m=\overline Y_{+++}$, $r_i=\overline Y_{i++}$ and $c_j=\overline Y_{+j+}$. The proposed [least-squares estimators](../../../../../ordinary-least-squares-estimators.md) satisfy the sum-to-zero constraints because $\sum_i r_i=Im$ and $\sum_j c_j=Jm$. Define $e_{ijk}=Y_{ijk}-r_i-c_j+m$. Direct summation gives

$$
\sum_{j,k}e_{ijk}=0\quad\hbox{for every }i,\qquad \sum_{i,k}e_{ijk}=0\quad\hbox{for every }j.
$$

Now write any other admissible parameters as $\mu=m+u$, $\alpha_i=r_i-m+a_i$, $\beta_j=c_j-m+b_j$, where $\sum_i a_i=\sum_j b_j=0$. Expanding the [ordinary least squares](../../../../../ordinary-least-squares.md) criterion, the cross-products with $e$ vanish by the preceding identities. The cross-products between $u$, $a_i$ and $b_j$ vanish by their zero sums. Consequently

$$
S=\sum_{i,j,k}e_{ijk}^2+IJK u^2+JK\sum_i a_i^2+IK\sum_j b_j^2.
$$

Every added term is nonnegative and all vanish only at $u=0$, $a_i=b_j=0$. This proves the unique constrained minimum, with

$$
\boxed{\widehat\mu=m,\qquad\widehat\alpha_i=r_i-m,\qquad\widehat\beta_j=c_j-m.}
$$

The additive-model [residual sum of squares](../../../../../residual-sum-of-squares.md) and intercept-only [residual sum of squares](../../../../../residual-sum-of-squares.md) are therefore

$$
\operatorname{RSS}_1=\sum_{i,j,k}(Y_{ijk}-r_i-c_j+m)^2,\qquad \operatorname{RSS}_0=\sum_{i,j,k}(Y_{ijk}-m)^2.
$$

The same [orthogonality](../../../../../orthogonal-vectors.md) gives the [analysis of variance](../../../../../analysis-of-variance.md) identity

$$
\operatorname{RSS}_0=\operatorname{RSS}_1+SS_A+SS_B,\qquad SS_A=JK\sum_i(r_i-m)^2,\quad SS_B=IK\sum_j(c_j-m)^2.
$$

Fitting factor B alone yields fitted values $c_j$ and residual sum $\operatorname{RSS}_0-SS_B$. Fitting A alone gives residual sum $\operatorname{RSS}_0-SS_A$. Adding B after A then reduces it to $\operatorname{RSS}_1$, a reduction of $SS_B$ again. **The reduction due to B is $SS_B$ in either order.** This is [balanced factorial orthogonality](../../../../../balanced-factorial-orthogonality.md); it generally fails for unequal cell replication.

There are $12$ observations. The additive model estimates $1+(3-1)+(2-1)=4$ independent parameters, so the missing [degrees of freedom](../../../../../degree-of-freedom.md) are **A: 2, B: 1, residuals: 8**. The individual requested residual sums are below.

To check for an [interaction](../../../../../interaction-statistics.md), extend the [normal linear model](../../../../../normal-linear-model.md) to $\mu+\alpha_i+\beta_j+\gamma_{ij}$, with each row and column sum of $\gamma$ zero. Equivalently, fit the six unrestricted cell means. Its [residual sum of squares](../../../../../residual-sum-of-squares.md) is the within-cell sum

$$
\operatorname{RSS}_{\mathrm{cell}}=\sum_{i,j,k}(Y_{ijk}-\overline Y_{ij+})^2.
$$

The interaction adds $(I-1)(J-1)=2$ parameters; the cell-means residual has $IJ(K-1)=6$ [degrees of freedom](../../../../../degree-of-freedom.md). Under the no-interaction [null hypothesis](../../../../../null-hypothesis.md) and the independent equal-variance [normal](../../../../../normal-distribution.md) error model,

$$
\boxed{F=\frac{(2.6867-\operatorname{RSS}_{\mathrm{cell}})/2}{\operatorname{RSS}_{\mathrm{cell}}/6}\sim F_{2,6}.}
$$

The numerator and denominator arise from orthogonal [Gaussian](../../../../../normal-distribution.md) projections, proving the exact [F-test](../../../../../f-test.md). Reject for a sufficiently large value. The printed additive [analysis of variance](../../../../../analysis-of-variance.md) table does not supply $\operatorname{RSS}_{\mathrm{cell}}$, so it cannot determine this test statistic numerically; the replicated cell data would do so.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
