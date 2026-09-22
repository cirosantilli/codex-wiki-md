<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $P_{\theta,n}=d^{-1}\sum_{S\in\mathcal S}P_{\theta,S}^{\otimes n}$. Expanding its [chi-squared divergence](../../../../../../chi-squared-divergence.md) by the [second moment of a mixture likelihood ratio](../../../../../../second-moment-of-a-mixture-likelihood-ratio.md), and using the supplied one-observation cross moment and [independence](../../../../../../independent-random-variables.md), gives

$$
\boxed{\chi^2(P_{\theta,n}\Vert P_0^{\otimes n})=\mathbb E_{S,T}\left[\left(1-\theta^2\frac{|S\cap T|^2}{k^2}\right)^{-n/2}\right]-1.}
$$

Here $S,T$ are independent uniform members of the specified family of cyclic intervals. Their overlap $R=|S\cap T|$ does not have the [hypergeometric distribution](../../../../../../hypergeometric-distribution.md) of arbitrary uniform $k$-subsets. The family's geometry must be retained.

Let $x=\theta^2R^2/k^2<1/4$. Since $-\log(1-x)\leq x/(1-x)\leq2x$ and $R^2/k^2\leq R/k$, we obtain $(1-x)^{-n/2}\leq e^{nx}\leq e^{n\theta^2R/k}$. Taking the [expected value](../../../../../../expected-value.md) proves the upper bound. The factor $n$ in the last exponent is present in the PDF and missing in the TeX aid.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
