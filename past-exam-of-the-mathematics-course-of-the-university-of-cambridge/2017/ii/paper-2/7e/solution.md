<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The given [Euler product for the gamma function](../../../../../euler-product-for-the-gamma-function.md) has the finite approximants

$$
\Gamma_m(z)=\frac{m!(m+1)^z}{z(z+1)\cdots(z+m)},\qquad\Gamma_m(z)\longrightarrow\Gamma(z)
$$

away from the poles. Split the denominator of $\Gamma_{2m+1}(2z)$ into even and odd factors. The resulting exact identity is

$$
\frac{\Gamma_{2m+1}(2z)}{2^{2z}\Gamma_m(z)\Gamma_m(z+\tfrac12)}
=\frac{(2m+1)!}{2^{2m+2}(m!)^2\sqrt{m+1}}.
$$

The right side does not depend on $z$, so its [limit](../../../../../limit-of-a-function.md) is a constant $C$. Evaluate the ratio at $z=1/2$: $\Gamma(1)=1$, and the [gamma reflection formula](../../../../../gamma-reflection-formula.md), together with positivity on the positive real axis, gives $\Gamma(1/2)=\sqrt\pi$. Hence

$$
\boxed{C=\frac1{2\sqrt\pi},\qquad\Gamma(2z)=\frac{2^{2z-1}}{\sqrt\pi}\Gamma(z)\Gamma(z+\tfrac12).}
$$

This is the [gamma duplication formula](../../../../../gamma-duplication-formula.md). The argument first applies where the factors are finite; the identity then holds as an identity of [meromorphic functions](../../../../../meromorphic-function.md), with values at poles interpreted accordingly.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
