<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a smooth $u$ and fixed $y$, the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives, for $0<x<1$,

$$
|u(0,y)|\leq |u(x,y)|+\int_0^1|D_xu(s,y)|\,ds.
$$

Average this inequality over $x\in(0,1)$, use [Holder inequality](../../../../../../holder-inequality.md) on that unit interval, raise to the power $p$, and integrate in $y$. This proves the estimate behind the [W1p trace theorem on a half-space](../../../../../../w1p-trace-theorem-on-a-half-space.md):

$$
\|u(0,\cdot)\|_{L^p(\mathbb R)}
\leq C_p\bigl(\|u\|_{L^p(U)}+\|D_xu\|_{L^p(U)}\bigr)
\leq C_p\|u\|_{W^{1,p}(U)}.
$$

Use the [Sobolev extension operator](../../../../../../sobolev-extension-operator.md) from part d, approximate $Eu$ in $W^{1,p}(\mathbb R^2)$ by smooth functions, and define $Tu$ as the $L^p(\mathbb R)$ limit of their restrictions to $x=0$. The trace inequality makes this limit independent of the approximation and proves that

$$
T:W^{1,p}(U)\longrightarrow L^p(\mathbb R)
$$

is linear and bounded. For a smooth function that extends continuously to the boundary, $Tu=u|_{\partial U}$, so this is the [trace operator](../../../../../../w1p-trace-theorem-on-a-half-space.md) required.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
