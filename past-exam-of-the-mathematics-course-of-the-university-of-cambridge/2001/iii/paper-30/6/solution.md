<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the general [normal linear model](../../../../../normal-linear-model.md), minimizing $\|Y-X\beta\|^2$ gives the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) $X^TX\widehat\beta=X^TY$. Full column rank makes $X^TX$ invertible, so

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad
\mathbb E\widehat\beta=\beta,\qquad
\operatorname{Cov}(\widehat\beta)=\sigma^2(X^TX)^{-1}.}
$$

The mean and covariance follow by substituting $Y=X\beta+\epsilon$ and using $\mathbb E\epsilon=0$, $\operatorname{Cov}(\epsilon)=\sigma^2I$. Normal errors also give the exact multivariate normal distribution of this estimator.

Use [coded experimental variables](../../../../../coded-experimental-variable.md)

$$
\boxed{x_1=\frac{\xi_1-95}{5},\qquad x_2=\frac{\xi_2-37.5}{2.5}.}
$$

Their origin is the middle of the allowed rectangle, and the stated endpoints become $\pm1$. The four corners and $n_0$ center runs give mutually orthogonal columns $1,x_1,x_2$, with

$$
X^TX=\operatorname{diag}(4+n_0,4,4).
$$

Writing $\bar Y_0=n_0^{-1}\sum_{i=5}^{4+n_0}Y_i$ when $n_0>0$, the [ordinary least squares](../../../../../ordinary-least-squares.md) estimates are

$$
\boxed{\begin{aligned}
\widehat\beta_0&=\frac{\sum_{i=1}^{4+n_0}Y_i}{4+n_0},\\
\widehat\beta_1&=\frac{Y_1+Y_2-Y_3-Y_4}{4},\\
\widehat\beta_2&=\frac{Y_1-Y_2-Y_3+Y_4}{4}.
\end{aligned}}
$$

Their variances are $\sigma^2/(4+n_0)$, $\sigma^2/4$, $\sigma^2/4$, with zero covariances.

The repeated center runs estimate [pure error](../../../../../pure-error.md) without requiring the fitted mean surface to be correct:

$$
s_{\rm PE}^2=\frac{\sum_{i=5}^{4+n_0}(Y_i-\bar Y_0)^2}{n_0-1}\quad(n_0\geq2).
$$

They also permit a [center-point curvature contrast](../../../../../center-point-curvature-contrast.md). Let $\bar Y_F=(Y_1+Y_2+Y_3+Y_4)/4$ and $\widehat\gamma=\bar Y_F-\bar Y_0$. Under the first-order model, $\mathbb E\widehat\gamma=0$ and $\operatorname{Var}(\widehat\gamma)=\sigma^2(1/4+1/n_0)$. Under a quadratic surface, its expectation is $\beta_{11}+\beta_{22}$, since the linear and $x_1x_2$ terms average to zero. Thus

$$
\frac{\widehat\gamma^2}{s_{\rm PE}^2(1/4+1/n_0)}\sim F_{1,n_0-1}
$$

under the first-order normal model. With only one center run there is no pure-error degree of freedom. A zero center contrast does not exclude all curvature, because the two quadratic coefficients can cancel. The corners also estimate an interaction contrast; the full [Lack-of-fit F-test](../../../../../lack-of-fit-f-test.md) compares the first-order fit with the five setting means, with two lack-of-fit and $n_0-1$ pure-error degrees of freedom.

If the first-order model is adequate and $\widehat b=(\widehat\beta_1,\widehat\beta_2)^T\ne0$, [steepest ascent in response surface methodology](../../../../../steepest-ascent-in-response-surface-methodology.md) uses the unit coded direction $d=\widehat b/\|\widehat b\|$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) proves that it maximizes the predicted directional derivative. Run sequential settings $x=hd$ for increasing feasible $h$, corresponding to physical increments $(5hd_1,2.5hd_2)$ from the center. Stop or reduce the steps when measured yield ceases to improve, and refit locally near promising settings. Respect the allowed rectangle; if a boundary is reached, investigate feasible boundary directions rather than extrapolating outside it. A near-zero gradient offers no first-order ascent direction and calls for further modeling.

If curvature is indicated, add the four axial settings $(1,0),(-1,0),(0,1),(0,-1)$, together with further center replication. This face-centered [central composite design](../../../../../central-composite-design.md) stays inside the allowed physical ranges and separates the two squared coordinates, which the corners alone cannot do. Fit the full [quadratic regression](../../../../../quadratic-regression.md) surface

$$
m(x)=\beta_0+\beta_1x_1+\beta_2x_2+\beta_{11}x_1^2+\beta_{12}x_1x_2+\beta_{22}x_2^2.
$$

Write its fitted quadratic part as $x^TBx$, where $B_{11}=\widehat\beta_{11}$, $B_{22}=\widehat\beta_{22}$ and $B_{12}=B_{21}=\widehat\beta_{12}/2$. Its gradient and Hessian are $\widehat b+2Bx$ and $2B$. If $B$ is nonsingular, the stationary setting is

$$
\boxed{x_*=-\tfrac12B^{-1}\widehat b.}
$$

If $B$ is [negative definite](../../../../../negative-definite-matrix.md) and $x_*$ is feasible, it is the fitted maximum. Otherwise compare feasible stationary settings, optima on each edge obtained from the restricted one-variable quadratic, and the corners. A singular or poorly determined $B$ calls for attention to ridge directions and more runs. Convert any chosen coded setting back using $\xi_1=95+5x_1$, $\xi_2=37.5+2.5x_2$, and confirm its yield experimentally. The fitted local surface guides the search; it does not establish an untested physical optimum.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
