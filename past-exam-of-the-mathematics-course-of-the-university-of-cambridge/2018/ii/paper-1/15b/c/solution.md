<h1 id="15b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $u=\tanh(\lambda t)=e^{\phi/\phi_0}$. The [hyperbolic cotangent](../../../../../../hyperbolic-cotangent.md) double-angle identity gives

$$
\coth(2\lambda t)=\frac{1+u^2}{2u}
=\cosh\left(\frac{\phi}{\phi_0}\right),
$$

so

$$
\boxed{\
H(\phi)=\lambda\frac{\phi_0^2}{M_{\rm Pl}^2}
\cosh\left(\frac{\phi}{\phi_0}\right)\
}.
$$

Also

$$
\operatorname{csch}^2(2\lambda t)
=\cosh^2\left(\frac{\phi}{\phi_0}\right)-1.
$$

Solving the [Friedmann equation](../../../../../../friedmann-equations.md) for the scalar potential,

$$
c^2V=3M_{\rm Pl}^2H^2-\frac12\dot\phi^2,
$$

therefore gives

$$
\boxed{\
V(\phi)=\frac{2\lambda^2\phi_0^2}{c^2}
\left[
\left(\frac{3\phi_0^2}{2M_{\rm Pl}^2}-1\right)
\cosh^2\left(\frac{\phi}{\phi_0}\right)+1
\right]\
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15B](../../15b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
