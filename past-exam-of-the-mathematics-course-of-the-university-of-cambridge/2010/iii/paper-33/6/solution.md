<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the [expectation-maximization algorithm](../../../../../expectation-maximization-algorithm.md), let $L(\vartheta)=\int f(x,z;\vartheta)\,dz$. At iteration $t$, the E-step forms the [conditional distribution](../../../../../conditional-distribution.md) of the missing data at the current parameter and the function

$$
Q(\vartheta\mid\vartheta^{(t)})=
\mathbb E_{\vartheta^{(t)}}[\log f(x,Z;\vartheta)\mid x].
$$

The M-step is

$$
\boxed{\vartheta^{(t+1)}\in\operatorname*{arg\,max}_{\vartheta}
Q(\vartheta\mid\vartheta^{(t)}).}
$$

In this maximization the [conditional distribution](../../../../../conditional-distribution.md) defining the expectation is held at the old parameter; it is not recomputed as $\vartheta$ varies. The [Jensen inequality](../../../../../jensen-s-inequality.md) gives

$$
\log L(\vartheta)-\log L(\vartheta^{(t)})
\ge Q(\vartheta\mid\vartheta^{(t)})-Q(\vartheta^{(t)}\mid\vartheta^{(t)}),
$$

by writing the [likelihood function](../../../../../likelihood-function.md) ratio as a [conditional expectation](../../../../../conditional-expectation.md) of $f(x,Z;\vartheta)/f(x,Z;\vartheta^{(t)})$. Hence an exact M-step does not decrease the observed-data [likelihood function](../../../../../likelihood-function.md). The algorithm does not in general guarantee convergence to its global maximum; initialization and the [likelihood function](../../../../../likelihood-function.md)'s geometry matter.

For the specified diagonal [bivariate normal distribution](../../../../../bivariate-normal-distribution.md), use $v_j=\sigma_j^2>0$. The two coordinates are independent, as are the four observations. Therefore the known second coordinate of the fourth observation gives no information about its first coordinate conditional on the parameters. The E-step is

$$
Z\mid x_{\mathrm{obs}},\vartheta^{(t)}\sim N(\mu_1^{(t)},v_1^{(t)}),
$$



$$
a_t:=\mathbb E_tZ=\mu_1^{(t)},\qquad
b_t:=\mathbb E_tZ^2=(\mu_1^{(t)})^2+v_1^{(t)}.
$$

These two moments suffice for the complete [Gaussian](../../../../../normal-distribution.md) log-likelihood. Discarding terms independent of the proposed parameters, its [conditional expectation](../../../../../conditional-expectation.md) is

$$
\begin{aligned}
Q(\mu_1,\mu_2,v_1,v_2\mid\vartheta^{(t)})
={}&-2\log v_1-\frac1{2v_1}
\left[\sum_{i=1}^3(x_{i1}-\mu_1)^2+b_t-2\mu_1a_t+\mu_1^2\right]\\
&-2\log v_2-\frac1{2v_2}\sum_{i=1}^4(x_{i2}-\mu_2)^2.
\end{aligned}
$$

Differentiating with respect to each mean gives four times that mean minus the corresponding expected sum of observations. Thus the updates in [EM for an independent missing normal coordinate](../../../../../em-for-an-independent-missing-normal-coordinate.md) are

$$
\boxed{\mu_1^{(t+1)}=\frac{x_{11}+x_{21}+x_{31}+\mu_1^{(t)}}4,\qquad
\mu_2^{(t+1)}=\frac{x_{12}+x_{22}+x_{32}+x_{42}}4.}
$$

For either [variance](../../../../../variance-split.md) the remaining criterion is $-2\log v-S/(2v)$; its derivative vanishes at $v=S/4$, which is its maximum when $S>0$. Evaluate the expected residual sum at the new means to obtain

$$
\boxed{v_1^{(t+1)}=\frac14\left[
\sum_{i=1}^3(x_{i1}-\mu_1^{(t+1)})^2
+v_1^{(t)}+(\mu_1^{(t)}-\mu_1^{(t+1)})^2\right],}
$$



$$
\boxed{v_2^{(t+1)}=\frac14\sum_{i=1}^4(x_{i2}-\mu_2^{(t+1)})^2.}
$$

The missing contribution is

$$
\mathbb E_t[(Z-\mu_1^{(t+1)})^2]
=v_1^{(t)}+(\mu_1^{(t)}-\mu_1^{(t+1)})^2.
$$

Its first term is essential. Substituting only the imputed mean for $Z$ would omit its uncertainty and would not maximize the required expected complete log-likelihood.

As a check, the observed-data [likelihood function](../../../../../likelihood-function.md) integrates out the missing first coordinate, leaving three first-coordinate and four second-coordinate normal densities. Put $\overline x_1=\sum_{i=1}^3x_{i1}/3$ and $s_1^2=\sum_{i=1}^3(x_{i1}-\overline x_1)^2/3$. The first-coordinate recurrence implies

$$
\mu_1^{(t+1)}-\overline x_1=\frac14(\mu_1^{(t)}-\overline x_1),
$$



$$
v_1^{(t+1)}=\frac34s_1^2+\frac14v_1^{(t)}
+\frac3{16}(\mu_1^{(t)}-\overline x_1)^2.
$$

Thus the iterates converge to the three-observation mean and maximum-likelihood [variance](../../../../../variance-split.md), while the second-coordinate estimates are reached after one update. If the observed values in a coordinate are all equal, its [likelihood function](../../../../../likelihood-function.md) instead has a zero-variance boundary degeneracy, and there is no positive-variance maximizer; the [variance](../../../../../variance-split.md) formulas then describe that boundary limit. For nonzero empirical spreads the displayed updates give the ordinary nonsingular EM iteration.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
