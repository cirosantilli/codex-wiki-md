<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With the normalization used in the question, [kernel ridge regression](../../../../../kernel-ridge-regression.md) minimizes

$$
\frac1n\left\{
\sum_{i=1}^n(Y_i-f(x_i))^2+\lambda\|f\|_{\mathcal H}^2
\right\}.
$$

The [representer theorem](../../../../../representer-theorem.md) and the normal equations give the fitted-value vector

$$
\widehat f_\lambda(X)
=K(K+\lambda I_n)^{-1}Y.
$$

Let $\mathcal H_X=\operatorname{span}\{k(x_i,\cdot):1\leq i\leq n\}$ and let $\bar f$ be the orthogonal projection of $f^0$ onto this space. The reproducing property makes $f^0(x_i)=\bar f(x_i)$ for every $i$. Writing $\bar f=\sum_j\alpha_jk(x_j,\cdot)$ gives

$$
f^0(X)=K\alpha,
\qquad
\|\bar f\|_{\mathcal H}^2=\alpha^TK\alpha
\leq\|f^0\|_{\mathcal H}^2.
$$

Conditionally on $X$, the covariance matrix of the fitted vector is

$$
\sigma^2K^2(K+\lambda I)^{-2}.
$$

Since the eigenvalues of $K$ are $n\widehat\mu_i$, the average conditional variance is

$$
\frac{\sigma^2}{n}\sum_{i=1}^n
\left(\frac{n\widehat\mu_i}{n\widehat\mu_i+\lambda}\right)^2.
$$

For $t\geq0$,

$$
\frac{t^2}{(1+t)^2}\leq\min(1,t/4).
$$

Taking $t=n\widehat\mu_i/\lambda$ and adding the supplied squared-bias bound gives

$$
\frac1n\sum_i
\mathbb E\!\left[
\{f^0(x_i)-\widehat f_\lambda(x_i)\}^2\mid X\right]
\leq
\frac{\sigma^2}{\lambda}
\sum_i\min\left(\frac{\widehat\mu_i}{4},\frac{\lambda}{n}\right)
+\frac{\lambda}{4n}.
$$

Because $\widehat\lambda$ minimizes this conditional upper bound, its expected value is at most the expected bound at any deterministic $\lambda=n\gamma$. Using the assumed eigenvalue comparison,

$$
\begin{aligned}
\frac1n\sum_i\mathbb E
\{f^0(x_i)-\widehat f_{\widehat\lambda}(x_i)\}^2
&\leq
\inf_{\gamma>0}\left\{
\frac{\sigma^2}{n\gamma}
\mathbb E\sum_i\min(\widehat\mu_i/4,\gamma)
+\frac\gamma4\right\}\\
&\leq
\inf_{\gamma>0}\left\{
\frac{\sigma^2}{n\gamma}
\sum_{j=1}^\infty\min(\mu_j/4,\gamma)
+\frac\gamma4\right\}.
\end{aligned}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
