<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After integration by parts, the quadratic action is

$$
S_0[x]=-\frac12\int dt\,x(t)(\partial_t^2+\omega^2)x(t).
$$

With the pole prescription appropriate to the conventions in the question, its inverse kernel is

$$
D(t)=\int\frac{dE}{2\pi}\frac{i\,e^{-iEt}}{\omega^2-E^2-i\epsilon}.
$$

For $t>0$ close the [contour](../../../../../../contour-integration.md) in the lower half-plane and for $t<0$ close it in the upper half-plane. The enclosed pole in each case gives

$$
D(t-t')=\frac1{2\omega}e^{i\omega|t-t'|},
$$

which equivalently satisfies $(\partial_t^2+\omega^2)D(t)=i\delta(t)$.

The source-dependent [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) is evaluated by translating the integration variable by the classical sourced solution. Completing the square gives

$$
Z_0[J]=Z_0[0]\exp\left[
-\frac12\int dt\,dt'\,J(t)D(t-t')J(t')
\right].
$$

Changes in the sign of the source term or of the path-integral phase move factors of $i$ between $D$ and the exponent but leave the contraction rules equivalent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
