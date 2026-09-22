<h1 id="36e/solution">Solution</h1>

↑ **Parent:** [36E](../36e.md)

The [electric-dipole approximation for radiation](../../../../../electric-dipole-approximation-for-radiation.md) requires the source size to be much smaller than the radiation wavelength:

$$
\frac{\omega a}{c}\ll1.
$$

The displayed $1/r$ fields also describe the [radiation zone](../../../../../radiation-zone.md), so the observation point must satisfy $r\gg a$ and $r\gg c/\omega$.

Write $t_r=t-r/c$. The given vector potential and the [time derivative of the electric dipole moment](../../../../../time-derivative-of-the-electric-dipole-moment.md) give

$$
\mathbf A(t,\mathbf x)
\simeq\frac{\mu_0}{4\pi r}\int\mathbf J(t_r,\mathbf x')\,d^3x'
=\frac{\mu_0}{4\pi r}\dot{\mathbf p}(t_r).
$$

When taking the [curl](../../../../../curl.md), differentiating $1/r$ produces a near-field term of order $r^{-2}$, while differentiating the retarded time produces the leading radiation term because $\nabla t_r=-\widehat{\mathbf x}/c$. Hence

$$
\boxed{
\mathbf B=\nabla\times\mathbf A
\simeq-\frac{\mu_0}{4\pi rc}
\widehat{\mathbf x}\times\ddot{\mathbf p}(t_r).}
$$

The assumed electric field $\mathbf E=-c\widehat{\mathbf x}\times\mathbf B$ and the transversality $\widehat{\mathbf x}\cdot\mathbf B=0$ make the [Poynting vector](../../../../../poynting-vector.md)

$$
\mathbf S=\frac1{\mu_0}\mathbf E\times\mathbf B
=\frac{c}{\mu_0}|\mathbf B|^2\widehat{\mathbf x}.
$$

On a sphere of radius $R$, the power through surface element $R^2d\Omega$ is therefore

$$
\boxed{
\frac{dP}{d\Omega}
=R^2\mathbf S\cdot\widehat{\mathbf x}
=\frac{\mu_0}{16\pi^2c}
|\widehat{\mathbf x}\times\ddot{\mathbf p}(t-R/c)|^2.}
$$

Choose the polar axis along $\ddot{\mathbf p}$ and use the [angular distribution of electric dipole radiation](../../../../../angular-distribution-of-electric-dipole-radiation.md), for which $|\widehat{\mathbf x}\times\ddot{\mathbf p}|^2=|\ddot{\mathbf p}|^2\sin^2\theta$. Since $\int\sin^2\theta\,d\Omega=8\pi/3$,

$$
\boxed{
P(t)=\frac{\mu_0}{6\pi c}
|\ddot{\mathbf p}(t-R/c)|^2.}
$$

For the charged particle in [simple harmonic motion](../../../../../simple-harmonic-motion.md),

$$
\mathbf p(t)=qA\sin(\omega t)\mathbf i_x,
\qquad
\ddot{\mathbf p}(t)=-qA\omega^2\sin(\omega t)\mathbf i_x.
$$

Thus

$$
\boxed{
P(t)=\frac{\mu_0q^2A^2\omega^4}{6\pi c}
\sin^2\!\bigl(\omega(t-R/c)\bigr),
\qquad
\langle P\rangle=\frac{\mu_0q^2A^2\omega^4}{12\pi c}.}
$$

Here the [angular frequency](../../../../../angular-frequency.md) obeys $\omega=2\pi/T$, and the average uses $\langle\sin^2\rangle=1/2$. The dipole condition is

$$
\boxed{\frac{A\omega}{c}\ll1.}
$$

Allow the amplitude to vary slowly as radiation removes energy. The mechanical energy is

$$
E=\frac12mA^2\omega^2,
$$

so the [radiation damping of a harmonically oscillating charge](../../../../../radiation-damping-of-a-harmonically-oscillating-charge.md) gives

$$
\frac{dE}{dt}=-\langle P\rangle
=-\frac{\mu_0q^2\omega^2}{6\pi mc}E.
$$

This is [exponential decay](../../../../../exponential-decay.md) with rate $\gamma=\mu_0q^2\omega^2/(6\pi mc)$. Its [half-life](../../../../../half-life.md) is

$$
\boxed{t_{1/2}=\frac{6\pi mc\log2}{\mu_0q^2\omega^2}.}
$$

Finally, the largest particle speed is $v_{\max}=A\omega$. Therefore the dipole condition $A\omega/c\ll1$ itself implies $v_{\max}\ll c$, precisely the [nonrelativistic limit](../../../../../nonrelativistic-limit.md) required by the mechanical energy formula.

## ↑ Ancestors (10)

1. [36E](../36e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
