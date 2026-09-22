<h1 id="12/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At height $z$, the [circular sector](../../../../../../circular-sector.md) has [radius](../../../../../../radius.md) $r(z)=Re^{-z/H}$ and [angle](../../../../../../angle.md) $\Theta(z)=2\pi-\pi z/H$. Its [area](../../../../../../surface-area.md) is $\Theta(z)r(z)^2/2$, so slicing by horizontal cross-sections gives the [volume integral](../../../../../../volume-integral.md)

$$
V=\pi R^2\int_0^H\left(1-\frac z{2H}\right)e^{-2z/H}\,dz.
$$

Use the [substitution rule](../../../../../../integration-by-substitution.md) $t=z/H$. Then

$$
V=\pi R^2H\int_0^1(1-t/2)e^{-2t}\,dt.
$$

An [integration by parts](../../../../../../integration-by-parts.md) gives the [antiderivative](../../../../../../antiderivative.md) $(t/4-3/8)e^{-2t}$, whose endpoint difference is $(3-e^{-2})/8$. Therefore

$$
\boxed{V=\frac{\pi R^2H}{8}(3-e^{-2}).}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
