<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The model is linear in each coded covariate on the log-hazard scale, not necessarily in the raw scientific variable. For a continuous variable $z$, begin with plots and a scientifically plausible range of forms. Compare $\beta z$ with a prespecified transformation such as $\beta\log z$ when $z>0$, or use a [restricted cubic spline](../../../../../../restricted-cubic-spline.md) or [fractional polynomial](../../../../../../fractional-polynomial.md) to represent a flexible smooth effect. Do not treat arbitrary integer category codes as a linear quantitative measurement without justification.

Plot [martingale residuals](../../../../../../martingale-residual.md) from a suitable model against $z$ with a smooth trend. A residual pattern can suggest a missing or misspecified effect; these residuals are asymmetric, so the smooth relationship is more informative than judging normality. A model omitting $z$ helps reveal its overall shape; plots after including it help assess remaining misspecification. Partial-residual displays or fitted effect curves with uncertainty give complementary information.

Assess nonlinearity with a joint [likelihood](../../../../../../likelihood-function.md)-ratio or score test for the nonlinear terms in a spline extension. The models containing only $z$ and only $\log z$ are generally nonnested, so a difference in their log-[likelihoods](../../../../../../likelihood-function.md) is not automatically chi-squared. They can be compared by a justified nonnested criterion or validation, or embedded in a model containing both $z$ and $\log z$ and tested by dropping one term. Such an encompassing model may be highly collinear, and its coefficients should not be interpreted in isolation. If $z$ can be zero or negative, $\log z$ is undefined; choose an appropriate form rather than silently adding an arbitrary offset. **Transformation choice is a question about the entire effect curve and its supported range**, not only one coefficient's significance. Recheck time constancy after revising the functional form, since misspecification can mimic nonproportionality.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
