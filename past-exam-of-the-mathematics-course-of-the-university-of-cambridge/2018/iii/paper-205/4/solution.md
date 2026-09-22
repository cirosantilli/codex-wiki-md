<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [convex function](../../../../../convex-function.md) $f$, its [subdifferential](../../../../../subdifferential.md) at $x$ is the set of supporting slopes

$$
\partial f(x)=\{g:f(y)\geq f(x)+g^T(y-x)\text{ for every }y\text{ in its domain}\}.
$$

The [subgradient optimality condition](../../../../../subgradient-optimality-condition.md) is

$$
\boxed{x\in\arg\min f\quad\Longleftrightarrow\quad0\in\partial f(x).}
$$

Indeed, the defining inequality with $g=0$ is exactly the global minimum inequality. For the [subdifferential of the L1 norm](../../../../../subdifferential-of-the-l1-norm.md), the coordinates vary independently:

$$
\boxed{\partial\|b\|_1=\{z:z_j=\operatorname{sgn}(b_j)\ (b_j\ne0),\quad z_j\in[-1,1]\ (b_j=0)\}.}
$$

Let $r=Y-X\widehat\beta_\lambda$. The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) for [Lasso](../../../../../lasso.md) give a vector $z\in\partial\|\widehat\beta_\lambda\|_1$ such that $X^Tr/n=\lambda z$. If $\widehat\sigma_\lambda=\|r\|_2/\sqrt n>0$, the unsquared residual norm is differentiable at this fit, with gradient

$$
-\frac{X^Tr}{\sqrt n\|r\|_2}=-\frac{X^Tr}{n\widehat\sigma_\lambda}.
$$

Using the [subdifferential sum rule](../../../../../subdifferential-sum-rule.md), choose $\gamma(\lambda)=\lambda/\widehat\sigma_\lambda$ to obtain

$$
-\frac{X^Tr}{n\widehat\sigma_\lambda}+\gamma(\lambda)z=0.
$$

Convexity now proves the [tuning relation between Lasso and square-root Lasso](../../../../../tuning-relation-between-lasso-and-square-root-lasso.md):

$$
\boxed{\widehat\beta_\lambda\in\arg\min_b Q_{\lambda/\widehat\sigma_\lambda}(b;Y).}
$$

The positive residual assumption is needed both for this gradient and for the quotient defining the tuning parameter.

For the final score calculation, use the usual fixed-design interpretation of the [normal linear model](../../../../../normal-linear-model.md): regard $X,Z$ and the tuning parameter $\gamma$ in the regression of $Z$ as fixed, and choose that regression's minimizer using only those inputs. Its nonzero residual $R=R_\gamma$ then has the [Square-root Lasso](../../../../../square-root-lasso.md) optimality condition

$$
\frac{X^TR}{\sqrt n\|R\|_2}=\gamma\widetilde z,
\qquad\widetilde z\in\partial\|\widetilde\beta_\gamma\|_1,
\qquad\|X^TR\|_\infty\leq\sqrt n\,\gamma\|R\|_2.
$$

Expanding the response residual gives

$$
T=\frac{R^T\varepsilon}{\|R\|_2}+\frac{R^TX(\beta^0-\widehat\beta_\lambda)}{\|R\|_2}=W+\Delta.
$$

Since $R/\|R\|_2$ is a fixed unit vector and $\varepsilon\sim N_n(0,\sigma^2I_n)$, a [linear image of a multivariate normal vector](../../../../../linear-image-of-a-multivariate-normal-vector.md) gives $W\sim N(0,\sigma^2)$. Finally, [Holder inequality](../../../../../holder-inequality.md) and the residual score bound yield

$$
\boxed{|\Delta|\leq\frac{\|X^TR\|_\infty}{\|R\|_2}\|\beta^0-\widehat\beta_\lambda\|_1\leq\sqrt n\,\gamma\|\beta^0-\widehat\beta_\lambda\|_1.}
$$

This is the [residual-score decomposition from square-root Lasso](../../../../../residual-score-decomposition-from-square-root-lasso.md). The normality statement also holds conditionally on a design independent of the noise. If $\gamma$ were chosen from the response noise, for example through the preceding $\gamma(\lambda)$ formula, the direction $R$ would require a separate independence argument; the final calculation treats $\gamma$ as fixed.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
