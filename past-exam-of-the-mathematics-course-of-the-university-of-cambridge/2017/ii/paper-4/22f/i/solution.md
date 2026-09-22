<h1 id="22f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $w(\xi)=(1+|\xi|^2)^{s/2}$. The map $U:f\mapsto w\widehat f$ is linear, and $\|U(f+g)\|_2\leq\|Uf\|_2+\|Ug\|_2$ proves the vector-subspace claim. The stated [inner product](../../../../../../inner-product.md) is $\int w^2\widehat f\,\overline{\widehat g}$. By the [Plancherel theorem](../../../../../../plancherel-theorem.md) it is positive definite.

More strongly, $U:H^s\to L^2$ is onto: for $h\in L^2$, $w^{-1}h\in L^2$, since $w\geq1$, and $f=\mathcal F^{-1}(w^{-1}h)$ satisfies $Uf=h$. Thus $U$ is an isometric linear bijection, and completeness of $L^2$ gives

$$
\boxed{H^s(\mathbb R^n)\text{ is a Hilbert space with }\|f\|_{H^s}=\|w\widehat f\|_2.}
$$

This argument includes $s=0$ if zero is allowed in the printed $\mathbb R_+$ convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
