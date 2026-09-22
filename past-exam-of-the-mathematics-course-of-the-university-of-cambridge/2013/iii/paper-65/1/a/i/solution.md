<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Differentiating the [velocity potential](../../../../../../../velocity-potential.md) gives $u=a\omega e^{kz}\cos(kx-\omega t)$ and $w=a\omega e^{kz}\sin(kx-\omega t)$. Let $A=a e^{kz}$ and $\vartheta=kx-\omega t$. To first order in the [wave steepness](../../../../../../../wave-steepness.md) $ka$, evaluate these velocities at the initial parcel position and integrate from time zero:

$$
\boxed{X-x=A[\sin(kx)-\sin\vartheta]+O(a^2k),\qquad
Z-z=A[\cos\vartheta-\cos(kx)]+O(a^2k).}
$$

These expressions satisfy both initial conditions and distinguish [initial and mean parcel labels in a surface wave](../../../../../../../initial-and-mean-parcel-labels-in-a-surface-wave.md). Their actual short-time limits are

$$
\boxed{X-x=a\omega e^{kz}\cos(kx)t+O(t^2),\qquad
Z-z=a\omega e^{kz}\sin(kx)t+O(t^2).}
$$

The printed expressions omit the integration constants and therefore cannot be the small-time displacement from the prescribed initial point. For example, at $x=0$, they give $Z(0)-z=a e^{kz}\ne0$. This is a genuine inconsistency, rather than a missing step in the calculation.

The intended oscillatory orbit is recovered by using mean parcel coordinates instead. Set $x_c=x+A\sin(kx)$ and $z_c=z-A\cos(kx)$ to this order. Then

$$
X-x_c\simeq-ae^{kz_c}\sin(kx_c-\omega t),\qquad
Z-z_c\simeq ae^{kz_c}\cos(kx_c-\omega t).
$$

Thus a [deep-water gravity wave](../../../../../../../deep-water-gravity-wave.md) produces approximately circular parcel orbits with radius $ae^{kz_c}$, decaying exponentially with depth. The approximation is one of small amplitude over a wave cycle, not an assertion that these oscillatory coordinates vanish at time zero.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
