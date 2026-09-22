<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume initially that the design points are distinct and ordered on $[a,b]$. The [cubic smoothing spline](../../../../../../cubic-smoothing-spline.md) minimizes

$$
\boxed{\sum_{i=1}^n\{Y_i-g(X_i)\}^2+\lambda\int_a^b\{g''(t)\}^2\,dt,\qquad\lambda>0,}
$$

over functions with an absolutely continuous first derivative and square-integrable second derivative. Dividing the residual term by $n$ simply changes the scaling assigned to $\lambda$. The [minimum roughness property of the natural cubic spline interpolant](../../../../../../minimum-roughness-property-of-the-natural-cubic-spline-interpolant.md) reduces the problem to [natural cubic splines](../../../../../../natural-cubic-spline.md) with knots at the design points: among functions with any prescribed fitted values, that interpolant has the smallest integrated squared curvature. The minimizer is therefore a [natural cubic smoothing spline](../../../../../../cubic-smoothing-spline.md), with natural second-derivative boundary conditions and linear tails when extended.

Choose a full basis $B_1,\ldots,B_n$ for this natural-spline space. Put $B_{ij}=B_j(X_i)$ and $\Omega_{jk}=\int_a^b B_j''(t)B_k''(t)\,dt$. Writing $g(t)=\sum_jc_jB_j(t)$ changes the objective to

$$
\|Y-Bc\|^2+\lambda c^T\Omega c.
$$

Differentiation gives $(B^TB+\lambda\Omega)\widehat c=B^TY$. Although the curvature penalty has an affine nullspace, the full basis at distinct design points makes the combined matrix [positive definite](../../../../../../positive-definite-matrix.md). Hence

$$
\boxed{\widehat Y=S_\lambda Y,\qquad
S_\lambda=B(B^TB+\lambda\Omega)^{-1}B^T.}
$$

Equivalently, use the cardinal basis that interpolates the observations, making $B=I$ and $S_\lambda=(I+\lambda\Omega)^{-1}$. These are [smoothing matrices](../../../../../../smoothing-matrix.md), symmetric but generally not idempotent. Their [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) are $\operatorname{tr}(S_\lambda)$. As $\lambda\downarrow0$ the fit interpolates; as $\lambda\uparrow\infty$ it approaches [ordinary least squares](../../../../../../ordinary-least-squares.md) on the affine functions. With replicated predictors, use a design matrix for distinct knots and observation weights; the basis form remains valid when identifiable.

Useful choices include [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md), [generalized cross-validation](../../../../../../generalized-cross-validation.md), and estimation of smoothness by [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md) through a mixed-model representation. For fixed $\lambda$, the [leave-one-out residual identity for a linear smoother](../../../../../../leave-one-out-residual-identity-for-a-linear-smoother.md) gives

$$
\mathrm{CV}(\lambda)=\frac1n\sum_i\left[\frac{Y_i-\widehat Y_i}{1-(S_\lambda)_{ii}}\right]^2,
\qquad
\mathrm{GCV}(\lambda)=\frac{\|Y-\widehat Y\|^2/n}{[1-\operatorname{tr}(S_\lambda)/n]^2}.
$$

Minimize these over a suitable range. Choose smoothing by predictive performance or a variance-component likelihood, not by arbitrarily forcing a visually appealing curve.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
