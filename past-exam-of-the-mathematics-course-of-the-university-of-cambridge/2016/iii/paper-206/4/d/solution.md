<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The proposed [generalized additive model](../../../../../../generalized-additive-model.md) retains the binary response and [logit link](../../../../../../logit.md), but replaces the linear age effect by a smooth function:

$$
Y_i\sim\operatorname{Bernoulli}(p_i),\qquad
\log\frac{p_i}{1-p_i}=\alpha+f(a_i)+\gamma d_i,\qquad\sum_i f(a_i)=0.
$$

A penalized [cubic regression spline](../../../../../../cubic-regression-spline.md) represents $f$; frailty remains a parametric coefficient. The plotted age smooth is centered, so its vertical values represent an age contribution to [log odds](../../../../../../log-odds.md), not probabilities or the entire fitted predictor.

**The plot gives no evidence that the nonlinear model improves the mean structure.** The fitted curve is essentially a straight descending line, and the label `s(age,1)` reports [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) close to one, consistent with a linear effect. The widening bands near the ends reflect sparse data and increasing uncertainty, not detected curvature. A linear-age [logistic regression](../../../../../../logistic-regression.md) is therefore adequate on this evidence and simpler to interpret. A formal comparative claim would need a suitable test or predictive/model-selection criterion, but the figure supplies no reason to retain extra nonlinear flexibility.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
