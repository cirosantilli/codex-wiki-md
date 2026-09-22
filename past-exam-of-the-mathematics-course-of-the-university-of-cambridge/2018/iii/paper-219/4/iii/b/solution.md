<h1 id="4/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The terms involving $E_s$ give

$$
p(E_s\mid\text{rest})\propto\exp\left[-\frac{(E_s-(o_s-C_s))^2}{2r_s}-\frac{E_s}{\tau}\right]\mathbf1_{\{E_s\ge0\}}.
$$

Completing the square produces the [truncated normal distribution](../../../../../../../truncated-normal-distribution.md)

$$
\boxed{E_s\mid\text{rest}\sim\operatorname{TN}_{[0,\infty)}\left(o_s-C_s-\frac{r_s}{\tau},\ r_s\right)}.
$$

For $m=o_s-C_s-r_s/\tau$, its normalized density is $\phi((E_s-m)/\sqrt{r_s})/[\sqrt{r_s}\Phi(m/\sqrt{r_s})]$ on $E_s\ge0$. The exponential prior shifts the untruncated conditional mean downwards before truncation; changing the [variance](../../../../../../../variance-split.md) here to the intrinsic [variance](../../../../../../../variance-split.md) would be incorrect. These are the other $N$ latent-variable updates of the formal [Gibbs sampler](../../../../../../../gibbs-sampler.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
