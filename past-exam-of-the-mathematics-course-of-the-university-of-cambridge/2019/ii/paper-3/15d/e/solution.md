<h1 id="15d/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Compose the two constructions in part (d) to obtain

$$
U_g=U_{f_2}U_{f_1},
\qquad g(x)=f(x+1)-f(x),
$$

using two queries to $U_f$. For

$$
f(x)=ax^2+bx+c
$$

over $\mathbb Z_3$, the [finite difference](../../../../../../finite-difference-split.md) is

$$
g(x)=a(2x+1)+b=2ax+(a+b).
$$

This is affine with slope $s_g=2a=-a$. Apply the one-query affine procedure from part (c) to the implemented oracle $U_g$. It returns $s_g$ with certainty, after which the fixed classical computation

$$
\boxed{a=2s_g\pmod3}
$$

recovers the quadratic coefficient. Since one use of $U_g$ consists of one use each of $U_{f_1}$ and $U_{f_2}$, the algorithm makes exactly two calls to the original oracle $U_f$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
