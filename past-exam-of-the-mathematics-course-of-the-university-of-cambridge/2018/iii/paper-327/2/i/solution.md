<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [space of test functions](../../../../../../space-of-test-functions.md) is $\mathcal D(\mathbb R)=C_c^\infty(\mathbb R)$. A sequence $\varphi_j$ converges to $\varphi$ when all functions eventually have [compact support](../../../../../../compact-support.md) in one [compact set](../../../../../../compact-space.md) $K$ and every derivative converges uniformly:

$$
\|\varphi_j^{(q)}-\varphi^{(q)}\|_\infty\longrightarrow0
\quad\text{for each integer }q\geq0.
$$

A [distribution](../../../../../../distribution-mathematical-analysis.md) is a continuous linear functional on this [space of test functions](../../../../../../space-of-test-functions.md). Equivalently, for each [compact set](../../../../../../compact-space.md) $K$, there are $C_K$ and a finite integer $m_K$ such that

$$
|\langle u,\varphi\rangle|\leq C_K\max_{0\leq q\leq m_K}\|\varphi^{(q)}\|_\infty
\quad\text{whenever }\operatorname{supp}\varphi\subseteq K.
$$

The integer $m_K$ is permitted to depend on $K$. The usual [weak convergence of distributions](../../../../../../weak-convergence-of-distributions.md) is

$$
\boxed{u_j\longrightarrow u\text{ in }\mathcal D'(\mathbb R)
\quad\Longleftrightarrow\quad
\langle u_j,\varphi\rangle\longrightarrow\langle u,\varphi\rangle
\text{ for every }\varphi\in\mathcal D(\mathbb R).}
$$

Thus the convergence convention on the [distribution](../../../../../../distribution-mathematical-analysis.md) space is its weak dual topology.

For the [principal-value reciprocal distribution](../../../../../../principal-value-reciprocal-distribution.md), the symmetric truncations can be written

$$
\left\langle\operatorname{pv}\frac1x,\varphi\right\rangle
=\lim_{\varepsilon\downarrow0}\int_{|x|>\varepsilon}\frac{\varphi(x)}x\,dx
=\int_0^\infty\frac{\varphi(x)-\varphi(-x)}x\,dx.
$$

The numerator is $O(x)$ near zero by the [mean value theorem](../../../../../../mean-value-theorem.md), and the integrand vanishes for large $x$ because $\varphi$ has [compact support](../../../../../../compact-support.md). For $\operatorname{supp}\varphi\subset[-R,R]$,

$$
\left|\left\langle\operatorname{pv}\frac1x,\varphi\right\rangle\right|
\leq2R\|\varphi'\|_\infty.
$$

Consequently the [Cauchy principal value](../../../../../../cauchy-principal-value.md) defines a [distribution](../../../../../../distribution-mathematical-analysis.md) of [order of a distribution](../../../../../../order-of-a-distribution.md) at most one.

The function $\log|x|$ has [local integrability](../../../../../../locally-integrable-function.md), since $\int_0^1|\log x|\,dx<\infty$, and therefore defines a [distribution](../../../../../../distribution-mathematical-analysis.md). For its [distributional derivative](../../../../../../distributional-derivative.md), remove $(-\varepsilon,\varepsilon)$ and use [integration by parts](../../../../../../integration-by-parts.md) on both remaining intervals:

$$
-\int_{|x|>\varepsilon}\log|x|\,\varphi'(x)\,dx
=\int_{|x|>\varepsilon}\frac{\varphi(x)}x\,dx
+\log\varepsilon\,[\varphi(\varepsilon)-\varphi(-\varepsilon)].
$$

The boundary term is $O(\varepsilon|\log\varepsilon|)$ and tends to zero. The omitted integral of $\log|x|\varphi'$ tends to zero by [local integrability](../../../../../../locally-integrable-function.md). Hence the [distributional derivative of the logarithmic modulus](../../../../../../distributional-derivative-of-the-logarithmic-modulus.md) satisfies

$$
\boxed{\frac{d}{dx}\log|x|=\operatorname{pv}\frac1x\quad\text{in }\mathcal D'(\mathbb R).}
$$

Symmetric truncation is essential to this normalization of the [principal-value reciprocal distribution](../../../../../../principal-value-reciprocal-distribution.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
