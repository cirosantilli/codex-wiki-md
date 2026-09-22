<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For word-count vector $x$, the fitted [logistic model](../../../../../../logistic-model.md) is

$$
\log\frac{\widehat p(x)}{1-\widehat p(x)}
=-5.391451+1.859318x_{\rm dollar}
+5.680691x_{\rm winner}+0.923072x_{\rm password}
-6.890095x_{\rm edu}+2.269523x_{\rm credit}
$$



$$
{}+1.198028x_{\rm discount}-3.176676x_{\rm as}
-1.866328x_{\rm I}+4.347929x_{\rm fun}
+0.864456x_{\rm trial}.
$$

Holding other counts fixed, one additional occurrence of "dollar" multiplies the fitted spam odds by $e^{1.859318}$.

The logistic classifier is

$$
\widehat C^{\rm logit}(x)
=\mathbf1_{\{\widehat p(x)>1/2\}}
=\mathbf1_{\{\widehat\beta_0+x^T\widehat\beta>0\}}.
$$

The coefficients maximize the [Bernoulli logistic-regression model](../../../../../../bernoulli-logistic-regression-model.md) likelihood over the training emails.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
