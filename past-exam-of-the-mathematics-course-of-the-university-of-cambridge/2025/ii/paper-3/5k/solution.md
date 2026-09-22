<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

Let $Y_1,\ldots,Y_n$ be independent. In the general exponential-dispersion formulation, with known weights $w_i>0$ and common dispersion $\phi>0$, their densities have the form

$$
f_i(y_i;\theta_i,\phi)
=\exp\left\{\frac{w_i}{\phi}
[y_i\theta_i-b(\theta_i)]
+c\left(y_i,\frac{\phi}{w_i}\right)\right\}.
$$

Thus

$$
\mu_i=\mathbb E Y_i=b'(\theta_i),
\qquad
\operatorname{Var}(Y_i)=\frac{\phi}{w_i}b''(\theta_i)
=\frac{\phi}{w_i}V(\mu_i).
$$

The systematic component is $\eta_i=x_i^T\beta$, and a specified one-to-one differentiable link relates it to the mean by

$$
g(\mu_i)=\eta_i.
$$

The unknown model parameters are the regression coefficient $\beta$ and, when it is not fixed by the family, the dispersion $\phi$.

The log-likelihood is

$$
\ell(\beta,\phi)
=\sum_{i=1}^n\left\{
\frac{w_i}{\phi}[y_i\theta_i-b(\theta_i)]
+c\left(y_i,\frac{\phi}{w_i}\right)
\right\},
$$

up to terms independent of the parameters, where $\theta_i$ is determined from $g^{-1}(x_i^T\beta)=b'(\theta_i)$.

For a Poisson response,

$$
f(y;\mu)=\exp\{y\log\mu-\mu-\log(y!)\},
$$

so the natural parameter is $\theta=\log\mu$ and $b(\theta)=e^\theta$. The canonical link sets the linear predictor equal to the natural parameter and is therefore

$$
\boxed{g(\mu)=\log\mu}.
$$

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
