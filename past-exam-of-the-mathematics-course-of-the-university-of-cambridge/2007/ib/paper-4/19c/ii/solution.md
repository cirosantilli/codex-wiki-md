<h1 id="19c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\operatorname{RSS}=\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)^2$. Differentiating the [log-likelihood](../../../../../../log-likelihood.md) in $v=\sigma^2$ gives

$$
\frac{\partial\ell}{\partial v}=-\frac n{2v}+\frac{\operatorname{RSS}}{2v^2}.
$$

For $\operatorname{RSS}>0$ this changes from positive to negative at $v=\operatorname{RSS}/n$, so

$$
\boxed{\widehat\sigma^2=\frac{\operatorname{RSS}}n.}
$$

To find its bias, substitute the model and use the orthogonal fit directions $\mathbf1$ and $\mathbf x$, obtaining

$$
\operatorname{RSS}=\sum_i\varepsilon_i^2-n\bar\varepsilon^2-\frac{(\sum_i x_i\varepsilon_i)^2}{S_{xx}}.
$$

The three expectations are $n\sigma^2$, $\sigma^2$, and $\sigma^2$, respectively: $\operatorname{Var}(\bar\varepsilon)=\sigma^2/n$ and $\operatorname{Var}(\sum_i x_i\varepsilon_i)=\sigma^2S_{xx}$. Hence $\mathbb E\operatorname{RSS}=(n-2)\sigma^2$, giving the [unbiased estimator](../../../../../../unbiased-estimator.md)

$$
\boxed{s^2=\frac{\operatorname{RSS}}{n-2}=\frac n{n-2}\widehat\sigma^2.}
$$

With $n>2$, a zero [residual sum of squares](../../../../../../residual-sum-of-squares.md) is a probability-zero event in the model. For that exceptional dataset the likelihood is unbounded as $\sigma^2\downarrow0$, rather than having a maximum at a positive [variance](../../../../../../variance-split.md). In the intercept-only case $S_{xx}=0$, the corresponding unbiased multiplier is $n/(n-1)$ for $n>1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [19C](../../19c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
