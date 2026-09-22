<h1 id="19d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $x$ and $\epsilon$ denote the design and error vectors, and put $P=xx^T/S_{xx}$. The residual vector is $r=(I-P)\epsilon$, while $\widehat\beta-\beta=x^T\epsilon/S_{xx}$. Since $(I-P)x=0$,

$$
\operatorname{Cov}(r,\widehat\beta)=\frac{\sigma^2}{S_{xx}}(I-P)x=0.
$$

These are jointly Gaussian linear functions of $\epsilon$, so the entire residual vector is independent of $\widehat\beta$, not merely uncorrelated with it. Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) whose first vector is $x/\sqrt{S_{xx}}$. In that basis $\epsilon/\sigma$ has independent standard normal coordinates, and the residual keeps exactly the remaining $n-1$ coordinates. Therefore

$$
\boxed{\widehat\beta\ \perp\!\!\!\perp\ \widehat\sigma^2,\qquad
\frac{n\widehat\sigma^2}{\sigma^2}=\frac{\mathrm{RSS}}{\sigma^2}\sim\chi^2_{n-1}.}
$$

Together with part (ii), this specifies the joint distribution as the product of the slope's normal law and the scaled [chi-squared distribution](../../../../../../chi-squared-distribution.md). In particular $E\widehat\sigma^2=(n-1)\sigma^2/n$: the variance maximum-likelihood estimator is biased downward.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [19D](../../19d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
