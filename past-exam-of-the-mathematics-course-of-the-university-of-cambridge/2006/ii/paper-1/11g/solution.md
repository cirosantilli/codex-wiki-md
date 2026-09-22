<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Parametrize the circle by $z=e^{it}$, $0\leq t\leq2\pi$. Choose a continuous argument $\vartheta(t)$ of $\phi(e^{it})$, so $\phi(e^{it})=|\phi(e^{it})|e^{i\vartheta(t)}$. Its [winding number](../../../../../winding-number.md) about zero is

$$
w(\phi)=\frac{\vartheta(2\pi)-\vartheta(0)}{2\pi}\in\mathbb Z.
$$

The two facts proved below determine the requested calculation without needing differentiability or contour [integration](../../../../../integral.md). Put $P(z)=(3z-2)(z-3)(2z+1)$. On $|z|=1$, $|P(z)|\geq1\cdot2\cdot1=2$, so adding one does not change its winding. The first and third factors have winding one, since their constant terms have modulus smaller than their linear terms; the second has winding zero, since its $z$ term has modulus smaller than its constant term. Nonzero constants have winding zero and $z$ has winding one. Thus

$$
\boxed{w(\phi)=1+0+1=2.}
$$

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
