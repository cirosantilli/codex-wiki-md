<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

Differentiate the normalization of the [exponential family](../../../../../exponential-family-split.md) density with respect to $\theta_i$, assuming the regularity that permits differentiation under its [integral](../../../../../integral.md). The density [derivative](../../../../../derivative.md) is $f(y_i\mid\theta_i,\phi)[y_i-b'(\theta_i)]/\phi$. Consequently

$$
0=\frac1\phi\bigl(EY_i-b'(\theta_i)\bigr),\qquad\boxed{\mu_i=b'(\theta_i).}
$$

Differentiating the expectation once more gives $d\mu_i/d\theta_i=\operatorname{Var}(Y_i)/\phi$, so

$$
\boxed{V_i=\operatorname{Var}(Y_i)=\phi b''(\theta_i).}
$$

The [log-likelihood](../../../../../log-likelihood.md) [derivative](../../../../../derivative.md) with respect to $\theta_i$ is $(y_i-\mu_i)/\phi$. For the [generalized linear model](../../../../../generalized-linear-model.md) with linear predictor $\eta_i=\beta^Tx_i=g(\mu_i)$, the [chain rule](../../../../../chain-rule.md) gives

$$
\frac{d\theta_i}{d\mu_i}=\frac1{b''(\theta_i)},\qquad\frac{\partial\mu_i}{\partial\beta}=\frac{x_i}{g'(\mu_i)}.
$$

Using independence to add the [log-likelihood](../../../../../log-likelihood.md) contributions proves the [score function](../../../../../informant-function.md)

$$
\boxed{\frac{\partial\ell}{\partial\beta}=\sum_{i=1}^n\frac{(y_i-\mu_i)x_i}{g'(\mu_i)V_i}.}
$$

Here $V_i$ includes the dispersion parameter $\phi$. Defining instead a unit-dispersion [variance function](../../../../../variance-function.md) $b''(\theta_i)$ would require retaining an explicit $\phi$ in the denominator.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
