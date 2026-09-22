<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the common dominating [probability measure](../../../../../../probability-measure.md) $\nu=(\mu+\mu')/2$ and let $p=d\mu/d\nu$, $q=d\mu'/d\nu$ be the [Radon-Nikodym derivatives](../../../../../../radon-nikodym-derivative.md). The assumed second [moments](../../../../../../moment.md) imply first-moment integrability by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Since $Y$ is a separable [Banach space](../../../../../../banach-space-split.md), the measurable $f$ is a [strongly measurable function](../../../../../../strongly-measurable-function.md), and both [expected values](../../../../../../expected-value.md) exist as [Bochner integrals](../../../../../../bochner-integral.md).

The difference of these [Bochner integrals](../../../../../../bochner-integral.md) satisfies

$$
\begin{aligned}
\|\mathbb E^\mu f-\mathbb E^{\mu'}f\|_Y
&=\left\|\int_Xf(p-q)\,d\nu\right\|_Y\\
&\leq\int_X\|f\|_Y\,|\sqrt p-\sqrt q|(\sqrt p+\sqrt q)\,d\nu\\
&\leq\left(\int_X\|f\|_Y^2(\sqrt p+\sqrt q)^2\,d\nu\right)^{1/2}
\left(\int_X(\sqrt p-\sqrt q)^2\,d\nu\right)^{1/2}.
\end{aligned}
$$

The first inequality is the norm bound for a [Bochner integral](../../../../../../bochner-integral.md), and the second is the scalar [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Since $(\sqrt p+\sqrt q)^2\leq2(p+q)$, the first factor is at most

$$
\sqrt{2}\left(\mathbb E^\mu\|f\|_Y^2+\mathbb E^{\mu'}\|f\|_Y^2\right)^{1/2}.
$$

With the [Hellinger distance](../../../../../../hellinger-distance.md) convention of the original PDF, the second factor is $\sqrt2\,d_{\mathrm{Hell}}(\mu,\mu')$. Multiplication proves the [Hellinger bound for differences of expectations](../../../../../../hellinger-bound-for-differences-of-expectations.md):

$$
\boxed{\|\mathbb E^\mu f-\mathbb E^{\mu'}f\|_Y
\leq2\left(\mathbb E^\mu\|f\|_Y^2+\mathbb E^{\mu'}\|f\|_Y^2\right)^{1/2}
d_{\mathrm{Hell}}(\mu,\mu').}
$$

The proof uses only the two laws and their common dominating measure; no [absolute continuity of measures](../../../../../../absolute-continuity-of-measures.md) assumption between $\mu$ and $\mu'$ is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
