<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $v=\sigma_{\rm int}^2$, $r_s=\sigma_{m,s}^2$ and $d_s=\mu(z_s;H_0,w,\Omega_M)$. The latent [absolute magnitude](../../../../../../absolute-magnitude.md) and measurement error are independent normal variables, so their [convolution](../../../../../../convolution.md) is normal. After integrating out the individual intrinsic magnitudes, each [apparent magnitude](../../../../../../apparent-magnitude.md) has distribution

$$
\widehat m_s\mid z_s,M_0,v,H_0,w,\Omega_M\sim N(M_0+d_s,V_s),\qquad V_s=v+r_s.
$$

Consequently the [likelihood function](../../../../../../likelihood-function.md) for the independent sample is

$$
\boxed{L=\prod_{s=1}^{N}(2\pi V_s)^{-1/2}\exp\left[-\frac{(\widehat m_s-M_0-d_s)^2}{2V_s}\right]}.
$$

This is the marginal observational likelihood of a [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md), not the likelihood conditional on each unknown intrinsic magnitude. The individual errors remain [heteroscedastic](../../../../../../heteroscedastic.md) through their known $r_s$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
