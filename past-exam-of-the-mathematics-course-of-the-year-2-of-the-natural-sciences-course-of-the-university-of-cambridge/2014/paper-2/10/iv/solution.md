<h1 id="10/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write the lower block of $T(a)$ as $B=\left(\begin{smallmatrix}0&b\\c&0\end{smallmatrix}\right)$. Then

$$
B^2=bcI_2,\qquad T(a)^2=\operatorname{diag}(1,bc,bc),\qquad T(a)^4=\operatorname{diag}(1,(bc)^2,(bc)^2).
$$

A representation of $C_4$ must satisfy its defining relation $T(a)^4=I_3$, so $(bc)^2=1$. For real $b,c$, this means $bc=1$ or $bc=-1$; it also ensures invertibility.

If $bc=-1$, then $T(a)^2\ne I_3$ while $T(a)^4=I_3$. The image of the generator has order four, so its four powers are distinct and the representation is faithful. If $bc=1$, then $T(a)^2=I_3$ but $T(a)\ne I_3$, since the lower block has zero diagonal. The image has order two and the kernel is $\{I,a^2\}$. Hence

$$
\boxed{\text{faithful exactly when }bc=-1;\qquad\text{unfaithful representation exactly when }bc=1.}
$$

For other values there is **no representation of $C_4$**, rather than an additional unfaithful case; in particular $bc=0$ would make the assigned matrix singular. These conclusions are the [faithfulness criterion for a block representation of the cyclic group of order four](../../../../../faithfulness-criterion-for-a-block-representation-of-the-cyclic-group-of-order-four.md). There is no requirement that the proposed representation be orthogonal, so no separate conditions $|b|=|c|=1$ should be imposed.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
