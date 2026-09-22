<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the speed as $v=\sqrt{\dot x^2+\dot y^2}>0$ and take

$$
\mathcal L=\frac12(x\dot y-y\dot x)+\lambda v.
$$

The two [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are

$$
\boxed{\dot y-\lambda\frac d{dt}\left(\frac{\dot x}{v}\right)=0,\qquad
-\dot x-\lambda\frac d{dt}\left(\frac{\dot y}{v}\right)=0.}
$$

For example $\mathcal L_x=\dot y/2$ and $\mathcal L_{\dot x}=-y/2+\lambda\dot x/v$, yielding the first equation. Integrating once gives constants $c_1,c_2$ with $\lambda\dot x/v=y+c_1$ and $\lambda\dot y/v=-x+c_2$. The case $\lambda=0$ would force both velocities to vanish, contrary to a regular curve. Squaring and adding therefore gives

$$
\boxed{(x-c_2)^2+(y+c_1)^2=\lambda^2.}
$$

Thus every regular stationary curve is a circle, whose center is set by the integration constants. A simple closed traversal of length $L$ has radius $L/(2\pi)$ and positive enclosed area $L^2/(4\pi)$. The [planar isoperimetric inequality](../../../../../planar-isoperimetric-inequality.md) proves that this stationary candidate is the global maximum; the necessary variational equations alone would not prove that inequality. The [stationary curves of the planar isoperimetric problem](../../../../../stationary-curves-of-the-planar-isoperimetric-problem.md) give this argument independently of the chosen parametrization.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
