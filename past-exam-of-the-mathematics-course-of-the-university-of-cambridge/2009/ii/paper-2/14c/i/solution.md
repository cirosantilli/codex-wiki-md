<h1 id="14c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the half-line transform $\widehat u(k,t)=\int_0^\infty e^{-ikx}u(x,t)\,dx$ and let $g_j(t)=\partial_x^j u(0,t)$. Integrating the [heat equation](../../../../../../heat-equation.md) twice by parts gives

$$
e^{k^2t}\widehat u(k,t)=\widehat u_0(k)-\widetilde g_1(k^2,t)-ik\widetilde g_0(k^2,t),\qquad
\widetilde g_j(k^2,t)=\int_0^te^{k^2s}g_j(s)\,ds.
$$

Here $\widehat u_0(k)=(1+ik)^{-2}$ and

$$
\widetilde g_0(k^2,t)=\frac{e^{k^2t}(k^2\sin t-\cos t)+1}{k^4+1},
$$

with removable singularities at the apparent denominator zeros. Let $D^+=\{\operatorname{Im}k>0,\operatorname{Re}k^2<0\}$, and orient its boundary from infinity on the $3\pi/4$ ray to zero and then out on the $\pi/4$ ray. Transform inversion and [contour deformation](../../../../../../contour-deformation.md) give

$$
\boxed{u(x,t)=\frac1{2\pi}\int_{\mathbb R}\frac{e^{ikx-k^2t}}{(1+ik)^2}\,dk
-\frac1{2\pi}\int_{\partial D^+}e^{ikx-k^2t}\left[\frac1{(1-ik)^2}+2ik\widetilde g_0(k^2,t)\right]dk.}
$$

To eliminate the unknown boundary [derivative](../../../../../../derivative.md), evaluate the transform identity at $-k$: $\widetilde g_1=\widehat u_0(-k)+ik\widetilde g_0-e^{k^2t}\widehat u(-k,t)$. The resulting extra [contour integral](../../../../../../contour-integral.md) of $e^{ikx}\widehat u(-k,t)$ vanishes by analyticity and decay in the upper half-plane. This proves that the boxed expression involves only the prescribed data. It is intended for $x,t>0$, with boundary and initial values obtained as limits.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14C](../../14c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
