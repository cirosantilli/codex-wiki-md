<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under the unrestricted model, insert the [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) $(\bar x,S)$. Under the diagonal-covariance restriction, the [quadratic form](../../../../../../quadratic-form.md) is minimized over the [mean](../../../../../../expected-value.md) at $\bar x$, and the remaining objective separates over the diagonal entries:

$$
-2\ell(\bar x,\operatorname{diag}(v_1,\ldots,v_p))
=\text{constant}+n\sum_{j=1}^p\left(\log v_j+\frac{S_{jj}}{v_j}\right).
$$

Differentiating in $v_j>0$ gives $\widehat v_j=S_{jj}$; the derivative changes from negative to positive there. Put $D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. The fitted [trace](../../../../../../matrix-trace.md) term is $p$ under either model, since $\operatorname{tr}(D^{-1}S)=p=\operatorname{tr}(S^{-1}S)$. Consequently the [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md) is determined by

$$
\Lambda=\frac{\sup_{H_0}L}{\sup L}
=\left(\frac{|S|}{\prod_jS_{jj}}\right)^{n/2}
=|R|^{n/2},\qquad R=D^{-1/2}SD^{-1/2}.
$$

This is the [Gaussian diagonal-covariance likelihood-ratio test](../../../../../../gaussian-diagonal-covariance-likelihood-ratio-test.md). **Reject for sufficiently small $\log|R|$**, equivalently for large $-n\log|R|$. Under the regular large-sample calibration, [Wilks theorem](../../../../../../wilks-theorem.md) gives $-n\log|R|\Rightarrow\chi^2_{p(p-1)/2}$, since diagonality removes that many free covariance parameters. The exact critical constant can instead be obtained from the null distribution at the actual sample size.

For $p=2$, write the [sample correlation coefficient](../../../../../../sample-correlation-coefficient.md) as $r$. Then $|R|=1-r^2$, so the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) rejects for **large $|r|$**, not merely for large positive $r$. Under the null, the two variables have a [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) and are [independent](../../../../../../independent-random-variables.md), and the exact test is

$$
\boxed{\left|r\sqrt{\frac{n-2}{1-r^2}}\right|>
 t_{n-2,\,1-\alpha/2}.}
$$

Indeed, condition on the centered first-variable observation vector. Decompose the second centered [Gaussian vector](../../../../../../gaussian-random-vector.md) into its component along that direction and the $n-2$-dimensional [orthogonal complement](../../../../../../orthogonal-complement.md). Their squared lengths give independent $\chi^2_1$ and $\chi^2_{n-2}$ variables. Their ratio shows that $r\sqrt{(n-2)/(1-r^2)}$ has [Student's t-distribution](../../../../../../student-s-t-distribution.md) with $n-2$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
