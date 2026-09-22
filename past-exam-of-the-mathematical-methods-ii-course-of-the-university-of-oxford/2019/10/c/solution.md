<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is a [scalar surface integral](../../../../scalar-surface-integral.md), not an oriented [flux](../../../../flux.md). Split the whole closed [surface](../../../../topological-surface-split.md) into the bottom disc, curved side and tilted top; shared edge curves have zero [surface area](../../../../surface-area.md).

On the bottom, $z=0$ and the integrand is $y$. Its integral over the symmetric disc $x^2+y^2\leq3$ vanishes by oddness:

$$
I_{\mathrm{bottom}}=0.
$$

On the top, $z=4-y$, so $y+z=4$. The graph has $z_x=0$, $z_y=-1$, giving $dS=\sqrt{1+z_x^2+z_y^2}\,dx\,dy=\sqrt2\,dx\,dy$. Hence

$$
I_{\mathrm{top}}=4\sqrt2\,(3\pi)=12\pi\sqrt2.
$$

For the side, let $R=\sqrt3$ and parametrize by $(R\cos\phi,R\sin\phi,z)$, with $0\leq z\leq4-R\sin\phi$. The [surface area element](../../../../surface-area-element.md) is $R\,dz\,d\phi$. Thus

$$
\begin{aligned}
I_{\mathrm{side}}
&=R\int_0^{2\pi}\int_0^{4-R\sin\phi}(R\sin\phi+z)\,dz\,d\phi\\
&=R\int_0^{2\pi}\left[8-\frac{R^2}2\sin^2\phi\right]d\phi\\
&=16\pi R-\frac{\pi R^3}{2}=\frac{29\pi\sqrt3}{2}.
\end{aligned}
$$

Adding all three pieces gives

$$
\boxed{\int_S(y+z)\,dS=\pi\left(12\sqrt2+\frac{29\sqrt3}{2}\right).}
$$

The tilted top remains above the bottom everywhere because $4-y\geq4-\sqrt3>0$. The calculation is an instance of a [scalar surface integral over a cylinder with one tilted cap](../../../../scalar-surface-integral-over-a-cylinder-with-one-tilted-cap.md); reversing a surface orientation would not change any of its terms.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
