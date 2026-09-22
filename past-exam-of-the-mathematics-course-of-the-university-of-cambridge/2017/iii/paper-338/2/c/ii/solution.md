<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\beta_0$ be the direction of the [optical camera](../../../../../../../optical-camera.md) [optical axis](../../../../../../../optical-axis.md). The [grating equation](../../../../../../../grating-equation.md) on that axis is

$$
m\lambda_m=d(\sin\alpha+\sin\beta_0)=K.
$$

The central [wavelengths](../../../../../../../wavelength.md) in adjacent [diffraction orders](../../../../../../../diffraction-order.md) are therefore $\lambda_m=K/m$ and $\lambda_{m+1}=K/(m+1)$, with separation

$$
\boxed{S_{\rm centres}=\lambda_m-\lambda_{m+1}=\frac{K}{m(m+1)},\qquad K=d(\sin\alpha+\sin\beta_0).}
$$

$K$ is the fixed order-times-wavelength product directed onto the [optical camera](../../../../../../../optical-camera.md) axis, or the optical path difference between adjacent grooves in that direction. In a [Littrow configuration](../../../../../../../littrow-configuration.md), $K=2d\sin\alpha$. This adjacent-central-wavelength spacing is a conventional [free spectral range of an echelle grating](../../../../../../../free-spectral-range-of-an-echelle-grating.md); at high order it is approximately $\lambda_m/m$.

There is a qualification in the wording of the printed definition. The exact interval for which order $m$ lies closest to the $y$ axis is not, in general, identical to the spacing of two adjacent order centres. For a concrete counterexample take $\beta_0=0$, $0<\alpha<\pi/2$, and a [photodetector](../../../../../../../photodetector.md) mapping $x=f_{\rm cam}\tan\beta$. Equality of the distances from the axis for orders $m,m+1$ means $\beta_m=-\beta_{m+1}$, so their common boundary is $\lambda=K/(m+1/2)$. The other boundary with order $m-1$ is $K/(m-1/2)$. Consequently the literal closest-order interval has width

$$
\boxed{S_{\rm nearest}=\frac{K}{m-1/2}-\frac{K}{m+1/2}=\frac{K}{m^2-1/4},}
$$

for $m\ge2$ and accessible non-grazing orders. This differs from the printed $K/[m(m+1)]$. For a nonzero $\beta_0$, the exact boundary is determined by $\beta_m+\beta_{m+1}=2\beta_0$ and need not even have the simple half-order form. The two definitions agree to leading order $K/m^2$ when $m$ is large. Thus the printed expression is correct as an adjacent-centre convention or a high-order coverage estimate, rather than an exact consequence of the literal nearest-axis definition. Gap-free coverage should be checked using the actual [photodetector](../../../../../../../photodetector.md) mapping and neighbouring order endpoints.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
