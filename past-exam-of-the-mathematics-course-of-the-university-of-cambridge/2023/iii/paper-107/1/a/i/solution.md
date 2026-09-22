<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $x\in\Omega$ and $R<\operatorname{dist}(x,\partial\Omega)$. The [mean value property for harmonic functions](../../../../../../../mean-value-property-for-harmonic-functions.md) is

$$
u(x)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}u\,dS
=\frac1{|B_r|}\int_{B_r(x)}u\,dy
\qquad(0<r\leq R).
$$

To prove the spherical identity, translate $x$ to the origin and put $F(r)=|S^{n-1}|^{-1}\int_{S^{n-1}}u(r\theta)\,dS_\theta$. The [divergence theorem](../../../../../../../divergence-theorem.md) gives

$$
F'(r)=\frac1{|S^{n-1}|r^{n-1}}\int_{B_r}\Delta u\,dy=0.
$$

**Hence $F(r)=\lim_{s\downarrow0}F(s)=u(0)$. Integrating the spherical identity in polar coordinates gives the ball identity.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
