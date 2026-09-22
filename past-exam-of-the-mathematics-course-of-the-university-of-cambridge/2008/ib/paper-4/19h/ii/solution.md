<h1 id="19h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $x_i=\sin(2\theta_i)$. The [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) formulas for [simple linear regression](../../../../../../simple-linear-regression.md) give

$$
\boxed{\widehat\beta=\frac{\sum_i(x_i-\bar x)(Y_i-\bar Y)}{\sum_i(x_i-\bar x)^2}=\frac{S_{xy}}{S_{xx}},\qquad\widehat\alpha=\bar Y-\widehat\beta\bar x.}
$$

Using the supplied rounded summaries gives $\widehat\beta\approx21082.7$ metres and $\widehat\alpha\approx312.0$ metres. Recomputing directly from the printed table gives approximately $21082.4$ and $312.0$ metres, respectively, so the small summary rounding differences do not affect the conclusion.

I would not accept the model merely because the [Student t-test](../../../../../../student-s-t-test.md) fails to reject a zero [regression intercept](../../../../../../regression-intercept.md). That [hypothesis test](../../../../../../statistical-hypothesis-test.md) tests one parameter restriction within the assumed model, not the adequacy of its error assumptions or its functional form. In particular, complementary elevations $\theta$ and $90^\circ-\theta$ have exactly the same $x_i$ and hence the same fitted mean, but their observed low-angle minus high-angle ranges are

$$
864,\quad1871,\quad1913,\quad1173\ \text{metres}
$$

for the four corresponding pairs. All four are positive, suggesting an elevation-dependent effect omitted by the mean model, such as air resistance, rather than random scatter determined only by $\sin(2\theta)$. This is a [regression diagnostics](../../../../../../regression-diagnostics.md) concern, not a claim that these finite data logically rule out the normal-error model. The correct conclusion is **nonrejection of the intercept restriction does not validate the regression model**; further checks of the residual pattern and error assumptions are needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
