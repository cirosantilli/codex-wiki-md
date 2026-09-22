<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the [Airy ordinary differential equation](../../../../../airy-ordinary-differential-equation.md) $y''=sy$ to obtain $y^{(3)}=y+sy'$. Combining part (a)'s [derivatives](../../../../../derivative.md) yields

$$
u_t+u_{xxx}=[at^{a-1}+b^{3a}t^{4a}][y(s)+sy'(s)].
$$

To make this vanish for an arbitrary Airy profile, the time powers must agree: $a-1=4a$, giving $a=-1/3$. Their common [coefficient](../../../../../coefficient.md) must then vanish, giving $-1/3+b^{-1}=0$, hence $b=3$. Therefore

$$
\boxed{a=-\frac13,\qquad b=3,\qquad
u(x,t)=t^{-1/3}y\left(\frac{x}{(3t)^{1/3}}\right).}
$$

For $t>0$ the two terms cancel exactly:

$$
u_t=-\frac13t^{-4/3}(y+sy'),\qquad
u_{xxx}=\frac13t^{-4/3}(y+sy').
$$

This is an [Airy similarity solution of the linear dispersive equation](../../../../../airy-similarity-solution-of-the-linear-dispersive-equation.md). The [Airy equation](../../../../../airy-equation.md) here is the linear partial [differential equation](../../../../../differential-equation-split.md) $u_t+u_{xxx}=0$, the reduced equation specified in the question; it is distinct from the profile's [Airy ordinary differential equation](../../../../../airy-ordinary-differential-equation.md). The construction works for every linear combination of its two independent profiles, including zero. No condition at $t=0$ is supplied, and this singular time is excluded. With real cube roots the final formula can also be used separately on $t<0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
