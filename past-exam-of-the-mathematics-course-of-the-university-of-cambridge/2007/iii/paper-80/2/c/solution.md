<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the unit-amplitude incident [plane wave](../../../../../../plane-wave.md) as $\psi_i=e^{ip_ix-iq_iz}$, with $q_i=\sqrt{k^2-p_i^2}>0$. The flat Dirichlet reflected field is $\psi_s^{[0]}=-e^{ip_ix+iq_iz}$, so the flat total field vanishes at $z=0$ and has [derivative](../../../../../../derivative.md) $\partial_z\psi^{[0]}(x,0)=-2iq_ie^{ip_ix}$.

For a controlled height expansion take $f=\varepsilon h$ with fixed regular bounded shape $h$. [Taylor expansion](../../../../../../taylor-expansion.md) at the moving boundary yields

$$
0=\psi^{[0]}(x,0)+f(x)\partial_z\psi^{[0]}(x,0)+\psi_s^{[1]}(x,0)+O(\varepsilon^2).
$$

Thus the first-order scattered trace is $\psi_s^{[1]}(x,0)=2iq_if(x)e^{ip_ix}$, and its transform follows by the [Translation property of the Fourier transform](../../../../../../translation-property-of-the-fourier-transform.md):

$$
\boxed{\widehat\psi_s^{[1]}(\nu)=2iq_i\widehat f(\nu-p_i),\qquad
\widehat\psi_{\rm sc}(\nu)=-2\pi\delta(\nu-p_i)+2iq_i\widehat f(\nu-p_i)+O(\varepsilon^2)}.
$$

The first formula is the roughness correction; the second includes the zeroth-order reflection. The small-height assumption controls the [Taylor expansion](../../../../../../taylor-expansion.md) for a fixed profile; arbitrarily fine surface scales can require additional [derivative](../../../../../../derivative.md) control, not merely a small height at fixed $k$.

If the mean roughness height is a constant $\bar f$, as for stationary roughness, then $\langle\widehat f(\nu-p_i)\rangle=2\pi\bar f\delta(\nu-p_i)$. Consequently the [specular first-order mean reflection](../../../../../../specular-first-order-mean-reflection.md) is

$$
\boxed{\langle\psi_{\rm sc}(x,z)\rangle
=(-1+2iq_i\bar f)e^{ip_ix+iq_iz}+O(\varepsilon^2)}.
$$

Its tangential [wavenumber](../../../../../../wavenumber.md) is unchanged and its normal [wavenumber](../../../../../../wavenumber.md) is reversed relative to incidence, which is precisely [specular reflection](../../../../../../specular-reflection.md). For zero mean height the first-order mean correction is zero, but the full mean reflected field is not zero: it still contains the flat reflection.

Small height alone does not imply the statistical conclusion. For example, deterministic mean height $\bar f(x)=a\cos Kx$ with $|ka|\ll1$ produces first-order mean sidebands at $p_i\pm K$ and is not purely specular. Constant mean is sufficient at first order; [stationarity](../../../../../../stationary-process.md) supplies it and, with suitable translation-invariant statistics, constrains higher-order coherent reflection as well.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
