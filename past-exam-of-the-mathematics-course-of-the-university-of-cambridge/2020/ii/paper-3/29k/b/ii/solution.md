<h1 id="29k/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the interior of the support $b<m$, differentiating the [joint distribution of Brownian motion and its running maximum](../../../../../../../joint-distribution-of-brownian-motion-and-its-running-maximum.md) gives the [joint probability density](../../../../../../../joint-probability-density.md)

$$
f_{B_t,M_t}(b,m)
=\frac{2(2m-b)}{\sqrt{2\pi}\,t^{3/2}}
\exp\!\left(-\frac{(2m-b)^2}{2t}\right).
$$

Make the [change-of-variables formula for a probability density](../../../../../../../change-of-variables-formula-for-a-probability-density.md) $y=m$ and $z=m-b$. Its inverse is $m=y$, $b=y-z$, and its [Jacobian determinant](../../../../../../../jacobian-determinant.md) has absolute value one. Since $2m-b=y+z$, for $y,z\geq0$ this yields

$$
\boxed{
f_{M_t,Z_t}(y,z)
=\frac{2(y+z)}{\sqrt{2\pi t}\,t}
e^{-(y+z)^2/(2t)}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [29K](../../../29k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
