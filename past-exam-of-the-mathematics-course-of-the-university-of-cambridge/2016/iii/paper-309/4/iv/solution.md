<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Take the oscillation to be $z(t)=L\cos\omega t$; a different initial phase does not affect a [period average](../../../../../../period-average.md). In the mass-density normalization of the [quadrupole formula](../../../../../../quadrupole-formula.md), the [second mass moment tensor](../../../../../../second-mass-moment-tensor.md) of the [point mass](../../../../../../point-mass.md) has only $I_{33}=mz^2$ nonzero. Its trace-free [mass quadrupole moment](../../../../../../mass-quadrupole-moment.md) is therefore

$$
Q_{ij}=mL^2\cos^2\omega t\;\operatorname{diag}\left(-\frac13,-\frac13,\frac23\right)_{ij}.
$$

The constant part does not radiate. Since $d^3(\cos^2\omega t)/dt^3=4\omega^3\sin2\omega t$, the [tensor contraction](../../../../../../tensor-contraction.md) is

$$
\dddot Q_{ij}\dddot Q_{ij}
=16m^2L^4\omega^6\sin^2(2\omega t)\left(\frac19+\frac19+\frac49\right)
=\frac{32}{3}m^2L^4\omega^6\sin^2(2\omega t).
$$

Using $\langle\sin^2(2\omega t)\rangle=1/2$ in the [quadrupole formula](../../../../../../quadrupole-formula.md) gives **the averaged positive radiated power**

$$
\boxed{\left\langle\frac{dE_{\rm rad}}{dt}\right\rangle=\frac{16Gm^2L^4\omega^6}{15c^5}.}
$$

The [mass quadrupole moment](../../../../../../mass-quadrupole-moment.md) oscillates at twice the source's [angular frequency](../../../../../../angular-frequency.md), and the source energy loss has the opposite sign. The expression uses the leading slow-motion [weak-field approximation](../../../../../../weak-field-approximation.md), $\omega L\ll c$. With SI [stress-energy tensor](../../../../../../stress-energy-tensor.md) components, the mass-density integrand is $T_{00}/c^2$; the displayed $c^{-5}$ [quadrupole formula](../../../../../../quadrupole-formula.md) uses that mass normalization. This is the point-mass contribution requested by the model: an apparatus maintaining an accelerating mass would also contribute its own [mass quadrupole moment](../../../../../../mass-quadrupole-moment.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
