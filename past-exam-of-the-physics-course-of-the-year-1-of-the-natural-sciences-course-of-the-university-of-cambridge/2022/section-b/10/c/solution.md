<h1 id="section-b/10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Read the original diagram as a clockwise arc carrying [electric current](../../../../../electric-current.md) from its upper endpoint to its lower endpoint, with tangent semi-infinite leads extending to the right. Their crossing is insulated, so there is no extra junction. Choose $+z$ out of the page. At the centre the arc produces a negative axial [magnetic field](../../../../../magnetic-field-split.md), and each straight lead a positive one, by the [right-hand rule](../../../../../right-hand-rule.md).

For the arc, every element is at distance $R$, with $d\mathbf l$ perpendicular to its displacement to the centre. The [Biot-Savart law](../../../../../biot-savart-law.md) therefore gives

$$
B_{z,\rm arc}=-\frac{\mu_0I}{4\pi R}\int_{-\theta/2}^{\theta/2}d\phi=-\frac{\mu_0I\theta}{4\pi R}.
$$

For each straight lead, write $s\ge0$ for distance along the tangent measured from its endpoint. Its perpendicular distance from the centre is $R$, so

$$
B_{z,\rm lead}=\frac{\mu_0I}{4\pi}\int_0^\infty\frac{R\,ds}{(R^2+s^2)^{3/2}}=\frac{\mu_0I}{4\pi R}.
$$

The integral equals $1/R$ because an [antiderivative](../../../../../antiderivative.md) is $s/[R\sqrt{R^2+s^2}]$. Adding both leads and the arc,

$$
B_z(0)=\frac{\mu_0I}{4\pi R}(2-\theta),\qquad\boxed{\theta=2\,\mathrm{rad}\simeq114.6^\circ.}
$$

Using the full infinite-wire [magnetic field](../../../../../magnetic-field-split.md) for either lead would incorrectly double its contribution.

## ↑ Ancestors (13)

1. [C](../c.md)
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
