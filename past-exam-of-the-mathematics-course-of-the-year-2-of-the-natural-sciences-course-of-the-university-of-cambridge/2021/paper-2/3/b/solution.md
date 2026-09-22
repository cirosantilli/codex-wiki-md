<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $C=A\sqrt{\pi/(2k)}$, so the radial field is $\Phi=C e^{-kr}/r$. Integrate its equation over a ball of radius $\epsilon$ centred at the source. The [divergence theorem](../../../../../divergence-theorem.md) gives

$$
4\pi\epsilon^2\Phi'(\epsilon)-k^2\int_{r<\epsilon}\Phi\,dV=1.
$$

The second term is $4\pi k^2C\int_0^\epsilon re^{-kr}dr=O(\epsilon^2)$ and vanishes in the limit. Meanwhile

$$
4\pi\epsilon^2\Phi'(\epsilon)=-4\pi C(1+k\epsilon)e^{-k\epsilon}\longrightarrow-4\pi C.
$$

Thus

$$
\boxed{C=-\frac1{4\pi},\qquad A=-\frac1{4\pi}\sqrt{\frac{2k}{\pi}},\qquad\Phi(r)=-\frac{e^{-kr}}{4\pi r}.}
$$

The minus sign follows from the convention $(\Delta-k^2)\Phi=\delta^{(3)}$, opposite to the positive [static Yukawa Green function](../../../../../static-yukawa-green-function.md) for $-\Delta+k^2$. For arbitrary real $k$, replace it in the exponential by $|k|$ to select decay at infinity. The $k=0$ limit is $-1/(4\pi r)$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
