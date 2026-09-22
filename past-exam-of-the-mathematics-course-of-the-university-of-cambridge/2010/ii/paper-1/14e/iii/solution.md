<h1 id="14e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $k=a+ib$, $\operatorname{Re}\omega=a^2-b^2+\beta b$. The upper contour is therefore the graph

$$
\boxed{L:\quad b=\frac{\beta+\sqrt{\beta^2+4a^2}}2,\quad -\infty<a<\infty,}
$$

oriented from left to right. Between the real axis and $L$, $b\geq0$ and $\operatorname{Re}\omega\geq0$. Hence $e^{ikx-\omega(t-s)}$ is bounded by $e^{-bx}$ for $0\leq s\leq t$. The boundary transforms are entire in $k$; with the standard smooth, compatible boundary data, [integration by parts](../../../../../../integration-by-parts.md) in the time integral gives the required polynomial bounds. Closing the intervening sectors and using exponential decay for $x>0$ deforms their real-line integrals onto $L$. Small endpoint truncations, followed by dominated limits, handle the sector boundaries.

For $k'= -k+i\beta$, $\omega(k')=\omega(k)$ and $\operatorname{Im}k'\leq0$ on $L$. Thus the already valid transformed equation at $k'$ says

$$
\widehat u(k',t)=e^{-\omega t}\widehat u(k',0)+ikf_0-f_1.
$$

It eliminates the unknown boundary derivative through

$$
\boxed{f_1=e^{-\omega t}\widehat u(k',0)+ikf_0-\widehat u(k',t).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
