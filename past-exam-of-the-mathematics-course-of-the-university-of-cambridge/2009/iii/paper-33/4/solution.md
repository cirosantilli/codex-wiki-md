<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Nadaraya–Watson estimator](../../../../../nadaraya-watson-estimator.md) is

$$
\boxed{\widehat m_n(h,x)=\frac{\sum_{i=1}^nY_iK((x-X_i)/h)}{\sum_{i=1}^nK((x-X_i)/h)}.}
$$

For the [unit-width box kernel](../../../../../unit-width-box-kernel.md), it averages the responses with design points in $[x-h/2,x+h/2]$. Define it to be zero if that window contains no observations; the supplied small-denominator bound must refer to a defined estimator.

Write $g=f^X$, $D_n=(nh)^{-1}\sum_i\mathbf1_{\{|X_i-x|\le h/2\}}$ and $U_n=(nh)^{-1}\sum_iY_i\mathbf1_{\{|X_i-x|\le h/2\}}$. Set $G_n=U_n-m(x)D_n$. On $D_n>\delta$,

$$
|\widehat m_n-m(x)|=|G_n|/D_n\le|G_n|/\delta.
$$

This is the [absolute error bound for a ratio estimator with a controlled denominator](../../../../../absolute-error-bound-for-a-ratio-estimator-with-a-controlled-denominator.md); it does not require the numerator and denominator to be independent.

The [conditional expectation](../../../../../conditional-expectation.md) definition of the [regression function](../../../../../regression-function.md) gives

$$
\mathbb EG_n=\frac1h\int_{-h/2}^{h/2}(m(x+u)-m(x))g(x+u)\,du.
$$

At this interior point, the [Taylor theorem](../../../../../taylor-theorem.md) expansions are $m(x+u)-m(x)=m'(x)u+\tfrac12m''(x)u^2+o(u^2)$ and $g(x+u)=g(x)+g'(x)u+o(|u|)$. Multiplying and using the symmetric interval removes the odd linear term. More precisely,

$$
\mathbb EG_n=\frac{h^2}{12}\left(m'(x)g'(x)+\tfrac12m''(x)g(x)\right)+o(h^2)=O(h^2).
$$

This cancellation underlies the [interior absolute-error rate of the Nadaraya-Watson estimator](../../../../../interior-absolute-error-rate-of-the-nadaraya-watson-estimator.md).

For the variance, [independence](../../../../../independent-random-variables.md) between observations gives

$$
\operatorname{Var}(G_n)\le\frac1{nh^2}\mathbb E[(Y-m(x))^2\mathbf1_{\{|X-x|\le h/2\}}].
$$

Conditional on $X=t$, the second moment is $V(t)+(m(t)-m(x))^2$. The bounded [conditional variance](../../../../../conditional-variance.md), local boundedness of $m$, and boundedness of $g$ consequently make the expectation at most $Ch$. Thus $\operatorname{Var}(G_n)=O((nh)^{-1})$. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md),

$$
\mathbb E[|\widehat m_n-m(x)|\mathbf1_{\{D_n>\delta\}}]
\le\delta^{-1}\left(|\mathbb EG_n|+\sqrt{\operatorname{Var}(G_n)}\right)
=O(h^2+(nh)^{-1/2}).
$$

The auxiliary result supplied in the question makes the expected error on $D_n\le\delta$ equal to $o(n^{-2/5})$. Combining both events, with $h_n\asymp n^{-1/5}$, proves

$$
\boxed{\mathbb E|\widehat m_n(h_n,x)-m(x)|=O(n^{-2/5}).}
$$

Both the squared-bandwidth bias and the inverse-square-root window-count error have this order. The supplied separate consistency result for the design-density estimator is not needed once the stronger small-denominator expectation bound is used.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
