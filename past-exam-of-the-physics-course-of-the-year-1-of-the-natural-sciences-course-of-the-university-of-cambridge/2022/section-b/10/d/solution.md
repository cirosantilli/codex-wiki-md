<h1 id="section-b/10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

To calculate [magnetic-field cancellation of an arc and tangent leads](../../../../../magnetic-field-cancellation-of-an-arc-and-tangent-leads.md) away from the plane, put $a^2=R^2+h^2$. Each point on the arc is distance $a$ from $(0,0,h)$, and the axial component of $d\mathbf l\times\mathbf s$ still has magnitude $R^2d\phi$. Thus its axial [magnetic field](../../../../../magnetic-field-split.md) is

$$
\boxed{B_{z,\rm arc}(h)=-\frac{\mu_0I\theta R^2}{4\pi(R^2+h^2)^{3/2}}.}
$$

For either tangent lead the axial numerator remains $R\,ds$, while the cubed distance is $(R^2+h^2+s^2)^{3/2}$. Hence

$$
\boxed{B_{z,\rm lead}(h)=\frac{\mu_0I}{4\pi}\int_0^\infty\frac{R\,ds}{(a^2+s^2)^{3/2}}=\frac{\mu_0IR}{4\pi(R^2+h^2)}.}
$$

Adding both leads gives

$$
\boxed{B_z(h)=\frac{\mu_0I}{4\pi R}\left[\frac2{1+(h/R)^2}-\frac{\theta}{[1+(h/R)^2]^{3/2}}\right].}
$$

For $\epsilon=h/R\ll1$, a [binomial series](../../../../../binomial-series.md) yields

$$
B_z(h)=\frac{\mu_0I}{4\pi R}\left[(2-\theta)+\left(-2+\frac32\theta\right)\epsilon^2+O(\epsilon^4)\right].
$$

The exact condition for cancellation of the axial component is

$$
\theta(h)=2\sqrt{1+\epsilon^2},\qquad\boxed{\theta(h)=2+\frac{h^2}{R^2}+O\!\left(\frac{h^4}{R^4}\right)\quad\text{in radians}.}
$$

For example, keeping $\theta=2$ would leave a small positive axial [magnetic field](../../../../../magnetic-field-split.md) proportional to $h^2/R^2$. Both contributions weaken with height, but the arc factor is $(1+\epsilon^2)^{-3/2}$ whereas the lead factor is $(1+\epsilon^2)^{-1}$. The arc therefore loses a greater fraction of its axial [magnetic field](../../../../../magnetic-field-split.md). Increasing its angle compensates for this loss. Physically, the arc is all at the same finite radius, whereas distant elements of the semi-infinite leads undergo a smaller fractional change in distance on moving a little out of the plane.

The cancellation here concerns $B_z$ only; off the plane it does not assert that every component of the [magnetic field](../../../../../magnetic-field-split.md) vanishes. The small-height result also stays within the tangent-lead geometry shown in the original paper.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [10](../../10.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
