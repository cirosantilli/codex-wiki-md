<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

For spherical symmetry, $r\widetilde p$ satisfies the one-dimensional [wave equation](../../../../../wave-equation-split.md), so an outgoing solution has the form $A(t-r/c)/r$. To relate $A$ to the source, use a [velocity potential](../../../../../velocity-potential.md) $\Phi$ with $u_r=\partial_r\Phi$ and $\widetilde p=-\rho\partial_t\Phi$. The outgoing monopole potential

$$
\Phi=-\frac{q(t-r/c)}{4\pi\rho r}
$$

has $4\pi r^2\rho u_r\to q(t)$ as $r\to0$, fixing its mass-flux normalization. It follows that

$$
\boxed{\widetilde p(r,t)=\frac{q'(t-r/c)}{4\pi r}.}
$$

For an element with displacement $f_0e^{i\omega t}$, its volume outflow is $i\omega f_0h^2e^{i\omega t}$ and mass outflow is $\rho$ times this. Thus $q'=-\rho\omega^2f_0h^2e^{i\omega t}$. A rigid wall imposes zero normal velocity away from the source. The [method of images](../../../../../method-of-images.md) uses a source of the same sign on the other side; a source on the plane and its image coincide, doubling the full-space monopole field. Equivalently its mass flux spreads over a hemisphere rather than a sphere. Hence

$$
\boxed{\widetilde p=-\frac{2\rho\omega^2f_0h^2}{4\pi R}e^{i\omega(t-R/c)}.}
$$

The small patch relative to wavelength justifies the point source, and the small displacement justifies linear acoustics.

Superposition over the aperture gives the [Rayleigh integral for baffled acoustic radiation](../../../../../rayleigh-integral-for-baffled-acoustic-radiation.md)

$$
\widetilde p(t,x,y,z)=-\frac{\rho\omega^2}{2\pi}
\iint\frac{f(y',z')}{R}e^{i\omega(t-R/c)}\,dy'\,dz',
\quad R=\sqrt{x^2+(y-y')^2+(z-z')^2}.
$$

For $r\gg L$, $R=r-(yy'+zz')/r+O(L^2/r)$ and $R^{-1}=r^{-1}[1+O(L/r)]$. The additional condition $r\gg\omega L^2/c$ makes the omitted phase small, so with the printed [Fourier transform](../../../../../fourier-transform.md) convention

$$
\boxed{\widetilde p\simeq-\frac{\rho\omega^2}{2\pi r}e^{i\omega(t-r/c)}\widehat f(m,n),
\quad m=-\frac{\omega y}{rc},\quad n=-\frac{\omega z}{rc}.}
$$

The minus signs in $m,n$ arise because the outgoing phase contributes $+i\omega(yy'+zz')/(rc)$.

For the rectangle the two integrals factor, giving

$$
\boxed{\widehat f(m,n)=\frac{4\sin(am)\sin(bn)}{mn}
=4ab\,\operatorname{sinc}(am)\operatorname{sinc}(bn),}
$$

where $\operatorname{sinc}u=\sin u/u$ and its zero-argument limit is one. If $k=\omega/c$, $kb\ll1$ implies $|bn|\leq kb\ll1$, so the $z$-direction factor is nearly one throughout the radiation hemisphere. With $ka$ of order one the $y$-direction factor varies appreciably: the long dimension gives stronger directivity in that angular direction, while the short dimension radiates broadly. The forward amplitude is proportional to the area $4ab$. Nulls have $ka\,y/r$ equal to nonzero integer multiples of $\pi$ when those values are physically accessible; order-one $ka$ does not automatically imply that the first null lies in the hemisphere.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
