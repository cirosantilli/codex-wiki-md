<h1 id="5/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The original PDF's age smooth is nearly flat, its uncertainty band includes zero across the age range, and its approximate [p-value](../../../../../../../p-value.md) is $0.859$. The exposure smooth is increasing and convex: it is fairly flat at low exposure and rises more steeply at high exposure. Its [effective degrees of freedom](../../../../../../../effective-degrees-of-freedom.md) $1.895$ suggest a modest departure from a straight line, rather than a highly oscillatory relationship.

A suitable simpler model is therefore the grouped [quasibinomial regression](../../../../../../../quasibinomial-regression.md)

$$
\boxed{\log\frac{p_i}{1-p_i}=\beta_0+\beta_1 e_i+\beta_2e_i^2,\qquad
\operatorname{Var}(Y_i)=\phi m_ip_i(1-p_i),}
$$

with age omitted and dispersion estimated. A positive quadratic coefficient captures the convex exposure relationship; retaining the linear term respects the usual polynomial hierarchy. This model should be refitted, rather than assigning coefficients from the smooth plot. Compare its residual pattern and dispersion-adjusted fit with the additive model to check that the quadratic approximation is adequate. **An exposure-only quadratic logit model is a justified parsimonious candidate**, while the graph does not justify a sharp threshold or a zero-dispersion model.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
