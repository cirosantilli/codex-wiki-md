<h1 id="30a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $r=e^x$, $\epsilon=\hbar/\sqrt{2m}$, $L=l+1/2$, and $\lambda=-|\lambda|$. Since $V(r)=-V_0/r$, the transformed equation has

$$
q(x)=|\lambda|e^{2x}-V_0e^x+\epsilon^2L^2.
$$

The two turning radii $a<b$ are the positive roots of

$$
|\lambda|r^2-V_0r+\epsilon^2L^2
=|\lambda|(r-a)(r-b),
$$

so

$$
a+b=\frac{V_0}{|\lambda|},
\qquad
ab=\frac{\epsilon^2L^2}{|\lambda|}.
$$

Inside the allowed interval,

$$
|q|=|\lambda|(r-a)(b-r),
\qquad dx=\frac{dr}{r}.
$$

The [semiclassical action integral](../../../../../../semiclassical-action-integral.md) is therefore

$$
\begin{aligned}
\frac1\epsilon\int_{x_a}^{x_b}|q(x)|^{1/2}\,dx
&=\frac{\sqrt{|\lambda|}}{\epsilon}
\int_a^b\frac{\sqrt{(r-a)(b-r)}}r\,dr\\
&=\frac{\pi\sqrt{|\lambda|}}{2\epsilon}(\sqrt b-\sqrt a)^2\\
&=\pi\left(\frac{V_0}{2\epsilon\sqrt{|\lambda|}}-L\right).
\end{aligned}
$$

Equating this with $(n+1/2)\pi$ from part (a), and using $L=l+1/2$, gives

$$
\frac{V_0}{2\epsilon\sqrt{|\lambda|}}=n+l+1.
$$

Since $\epsilon^2=\hbar^2/(2m)$,

$$
|\lambda|=\frac{V_0^2}{4\epsilon^2(n+l+1)^2}
=\frac{mV_0^2}{2\hbar^2(n+l+1)^2}.
$$

Thus the [Coulomb WKB quantization with the Langer correction](../../../../../../coulomb-wkb-quantization-with-the-langer-correction.md) yields

$$
\boxed{E=\lambda=-\frac{mV_0^2}{2\hbar^2(n+l+1)^2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30A](../../30a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
