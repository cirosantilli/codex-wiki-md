<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

For a localized charge and current distribution, take the retarded vector potential

$$
A(x,t)=\frac{\mu_0}{4\pi}
\int\frac{J(x',t-|x-x'|/c)}{|x-x'|}\,d^3x'.
$$

Let $R=|x|$, $n=x/R$, and $t_R=t-R/c$. If the source size is much smaller than both $R$ and the characteristic radiation wavelength, the leading dipole term is

$$
A(x,t)\simeq\frac{\mu_0}{4\pi R}\int J(x',t_R)\,d^3x'
=\frac{\mu_0}{4\pi R}\dot p(t_R),
$$

where the last identity follows from charge conservation.

Keeping only the $1/R$ terms in the [radiation zone](../../../../../radiation-zone.md) gives the transverse fields

$$
E_{\rm rad}
=\frac{\mu_0}{4\pi R}n\times(n\times\ddot p(t_R)),
\qquad
B_{\rm rad}=\frac1c n\times E_{\rm rad}.
$$

The radial [Poynting vector](../../../../../poynting-vector.md) therefore yields

$$
\frac{d\mathcal P}{d\Omega}
=\frac{\mu_0}{16\pi^2c}
|n\times\ddot p(t_R)|^2.
$$

Using

$$
\int n_i n_j\,d\Omega=\frac{4\pi}{3}\delta_{ij}
$$

or equivalently $\int\sin^2\theta\,d\Omega=8\pi/3$, we recover the [electric dipole radiation](../../../../../electric-dipole-radiation.md) formula

$$
\boxed{\mathcal P\simeq
\frac{\mu_0}{6\pi c}|\ddot p(t-R/c)|^2}.
$$

This requires a localized, nonrelativistic source of size $d\ll\lambda$, observation distance $R\gg d$ and $R\gg\lambda$, and neglect of higher multipoles and faster-decaying near fields.

For the pulsar, write its magnetic dipole moment as $m(t)$ to distinguish it from the electric dipole above. The [magnetic dipole radiation](../../../../../magnetic-dipole-radiation.md) formula differs by a factor $c^{-2}$:

$$
\mathcal P=\frac{\mu_0}{6\pi c^3}|\ddot m|^2.
$$

Here

$$
\ddot m(t)=-p_0\Omega^2\sin\alpha
[\cos(\Omega t)\widehat x+\sin(\Omega t)\widehat y],
$$

and hence

$$
\boxed{\mathcal P=C\Omega^4,
\qquad
C=\frac{\mu_0p_0^2\sin^2\alpha}{6\pi c^3}}.
$$

On the slow spin-down timescale, energy conservation gives the [magnetic-dipole spin-down](../../../../../magnetic-dipole-spin-down.md) equation

$$
I\Omega\dot\Omega=-C\Omega^4,
$$

so

$$
\frac1{\Omega(t)^2}=\frac1{\Omega_0^2}+\frac{2C}{I}t.
$$

Half of the initial rotational energy remains when $\Omega=\Omega_0/\sqrt2$. Therefore

$$
t_{1/2}=\frac{I}{2C\Omega_0^2}
=\boxed{\frac{6\pi M\mathcal R^2c^3}
{5\mu_0p_0^2\Omega_0^2\sin^2\alpha}},
$$

where $I=2M\mathcal R^2/5$. Since $E_0=I\Omega_0^2/2$, the equivalent expression is

$$
\boxed{t_{1/2}=\frac{6\pi M^2\mathcal R^4c^3}
{25\mu_0p_0^2E_0\sin^2\alpha}}.
$$

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
