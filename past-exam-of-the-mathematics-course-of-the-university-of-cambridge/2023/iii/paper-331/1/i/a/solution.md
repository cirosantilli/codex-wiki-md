<h1 id="1/i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Rayleigh equation for inviscid shear flow](../../../../../../../rayleigh-equation-for-inviscid-shear-flow.md) as

$$
\phi''-\alpha^2\phi-
\frac{U''}{U-c}\phi=0,
\qquad \phi(0)=\phi(1)=0.
$$

Multiply by $\phi^*$, integrate, and use [integration by parts](../../../../../../../integration-by-parts.md):

$$
\int_0^1(|\phi'|^2+\alpha^2|\phi|^2)\,dz
+\int_0^1\frac{U''(U-c^*)}{|U-c|^2}|\phi|^2\,dz=0.
$$

Its imaginary part is

$$
c_i\int_0^1\frac{U''}{|U-c|^2}|\phi|^2\,dz=0.
$$

For an unstable mode $c_i>0$, the integral can vanish only if $U''$ changes sign somewhere in the flow. Thus the velocity profile must have an inflection point. This is [Rayleigh's inflection-point theorem](../../../../../../../rayleigh-s-inflection-point-theorem.md); it is necessary, not sufficient, for inviscid instability.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [I](../../i.md)
3. [1](../../../1.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
