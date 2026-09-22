<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Differentiate the [point mass](../../../../../../point-mass.md) [thin gravitational lens equation](../../../../../../thin-gravitational-lens-equation.md):

$$
\frac{d\beta}{d\theta}=1+\frac{\theta_E^2}{\theta^2},\qquad
\frac\beta\theta=1-\frac{\theta_E^2}{\theta^2}.
$$

Hence the specified signed [lensing magnification](../../../../../../lensing-magnification.md) is

$$
\boxed{\mu=\frac{\theta}{\beta}\frac{d\theta}{d\beta}
=\frac1{1-\theta_E^4/\theta^4}.}
$$

The outer image has positive parity and the inner image has negative parity. [Gravitational lensing](../../../../../../gravitational-lensing.md) preserves [surface brightness](../../../../../../surface-brightness.md); amplification comes from increased angular image area. The observed flux magnifications are $|\mu_+|$ and $|\mu_-|$; a negative determinant reverses orientation, not flux. Substitution of the two roots, with $u=|\beta|/\theta_E$, gives

$$
\mu_\pm=\frac12\pm\frac{u^2+2}{2u\sqrt{u^2+4}},\qquad
\mu_{\rm tot}=|\mu_+|+|\mu_-|=\frac{u^2+2}{u\sqrt{u^2+4}}>1.
$$

At $\beta=0$, axial symmetry produces an [Einstein ring](../../../../../../einstein-ring.md). For an ideal [point-like astronomical source](../../../../../../point-like-astronomical-source.md), the [lensing magnification](../../../../../../lensing-magnification.md) diverges: near alignment $\mu_{\rm tot}\sim1/u$. Finite source size gives a finite observed flux and a ring of finite thickness.

For $0<\beta<\theta_E$, there are two images on opposite sides. Their separation is $\sqrt{\beta^2+4\theta_E^2}$, approaching $2\theta_E$ at alignment. For $\beta\ll\theta_E$, their positions are $\theta_\pm\simeq\pm\theta_E+\beta/2$ and $\mu_\pm\simeq1/2\pm\theta_E/(2\beta)$: both images are bright, with the outer one slightly brighter. Moving away from alignment reduces the total amplification and makes the inner image relatively fainter.

For $\beta\gg\theta_E$, expanding the two image roots gives

$$
\theta_+\simeq\beta+\frac{\theta_E^2}{\beta},\qquad
\theta_-\simeq-\frac{\theta_E^2}{\beta},\qquad
\mu_+\simeq1+\frac{\theta_E^4}{\beta^4},\qquad
\mu_-\simeq-\frac{\theta_E^4}{\beta^4}.
$$

Thus **the distant source has one almost unaltered bright image and an extremely faint opposite-parity secondary**, with total flux magnification $1+2\theta_E^4/\beta^4+O((\theta_E/\beta)^6)$. The secondary persists for every finite nonzero source offset in the [point mass](../../../../../../point-mass.md) model.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
