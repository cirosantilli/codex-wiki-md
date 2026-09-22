<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Difference the [local-level state-space model](../../../../../../local-level-state-space-model.md) to eliminate its latent level:

$$
D_t=X_t-X_{t-1}=w_t+v_t-v_{t-1}.
$$

[Independence](../../../../../../independent-random-variables.md) and Gaussianity give a stationary Gaussian process with

$$
\gamma_D(0)=W+2V,
\qquad\gamma_D(1)=\gamma_D(-1)=-V,
\qquad\gamma_D(h)=0\quad(|h|>1).
$$

For $V,W>0$, let

$$
q=\frac{W+2V+\sqrt{W^2+4WV}}2,
\qquad\vartheta=-\frac Vq\in(-1,0).
$$

These satisfy $q(1+\vartheta^2)=W+2V$ and $q\vartheta=-V$. Therefore $D$ has the [covariance](../../../../../../covariance.md) of the [moving-average model](../../../../../../moving-average-model.md) $\varepsilon_t+\vartheta\varepsilon_{t-1}$, where $\varepsilon$ is Gaussian [white noise](../../../../../../white-noise.md) of [variance](../../../../../../variance-split.md) $q$. This is an actual representation, not just [covariance](../../../../../../covariance.md) matching: define $\varepsilon_t=\sum_{j\geq0}(-\vartheta)^jD_{t-j}$. The convergent inverse filter has constant [spectral density](../../../../../../spectral-density-of-a-stationary-process.md) $q/(2\pi)$, so its Gaussian coordinates are [independent](../../../../../../independent-random-variables.md), and multiplication by $1+\vartheta B$ recovers $D$.

Thus

$$
\boxed{(1-B)X_t=(1+\vartheta B)\varepsilon_t,
\qquad \operatorname{Var}(\varepsilon_t)=q.}
$$

This is the formal [ARMA](../../../../../../autoregressive-moving-average-model.md) equation with autoregressive coefficient one. Its unit root [means](../../../../../../expected-value.md) that the levels are generally not stationary: if the initial state has finite [variance](../../../../../../variance-split.md) and is [independent](../../../../../../independent-random-variables.md) of future noises, $\operatorname{Var}(S_t)=\operatorname{Var}(S_0)+tW$. In stationary-model terminology the correct classification is [ARIMA](../../../../../../autoregressive-integrated-moving-average.md)(0,1,1). The requested ARMA description must therefore allow a unit-root equation.

When $V=0$, the differences are just $w_t$; when $W=0$ and $V>0$, they are $v_t-v_{t-1}$, a noninvertible MA(1) with coefficient $-1$. If both [variances](../../../../../../variance-split.md) vanish, the model is deterministic apart from a possible initial random level. These limits explain the qualifications on the invertible representation above.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
