<h1 id="39b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\widehat\eta(k,t)=\int_{-\infty}^{\infty}\eta(x,t)e^{-ikx}\,dx,
\qquad
\eta(x,t)=\frac1{2\pi}\int_{-\infty}^{\infty}\widehat\eta(k,t)e^{ikx}\,dk.
$$

The [deep-water capillary-wave dispersion relation](../../../../../../deep-water-capillary-wave-dispersion-relation.md) makes each Fourier mode satisfy

$$
\partial_t^2\widehat\eta+S^2|k|^3\widehat\eta=0.
$$

The transformed initial data are

$$
\widehat\eta(k,0)=0,
\qquad
\partial_t\widehat\eta(k,0)
=-W\int_{-\epsilon}^{\epsilon}e^{-ikx}\,dx
=-\frac{2W\sin(k\epsilon)}k.
$$

Therefore

$$
\widehat\eta(k,t)
=-\frac{2W\sin(k\epsilon)}{kS|k|^{3/2}}
\sin(S|k|^{3/2}t).
$$

The integrand is even, so Fourier inversion gives the [surface response to a localized impulsive velocity](../../../../../../surface-response-to-a-localized-impulsive-velocity.md)

$$
\boxed{
\eta(x,t)=-\frac{2W}{\pi S}
\int_0^\infty
\frac{\sin(k\epsilon)\sin(Sk^{3/2}t)\cos(kx)}{k^{5/2}}\,dk}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [39B](../../39b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
