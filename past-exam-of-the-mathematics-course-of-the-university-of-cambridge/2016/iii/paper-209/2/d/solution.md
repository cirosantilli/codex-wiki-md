<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $J_{n,h}$ for the squared integral norm in question. The [scaling property of the Fourier transform](../../../../../../scaling-property-of-the-fourier-transform.md) gives $\mathcal F K_h(u)=\mathcal F K(hu)$, which vanishes outside $[-1/h,1/h]$. Also $|\mathcal F K(v)|\leq\|K\|_1$. The condition $\int K=1$ does not imply $\|K\|_1=1$, because $K$ need not be nonnegative.

Part (b), now for observations of $Y$, gives $\mathbb E|\varphi_n^Y(u)-\varphi^Y(u)|^2\leq1/n$. Apply the [Tonelli theorem](../../../../../../tonelli-theorem.md) to this nonnegative integrand, use the bound on $1/\varphi_\epsilon$, and change variables $v=hu$:

$$
\mathbb E J_{n,h}
\leq\frac{\widetilde M_h^2}{n}\int_{-1/h}^{1/h}|\mathcal F K(hu)|^2\,du
=\frac{\widetilde M_h^2}{nh}\int_{-1}^1|\mathcal F K(v)|^2\,dv
\leq\frac{2\|K\|_1^2\widetilde M_h^2}{nh}.
$$

The [characteristic function](../../../../../../characteristic-function.md) $\varphi_\epsilon$ is continuous and nonzero on the compact interval of integration, so $\widetilde M_h<\infty$ for every $h>0$. The [Markov inequality](../../../../../../markov-inequality.md) gives, for every $z>0$,

$$
\mathbb P\left(J_{n,h}^{1/2}>z\frac{\widetilde M_h}{\sqrt{nh}}\right)
\leq\frac{2\|K\|_1^2}{z^2}.
$$

Consequently **$J_{n,h}^{1/2}=O_{\mathbb P}(\widetilde M_h/\sqrt{nh})$**, including for any deterministic bandwidth sequence $h=h_n>0$. The [stochastic order](../../../../../../stochastic-order.md) follows directly from this uniform probability bound. Independence of $X$ and $\epsilon$ gives $\varphi^Y=\varphi^X\varphi_\epsilon$, explaining why division by $\varphi_\epsilon$ is the [Fourier deconvolution](../../../../../../fourier-deconvolution.md) operation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
