<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Orient the three faces outward from the tetrahedron. The two coordinate-plane faces have normals parallel to $-\mathbf e_x$ or $-\mathbf e_y$, so their flux of the [curl](../../../../../curl.md) is zero. On the inclined face $z=1-x-y$, its upward vector area is $(1,1,1)\,dx\,dy$, with $x,y\geq0$, $x+y\leq1$. Thus the direct [surface integral](../../../../../surface-integral.md) is

$$
\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS=\int_0^1\int_0^{1-x}1\,dy\,dx=\frac12.
$$

This surface induces the counterclockwise boundary $O\to X\to Y\to O$ viewed from above, where $X=(1,0,0)$ and $Y=(0,1,0)$. At $z=0$, $\mathbf A=(2x-y,0,0)$. On $OX$, take $(x,y)=(t,0)$, giving integral $\int_0^12t\,dt=1$. On $XY$, take $(x,y)=(1-t,t)$, giving $\int_0^1(-2+3t)dt=-1/2$. On $YO$, $dx=0$ and the integral vanishes. Therefore

$$
\boxed{\oint_C\mathbf A\cdot d\mathbf r=1-\frac12+0=\frac12=\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS.}
$$

Both sides have been calculated directly, verifying the [Stokes theorem](../../../../../stokes-theorem.md) with consistent orientations.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
