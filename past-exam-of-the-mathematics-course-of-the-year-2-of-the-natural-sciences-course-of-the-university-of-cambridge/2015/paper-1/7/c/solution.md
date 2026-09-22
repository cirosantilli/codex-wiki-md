<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $g=u+iv$ and assume its domain is open and connected. If the constant modulus is zero then $g=0$. Otherwise let $u^2+v^2=c^2>0$. Differentiating this identity and using the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) gives

$$
u u_x+v v_x=0,\qquad u u_y+v v_y=-u v_x+v u_x=0.
$$

These are a linear system for $u_x,v_x$ with coefficient [matrix](../../../../../matrix.md) $\begin{pmatrix}u&v\\v&-u\end{pmatrix}$, whose [determinant](../../../../../determinant.md) is $-c^2\neq0$. Therefore $u_x=v_x=0$, and the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) also give $u_y=v_y=0$. It follows that

$$
\boxed{g\text{ is constant on its connected domain}.}
$$

This proves the [constant-modulus holomorphic function](../../../../../constant-modulus-holomorphic-function.md) result directly. On a disconnected domain the same conclusion holds separately on each [connected component](../../../../../connected-component.md), but the constants can differ.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
