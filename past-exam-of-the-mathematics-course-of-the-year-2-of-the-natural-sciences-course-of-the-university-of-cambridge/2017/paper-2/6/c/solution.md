<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [vector triple product](../../../../../vector-triple-product.md) expression from part (a). Put $s=\Omega\cdot x$ and $r^2=x\cdot x$. Since $u=\Omega+\beta x$,

$$
u\cdot u=\Omega^2+2\beta s+\beta^2r^2,\qquad u\cdot\Omega=\Omega^2+\beta s.
$$

Expanding $W=(u\cdot u)\Omega-(u\cdot\Omega)u$ and canceling the zeroth-order terms gives

$$
\boxed{W(x)=\beta\big[(\Omega\cdot x)\Omega-\Omega^2x\big]+\beta^2\big[r^2\Omega-(\Omega\cdot x)x\big].}
$$

The first bracket is odd in $x$ and integrates to zero over the centred ball. With $\alpha=4\pi a^5/15$, the [Cartesian moments of a three-dimensional ball](../../../../../cartesian-moments-of-a-three-dimensional-ball.md) give

$$
\int_Vr^2\,dV=3\alpha,\qquad\int_V(\Omega\cdot x)x_i\,dV=\Omega_j\int_Vx_jx_i\,dV=\alpha\Omega_i.
$$

Therefore

$$
\boxed{\int_VW_i\,dV=2\alpha\beta^2\Omega_i=\frac{8\pi a^5\beta^2}{15}\Omega_i.}
$$

The resulting [vector](../../../../../vector.md) is parallel to $\Omega$, as the rotational symmetry of the centred domain requires.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
