<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the interior $\Omega=\{1/2<|x|<2\}$ for the [Sobolev space](../../../../../../sobolev-space-split.md) notation; the closed shell in the PDF specifies its boundary. Put $A(x)=\operatorname{diag}(1,1,g(|x|))$. A [weak solution](../../../../../../weak-solution.md) has zero boundary trace in the sense of the [Sobolev trace theorem](../../../../../../sobolev-trace-theorem.md), equivalently $u\in H_0^1(\Omega)$, and satisfies

$$
\boxed{\int_\Omega\bigl(u_1\varphi_1+u_2\varphi_2+g(|x|)u_3\varphi_3\bigr)\,dx=-\int_\Omega f\varphi\,dx\quad(\varphi\in H_0^1(\Omega)).}
$$

The minus sign is necessary because the operator in the paper is positive divergence, not its negative. One can first test with $C_c^\infty$ functions and then use density in the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md). Smoothness of $g$ makes its restriction to the compact radial interval bounded, so both sides define continuous functionals on this space. Merely belonging to $H^1$ without the zero trace would omit the [boundary condition](../../../../../../boundary-condition.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
