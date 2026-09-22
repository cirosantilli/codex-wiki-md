<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write the binary [incidence matrix of a set system](../../../../../incidence-matrix-of-a-set-system.md) as $N$ to avoid confusing it with a sample size. Then

$$
(NN^T)_{ii}=\sum_jN_{ij}
$$

counts the number of blocks containing treatment $i$, and for $i\ne l$, $(NN^T)_{il}=\sum_jN_{ij}N_{lj}$ counts blocks containing both treatments. The displayed structure therefore makes every treatment replication equal to $r$ and every pair concurrence equal to $\lambda$.

Assume the usual nonempty [block design](../../../../../block-design.md), with $r>0$ and $k>0$. If $r=\lambda$, any block containing one treatment contains every other treatment: otherwise that treatment's replication would exceed its concurrence with the omitted one. Every block is consequently complete, so **$k=t$ and $r=b$**. With random allocation within blocks this is a [randomized complete block design](../../../../../randomized-complete-block-design.md). If $\lambda<r$, the design is a [balanced incomplete block design](../../../../../balanced-incomplete-block-design.md). Counting partners of a fixed treatment in its $r$ blocks gives

$$
r(k-1)=\lambda(t-1),\qquad tr=bk.
$$

For $t>1$, $\lambda/r<1$ gives $k-1<t-1$, hence $k<t$. Moreover $NN^T$ has [eigenvalue](../../../../../eigenvalue.md) $r-\lambda>0$ on the $(t-1)$-dimensional zero-sum subspace and [eigenvalue](../../../../../eigenvalue.md) $r+(t-1)\lambda>0$ on the constant direction. Thus $\operatorname{rank}(NN^T)=t$, while $\operatorname{rank}(NN^T)\leq\operatorname{rank}(N)\leq b$. This proves **$b\geq t$**, the [Fisher's inequality for block designs](../../../../../fisher-s-inequality-for-block-designs.md). The case $\lambda=0$ allows singleton blocks; their lack of connectedness prevents general treatment comparison after block adjustment, but does not invalidate the rank inequality.

First ignore the day information and use a [one-way normal linear model](../../../../../one-way-normal-linear-model.md) with five group means and independent errors of common [variance](../../../../../variance-split.md). There are $20$ observations. The [analysis of variance](../../../../../analysis-of-variance.md) has treatment, residual and corrected-total [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) $4,15,19$, respectively. The [mean squares in ANOVA](../../../../../mean-square-in-anova.md) give

$$
\boxed{F_{\mathrm{unblocked}}=
\frac{42.4/4}{46.7/15}=3.4047.}
$$

Under equal treatment means this has the [F-distribution](../../../../../f-distribution.md) with $(4,15)$ degrees. It exceeds the given $5\%$ upper critical value $3.06$, so **the unblocked analysis rejects equality at $5\%$**.

The actual day allocation omits a different treatment on each of the five days. Hence it is a [balanced incomplete block design](../../../../../balanced-incomplete-block-design.md) with

$$
\boxed{t=b=5,\qquad r=k=4,\qquad\lambda=3.}
$$

Every pair occurs on exactly the three days omitting neither member. In the additive [two-way analysis of variance](../../../../../two-way-analysis-of-variance.md), use an intercept, four independent treatment contrasts and four day contrasts. The design is connected, so the model rank is $9$ and its residual has $20-9=11$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). Day effects and treatment effects are not orthogonal, because a different treatment is absent each day; the unadjusted treatment sum of squares cannot be used for the adjusted test.

Enter days first and then treatments. The supplied [sequential sums of squares](../../../../../sequential-sum-of-squares.md) give

$$
\mathrm{SS}_{E}=89.1-28.4-18.3=42.4,\qquad
\boxed{F_{\mathrm{adjusted}}=
\frac{18.3/4}{42.4/11}=1.1869.}
$$

The day, treatment-after-day, residual and corrected-total [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) are $4,4,11,19$. Under the additive [normal linear model](../../../../../normal-linear-model.md) and the null of equal treatment effects, the adjusted numerator and residual squared lengths are independent [chi-squared](../../../../../chi-squared-distribution.md) quantities, so the ratio has the [F-distribution](../../../../../f-distribution.md) with $(4,11)$ degrees. It is below even the given $10\%$ critical value $2.54$. **After accounting for days there is no significant treatment difference at either $10\%$ or $5\%$.** This inference assumes independent homoscedastic normal errors and an additive day effect; with one observation per observed treatment–day cell, unrestricted interactions cannot also be fitted.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
