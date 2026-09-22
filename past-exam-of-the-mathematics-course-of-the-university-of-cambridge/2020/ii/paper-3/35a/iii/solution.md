<h1 id="35a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md) is

$$
dE=T\,dS-P\,dV,
$$

so, regarding $S$ as a function of $(T,V)$,

$$
\left(\frac{\partial S}{\partial T}\right)_V
=\frac1T\left(\frac{\partial E}{\partial T}\right)_V,
\qquad
\left(\frac{\partial S}{\partial V}\right)_T
=\frac1T\left[
\left(\frac{\partial E}{\partial V}\right)_T+P
\right].
$$

Equality of mixed [partial derivatives](../../../../../../partial-derivative.md) gives the [thermodynamic derivation of blackbody radiation pressure](../../../../../../thermodynamic-derivation-of-blackbody-radiation-pressure.md)

$$
\boxed{
\left(\frac{\partial E}{\partial V}\right)_T
=T\left(\frac{\partial P}{\partial T}\right)_V-P}.
$$

Writing $a=\pi^2/(15\hbar^3c^3)$, we have $E=aVT^4$, and hence

$$
T\frac{dP}{dT}-P=aT^4.
$$

Equivalently, $d(P/T)/dT=aT^2$, so

$$
P=\frac a3T^4+CT.
$$

The condition $P=o(T)$ as $T\to0$ forces $C=0$. Therefore the [radiation pressure](../../../../../../radiation-pressure.md) is

$$
\boxed{P=\frac{\pi^2T^4}{45\hbar^3c^3}
=\frac{E}{3V}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [35A](../../35a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
