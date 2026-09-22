<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the observation point as $r\widehat r$, put $q=k_0(\widehat r-\widehat r_0)$, and take $\psi_0(r\widehat r)=e^{ik_0r\widehat r_0\cdot\widehat r}$. For a bounded medium, the [far-field approximation for an outgoing source](../../../../../../far-field-approximation-for-an-outgoing-source.md) uses

$$
|r\widehat r-r'|=r-\widehat r\cdot r'+O(\ell^2/r),\qquad G_0\simeq\frac{e^{ik_0r}}{4\pi r}e^{-ik_0\widehat r\cdot r'}.
$$

For finite-distance accuracy require $r\gg\ell$ and $k_0\ell^2/r\ll1$ as well as being in the radiation region. Define the [Fourier transform](../../../../../../fourier-transform.md) sample $S(q)=\int_DV(r')e^{-iq\cdot r'}\,d^3r'$ and the known factor

$$
B(r,\widehat r)=\frac{e^{ik_0r(1-\widehat r_0\cdot\widehat r)}}{4\pi r}.
$$

Then the required total [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md) and total [Rytov approximation](../../../../../../rytov-approximation.md) are

$$
\boxed{\psi_B(r\widehat r)\simeq e^{ik_0r\widehat r_0\cdot\widehat r}+\frac{e^{ik_0r}}{4\pi r}S(q),\qquad \psi_R(r\widehat r)\simeq e^{ik_0r\widehat r_0\cdot\widehat r}\exp\{B S(q)\}.}
$$

The first [Born approximation](../../../../../../born-approximation.md) [far-field pattern](../../../../../../far-field-pattern.md) is $S(q)/(4\pi)$. In both formulas the incident field is retained; an outgoing scattered term alone would not be a total-field answer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
