<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix time dependence $e^{-i\omega t}$ and use [pressure](../../../../../../pressure.md) [amplitude](../../../../../../wave-amplitude.md) for $\psi$. Write the incident [acoustic plane wave](../../../../../../acoustic-plane-wave.md) as $\psi_i=Ae^{i\alpha x-i\beta z}$, where $\alpha=k\cos\theta$, $\beta=k\sin\theta>0$. “Perfectly reflecting” specifies zero absorbed energy but does not uniquely select a boundary condition: a rigid wall has a [Neumann boundary condition](../../../../../../neumann-boundary-condition.md), whereas a [pressure](../../../../../../pressure.md)-release surface has a [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md). We first give the rigid-wall result, and then the alternative [pressure](../../../../../../pressure.md)-release result.

For the rigid surface the normal-[velocity](../../../../../../velocity.md) condition, without an immaterial normalizing factor, is

$$
(\partial_z-h'(x)\partial_x)\psi(x,h(x))=0.
$$

Expand $\psi=\psi^{[0]}+\psi^{[1]}+\psi^{[2]}+\cdots$ in the height [amplitude](../../../../../../wave-amplitude.md), scaling a fixed differentiable profile. The flat total field is $\psi^{[0]}=Ae^{i\alpha x}(e^{-i\beta z}+e^{i\beta z})$. Taylor expansion gives

$$
\partial_z\psi^{[1]}(x,0)=-h\partial_z^2\psi^{[0]}(x,0)+h'\partial_x\psi^{[0]}(x,0)
=2Ae^{i\alpha x}(\beta^2h+i\alpha h').
$$

Let $\widehat h(q)=\int h(x)e^{-iqx}dx$ and $\beta(q)=\sqrt{k^2-q^2}$ on the outgoing sheet: it is positive real for propagating modes and positive imaginary for evanescent modes. Fourier transforming this boundary derivative gives $2A(k^2-\alpha q)\widehat h(q-\alpha)$. The [outgoing angular spectrum](../../../../../../outgoing-angular-spectrum.md) therefore yields the [small-height Neumann scattering](../../../../../../small-height-neumann-scattering.md) field

$$
\boxed{\psi_s(x,z)=Ae^{i\alpha x+i\beta z}
+\frac{2A}{2\pi i}\int_{\mathbb R}\frac{k^2-\alpha q}{\beta(q)}\widehat h(q-\alpha)e^{iqx+i\beta(q)z}\,dq+O(h^2).}
$$

For an infinite stationary surface the Fourier quantities may be interpreted as random distributions or through a finite illumination window and its limiting mean. The correction is linear in $h$ and $h'$, so zero mean height and stationarity give

$$
\boxed{\langle\psi_s\rangle=Ae^{i\alpha x+i\beta z}+O(h^2)\quad\text{for a rigid reflector}.}
$$

Only the rough correction has zero mean at first order; the flat reflected wave remains.

The first nontrivial coherent correction depends on correlation, not just the r.m.s. height. Define $C_h(s)=\langle h(x+s)h(x)\rangle$, its [power spectrum of surface height](../../../../../../power-spectrum-of-surface-height.md) $S_h(q)=\int C_h(s)e^{-iqs}ds$, and $\sigma^2=(2\pi)^{-1}\int S_h(q)dq$. At second order the flat-field third normal derivative and mixed derivative vanish at zero, leaving

$$
\partial_z\psi^{[2]}(x,0)=-h\partial_z^2\psi^{[1]}(x,0)+h'\partial_x\psi^{[1]}(x,0).
$$

For each first-order outgoing Fourier component, its derivative data are $g_1(q)=2A(k^2-\alpha q)\widehat h(q-\alpha)$, its second normal derivative is $i\beta(q)g_1(q)$, and its tangential derivative is $qg_1(q)/\beta(q)$. Averaging their products with $h,h'$ gives the mean derivative

$$
\langle\partial_z\psi^{[2]}(x,0)\rangle
=-2iAe^{i\alpha x}\int\frac{(k^2-\alpha q)^2}{\beta(q)}S_h(q-\alpha)\,\frac{dq}{2\pi}.
$$

Dividing by the specular outgoing derivative $i\beta$ therefore gives [oblique coherent reflection from a stationary rigid rough surface](../../../../../../oblique-coherent-reflection-from-a-stationary-rigid-rough-surface.md):

$$
\boxed{\langle\psi_s\rangle=Ar_Ne^{i\alpha x+i\beta z},\qquad
r_N=1-\frac1{\pi\beta}\int\frac{(k^2-\alpha q)^2}{\beta(q)}S_h(q-\alpha)\,dq+O(h^3).}
$$

This second-order expression requires the relevant spectral moments to exist and the boundary expansion to remain controlled. Small $|kh|$ alone does not control arbitrarily large slopes or high-frequency roughness. The given stationarity and $\sigma$ determine the first-order mean above, but do not determine this spectrum-weighted correction numerically.

For a [pressure](../../../../../../pressure.md)-release surface, instead impose $\psi(x,h)=0$. The flat reflected coefficient is $-1$, and Taylor expansion gives $\psi^{[1]}(x,0)=2i\beta Ahe^{i\alpha x}$. Thus [small-height Dirichlet scattering](../../../../../../small-height-dirichlet-scattering.md) gives

$$
\boxed{\psi_s=-Ae^{i\alpha x+i\beta z}
+\frac{2i\beta A}{2\pi}\int\widehat h(q-\alpha)e^{iqx+i\beta(q)z}\,dq+O(h^2).}
$$

The zero-mean first correction again vanishes on averaging. At second order $\psi^{[2]}(x,0)=-h\partial_z\psi^{[1]}(x,0)$, giving

$$
\boxed{\langle\psi_s\rangle=Ar_De^{i\alpha x+i\beta z},\qquad
r_D=-1+\frac\beta\pi\int\beta(q)S_h(q-\alpha)\,dq+O(h^3).}
$$

If the roughness spectrum is concentrated near $q=\alpha$ after the incident tangential shift, the additional long-correlation approximation yields $r_N\simeq1-2\beta^2\sigma^2$ and $r_D\simeq-1+2\beta^2\sigma^2$. A local Gaussian random-height phase model would then give $r_N=e^{-2\beta^2\sigma^2}$ and $r_D=-e^{-2\beta^2\sigma^2}$, but Gaussian statistics and that local approximation were not supplied. They must not be inferred from stationarity and r.m.s. height alone.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
