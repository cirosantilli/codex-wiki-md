<h1 id="section-b/b7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p$ and $q$ for the axial source and observation distances, and put $R_{\rm eff}=pq/(p+q)$. The aperture is $-d/2<x,y<d/2$. Under the [Fresnel diffraction](../../../../../../fresnel-diffraction.md), the spherical incident [wave amplitude](../../../../../../wave-amplitude.md) is effectively constant over this small aperture, while its quadratic [wave phase](../../../../../../phase-waves.md) must be retained. Therefore the two transverse [integrals](../../../../../../integral-split.md) separate:

$$
\psi_P=K\left[\int_{-d/2}^{d/2}\exp\left(\frac{i\pi x^2}{\lambda R_{\rm eff}}\right)dx\right]^2,
$$

where $K$ contains the source strength, the propagation distances and a common [phase factor](../../../../../../phase-factor.md).

Use the dimensionless variable $u=x\sqrt{2/(\lambda R_{\rm eff})}$ and define the [optical normalization of Fresnel integrals](../../../../../../optical-normalization-of-fresnel-integrals.md)

$$
F(w)=C(w)+iS(w)=\int_0^w e^{i\pi u^2/2}\,du,\qquad
w=\frac d2\sqrt{\frac{2}{\lambda R_{\rm eff}}}.
$$

The oddness of $F$ makes the bracket $\sqrt{2\lambda R_{\rm eff}}F(w)$, so

$$
\boxed{\psi_P=2K\lambda R_{\rm eff}[C(w)+iS(w)]^2.}
$$

This [square-aperture Fresnel diffraction](../../../../../../square-aperture-fresnel-diffraction.md) normalization is especially useful for comparing with no aperture. In the same [Fresnel diffraction](../../../../../../fresnel-diffraction.md), the unrestricted one-dimensional [Fresnel integral](../../../../../../fresnel-integral.md) is $\sqrt{\lambda R_{\rm eff}}e^{i\pi/4}$; its square is $i\lambda R_{\rm eff}$. Thus, writing $\psi_0$ for the unobscured field at the same point,

$$
\boxed{\frac{\psi_P}{\psi_0}=-2i[C(w)+iS(w)]^2,\qquad
\frac{I_P}{I_0}=4[C(w)^2+S(w)^2]^2.}
$$

The normalization has the correct no-aperture limit because $C(\infty)=S(\infty)=1/2$ in this convention.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
