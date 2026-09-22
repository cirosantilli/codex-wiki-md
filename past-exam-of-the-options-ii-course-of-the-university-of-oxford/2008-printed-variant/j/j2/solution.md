<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

The source-free [Maxwell equations](../../../../maxwell-equations-split.md) in vacuum are

$$
\nabla\cdot E=\nabla\cdot B=0,\qquad \nabla\times E=-\partial_t B,\qquad \nabla\times B=c^{-2}\partial_t E.
$$

Their real and imaginary parts are exactly

$$
\nabla\cdot W=0,\qquad \nabla\times W=(i/c)\partial_t W,\qquad W=E+icB.
$$

Put $\theta=\omega t-K\cdot x$. Differentiating gives $\nabla\cdot W=(\Omega\cdot K)\sin\theta$ and $\nabla\times W=-(\Omega\times K)\sin\theta$, while $(i/c)\partial_tW=-i\omega\Omega\sin\theta/c$. Thus the necessary and sufficient conditions are

$$
\Omega\cdot K=0,\qquad \Omega\times K=i\omega\Omega/c.
$$

Here the complex dot product is bilinear, without [complex conjugation](../../../../complex-conjugation.md). Taking the dot product of the second equation with $\Omega$ gives $\Omega\cdot\Omega=0$. Crossing it with $K$ gives

$$
-|K|^2\Omega=(i\omega/c)^2\Omega,
$$

so, since $\Omega\ne0$, $|K|^2=\omega^2/c^2$. Writing $\Omega=e+icb$, the real conditions are

$$
\boxed{e\cdot K=b\cdot K=e\cdot b=0,\quad |e|=c|b|,\quad K\times e=\omega b,\quad K\times b=-\omega e/c^2}.
$$

Both physical fields are **linearly polarized**: $E=e\cos\theta$ and $B=b\cos\theta$ each oscillate along a fixed real direction. Combining two fields as $E+icB$ does not turn the electric field into a circularly polarized field.

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
3. [2008 printed variant](../../../2008-printed-variant-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
