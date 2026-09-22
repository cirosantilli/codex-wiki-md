<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For any prior density $\pi(p)$, the Bayes estimate under [squared-error loss](../../../../../../squared-error-loss.md) is the [posterior mean](../../../../../../posterior-mean.md):

$$
\widehat p_{\mathrm B}
=\frac{\int_0^1 p\,p^9(1-p)^{81}\pi(p)\,dp}{\int_0^1p^9(1-p)^{81}\pi(p)\,dp}.
$$

For the matched [Beta distribution](../../../../../../beta-distribution.md), the integrals are beta integrals and their ratio is

$$
\boxed{\widehat p_{\mathrm B}=\frac{B(\alpha+10,\beta+81)}{B(\alpha+9,\beta+81)}
=\frac{\alpha+9}{\alpha+\beta+90}=0.07166065.}
$$

The posterior mean minimizes posterior expected squared error because $\mathbb E[(p-a)^2\mid D]=\operatorname{Var}(p\mid D)+(a-\mathbb E[p\mid D])^2$. The phrase Bayes point estimate depends on the loss: under [absolute-error loss](../../../../../../absolute-error-loss.md) it would be a posterior median, while the posterior mode is a different summary and here equals $(14.8875-1)/(207.75-2)\approx0.06750$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
