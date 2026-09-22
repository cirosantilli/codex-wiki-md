<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

Multiplication by $(1-x^2)^{-1/2}$ puts the equation in [Sturm-Liouville theory](../../../../../sturm-liouville-theory.md) form:

$$
\boxed{
\frac d{dx}\left(\sqrt{1-x^2}\,T_n'\right)
+\frac{n^2}{\sqrt{1-x^2}}T_n=0}.
$$

Multiply the equations for $T_n,T_m$ by $T_m,T_n$, subtract and integrate. The boundary term vanishes because $\sqrt{1-x^2}=0$ at both endpoints and the [polynomial](../../../../../polynomial-split.md) [derivatives](../../../../../derivative.md) are bounded. Therefore, for $n^2\ne m^2$,

$$
\boxed{
\int_{-1}^1\frac{T_n(x)T_m(x)}{\sqrt{1-x^2}}\,dx=0}.
$$

This is the usual [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) orthogonality.

Differentiating the original equation and writing $U_n=T_n'$ gives

$$
\boxed{(1-x^2)U_n''-3xU_n'+(n^2-1)U_n=0}.
$$

Its self-adjoint form is

$$
\boxed{
\frac d{dx}\left((1-x^2)^{3/2}U_n'\right)
+(n^2-1)\sqrt{1-x^2}\,U_n=0}.
$$

The same subtraction argument now yields, for $n^2\ne m^2$,

$$
\boxed{
\int_{-1}^1U_n(x)U_m(x)\sqrt{1-x^2}\,dx=0}.
$$

These two relations form the [Chebyshev derivative Sturm-Liouville pair](../../../../../chebyshev-derivative-sturm-liouville-pair.md).

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
