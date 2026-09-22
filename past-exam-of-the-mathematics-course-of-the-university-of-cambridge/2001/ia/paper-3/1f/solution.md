<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Put $t=\operatorname{tr}A=a+d$ and $\delta=\det A=ad-bc$. Direct [matrix](../../../../../matrix.md) multiplication gives the two-dimensional [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) identity $A^2-tA+\delta I=0$. If $A^2=0$, [determinant](../../../../../determinant.md) multiplicativity gives $\delta^2=0$, hence $\delta=0$. The identity then says $tA=0$. If $A=0$, its [trace](../../../../../matrix-trace.md) is zero; otherwise a nonzero entry forces $t=0$. Thus $d=-a$ and $bc=ad=-a^2$.

Conversely, those two scalar relations give $t=\delta=0$, so the same [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) identity implies $A^2=0$. Therefore

$$
\boxed{A^2=0\iff d=-a\text{ and }bc=-a^2.}
$$

This is the [square-zero criterion for a two-by-two matrix](../../../../../square-zero-criterion-for-a-two-by-two-matrix.md). If $A^3=0$, [determinant](../../../../../determinant.md) multiplicativity first gives $\delta^3=0$, hence $\delta=0$. Now $A^2=tA$ and $A^3=t^2A$. Either $A=0$, or a nonzero entry gives $t^2=0$ and hence $t=0$; in both cases $A^2=0$. The converse follows by multiplying $A^2=0$ by $A$. Consequently **$A^3=0\iff A^2=0$**. A nonzero [nilpotent matrix](../../../../../nilpotent-matrix.md) of this size therefore has nilpotency index two.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
