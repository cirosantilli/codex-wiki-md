<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the convention that [ridge regression](../../../../../ridge-regression.md) minimizes $\|Y-Xb\|_2^2/(2n)+(\gamma/2)\|b\|_2^2$. Its [closed-form ridge regression estimator](../../../../../closed-form-ridge-regression-estimator.md) is

$$
\boxed{\widehat b_\gamma=(X^TX+n\gamma I_p)^{-1}X^TY.}
$$

The factors $n$ and $1/2$ here specify the tuning convention. No intercept is needed for the centred responses and predictors.

For the two-component procedure, fix $\delta$ and put $\theta=Y-X\delta$. Differentiating the objective with respect to its dense coefficient $\beta$ gives

$$
-\frac1nX^T(\theta-X\beta)+2\lambda_2\beta=0.
$$

Thus, with $Q=(X^TX+2n\lambda_2I_p)^{-1}$,

$$
\boxed{\widehat\beta_\lambda=QX^T(Y-X\widehat\delta_\lambda).}
$$

The inverse exists because $\lambda_2>0$, even for a rank-deficient design. The sum of the fitted sparse and dense components is the [Lava estimator](../../../../../lava-estimator.md).

Multiplying by $2n$ and completing the square gives the exact profile calculation

$$
\begin{aligned}
\|\theta-X\beta\|_2^2+2n\lambda_2\|\beta\|_2^2
&=\theta^T\theta-2\beta^TX^T\theta+\beta^TQ^{-1}\beta\\
&=(\beta-QX^T\theta)^TQ^{-1}(\beta-QX^T\theta)+\theta^T(I_n-XQX^T)\theta.
\end{aligned}
$$

Let $B=I_n-XQX^T$. A [singular value decomposition](../../../../../singular-value-decomposition.md) of $X$ shows that its eigenvalues are $2n\lambda_2/(r_i^2+2n\lambda_2)$ in nonzero singular directions and one in the orthogonal complement. Hence $B$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md). Take its symmetric [principal square root of a positive semidefinite matrix](../../../../../principal-square-root-of-a-positive-semidefinite-matrix.md), $A=B^{1/2}$. Profiling out $\beta$ therefore yields the [Lasso reduction for the Lava estimator](../../../../../lasso-reduction-for-the-lava-estimator.md):

$$
\boxed{\widehat\delta_\lambda\in\arg\min_\delta\left\{\frac1{2n}\|AY-AX\delta\|_2^2+\lambda_1\|\delta\|_1\right\},\qquad A=(I_n-XQX^T)^{1/2}.}
$$

No restandardization of $AX$ is needed: this is the exact transformed objective with its original penalty.

Write $\widetilde X=AX$, $h=\widehat\delta_\lambda-\delta^0$, and $\eta=\widetilde X\beta^0+A\varepsilon$. Then $AY=\widetilde X\delta^0+\eta$. Comparing the transformed [Lasso](../../../../../lasso.md) objective at $\widehat\delta_\lambda$ and $\delta^0$ gives the [Basic inequality for the Lasso](../../../../../basic-inequality-for-the-lasso.md)

$$
\frac1{2n}\|\widetilde Xh\|_2^2\leq\frac1n\eta^T\widetilde Xh+\lambda_1(\|\delta^0\|_1-\|\widehat\delta_\lambda\|_1).
$$

On $\Omega$, [Holder inequality](../../../../../holder-inequality.md) bounds the score by $\lambda_1\|h\|_1$. Using $\|h\|_1\leq\|\widehat\delta_\lambda\|_1+\|\delta^0\|_1$ cancels the fitted penalty and yields the [slow-rate prediction bound for the Lasso](../../../../../slow-rate-prediction-bound-for-the-lasso.md):

$$
\boxed{\frac1n\|\widetilde Xh\|_2^2\leq4\lambda_1\|\delta^0\|_1.}
$$

Finally, if $\kappa=\lambda_{\max}(XQX^T)<1$, then $B\succeq(1-\kappa)I_n$, so

$$
\|\widetilde Xh\|_2^2=(Xh)^TB(Xh)\geq(1-\kappa)\|Xh\|_2^2.
$$

Consequently

$$
\boxed{\frac1n\|X(\widehat\delta_\lambda-\delta^0)\|_2^2\leq\frac{4\lambda_1\|\delta^0\|_1}{1-\kappa}.}
$$

Positive $\lambda_2$ actually guarantees $\kappa<1$ for every finite design; the factor measures how much prediction norm the profiling transformation can remove.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
