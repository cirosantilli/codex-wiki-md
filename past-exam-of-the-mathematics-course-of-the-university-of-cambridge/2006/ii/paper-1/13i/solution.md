<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

The fitted [grouped-binomial logistic regression](../../../../../grouped-binomial-logistic-regression.md) [generalized linear model](../../../../../generalized-linear-model.md) treats seasonal hits $H_i$ as independent $\operatorname{Bin}(n_i,p_i)$ variables, with $n_i=\mathrm{AB}_i$ and

$$
\log\frac{p_i}{1-p_i}=\beta_0+\beta_1a_i+\beta_2a_i^2.
$$

Thus the response supplied to `glm` is a proportion, and `weights=AB` supplies its binomial denominator; it is not a regression with equally precise seasonal averages. `I(Age^2)` forms the numerical square rather than using a formula operator. The estimates maximize $\ell(\beta)=\sum_i[H_i\eta_i-n_i\log(1+e^{\eta_i})]$ up to a constant, where $\eta_i=x_i^T\beta$, $x_i=(1,a_i,a_i^2)^T$.

The observed negative [Hessian](../../../../../hessian-matrix.md) is $X^TWX$, $W_{ii}=n_i\widehat p_i(1-\widehat p_i)$. Expanding the score around the true parameter and applying a central-limit approximation gives $\widehat\beta\approx N(\beta,(X^TWX)^{-1})$. The reported [standard errors](../../../../../standard-error.md) are square roots of the diagonal entries of this inverse; the binomial dispersion is fixed at one. Each `z value` divides the coefficient estimate by its [standard error](../../../../../standard-error.md), and the reported two-sided [Wald test](../../../../../wald-test.md) uses a standard normal approximation under the corresponding zero-coefficient hypothesis.

The last line reports the [deviance](../../../../../exponential-family-deviance.md) against the saturated model,

$$
D=2\sum_i\left[H_i\log\frac{H_i}{n_i\widehat p_i}+(n_i-H_i)\log\frac{n_i-H_i}{n_i(1-\widehat p_i)}\right],
$$

with $0\log0=0$. There are 22 seasonal observations and three fitted parameters, so 19 [degrees of freedom](../../../../../degree-of-freedom.md). Under the quadratic-logit model, independent binomial sampling and sufficiently large expected counts, $D\approx\chi^2_{19}$. The value 23.345 gives an upper-tail [probability](../../../../../probability.md) about 0.22, **no evidence of lack of fit at conventional levels**. This approximation and the independence assumption should not be confused with an exact test of a player's ability.

The final commands recover the coefficients, apply the inverse logit $p=(1+e^{-\eta})^{-1}$, plot the observed averages against age, and join the fitted [probabilities](../../../../../probability.md) at the observed ages. The fitted curve is smooth, rises towards its peak at $a=-\widehat\beta_1/(2\widehat\beta_2)\approx29.95$, then falls. Its maximum is about 0.373; the early and late observed points include markedly lower averages. The plot uses equally sized points even though their binomial precisions differ.

<a id="13i/image-observed-seasonal-batting-averages-and-the-fitted-quadratic-logistic-curve"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1-batting-fit.png)

**[Figure 2](#13i/image-observed-seasonal-batting-averages-and-the-fitted-quadratic-logistic-curve). Observed seasonal batting averages and the fitted quadratic logistic curve**.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
