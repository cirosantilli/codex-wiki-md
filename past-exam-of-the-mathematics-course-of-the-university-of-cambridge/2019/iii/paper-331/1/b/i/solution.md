<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a possibly unstable [normal mode](../../../../../../../normal-mode.md), $c_i\ne0$ ensures $V=U-c$ never vanishes, so choose one continuous branch of $V^a$. Substitute $\widehat w=V^aq$ into the [Taylor–Goldstein equation](../../../../../../../taylor-goldstein-equation.md) and collect terms:

$$
q''+2a\frac{U'}Vq'+\left[-k^2+(a-1)\frac{U''}V+\frac{N^2+a(a-1)(U')^2}{V^2}\right]q=0.
$$

Multiplication by $V^{2a}$ puts its first two terms in [divergence form](../../../../../../../divergence-form.md):

$$
(V^{2a}q')'-k^2V^{2a}q+\left[(a-1)U''V^{2a-1}+\{N^2+a(a-1)(U')^2\}V^{2a-2}\right]q=0.
$$

Multiply by the [complex conjugate](../../../../../../../complex-conjugate.md) $\overline q$ and apply [integration by parts](../../../../../../../integration-by-parts.md). Since $q(\pm L)=0$, the boundary term vanishes and the [power-transformed Taylor–Goldstein energy identity](../../../../../../../power-transformed-taylor-goldstein-energy-identity.md) is

$$
\boxed{\int_{-L}^LV^{2a}(|q'|^2+k^2|q|^2)dz=\int_{-L}^L\left[\{N^2+a(a-1)(U')^2\}V^{2a-2}+(a-1)U''V^{2a-1}\right]|q|^2dz.}
$$

The weight is $V^{2a}$, not $|V|^{2a}$: preserving its complex phase is essential for the subsequent stability proofs.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
