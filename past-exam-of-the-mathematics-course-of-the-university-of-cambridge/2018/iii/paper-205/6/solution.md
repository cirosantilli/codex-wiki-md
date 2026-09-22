<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the unscaled penalty convention consistent with the displayed bound:

$$
\boxed{\widehat f_\lambda=\arg\min_{f\in\mathcal H}\left\{\sum_{i=1}^n(Y_i-f(x_i))^2+\lambda\|f\|_{\mathcal H}^2\right\}.}
$$

For an objective with averaged squared loss, the corresponding penalty parameter would be $\lambda/n$. We retain the unscaled $\lambda$ throughout.

By the [representer theorem](../../../../../representer-theorem.md), the [kernel ridge regression](../../../../../kernel-ridge-regression.md) minimizer lies in the span of $k(x_i,\cdot)$. A valid coefficient vector is $\widehat a=(K+\lambda I_n)^{-1}Y$, giving

$$
\widehat f_\lambda(\cdot)=\sum_i\widehat a_i k(x_i,\cdot),\qquad\widehat m=HY,\qquad H=K(K+\lambda I_n)^{-1}.
$$

The [kernel matrix](../../../../../kernel-matrix.md) is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md), so the inverse exists even if $K$ is singular. In the coefficient objective $\|Y-Ka\|_2^2+\lambda a^TKa$, this choice satisfies $K\{(K+\lambda I_n)a-Y\}=0$; there is no need to cancel $K$. The function itself is unique because of the strictly convex squared Hilbert norm. The matrix $H$ is the [kernel-ridge hat matrix](../../../../../kernel-ridge-hat-matrix.md) in the present normalization.

Let $m^0=(f^0(x_i))_{i=1}^n$. Since $Y=m^0+\varepsilon$, the zero mean and covariance assumption give the exact [bias-variance decomposition for linear prediction](../../../../../bias-variance-decomposition-for-linear-prediction.md)

$$
\frac1n\mathbb E\|\widehat m-m^0\|_2^2=\frac1n\|(I_n-H)m^0\|_2^2+\frac{\sigma^2}{n}\operatorname{tr}(H^2).
$$

No normality of the noise is required for this identity.

Choose an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) $v_i$ of $K$, with eigenvalues $d_i\geq0$. Its shrinkage factors are $d_i/(d_i+\lambda)$, so

$$
\operatorname{tr}(H^2)=\sum_i\frac{d_i^2}{(d_i+\lambda)^2}\leq\sum_i\min\left\{\frac{d_i}{4\lambda},1\right\}=\frac1\lambda\sum_i\min(d_i/4,\lambda).
$$

The first bound follows from $(d_i+\lambda)^2\geq4d_i\lambda$ and from each shrinkage factor being at most one.

To control the bias by the [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md) norm, for $d_i>0$ define

$$
g_i=\frac1{\sqrt{d_i}}\sum_j(v_i)_j k(x_j,\cdot)\in\mathcal H.
$$

The [reproducing property](../../../../../reproducing-property.md) gives $\langle g_i,g_\ell\rangle_{\mathcal H}=\delta_{i\ell}$ and

$$
v_i^Tm^0=\sqrt{d_i}\langle g_i,f^0\rangle_{\mathcal H}.
$$

If $d_i=0$, the corresponding unscaled kernel combination has Hilbert norm squared $v_i^TKv_i=0$, so $v_i^Tm^0=0$. There is therefore no bias component in a zero-eigenvalue direction. For the remaining directions,

$$
\begin{aligned}
\|(I_n-H)m^0\|_2^2
&=\sum_{d_i>0}\frac{\lambda^2d_i}{(d_i+\lambda)^2}|\langle g_i,f^0\rangle_{\mathcal H}|^2\\
&\leq\frac\lambda4\sum_{d_i>0}|\langle g_i,f^0\rangle_{\mathcal H}|^2\\
&\leq\frac\lambda4\|f^0\|_{\mathcal H}^2.
\end{aligned}
$$

The scalar bound is again $(d_i+\lambda)^2\geq4d_i\lambda$, and the final step is [Bessel inequality](../../../../../bessel-s-inequality.md). Combining the variance and bias bounds proves the [prediction-risk bound for kernel ridge regression](../../../../../prediction-risk-bound-for-kernel-ridge-regression.md):

$$
\boxed{\frac1n\mathbb E\sum_i\{f^0(x_i)-\widehat f_\lambda(x_i)\}^2\leq\frac{\sigma^2}{n\lambda}\sum_i\min(d_i/4,\lambda)+\frac\lambda{4n}\|f^0\|_{\mathcal H}^2.}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
