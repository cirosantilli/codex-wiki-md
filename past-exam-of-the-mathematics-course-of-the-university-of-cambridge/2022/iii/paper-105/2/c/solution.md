<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The assumed inequality is equivalent to

$$
J(u):=\lVert Du\rVert_2^2-\gamma\lVert u\rVert_2^2\geq0,
$$

and equality holds at $w$. For $v\in H$ and $t\in\mathbb R$, expand $J(w+tv)\geq0$ and use $J(w)=0$:

$$
0\leq2t\big((Dw,Dv)_2-\gamma(w,v)_2\big)
+t^2\big(\lVert Dv\rVert_2^2-\gamma\lVert v\rVert_2^2\big).
$$

Since this holds for both signs of arbitrarily small $t$, the linear coefficient vanishes:

$$
\int_UDw\cdot Dv=\gamma\int_Uwv
\qquad(v\in H).
$$

Every $v\in H^1(U)$ is a mean-zero function plus a constant. The same identity holds for constants because $\int_Uw=0$, so it holds for all $v\in H^1(U)$. This is precisely the weak formulation of

$$
-\Delta w=\gamma w,
\qquad
\partial_\nu w=0,
\qquad
\int_Uw=0,
$$

where the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) is the natural boundary condition encoded by the weak formulation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
