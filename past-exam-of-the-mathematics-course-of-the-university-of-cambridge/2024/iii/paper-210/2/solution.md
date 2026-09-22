<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is an integrable function $K$ with $\int K=1$. With $K_h(u)=h^{-1}K(u/h)$, the [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\widehat f_{n,h,K}(x)=\frac1n\sum_{i=1}^nK_h(x-X_i).
$$

A [kernel of order ell](../../../../../kernel-of-order-ell.md) satisfies

$$
\int u^jK(u)\,du=0\quad(1\leq j<\ell),
\qquad
\int|u|^\ell|K(u)|\,du<\infty.
$$

Split the integrated $L^p$ risk into stochastic and bias terms:

$$
\mathbb E\lVert\widehat f-f\rVert_p^p
\leq2^{p-1}\mathbb E\lVert\widehat f-\mathbb E\widehat f\rVert_p^p
+2^{p-1}\lVert K_h*f-f\rVert_p^p.
$$

For fixed $x$, put $A_i(x)=K_h(x-X_i)$ and $W_i(x)=A_i(x)-\mathbb EA_i(x)$. The supplied [Rosenthal inequality](../../../../../rosenthal-inequality.md) gives

$$
\mathbb E\left|\frac1n\sum_iW_i(x)\right|^p
\leq C_p\left\{
\frac{\mathbb E|W_1(x)|^p}{n^{p-1}}
+\frac{(\mathbb EW_1(x)^2)^{p/2}}{n^{p/2}}
\right\}.
$$

Now

$$
\int\mathbb E|W_1(x)|^pdx
\leq2^p\int\mathbb E|A_1(x)|^pdx
=2^ph^{1-p}R_p(K).
$$

Also $\mathbb EW_1(x)^2\leq(K_h^2*f)(x)$. The [Young convolution inequality](../../../../../young-s-convolution-inequality.md) with exponent $p/2$ gives

$$
\int(K_h^2*f)(x)^{p/2}dx
\leq\left(\frac{R(K)}h\right)^{p/2}
\lVert f\rVert_{p/2}^{p/2}.
$$

After integration and multiplication by the outer factor $2^{p-1}$, the stochastic contribution is at most

$$
\frac{2^{2p-1}C_pR_p(K)}{(nh)^{p-1}}
+\frac{2^{p-1}C_pR(K)^{p/2}\lVert f\rVert_{p/2}^{p/2}}
{(nh)^{p/2}}.
$$

It remains to control the bias. Here $\ell=\lceil\beta\rceil=m+1$. The [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md), the vanishing kernel moments, and [Minkowski integral inequality](../../../../../minkowski-integral-inequality.md) give

$$
\lVert K_h*f-f\rVert_p
\leq\frac1{m!}\int|K(u)|
\lVert f^{(m)}(\,\cdot-hu)-f^{(m)}\rVert_p
|hu|^mdu.
$$

The defining Nikol'skii smoothness bound is $L|hu|^{\beta-m}$, so

$$
\lVert K_h*f-f\rVert_p
\leq\frac{L}{m!}h^\beta\mu_\beta(K).
$$

Raising to the $p$th power and applying the outer factor $2^{p-1}$ proves

$$
\boxed{\mathbb EL(\widehat f_{n,h,K},f)
\leq
\frac{2^{2p-1}C_pR_p(K)}{(nh)^{p-1}}
+\frac{2^{p-1}C_pR(K)^{p/2}\lVert f\rVert_{p/2}^{p/2}}{(nh)^{p/2}}
+\frac{2^{p-1}L^p}{(m!)^p}\mu_\beta(K)^ph^{p\beta}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
