<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $\sigma_1,\sigma_2>0$ and $|\rho|<1$, as required for the displayed nonsingular [probability density function](../../../../../../probability-density-function.md). Put $z_j=(x_j-\mu_j)/\sigma_j$. Its quadratic exponent is

$$
Q(x)=\frac{z_1^2-2\rho z_1z_2+z_2^2}{1-\rho^2}
=\frac{(z_1-\rho z_2)^2}{1-\rho^2}+z_2^2.
$$

Holding $x_2$ fixed and normalizing the term depending on $x_1$ gives

$$
\boxed{X_1\mid X_2=x_2\sim
N\!\left(\mu_1+\rho\frac{\sigma_1}{\sigma_2}(x_2-\mu_2),
\sigma_1^2(1-\rho^2)\right).}
$$

The analogous completion of the square gives

$$
\boxed{X_2\mid X_1=x_1\sim
N\!\left(\mu_2+\rho\frac{\sigma_2}{\sigma_1}(x_1-\mu_1),
\sigma_2^2(1-\rho^2)\right).}
$$

Using [independent](../../../../../../independent-random-variables.md) draws $\eta_{1,r},\eta_{2,r}$ from the [standard normal distribution](../../../../../../standard-normal-distribution.md), a sweep is

$$
X_1^{(r)}=\mu_1+\rho\frac{\sigma_1}{\sigma_2}(X_2^{(r-1)}-\mu_2)
+\sigma_1\sqrt{1-\rho^2}\,\eta_{1,r},
$$



$$
X_2^{(r)}=\mu_2+\rho\frac{\sigma_2}{\sigma_1}(X_1^{(r)}-\mu_1)
+\sigma_2\sqrt{1-\rho^2}\,\eta_{2,r}.
$$

Use the newly drawn first coordinate in the second update. Recording the pairs after each sweep gives the dependent sample.

The [Gaussian Gibbs sweep autocorrelation](../../../../../../gaussian-gibbs-sweep-autocorrelation.md) makes the dependence explicit. In standardized coordinates, substitution yields

$$
Z_{2,r}=\rho^2Z_{2,r-1}
+\sqrt{1-\rho^2}(\rho\eta_{1,r}+\eta_{2,r}).
$$

The new noise has [variance](../../../../../../variance-split.md) $1-\rho^4$, so the stationary [variance](../../../../../../variance-split.md) is one and the lag-$h$ sweep [autocorrelation](../../../../../../autocorrelation.md) is $\rho^{2h}$. Thus the sampler converges geometrically for $|\rho|<1$, but becomes slow near perfect [correlation](../../../../../../pearson-correlation-coefficient.md). When $\rho=0$, complete sweeps yield [independent](../../../../../../independent-random-variables.md) pairs. The singular cases $|\rho|=1$ do not have the stipulated two-dimensional [probability density function](../../../../../../probability-density-function.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
