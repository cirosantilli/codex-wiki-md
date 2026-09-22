<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [ordinary least squares](../../../../../ordinary-least-squares.md) objective has [gradient](../../../../../gradient.md) $2X^TX\beta-2X^TY$. The [normal equation](../../../../../normal-equation.md) therefore gives

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

The [Gram matrix](../../../../../gram-matrix.md) $X^TX$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md) because $X$ has full column rank. More explicitly, for any $b$,

$$
R(b)=R(\widehat\beta)+(b-\widehat\beta)^TX^TX(b-\widehat\beta),
$$

since $X^T(Y-X\widehat\beta)=0$. This proves that the displayed solution is the unique global minimum.

The [fitted values](../../../../../fitted-values.md) are $\widehat Y=X\widehat\beta=HY$, where the [hat matrix](../../../../../hat-matrix.md) is

$$
H=X(X^TX)^{-1}X^T.
$$

The inverse of the symmetric matrix $X^TX$ is symmetric, so $H^T=H$. Multiplication gives $H^2=X(X^TX)^{-1}(X^TX)(X^TX)^{-1}X^T=H$. Thus $H$ is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the [column space](../../../../../column-space.md) of the [design matrix](../../../../../design-matrix.md).

The [regression residual](../../../../../regression-residual.md) vector is $e=Y-\widehat Y=GY$ with $G=I_n-H$. Consequently $G^T=G$, $G^2=I_n-2H+H^2=G$, and the [residual sum of squares](../../../../../residual-sum-of-squares.md) is

$$
\boxed{e^Te=Y^TG^TGY=Y^TGY.}
$$

By [fitted-residual orthogonality](../../../../../fitted-residual-orthogonality.md), $GH=0$. Using $\operatorname{Cov}(Y)=\sigma^2I_n$, the cross-[covariance matrix](../../../../../covariance-matrix.md) is

$$
\boxed{\operatorname{Cov}(e,\widehat Y)=G\sigma^2I_nH^T=0.}
$$

Both vectors are jointly normal, so they are also independent by [independence of uncorrelated jointly normal variables](../../../../../independence-of-uncorrelated-jointly-normal-variables.md). The zero covariance calculation itself only needs the common error variance and lack of error correlations.

For the first wind fit, let $v_i$ be wind velocity and $Y_i$ electrical output. The [simple linear regression](../../../../../simple-linear-regression.md) is $Y_i=\alpha+\beta v_i+\varepsilon_i$, with independent $\varepsilon_i\sim N(0,\sigma^2)$. It has two fitted mean parameters and $25-2=23$ [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md). The missing [analysis of variance](../../../../../analysis-of-variance.md) entries are therefore **velocity degrees of freedom $1$, velocity mean square $8.9296$, and residual degrees of freedom $23$**. The residual mean square is $1.2816/23\simeq0.05572$, and $8.9296/(1.2816/23)\simeq160.25$, consistent with the printed value after rounding.

Because the model includes a [regression intercept](../../../../../regression-intercept.md), the [coefficient of determination](../../../../../coefficient-of-determination.md) is the explained sum of squares divided by the total centered sum of squares:

$$
R^2=\frac{8.9296}{8.9296+1.2816}=1-\frac{1.2816}{10.2112}\simeq\boxed{0.8745}.
$$

A large [coefficient of determination](../../../../../coefficient-of-determination.md) does not rule out a wrong mean function. In the PDF's first [residual-versus-fitted plot](../../../../../residual-versus-fitted-plot.md), residuals are negative at both ends and positive in the middle. This curved pattern agrees with the visibly flattening output-versus-velocity relationship and motivates a [polynomial regression](../../../../../polynomial-regression.md) with a quadratic term.

The second wind model is $Y_i=\alpha+\beta_1v_i+\beta_2v_i^2+\varepsilon_i$, again with independent common-variance normal errors. Its fitted mean is $-1.155898+0.722936v_i-0.038121v_i^2$. The line marked (A) is a two-sided [Student t-test](../../../../../student-s-t-test.md) of $H_0:\beta_2=0$ against $H_1:\beta_2\ne0$, conditional on retaining the intercept and linear term. Under the [null hypothesis](../../../../../null-hypothesis.md),

$$
t=\frac{-0.038121}{0.004797}\simeq-7.947\sim t_{22}.
$$

Its two-sided [p-value](../../../../../p-value.md) is $6.59\times10^{-8}$. This is far below $0.05$, so **reject a purely linear mean in favour of the quadratic fit**. Equivalently, the extra-term [nested-model F-test](../../../../../nested-model-f-test.md) has $F=t^2\simeq63.15$ and null law $F_{1,22}$.

The third fit is a [reciprocal-predictor regression](../../../../../reciprocal-predictor-regression.md), $Y_i=a+b/v_i+\varepsilon_i$, with estimated mean $2.9789-6.9345/v_i$. It has two mean parameters rather than the quadratic model's three. Its residual standard error is smaller, $0.09417$ versus $0.1227$, and its [coefficient of determination](../../../../../coefficient-of-determination.md) is larger, $0.9800$ versus $0.9676$. The corresponding [residual sums of squares](../../../../../residual-sum-of-squares.md) are approximately $23(0.09417)^2=0.20396$ and $22(0.1227)^2=0.33122$. **The reciprocal fit is preferable on both these fit measures and parsimony.** The two models are not nested, so an ordinary extra-term [F-test](../../../../../f-test.md) between them is inappropriate. On the common normal-error likelihood, the difference $\operatorname{AIC}_3-\operatorname{AIC}_2=25\log(0.20396/0.33122)-2\simeq-14.12$ also favours the third model.

Neither lower [residual sum of squares](../../../../../residual-sum-of-squares.md) nor a higher [coefficient of determination](../../../../../coefficient-of-determination.md) establishes adequate assumptions. The quadratic [residual-versus-fitted plot](../../../../../residual-versus-fitted-plot.md) removes the original pronounced curvature; the reciprocal plot also has no comparably obvious mean trend. The low-output residuals appear somewhat more spread out, so check [scale-location plots](../../../../../scale-location-plot.md) and residuals against velocity for [heteroscedasticity](../../../../../heteroscedastic.md). [Q-Q plots](../../../../../q-q-plot.md) assess normality; residuals against observation order assess serial dependence; [regression leverage](../../../../../regression-leverage.md) and [Cook's distance](../../../../../cook-s-distance.md) identify influential observations. Further [cross-validation](../../../../../cross-validation.md), replicate observations at comparable velocities, and prediction errors would help choose between their extrapolation behaviours. Both fitted shapes should be judged principally over the observed positive-velocity range.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
