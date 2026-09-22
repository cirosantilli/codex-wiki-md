<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a$ be a characteristic crack depth and $Y$ its geometry factor. A simple fast-fracture condition is

$$
K_I=Y\sigma\sqrt{\pi a}=K_{IC},\qquad
 a_c=\frac1\pi\left(\frac{K_{IC}}{Y\sigma}\right)^2.
$$

The crack should penetrate a wall of thickness $t$ before reaching the critical size, so the simplified [leak-before-break criterion](../../../../../leak-before-break-criterion.md) is $t<a_c$, with appropriate geometry and stable-through-wall-crack assumptions.

**The conventional material-based maximum thickness uses the yield [stress](../../../../../stress.md) as a conservative limiting operating [stress](../../../../../stress.md)**:

$$
\boxed{t<t_{\max}^{(\sigma_y)}=
\frac1\pi\left(\frac{K_{IC}}{Y\sigma_y}\right)^2.}
$$

It ensures that the depth required for penetration is subcritical even at the stated limiting [stress](../../../../../stress.md). Geometrical factors depend on crack shape and orientation; this is an educational screening estimate rather than a full crack-growth or leak-detection analysis. The handbook's fracture formula uses the same stress-intensity and geometry-factor convention.[2011 edition revised2019, printed p.6, Fast Fracture; this confirms the formula convention, not the exact2018NST supplied values](../../../../../materials-data-book-by-cambridge-university-engineering-department.md)

There is an important distinction if the actual pressure and radius are fixed while thickness varies. Substituting $\sigma=Pr/t$ at penetration $a=t$ gives

$$
K_I(t)=YPr\sqrt{\frac\pi t},
\qquad
\boxed{t>\pi\left(\frac{YPr}{K_{IC}}\right)^2.}
$$

That is a **lower**, not upper, bound on thickness under the fixed-pressure model. Yield avoidance additionally requires $t\gtrsim Pr/\sigma_y$. It would be inconsistent to derive the fixed-pressure expression and call it a maximum. The standard maximum quoted above answers a different, yield-limited material-selection comparison.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the materials science course of the University of Cambridge](../../../../split.md)
6. [Materials science course of the University of Cambridge](../../../../../materials-science-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
