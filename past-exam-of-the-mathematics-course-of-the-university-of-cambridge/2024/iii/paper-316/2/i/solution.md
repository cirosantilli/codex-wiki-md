<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the distributed fragment [power-law size distribution](../../../../../../power-law-size-distribution.md) as $n(D_f)=K_fD_f^{-\alpha_f}$. A spherical fragment has mass $\pi\rho D_f^3/6$. Since this population contains one half of the target mass,

$$
\frac12\frac{\pi\rho D_t^3}{6}
=\frac{\pi\rho K_f}{6}
\int_{D_{\min,f}}^{D_{\max,f}}D_f^{3-\alpha_f}\,dD_f,
$$

and hence

$$
K_f=\frac{D_t^3}{2}
\frac{4-\alpha_f}
{D_{\max,f}^{4-\alpha_f}-D_{\min,f}^{4-\alpha_f}}.
$$

The distributed fragments have total [geometric cross-section](../../../../../../geometric-collision-cross-section.md)

$$
\sigma_{\rm dist}
=\frac{\pi K_f}{4}
\int_{D_{\min,f}}^{D_{\max,f}}D_f^{2-\alpha_f}\,dD_f
$$



$$
=\frac{\pi D_t^3}{8}
\frac{4-\alpha_f}{\alpha_f-3}
\frac{D_{\min,f}^{3-\alpha_f}-D_{\max,f}^{3-\alpha_f}}
{D_{\max,f}^{4-\alpha_f}-D_{\min,f}^{4-\alpha_f}}.
$$

The single fragment containing the other half of the mass has diameter $2^{-1/3}D_t$ and cross-section $\pi D_t^2/(4\,2^{2/3})$. Therefore the exact result within the model is

$$
\boxed{\sigma_{{\rm tot},1}=
\frac{\pi D_t^2}{4\,2^{2/3}}+\sigma_{\rm dist}}.
$$

For $D_{\max,f}\gg D_{\min,f}$ and $3\lt\alpha_f\lt4$, area is dominated by the smallest distributed fragments while mass is dominated by the largest, so normally the first term is negligible and

$$
\boxed{\sigma_{{\rm tot},1}\simeq
\frac{\pi D_t^3}{8}
\frac{4-\alpha_f}{\alpha_f-3}
D_{\min,f}^{3-\alpha_f}D_{\max,f}^{\alpha_f-4}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
