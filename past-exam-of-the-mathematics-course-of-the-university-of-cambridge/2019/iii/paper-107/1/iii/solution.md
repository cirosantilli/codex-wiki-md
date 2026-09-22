<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Radiality gives $\phi_\varepsilon(x-y)=\phi_\varepsilon(y-x)$. Since $\phi_\varepsilon$ is supported in $B(0,\varepsilon)$, the changes of variables $y=x+z$ and then $z=\varepsilon r\omega$ in [spherical coordinates](../../../../../../spherical-coordinate-system.md) give

$$
\begin{aligned}
(u*\phi_\varepsilon)(x)
&=\int_{B(0,\varepsilon)}u(x+z)\varepsilon^{-d}\phi(z/\varepsilon)\,dz\\
&=\boxed{\int_0^1\int_{S^{d-1}}u(x+\varepsilon r\omega)\phi(r\omega)r^{d-1}\,d\omega\,dr.}
\end{aligned}
$$

The restriction $\varepsilon<\operatorname{dist}(x,\partial\Omega)$ ensures that every sampled point remains in $\Omega$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
