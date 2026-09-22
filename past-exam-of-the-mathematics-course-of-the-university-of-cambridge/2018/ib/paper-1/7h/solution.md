<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

The distribution function is $F(x)=x^2/\theta^2$ on $[0,\theta]$, so its median is $\theta/\sqrt2$. The [likelihood function](../../../../../likelihood-function.md) is

$$
L(\theta)=2^n\left(\prod_iX_i\right)\theta^{-2n}\mathbf1_{\{\theta\geq X_{(n)}\}},
$$

which decreases over its admissible range. Hence $\widehat\theta=X_{(n)}=\max_iX_i$. By the [invariance property of maximum likelihood estimation](../../../../../invariance-property-of-maximum-likelihood-estimation.md),

$$
\boxed{\widehat m=\frac{X_{(n)}}{\sqrt2}.}
$$

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
