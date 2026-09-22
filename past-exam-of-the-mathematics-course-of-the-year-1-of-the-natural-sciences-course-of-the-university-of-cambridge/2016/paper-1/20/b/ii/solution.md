<h1 id="20/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The integrand field is exactly the [curl](../../../../../../curl.md) computed in part (a), so use its [polynomial](../../../../../../polynomial-split.md) [vector potential](../../../../../../vector-potential.md) $\mathbf G=(z^3,x^3,y^3)/3$. The upper cap meets the plane $z=0$ in an [ellipse](../../../../../../ellipse.md). Since the parameters are only assumed nonzero, set $a_0=|a|$ and $b_0=|b|$ to use positive semiaxes. Its correctly oriented boundary is

$$
\mathbf r(t)=(a_0\cos t,b_0\sin t,0),\qquad0\leq t\leq2\pi.
$$

On that boundary, $G_x=0$ and $dz=0$, so only $G_y\,dy=x^3dy/3$ contributes. The [Stokes theorem](../../../../../../stokes-theorem.md) therefore gives

$$
\begin{aligned}
A&=\oint_C\mathbf G\cdot d\mathbf r
=\frac13\int_0^{2\pi}(a_0\cos t)^3(b_0\cos t)dt\\
&=\frac{a_0^3b_0}{3}\int_0^{2\pi}\cos^4t\,dt
=\frac{a_0^3b_0}{3}\frac{3\pi}{4}.
\end{aligned}
$$

The last integral follows by expanding $\cos^4t=(3+4\cos2t+\cos4t)/8$. Thus

$$
\boxed{A=\frac\pi4|a|^3|b|=\frac\pi4a^2|ab|.}
$$

The result is independent of $c$. A sign check uses the [divergence theorem](../../../../../../divergence-theorem.md): closing the cap with its base disk adds outward normal $-\widehat{\mathbf z}$ there. Since $\boldsymbol\nabla\cdot\mathbf F=0$, the cap [flux](../../../../../../flux.md) equals $\int_{\rm disk}x^2\,dx\,dy>0$, consistent with the boxed expression and its absolute values.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [20](../../../20.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
