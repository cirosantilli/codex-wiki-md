<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Hellinger distance](../../../../../../hellinger-distance.md) convention in the original PDF:

$$
d_{\mathrm{Hell}}(\mu,\mu')^2=\frac12\int(\sqrt p-\sqrt q)^2\,d\nu
=1-\int\sqrt{pq}\,d\nu,
\qquad p=\frac{d\mu}{d\nu},\quad q=\frac{d\mu'}{d\nu}.
$$

The TeX transcription incorrectly places the integral outside the outer square root in the definition; the displayed formula for the squared distance and the original PDF both use the convention above. Although [Lebesgue measure](../../../../../../lebesgue-measure.md) is not a probability measure, we may use it as the common dominating measure: the integral is unchanged by replacing it with any equivalent dominating [probability measure](../../../../../../probability-measure.md).

For unit-variance [normal distributions](../../../../../../normal-distribution.md), put $\bar\theta=(\theta_1+\theta_2)/2$ and $\Delta=\theta_1-\theta_2$. The product of the square roots of their [probability density functions](../../../../../../probability-density-function.md) is

$$
\sqrt{p_1(x)p_2(x)}
=\frac1{\sqrt{2\pi}}\exp\left[-\frac{(x-\theta_1)^2+(x-\theta_2)^2}{4}\right]
=e^{-\Delta^2/8}\frac1{\sqrt{2\pi}}e^{-(x-\bar\theta)^2/2}.
$$

The final factor integrates to one, so

$$
\boxed{d_{\mathrm{Hell}}(\mu_1,\mu_2)^2=1-e^{-(\theta_1-\theta_2)^2/8}.}
$$

For the bound at arbitrary $\sigma_1,\sigma_2>0$, use the given formula for the [Hellinger distance between normal distributions](../../../../../../hellinger-distance-between-normal-distributions.md) and write

$$
S=\sigma_1^2+\sigma_2^2,\qquad
B=\sqrt{\frac{2\sigma_1\sigma_2}{S}}\leq1,\qquad
x=\frac{(\theta_1-\theta_2)^2}{4S}.
$$

Since $1-e^{-x}\leq x$ for $x\geq0$,

$$
\begin{aligned}
d_{\mathrm{Hell}}^2
&=(1-B)+B(1-e^{-x})\\
&\leq\frac{1-B^2}{1+B}+x\\
&=\frac{(\sigma_1-\sigma_2)^2}{S(1+B)}
+\frac{(\theta_1-\theta_2)^2}{4S}\\
&\leq\frac{(\sigma_1-\sigma_2)^2+(\theta_1-\theta_2)^2}{S}.
\end{aligned}
$$

Therefore one valid choice is $\boxed{C_{\sigma_1,\sigma_2}=1/(\sigma_1^2+\sigma_2^2)}$. In particular this bound is uniform when the two standard deviations stay bounded away from zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
