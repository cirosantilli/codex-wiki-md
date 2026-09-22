<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

Applying [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md) to a pillbox and [Ampère's law](../../../../../ampere-s-circuital-law.md) to an interface-crossing rectangle gives

$$
\boxed{\hat n\cdot(\mathbf B_2-\mathbf B_1)=0,\qquad
\hat n\times(\mathbf H_2-\mathbf H_1)=\mathbf K_f.}
$$

Here $\hat n$ points from material 1 to 2 and $\mathbf K_f$ is free surface current. With no such current, $B_n$ and $H_t$ are continuous. For linear isotropic media, $B_{t2}/\mu_2=B_{t1}/\mu_1$ and $\mu_2H_{n2}=\mu_1H_{n1}$. The [magnetic fields](../../../../../magnetic-field-split.md) need not have equal magnitudes on either side.

With negligible leakage, [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md) makes each cross-section of a [magnetic flux](../../../../../magnetic-flux.md) tube carry the same flux $\mathcal F$. High permeability guides it through the core; a short gap permits neglect of fringing. Flux conservation across these particular geometric sections is an approximation, not a consequence of zero divergence without controlling side leakage.

Let $L$ be the constant-radius arc marked in the figure, and $\mu_r=\mu/\mu_0$. For each straight taper, the [radius](../../../../../radius.md) changes linearly from $R$ to $r$, giving the [reluctance of a conical magnetic pole](../../../../../reluctance-of-a-conical-magnetic-pole.md)

$$
\int_{\rm taper}\frac{dx}{\mu\pi a(x)^2}=\frac{s}{\mu\pi Rr}.
$$

Summing [magnetic reluctances](../../../../../magnetic-reluctance.md) to find the [gap field of a tapered electromagnet](../../../../../gap-field-of-a-tapered-electromagnet.md), and using $B_g=\mathcal F/(\pi r^2)$ gives

$$
NI=\mathcal F\left(\frac{L}{\mu\pi R^2}+\frac{2s}{\mu\pi Rr}+\frac{h}{\mu_0\pi r^2}\right),\qquad
\boxed{H_g=\frac{NI}{h+\mu_r^{-1}(Lr^2/R^2+2sr/R)},\quad B_g=\mu_0H_g.}
$$

If $L$ is instead defined as the total magnetic-material [length](../../../../../length.md), replace the displayed uniform-arc [length](../../../../../length.md) by $L-2s$. The comparison untapered core has uniform [radius](../../../../../radius.md) $R$ and material [length](../../../../../length.md) $L+2s$, so

$$
\boxed{\frac{H_g}{H_{g0}}=
\frac{h+(L+2s)/\mu_r}{h+(Lr^2/R^2+2sr/R)/\mu_r}.}
$$

**The original PDF specifies $s/L\ll r/R$**; the TeX transcription reverses this inequality. In the printed limit the taper reluctances are small relative to that of the broad arc. The gain is approximately $[h+L/\mu_r]/[h+Lr^2/(\mu_rR^2)]$, approaching $(R/r)^2$ if the gap reluctance is also negligible. If the gap dominates, both fields instead approach $NI/h$ and the gain approaches one. [magnetic saturation](../../../../../magnetic-saturation.md) near the small poles, gap fringing, leakage and winding heating limit practical enhancement.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
