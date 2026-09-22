<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define a new probability measure by the strictly positive [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md)

$$
\frac{d\mathbb Q}{d\mathbb P}
=\exp\!\left(\widetilde\sigma Z-\frac12\widetilde\sigma^2\right),
\qquad
\widetilde\sigma=-\frac{m+\sigma^2/2}{\sigma}.
$$

The [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) shows that this density has expectation one, so $\mathbb Q$ is a probability measure equivalent to $\mathbb P$. Moreover,

$$
\begin{aligned}
\mathbb E_{\mathbb Q}[S_1^1]
&=\mathbb E_{\mathbb P}\!\left[
e^{\widetilde\sigma Z-\widetilde\sigma^2/2}
e^{\sigma Z+m}\right]\\
&=\exp\!\left(m+\frac{\sigma^2}{2}
+\sigma\widetilde\sigma\right)=1=S_0^1.
\end{aligned}
$$

**Thus the discounted risky asset is a one-period $\mathbb Q$-martingale. The [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md) implies that there is no arbitrage.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
