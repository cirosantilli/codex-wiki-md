<h1 id="14e/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $\widehat u_0(k)=\widehat u(k,0)$ and retain the left-to-right orientation of $L$. Substituting the previous relation into the deformed inverse [Fourier transform](../../../../../../fourier-transform.md) gives the data-only representation

$$
\boxed{\begin{aligned}
u(x,t)={}&\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}\widehat u_0(k)\,dk\\
&-\frac1{2\pi}\int_L e^{ikx-\omega(k)t}\widehat u_0(-k+i\beta)\,dk\\
&-\frac1{2\pi}\int_L e^{ikx}(2ik+\beta)f_0(\omega(k),t)\,dk.
\end{aligned}}
$$

The formally remaining integral is $\int_L e^{ikx}\widehat u(-k+i\beta,t)\,dk$. Above $L$, its reflected argument lies strictly in the lower half-plane, where the transform is analytic. At large radius, $L$ approaches the rays of angles $\pi/4$ and $3\pi/4$. Close it by the upper arc between these rays. Along that arc $\operatorname{Im}k$ is bounded below by a positive multiple of its radius, whereas the reflected transform is bounded by $\int_0^\infty|u(s,t)|\,ds$. Thus the arc integral is bounded by a constant times $R e^{-cRx}$ and tends to zero for $x>0$. There are no enclosed singularities, so [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) proves

$$
\int_L e^{ikx}\widehat u(-k+i\beta,t)\,dk=0.
$$

This is the needed closure argument; it does not assume the unknown transform vanishes. The representation holds for smooth decaying compatible data, and extends to weaker data by the usual limiting heat-kernel interpretation.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
