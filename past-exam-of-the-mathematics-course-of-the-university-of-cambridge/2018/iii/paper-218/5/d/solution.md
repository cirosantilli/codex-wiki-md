<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply [EM for a missing observation in a Gaussian AR1 process](../../../../../../em-for-a-missing-observation-in-a-gaussian-ar1-process.md), starting from $\theta^{old}=(\mu^{old},\phi^{old},(\sigma^2)^{old})$ in the stationary parameter space. The [Gaussian AR1 bridge](../../../../../../gaussian-ar1-bridge.md) gives the E-step quantities

$$
m=\mu^{old}+\frac{\phi^{old}(x_1+x_3-2\mu^{old})}{1+(\phi^{old})^2},\qquad v=\frac{(\sigma^2)^{old}}{1+(\phi^{old})^2}.
$$

Thus $\mathbb E[X_2\mid x_{obs}]=m$, $\mathbb E[X_2^2\mid x_{obs}]=m^2+v$, and $\mathbb E[X_1X_2\mid x_{obs}]=x_1m$, $\mathbb E[X_2X_3\mid x_{obs}]=mx_3$.

Let $x_2^*=m$ and $x_t^*=x_t$ otherwise. Keeping $m,v$ fixed throughout the M-step, define

$$
R(\mu,\phi)=(1-\phi^2)(x_1-\mu)^2+\sum_{t=2}^{31}\{(x_t^*-\mu)-\phi(x_{t-1}^*-\mu)\}^2+(1+\phi^2)v.
$$

The last term comes from the missing observation's conditional variance in the two adjacent innovation squares. The expected complete-data [log-likelihood](../../../../../../log-likelihood.md) is

$$
Q(\mu,\phi,\sigma^2\mid\theta^{old})=C-\frac{31}{2}\log\sigma^2+\frac12\log(1-\phi^2)-\frac{R(\mu,\phi)}{2\sigma^2}.
$$

For fixed $\phi$, differentiating the quadratic in $\mu$ gives

$$
\mu_*(\phi)=\frac{(1-\phi^2)x_1+(1-\phi)\sum_{t=2}^{31}(x_t^*-\phi x_{t-1}^*)}{(1-\phi^2)+30(1-\phi)^2}.
$$

Also the maximizing variance is $\sigma^2=R(\mu,\phi)/31$. The M-step is therefore a one-dimensional [profile likelihood](../../../../../../profile-likelihood.md) maximization:

$$
\boxed{\phi^{new}\in\arg\max_{|\phi|<1}\left\{\frac12\log(1-\phi^2)-\frac{31}{2}\log R(\mu_*(\phi),\phi)\right\},\quad\mu^{new}=\mu_*(\phi^{new}),\quad(\sigma^2)^{new}=\frac{R(\mu^{new},\phi^{new})}{31}.}
$$

Repeat the E- and M-steps until the observed-data likelihood and parameters stabilize. Exact M-steps make that likelihood nondecreasing; different initializations help detect different local optima, and convergence alone is not a guarantee of a global maximum. At an interior local maximum, impute the missing temperature by its conditional mean $m$ evaluated at the fitted parameters, retaining $v$ as its conditional uncertainty. Replacing $X_2$ by $m$ and discarding $v$ would not implement the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
