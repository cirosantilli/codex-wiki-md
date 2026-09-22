<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an [equatorial Kelvin wave](../../../../../../equatorial-kelvin-wave.md), set $\widehat v=0$. The zonal and meridional momentum equations give

$$
\widehat u=\frac{k}{\omega}\widehat\phi,
\qquad
\frac{d\widehat\phi}{dy}
=-\frac{\beta k}{\omega}y\widehat\phi,
$$

so

$$
\widehat\phi=\phi_0
\exp\left(-\frac{\beta k}{2\omega}y^2\right).
$$

Hydrostatic balance and buoyancy evolution give $\widehat\sigma=im\widehat\phi$ and $\widehat w=-\omega m\widehat\phi/N^2$. Continuity then gives

$$
\omega^2=\frac{N^2k^2}{m^2}.
$$

Because the mode must decay as $|y|\to\infty$, one needs $k/\omega>0$. With the stipulated $\omega>0$, the acceptable branch is therefore

$$
\boxed{\omega=\frac{Nk}{|m|},\qquad k>0.}
$$

The branch $\omega=-Nk/|m|$ would require $k<0$ when $\omega>0$, making the Gaussian exponent positive and the mode unbounded; it is not an equatorially trapped solution.

For real $k,m,\omega$,

$$
\overline{u'w'}
=\frac12\operatorname{Re}(\widehat u\widehat w^*)
=\boxed{-\frac12\frac{km}{N^2}|\widehat\phi|^2.}
$$

Upward group propagation has $m<0$, while a Kelvin wave has $k>0$, so $\overline{u'w'}>0$. Dissipation makes this eastward momentum flux decrease with height; therefore $-\partial_z\overline{u'w'}>0$ and the wave exerts an eastward force on the mean flow.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
