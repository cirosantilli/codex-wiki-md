<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the spatial [Fourier transform](../../../../../../fourier-transform.md) of the causal [Green function](../../../../../../green-s-function.md). The transformed equation is $\widehat G_t=(\mu-iUk-\gamma k^2)\widehat G+\delta(t)$, with zero response for $t<0$. Integration across the impulse sets $\widehat G(k,0^+)=1$, so

$$
\widehat G(k,t)=H(t)e^{\mu t-iUkt-\gamma k^2t}.
$$

Inverting the [Gaussian Fourier transform](../../../../../../fourier-transform-of-a-gaussian.md) gives

$$
\boxed{G(x,t)=\frac{H(t)}{\sqrt{4\pi\gamma t}}\exp\!\left(\mu t-\frac{(x-Ut)^2}{4\gamma t}\right).}
$$

This solves the homogeneous equation for $t>0$ and tends to the [Dirac delta distribution](../../../../../../dirac-delta-function.md) as $t\downarrow0$. Its spatial integral is $e^{\mu t}$, as required by the zero-wavenumber growth law.

Along a ray $x=vt$, the exponential [growth rate](../../../../../../growth-rate.md) is

$$
s(v)=\mu-\frac{(v-U)^2}{4\gamma}.
$$

The impulse grows in the moving interval of rays $U-2\sqrt{\gamma\mu}<v<U+2\sqrt{\gamma\mu}$, while its peak at $x=Ut$ grows as $t^{-1/2}e^{\mu t}$. At a fixed position,

$$
G(x,t)\sim\frac{e^{Ux/(2\gamma)}}{\sqrt{4\pi\gamma t}}e^{(\mu-U^2/(4\gamma))t}.
$$

Thus, under the printed assumption $\mu>0$, **$0<\mu<U^2/(4\gamma)$ gives convective wave-packet instability**, because the growing disturbance is swept away from each fixed observation point. **$\mu>U^2/(4\gamma)$ gives absolute wave-packet instability**, with exponential growth at fixed position. At equality the fixed-position exponential rate is zero and the impulse decays algebraically as $t^{-1/2}$, even though its moving peak grows. The two bounding rays have the same algebraic prefactor.

These statements classify the [Green function](../../../../../../green-s-function.md) and localized initial disturbances propagated by its convolution. They do not assert that every possible initial condition decays at fixed position in the convective case: spatially uniform initial data instead produce $e^{\mu t}$. Persistent external forcing can likewise change the observed late-time response. The distinction between [convective wave-packet instability](../../../../../../convective-wave-packet-instability.md) and [absolute wave-packet instability](../../../../../../absolute-wave-packet-instability.md) concerns localized disturbances in a specified frame.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
