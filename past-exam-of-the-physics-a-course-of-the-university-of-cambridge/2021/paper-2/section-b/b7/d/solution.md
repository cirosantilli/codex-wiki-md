<h1 id="section-b/b7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the source remain at $(0,0,-p)$ and let the observation point be $(X,Y,q)$. The [paraxial approximation](../../../../../../paraxial-approximation.md) to the source-to-aperture-to-observer [optical path length](../../../../../../optical-path-length.md) is

$$
p+q+\frac{x^2+y^2}{2p}+\frac{(X-x)^2+(Y-y)^2}{2q}.
$$

Completing the squares gives

$$
p+q+\frac{X^2+Y^2}{2(p+q)}
+\frac{(x-x_0)^2+(y-y_0)^2}{2R_{\rm eff}},\qquad
x_0=\frac{pX}{p+q},\quad y_0=\frac{pY}{p+q}.
$$

The point $(x_0,y_0)$ is where the straight source-observer line intersects the aperture. Define the four dimensionless edge positions

$$
u_{x,\pm}=\sqrt{\frac{2}{\lambda R_{\rm eff}}}\left(\pm\frac d2-x_0\right),\qquad
u_{y,\pm}=\sqrt{\frac{2}{\lambda R_{\rm eff}}}\left(\pm\frac d2-y_0\right).
$$

On the [Cornu spiral](../../../../../../euler-spiral.md) $F(u)=C(u)+iS(u)$, draw the directed chord from $F(u_{x,-})$ to $F(u_{x,+})$, and a second directed chord from $F(u_{y,-})$ to $F(u_{y,+})$. Denote their complex differences by $D_x$ and $D_y$. The [complex amplitude](../../../../../../complex-amplitude.md) is proportional to their product: multiply their lengths and add their arguments, including the common propagation [phase factor](../../../../../../phase-factor.md).

More explicitly, normalize by the unobscured field $\psi_0(X,Y)$ at this same observation point. The constant [wave phase](../../../../../../phase-waves.md) from completing the square is then already included in $\psi_0$, and

$$
\boxed{\frac{\psi(X,Y)}{\psi_0(X,Y)}=\frac{D_xD_y}{2i},\qquad
\frac{I(X,Y)}{I_0(X,Y)}=\frac{|D_x|^2|D_y|^2}{4}.}
$$

Each directed chord is a one-dimensional [Fresnel diffraction](../../../../../../fresnel-diffraction.md) factor. One must multiply the two factors, rather than add the chords or use just one chord length for the square aperture. Setting $X=Y=0$ recovers $D_x=D_y=2F(w)$ and the on-axis answer.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
