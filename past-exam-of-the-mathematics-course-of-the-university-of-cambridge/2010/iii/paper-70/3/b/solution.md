<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Illuminate a surface window of length $D$, and define $\widehat h_D(Q)=\int_{-D/2}^{D/2}h(x)e^{-iQx}dx$. In the far field put $(x,z)=r(\sin\theta_s,\cos\theta_s)$, with $|\theta_s|<\pi/2$ away from grazing. The spectral phase $\xi\sin\theta_s+\beta(\xi)\cos\theta_s$ has stationary point $\xi_s=k\sin\theta_s$, value $k$, and second [derivative](../../../../../../derivative.md) $-1/(k\cos^2\theta_s)$. [Stationary phase](../../../../../../stationary-phase-method.md) therefore gives

$$
\psi_s^{[1]}\sim iq_iA_i\sqrt{\frac{2k}{\pi r}}\cos\theta_s\,
\widehat h_D(Q)e^{ikr-i\pi/4},\qquad Q=k\sin\theta_s-p_i.
$$

Let $C_h(s)=\langle h(x+s)h(x)\rangle$ and $S_h(Q)=\int C_h(s)e^{-iQs}ds$. Statistical [stationarity](../../../../../../stationary-process.md) gives exactly

$$
\left\langle|\widehat h_D(Q)|^2\right\rangle
=\int_{-D}^D(D-|s|)C_h(s)e^{-iQs}ds.
$$

If $C_h$ is integrable, division by $D$ and [dominated convergence](../../../../../../dominated-convergence-theorem.md) yield $\langle|\widehat h_D(Q)|^2\rangle/D\to S_h(Q)$. Thus the leading [rough-surface far-field intensity per illuminated length](../../../../../../rough-surface-far-field-intensity-per-illuminated-length.md) is

$$
\boxed{\frac{\langle|\psi_s^{[1]}(r,\theta_s)|^2\rangle}{D}
\sim\frac{2kq_i^2|A_i|^2\cos^2\theta_s}{\pi r}\,S_h(k\sin\theta_s-p_i).}
$$

This uses the field-intensity convention $I=|\psi|^2$; if $\psi$ is acoustic pressure, multiply by $1/(2\rho c)$ for physical far-field energy flux. The [variance](../../../../../../variance-split.md) normalization is $\sigma^2=C_h(0)=(2\pi)^{-1}\int S_h(Q)dQ$. Consequently the diffuse intensity is of order $\sigma^2$ and samples the surface spectrum at the tangential momentum transfer. Its value is not determined by the r.m.s. height alone.

The finite window must first be in its far field, for example $r\gg kD^2$, before interpreting the large-window intensity density. An infinitely long stationary surface has infinite illuminated power and no finite total far-field intensity at a fixed point. For nonintegrable correlations the analogous result is a spectral measure, possibly with atoms. Zero mean height makes the linear rough mean field zero, but does not make its mean intensity zero; the flat specular reflection remains separate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
